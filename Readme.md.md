# RSAT Password Reset Simulation (Local User)

## SCenario
 Simulated support ticket: user 'jdoe' was locked out and requested a password reset. I acted a SHepl Desk support using PowerShell and RSAT tools.
 
## Actions Taken
 1. Created user: 'net user jdoe MyInitialPass /add'
 2. Locked account: 'net user jdoe /active:no'
 3. Reset password: 'net user jdoe NewTempPass'
 4. Reactivated account: 'net user jdoe /active:yes'
 5. Forced password reset on next login: 'net user jdoe /logonpasswordchg:yes'

## Outcome
 - Password was successfully reset
 - Account reactivated and forced password reset policy in place

## Tools Used
 - Windows PowerShell
 - RSAT concepts simulated on local system

## Related Exam Domain
 - Network+ Domain 4: Access Management