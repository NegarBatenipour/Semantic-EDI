# Semantic-EDI
Semantic EDI

To transform EDI order messages into Semantic EDI order messages, we developed a translator in Python, one for the EDIFACT version D.03B (2003) and one for
the D.16B (2016) version. Semantic EDI represents EDI messages in a machine-interpretable format (RDF), and it has less processing time and less human effort.
We prepared three order messages for each version. Order1.txt, Order2.txt, and Order3.txt for D.16B (2016), and Order1-2003.txt, Order2-2003.txt, and Order3-2003.txt for D.03 (2003). Each EDI order includes components, elements, and segments. 

Also, we have designed a Smart Client to demonstrate the use of our translator. The Smart Client performs queries on turtle files using SPARQL.In our Smart Client, we consider three different ordering messages. Each of them has different Item Identifier, Quantity, and Price; therefore, our given inputs
are output1.ttl, output2.ttl, and output3.ttl files (outputs of translator for three different EDI ordering messages) and data.ttl. Data.ttl contains information about the company and its products like the production process and the corresponding production line of each product. It also contains information about the machines needed to produce a product and when those machines are free and how long it takes to produce the product once.

Please go through these steps:
1. Copy all the files in the same folder.
2. Import RDF library before running the codes.
3. For running all the .py files, you can use PyCharm, or any related softwares. You can also use this command in the terminal: python (name of the file).py
4. Run EDIOrderingMessage2016-Order1.py----->input:order1.txt....output:output1.ttl
5. Run EDIOrderingMessage2016-Order2.py----->input:order2.txt....output:output2.ttl
6. Run EDIOrderingMessage2016-Order3.py----->input:order3.txt....output:output3.ttl
7. Repeat these steps for EDIOrderingMessage2003.py
8. Run SmartClient.py----->input:output1.ttl,output2.ttl,output3.ttl,data.ttl
9. Finish.
10. Furthermore, we have uploaded our Report for your consideration.
