# Assignement
## Test Case 1
### Pre-requisites:
- Download a graphics benchamrk (3dmark or specviewperf or something similar)
### Steps
- Create a batch script with the following steps
- Create a test directory
- Copy the downloaded file (.msi/.exe) from the downloaded/remote location to local test directory
- Install the benchmark (use silent installation)
    - while install is happening, you need to wait till the end
    - or run the install in the background
- Verify bechmark is installed successfully
    - Abort the test if benchmark failed/not installed properly
    - if installation fails, 
        - remove the installed directory or any files exists
        - fail the test / kill the batch job with error message
- Launch the exe from the batch script, pass if any command line arguments are required to run the test. use (/help or --help to get list of supported commands)
- Wait for the test to complete
- Verify logs are created
- Read the log file or search log file for required results or test status
- Copy the log file to test directory
- Print the overall test status



