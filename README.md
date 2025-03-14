# Supply chain CVE analyzer for container images

## Objective
The goal of this assignment is to build an CVE scanner for container images. The scanner should open a container image, check the packages and versions it contains, and then compare the versions to OpenCVE database to check if there are packages in the container image that have vulnerabilities.

## Repository Setup
Clone this repository.

## Implementation Details
1. Take a container image as an argument.
2. If the image is a file locally then work with it, otherwise pull the image from a container repository
3. Open up the image and scan the image for different packages and versions. Packages can be of multiple types - rpms, debs, python, go, etc
4. Connect to OpenCVE with the package and version and check for CVEs
5. Create a report of the number of critical, high, medium and low severity CVEs

## Documentation Requirements
1. README.md file with installation instructions and how to run
2. Code
3. Unit test scripts

## Judgement Criteria
The submission will be judged on how many container image types it can scan, the kinds of packages it can scan and how many CVEs are detected
The submission should also have a command line filters to scan for specific CVEs, specific severity values. The more the filters types the better

## Submission Instructions
1. Complete the implementation
2. Complete the README.md
3. Make a PR to submit your final code
4. Your PR should include:
   - Description of your implementation
   - Any limitations or known issues
   - Example test cases
