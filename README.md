# Blockchain_based_ledger
Blockchain based ledger

# Background

You’re a fintech engineer who’s working at one of the five largest banks in the world. You were recently promoted to act as the lead developer on their decentralized finance team. Your task is to build a blockchain-based ledger system, complete with a user-friendly web interface. This ledger should allow partner banks to conduct financial transactions (that is, to transfer money between senders and receivers) and to verify the integrity of the data in the ledger.

# What You're Creating

You’ll make the following updates to the provided Python file for this Challenge, which already contains the basic PyChain ledger structure that you created throughout the module:
1. Create a new data class named Record. This class will serve as the blueprint for the financial transaction records that the blocks of the ledger will store.
2. Change the existing Block data class by replacing the generic data attribute with a record attribute that’s of type Record.
3. Create additional user input areas in the Streamlit application. These input areas should collect the relevant information for each financial record that you’ll store in the PyChain ledger.
4. Test your complete PyChain ledger.

# Instructions

Open the pychain.py file that your Challenge files include. You’ll use this file to complete the steps for this Challenge. Notice that the PyChain ledger that you built throughout this module already includes the functionality to create blocks, perform the proof of work consensus protocol, and validate blocks in the chain.
The steps for this Challenge are divided into the following sections:
1. Create a Record Data Class
2. Modify the Existing Block Data Class to Store Record Data
3. Add Relevant User Inputs to the Streamlit Interface
4. Test the PyChain Ledger by Storing Records

# Step 1: Create a Record Data Class

Define a new Python data class named Record. Give this new class a formalized data structure that consists of the sender, receiver, and amount attributes. To do so, complete the following steps:
Define a new class named Record.
Add the @dataclass decorator immediately before the Record class definition.
Add an attribute named sender of type str.
Add an attribute named receiver of type str.
Add an attribute named amount of type float.
Note that you’ll use this new Record class as the data type of your record attribute in the next section.

# Step 2: Modify the Existing Block Data Class to Store Record Data

Rename the data attribute in your Block class to record, and then set it to use an instance of the new Record class that you created in the previous section. To do so, complete the following steps:
In the Block class, rename the data attribute to record.
Set the data type of the record attribute to Record.

# Step 3: Add Relevant User Inputs to the Streamlit Interface

Code additional input areas for the user interface of your Streamlit application. Create these input areas to capture the sender, receiver, and amount for each transaction that you’ll store in the Block record. To do so, complete the following steps:
Delete the input_data variable from the Streamlit interface.
Add an input area where you can get a value for sender from the user.
Add an input area where you can get a value for receiver from the user.
Add an input area where you can get a value for amount from the user.
As part of the Add Block button functionality, update new_block so that Block consists of an attribute named record, which is set equal to a Record that contains the sender, receiver, and amount values. The updated Blockshould also include the attributes for creator_id and prev_hash.

# Step 4: Test the PyChain Ledger by Storing Records

Test your complete PyChain ledger and user interface by running your Streamlit application and storing some mined blocks in your PyChain ledger. Then test the blockchain validation process by using your PyChain ledger. To do so, complete the following steps:
In the terminal, navigate to the project folder where you've coded the Challenge.
In the terminal, run the Streamlit application by using streamlit run pychain.py.
Enter values for the sender, receiver, and amount, and then click the Add Block button. Do this several times to store several blocks in the ledger.
![Screen Shot 2022-08-06 at 1 38 59 PM](https://user-images.githubusercontent.com/101524382/183265604-f8c33933-97a4-429b-8b9c-1be15f36eccf.png)
![Screen Shot 2022-08-06 at 1 38 43 PM](https://user-images.githubusercontent.com/101524382/183265606-9d63373c-95a0-4dd9-8bc8-86b8b2d5671d.png)
![Screen Shot 2022-08-06 at 1 37 14 PM](https://user-images.githubusercontent.com/101524382/183265607-c00afc06-3a3e-4f6c-b0d6-860fa85d059b.png)
![Screen Shot 2022-08-06 at 12 41 15 PM](https://user-images.githubusercontent.com/101524382/183265608-b75f74f0-12c5-4efe-af03-57259fe1765f.png)


