## Mock Transfer Reciept Pipeline - Nordstrom

This repo is to develop workflows for Nordstrom's usecases described by EPAM here: (https://docs.google.com/document/d/1Nq_ZPsC2p7fxeQcueEgFCz3YIGVwRlxnizQOV37Sg6o/edit?usp=sharing) transfer_receipt flow description and challenges

## Configuration

Two options:
1. Run the server locally  [local Temporal Server](https://docs.temporal.io/cli#starting-the-temporal-server)  on localhost:7233.


````

## Workflows
1.TransferReceipt
Temporal Workflow that orchestrates the underlying APIs, ultimately flushing to storage.
2.TransferReceiptSupervisor
A Temporal Workflow with one activity...a consumer of the Kafka topic that routes/starts TransferReceipt Workflows.

