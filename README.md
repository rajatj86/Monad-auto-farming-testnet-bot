Monad Testnet Interaction Guide
Step 1: Set Up Your Computer
Install Python
If Python isn’t installed on your computer, follow these steps to download and install it:

Go to the official Python website: https://www.python.org/downloads/.
Download the latest version (e.g., Python 3.11 or higher).
During installation:
Check the box that says “Add Python to PATH” (important for running Python from the command line).
Select “Install Now”.


After installation, open the Command Prompt (press Win + R, type cmd, and press Enter) and type the following to verify:
```bash
python --version
```
Step 2: Create a Folder for Your Project
Run the following commands in the Command Prompt to create a project folder on your Desktop:
```bash
cd Desktop
mkdir monad_testnet
cd monad_testnet
```

 Set Up a Virtual Environment

Using a virtual environment ensures that your project dependencies are isolated from other Python projects.

Install Virtual Environment Package

If virtualenv is not installed, install it using:
```bash
pip install virtualenv
```

Create a Virtual Environment

Create a virtual environment named venv in your project folder:
```bash
virtualenv venv
```

Activate the Virtual Environment
```bash
venv\Scripts\activate
```

After running this command, you should see (venv) in your Command Prompt, indicating the virtual environment is active.

Deactivate the Virtual Environment (Optional)

To deactivate the virtual environment later, simply run:

```plain
deactivate
```


Step 3: Install Required Python Libraries
Install the necessary Python libraries by running:
```bash
pip install web3>=6.21.0 python-dotenv==1.0.0 colorama==0.4.6 eth-account>=0.13.0 py-solc-x>=2.0.3 tk>=0.1.0
```
if this command is not working then use this one

```plain
pip install -r requirements.txt
```
Step 4: Create the Script File (main.py)

You can create the main.py file directly from the Command Prompt or manually using a text editor.

Create main.py Using Command Prompt

Run the following command to create an empty main.py file:

```plain
echo. > main.py
```

Add the Python Script to main.py
Open the main.py file in a text editor:
If you have Notepad++, open it and then drag the main.py file into Notepad++ to edit it.
Alternatively, you can use Notepad by right-clicking main.py in the monad_testnet folder and selecting "Edit with Notepad".
Copy the entire Python script provided to you earlier.
Paste the script into the main.py file in your text editor.
Save the file:
In Notepad++, click File > Save.
In Notepad, click File > Save.
Alternative: Create main.py Manually
If you prefer to create the file manually:
Open Notepad++ (or Notepad if you didn’t install Notepad++).
Copy the entire Python script provided earlier.
Paste the script into a new file in the text editor.
Click File > Save As.
Navigate to the monad_testnet folder on your Desktop (e.g., C:\Users\YourUsername\Desktop\monad_testnet).
Name the file main.py (make sure to include .py at the end)
Click Save.



Step 5: Create the Private Key File
The script requires a file named pvkey.txt containing your wallet’s private key. This is sensitive information, so handle it carefully.

Get Your Private Key: Obtain the private key of your Monad testnet wallet (e.g., from MetaMask or another wallet).

```plain
echo YOUR_PRIVATE_KEY > pvkey.txt
```
Set “Save as type” to “All files (.)” in Notepad (not needed in Notepad++).
Click Save.



Step 6: Fund Your Wallet with Testnet MON

Ensure your wallet is funded with testnet MON tokens. You may need to use a Monad testnet faucet or request tokens from the Monad community.

Step 7: Run the Script

Navigate to the Project Folder: In the Command Prompt, ensure you’re in the monad_testnet folder. If not, type:
```bash
cd C:\Users\YourUsername\Desktop\monad_testnet
```
Replace YourUsername with your actual Windows username.

Execute the Script: Run the script using:
```bash
python main.py
```
Script Output
After running the script, you’ll see the following interface:
════════════════════════════════════════════════════════════
│                MONAD TESTNET INTERACTION                 │
════════════════════════════════════════════════════════════
👥 Accounts: 1
┌──────────────────────────────────────────────────────────┐
│                    SELECT PLATFORM                       │
└──────────────────────────────────────────────────────────┘
1. Apriori
2. Ambient DEX
3. Magma
4. iZumi
5. Bima
6. Kintsu
7. Monorail
8. Rubic
9. Custom Swap
0. Exit
➤ Enter choice:

Interact with the Script

The script shows a list of platforms (Apriori, Ambient DEX, etc.).
Type a number (e.g., 1 for Apriori, 6 for Kintsu) and press Enter.
Next, it asks for the number of cycles (how many times to run the action). Type 1 (or another number) and press Enter.
The script will perform actions (e.g., stake, unstake) and show progress with messages like:

➤ stake          | Amount: 0.0423 MON
➤ stake          | Tx: https://testnet.monadexplorer.com/tx/0x...

If You Need Help
If any step fails (e.g., an error during installation, script execution, or funding), let me know the following:

The exact step number.
The error message (copy-paste it).
Your operating system (Windows, Linux, Mac).
If you’re unsure about your wallet, private key, or testnet setup, I can provide more details.
For funding issues, I can search for alternative faucets or guide you through community channels.

