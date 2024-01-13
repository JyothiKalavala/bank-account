# bank-account
#Bank operation using oop
class Bank:
    bankname="Union Bank"
    branch="A23,BBSR,Rjy"
    #Create account
    def_init_(self, username,pan, address):
        self.username = username
        self.pan = pan
        self.address = address
        self.balance = 0.0
        print(f'Hello{self.username} cong! your account created successfully')
    #deposit
    def deposit (self, amount):
        self balance = self.balance+amount
         print(f'{amount}deposited successfully')
    #withdraw
    def withdraw(self,amount):
        if amount<self.balance:
            self.balence = self.balance-amount
            print(f'{amount} withdraw successfully')
        else:
            print('Insufficient Fund...')
    #ministatement
    def ministatement(self):
        print(f'Your account balance is {self.balance}')
print(f'welcome to {Bank.bankname},{Bank.branch}')
username = input('Enter your name: ')
pan = input('Enter PAN Card number: ')
address = input('Enter your address: ')
b = Bank(username,pan, address)
while True:
    print('\nPlease select any option: ')
    Print ('1.Deposit\n2.Withdraw\n3.Ministatement\n4.Stop')
     if option == 1:
         amount = float(input('Enter Deposited amount:'))
          b.deposit(amount)
      elif option == 2:
          amount= float(input('Enter withdraw amount: '))
      elif option == 3:
           b.ministatement( )
      elif option == 4:
          print("Thanks for using Union Bank...')
           break
      else:
          print('Invalid option pls select a valid option')
