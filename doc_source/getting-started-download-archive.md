# Step 4: Download an Archive from a Vault in Amazon Glacier<a name="getting-started-download-archive"></a>

In this step, you download the sample archive you uploaded previously in [Step 3: Upload an Archive to a Vault in Amazon Glacier](getting-started-upload-archive.md)\.

**Important**  
Any archive operation, such as upload, download, or deletion, requires that you use the AWS Command Line Interface \(AWS CLI\) or write code\. There is no console support for archive operations\. For example, to upload data, such as photos, videos, and other documents, you must either use the AWS CLI or write code to make requests, using either the REST API directly or the AWS SDKs\. For more information about using Amazon Glacier with the AWS CLI, see [AWS CLI Reference for Amazon Glacier](http://docs.aws.amazon.com/cli/latest/reference/glacier/index.html)\. To install the AWS CLI, see [AWS Command Line Interface](http://aws.amazon.com/cli/)\.

In general, retrieving your data from Amazon Glacier is a two\-step process: 

1. Initiate a retrieval job\.

1. After the job completes, download the bytes of data\. 

To retrieve an archive from Amazon Glacier, you first initiate a job\. After the job completes, you download the data\. For more information about archive retrievals, see [Retrieving Amazon Glacier Archives](downloading-an-archive-two-steps.md)\.

The access time of your request depends on the retrieval option you choose: Expedited, Standard, or Bulk retrievals\. For all but the largest archives \(250 MB\+\), data accessed using Expedited retrievals are typically made available within 1–5 minutes\. Archives retrieved using Standard retrievals typically complete between 3–5 hours\. Bulk retrievals typically complete within 5–12 hours\. For more information about the retrieval options, see the [Amazon Glacier FAQ](http://aws.amazon.com/glacier/faqs/#Data-retrievals)\. For information about data retrieval charges, see the [Amazon Glacier detail page](http://aws.amazon.com/glacier)\.

The code examples shown in the following topics initiate the job, wait for it to complete, and then download the archive's data\. 


+ [Download an Archive from a Vault in Amazon Glacier Using the AWS SDK for Java](getting-started-download-archive-java.md)
+ [Download an Archive from a Vault in Amazon Glacier Using the AWS SDK for \.NET](getting-started-download-archive-dotnet.md)