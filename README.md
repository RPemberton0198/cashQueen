# atm
For Lab3 you will be creating an ATM program.

* Write a program that behaves like an ATM that you can interact with. You should be able to:

    * If you have a bank account, access it with a pin

    * Create a new bank account with a unique pin

    * Deposit money into the bank account and print the new balance

    * Withdraw money from the bank account and print the new balance

    * Get the balance of the bank account

    * Change the pin of the bank account
	
	* Optionally: 
	    * Your accounts should persist across sessions.

* You should take advantage of objects and functions to organize your ATM simulator.

* The code should be well documented with comments, have good code structure, and follow naming conventions.

* Push your code to your repository.

<!--Comments on JS functions:
loginPin

createPin

withdrawal

deposit

updatePin

logOff



-->




<!--My Psuedo coding used for this exercise

log-in with pin
                             create account with PIN (check if unique)
                              depoit money
                              print balance (display)
                              withdrawl
                              change pin

                    HTML first
                              what elements
                                   buttons
                                   input boxes
                                        login with pin
                                        change PIN
                                        create account with PIN
                                        deposit
                                        withdrawl
                                   success/failure message
                                   Alert Boxes
                    LogIn Account
                         if user presses loginPINBtn
                         (reminder is blank () )
                         check the user value against local storage
                         if login is invalid then display alert "invalid PIN"
                         elsewise  valid - hide login div and show withdrawl div and load infor from local storage
                         user acceses homepage
                         balance
                    Create Account
                         if the user presses createPinBtn
                         (reminder is blank () )
                              check user input against local storage
                                   if PIN is listed in local storage
                                   diplay error message PIN unavailable

                              elsewise PIN is available
                                   store PIN in local storage
                                   set balance to $0
                                   hide the login div
                                   show the withdrawl view (page)
                                   get balance from  local storage
                                   show balance
                    Make deposits/withdrawal
                         if user presses deposit button
                              get the value from the textbox
                              get their balance from localStorage
                              if value is < = zero
                                   display error message alert
                              elsewise valid  allow deposit
                                   balance +  value
                                   display balance
                                   store balance  local storage

                    the user presses the update pin button
                              value is a blank string -
                                   (() )
                                   display error
                              check value against local storage
                                   if value exists
                                        display error
                              otherwise
                                   update pin in localStorage
                            event listeners - onclicks html - click js
                    the user presses log off after all transactions complete 

              will need to create an array of objects
              then convert objects to strings for local storage and then back to objects from local storage
              Json stringify when sending data to web server the data has to be a string dot convert a JavaScript object into a string using json dot strigify ()

              objects = accounts - example of json dot stringify () = json dot strigify (account1) or you can stringify an array the result will be a string you can send to server
                    how to unstringify json parse */

      /*let account1 = {
                                  pin: "0001"
                                  balance: "0"

                             }
                               let account2 = {
                                  pin: "0002"
                                  balance: "0"

                             }  let account3 = {
                                  pin: "0003"
                                  balance: "0"

                             }  let account4 = {
                                  pin: "0004"
                                  balance: "0"

                             }  let account5 = {
                                  pin: "0005"
                                  balance: "0"

                             }  let account6 = {
                                  pin: "0006"
                                  balance: "0"

                             }  let account7 = {
                                  pin: "0007"
                               balance: "0"

                             }
                             let accounts = [account1, account2, account3, account4, account5, account6, account7, ]-->


<!--code to toggle back to login screen - not what I needed but good snippet to keep-->

<!--<button onclick="toggleClock()" id="clockButton">Show clock</button>-->

  <!--function toggleClock() {
    // get the clock
    var myClock = document.getElementById('clock');

    // get the current value of the clock's display property
    var displaySetting = myClock.style.display;

    // also get the clock button, so we can change what it says
    var clockButton = document.getElementById('clockButton');

    // now toggle the clock and the button text, depending on current state
    if (displaySetting == 'block') {
      // clock is visible. hide it
      myClock.style.display = 'none';
      // change button text
      clockButton.innerHTML = 'Show clock';
    }
    else {
      // clock is hidden. show it
      myClock.style.display = 'block';
      // change button text
      clockButton.innerHTML = 'Hide clock';
    }
  }-->