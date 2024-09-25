def check_loan_eligibility():

    salary = float(input("Enter your monthly salary: 35,000"))
    loan_amount = float(input("Enter the loan amount you are requesting: 350,000"))

if salary >= 30000 and loan_amount <= salary * 10:

    print("You are eligible for the loan.")

    months = int(input("Enter the numbers of months to pay the loan: 12"))

    loan_interest = loan_amount = 1.10
    monthly_payment = loan_interest / months 

    print(f"your loan amount with 10% interest is: {loan_interest:.2f}")
    print(f"your monthly payment wil {monthly_payment:.2f}")

else:
    if salary < 30000:
        print("you are not eligible because the salary is too low.")
    if loan_amount > salary * 10:
        print("you are not eligible because the loan amount request is too high.")
