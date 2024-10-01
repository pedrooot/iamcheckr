**Iam-Checkr: A Tool to Identify Unused IAM Policies in AWS**

**Description**
--------------

Iam-Checkr is a tool designed to scan IAM (Identity and Access Management) policies in AWS and report on those that are not being used since a specific timestamp. This allows security and access administrators to identify opportunities to improve permission management and reduce the risk of exposure.

**Features**
------------

* **Automated Scanning**: Iam-Checkr scans IAM policies in your AWS account and analyzes their usage.
* **Detailed Report**: Receives a report showing unused policies, including policy name, permission type, and last access timestamp.
* **Configurable**: You can configure the tool to scan only specific regions or accounts.

**How it Works**
----------------

1. **Connects to AWS**: Iam-Checkr connects to your AWS account using your access credentials.
2. **Scans Policies**: The tool scans IAM policies in each region and account configured.
3. **Analyzes Usage**: Analyzes the usage of each policy to determine if it is being used or not.
4. **Detailed Report**: Generates a report showing unused policies.

**Requirements**
--------------

* Python 3.x installed on your system
* `boto3` library installed for interacting with AWS
* Access credentials for your AWS account

# WIP

**Installation**
----------------

You can install Iam-Checkr using pip:
```bash
pip install iam-checkr
```

**Usage**
---------

```python
import iam_checkr

# Configure your AWS access credentials
aws_access_key_id = 'YOUR_ACCESS_KEY_ID'
aws_secret_access_key = 'YOUR_SECRET_ACCESS_KEY'

# Configure the region and account you want to scan
region = 'your-region'
account_id = 'your-account-id'

# Run the scan
iam_checkr.scan_iam_policies(aws_access_key_id, aws_secret_access_key, region, account_id)

# Check the results of the scan
print(iam_checkr.get_unused_policies())
```

**License**
------------

Iam-Checkr is distributed under the Apache 2.0 license. You can find more information in the `LICENSE` file.

**Contact**
------------

If you have any questions or need help, please contact us at [email](pedromarting3@gmail.com) or [Twitter](https://x.com/pdrmrtn).

**Notes**
------

* This project uses the `boto3` library to interact with AWS. You can find more information about its use in the `README` file of the library.
* For additional help, please consult the official documentation of `boto3` or contact us through the channels mentioned above.