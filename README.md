# function_as_a_service
example using cloud functions

Instructions AWS Lambda Website
Use AWS Cloud9 and "right click" to a new lambda function (as shown in screencast "A Tale of Three Websites")

Paste the code below into the editor.

The following example demonstrates the Python code necessary to build a Lambda function that returns HTML.

def lambda_handler(event, context):
    content = """
    <html>
    <p> Hello website Lambda </p>
    </html>
    """
    response = {
        "statusCode": 200,
        "body": content,
        "headers": {"Content-Type": "text/html",},
    }
    return response
"Right-click" deploy the lambda function
Log into AWS console and click on the API Gateway icon in the AWS Lambda section. Verify that it returns "Hello website Lambda".
