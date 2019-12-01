## Homework_1

With the rapid development of Wechat salesmen （multinational purchasing agents）, more and more people choose to buy things through Wechat. But actually the ways of recommend and trade are every tradition, sometimes it is hard for the seller to provide considerable service to every customers, which will result the loss of business and customers. After several years of development, this market has accumulated huge amounts of data. So I want to design an intelligent recommendation and trade system to provide better service to customers and save time for sellers. 

This system combined with two objectives, which are intelligent recommendation and automatic trade system.

It is like a plugin to Wechat, which can be installed as a mini program. It won’t take to much storage or computing power to execute. Once the seller open this mini program, it can automatic retravel the chatting record and the Moment to get useful information. Using the data from the historical shopping record, moment recommend, and chatting box, this program can form a intelligent recommendation of specific items for the customer. This program also provides the automatic trading system, linked to Wechat pay. After every recommendation, the historical shopping record can be updated.

## Objectives:

# Intelligent recommendation
After the customer send message to the seller about their requirement, the intelligent recommendation process will wake up and start working. The input of this process is the content of Wechat box and trend recommendation. it also call the data in historical shopping record and moment record to get the preference of this customer and the price and detail of items to recommend. First, we have to extract, transform and load the data, and transfer data to the recommend engine. We also need to call the chatting database to form the proper phrase to communicate with customers. 

# Automatic trade system
After recommend products to customer, the customer will give a feedback whether to buy or not. If choose to buy the product, the trade engine start working, it interact with Wechat pay to complete the deal. Also, we have to update the historical shopping record. If the buyer says that she will consider or refuse the suggestions, we update the historical shopping record either.

The database we use is RDBMS, since RDBMS is easy to maintain and use. Also the data we use always related to specific customers, the data are used to describe the character and shopping habits. Using RDBMS, we can easily call all the information related to the user and store it in categories.

# Work flow
![](https://github.com/lal0904/PHBS_BigData_2019/blob/master/workflow.jpg)  
