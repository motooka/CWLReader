# CWLReader
A simple reader of [Amazon CloudWatch Logs](http://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/WhatIsCloudWatchLogs.html) LogGroups.

## How To Use

- Make an IAM user which have permissions of
  - `logs:DescribeLogGroups`
  - `logs:FilterLogEvents`
- Download Access Key & Secret of the IAM user
- Load the html file on your browser
- Fill the credentials
- Select Region
- (optional) Save credentials and region. These data will be stored on your browser's LocalStorage. If you save these information, these will be automatically loaded on your next visit.
- Load LogGroups
- Select a LogGroup
- Read the logs and 

## Dependencies

- [AWS SDK for JavaScript](http://docs.aws.amazon.com/AWSJavaScriptSDK/latest/index.html) for Browsers.

## Installation

Just place the `CWLReader.html` file on your HTTP server. Your browser will try to load the dependencies listed above.

You can also place the HTML file on your local drive and load it via `file://` protocol, but it is not recommended because your credentials are save on [HTML5 LocalStorage](http://www.w3schools.com/html/html5_webstorage.asp) and any other your local scripts can read your credentials. It would be insecure.

## Supported Browsers

Browsers which are not supported by [AWS SDK for JavaScript](http://docs.aws.amazon.com/AWSJavaScriptSDK/latest/index.html) are explicitly unsupported.

## License

MIT License.

Full description of the license will be found in the `CWLReader.html`.
