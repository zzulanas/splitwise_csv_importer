# Splwiswise CSV Importer

This is a simple utility to import a CSV file into Splitwise.

Create a `.env` file in the same directory as `splitwise_importer` with the following contents:

```
SPLITWISE_API_KEY=<your api key>
SPLITWISE_API_SECRET=<your api secret>
SPLITWISE_API_TOKEN=<your api token>
```

Run the script with the following command:

```
python3 splitwise_importer <csv file> <tag name>
```

The CSV file should be in the following format:

| Date       | Account   | Description                     | Category    | Tags                | Amount |
| ---------- | --------- | ------------------------------- | ----------- | ------------------- | ------ |
| 2024-05-01 | Amex Gold | Aplpay Pueblo Queridbrooklyn Ny | Restaurants | {TAG NAME TO MATCH} | -23.4  |
| 2024-05-01 | Amex Gold | Baby's Buns & Bucketbrooklyn Ny | Restaurants |                     | 26.67  |
| 2024-05-01 | Venture X | New York City Transit           | Travel      |                     | 2.9    |
| 2024-05-01 | Venture X | New York City Transit           | Travel      |                     | 2.9    |
