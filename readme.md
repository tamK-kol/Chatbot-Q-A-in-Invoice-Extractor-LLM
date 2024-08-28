## Readme for for Chatbot Q&A in Invoice Extractor 
=====================================

![alt text](<Tamal single invoice extractor.PNG>)

### Q: What is the Invoice Extractor?
The Invoice Extractor markdown is a specific format used to extract relevant information from invoices. It's a standardized way to annotate invoices with key information, making it easier to automate the extraction process.

* Here's a breakdown of the typical components of an Invoice Extractor markdown (Example):

![alt text](<invoice demo.jpg>)


1. Header
* invoice_date: The date of the invoice
* invoice_number: The unique identifier of the invoice
* bill_to: The company or individual being billed
* ship_to: The company or individual receiving the goods or services

2. Line Items
* item_description: A brief description of the item or service
* item_quantity: The quantity of the item or service
* item_unit_price: The price per unit of the item or service
* item_total: The total cost of the item or service

3. Footer
* sub_total: The subtotal of all line items
* tax: The total tax amount
* total: The grand total of the invoice

### Q: What is its Purpose?
The purpose of this Chatbot Q&A is to provide a conversational interface for users to interact with multilanguage invoices on single window and with only one file only.

### Q: How to use?
* Upload an Invoice Image: Click on "Choose an image of the invoice" and select an image file.
* Enter a Prompt: Provide a text prompt for querying the invoice content.

![alt text](input_demo.png)

* Submit: Click the "Tell me about the invoice" button to receive a response.

![alt text](output_demo.png)