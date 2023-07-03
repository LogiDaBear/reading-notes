# What are the key characteristics of serverless computing, and how does it differ from traditional server-based architectures?
- Provisioning time: Measured in milliseconds for serverless, vs. minutes to hours for the other models.

 

- Administrative burden: None for serverless, compared to a continuum from light to medium to heavy for PaaS, containers and VMs respectively.

 

- Maintenance: Serverless architectures are managed 100% by the provider. The same is true for PaaS, but containers and VMs require significant maintenance including updating/managing operating systems, container images, connections, etc.

 

- Scaling: Auto-scaling—including auto-scaling to zero—is instant and inherent for serverless. The other models offer automatic but slow scaling that requires careful tuning of auto-scaling rules, and no scaling to zero.

 

- Capacity planning: None needed for serverless. The other models require a mix of some automatic scalability and some capacity planning.

 

- Statelessness: Inherent for serverless, which means scalability is never a problem; state is maintained in an external service or resource. PaaS, containers and VMs can leverage HTTP, keep an open socket or connection for long periods of time, and store state in memory between calls.

 

- High availability (HA) and disaster recovery (DR): Both are inherent in serverless with no extra effort and at no additional cost. The other models require additional cost and management effort. In the case of both VMs and containers, infrastructure can be restarted automatically.

- Resource utilization: Serverless is 100% efficient because there are no such things thing as idle capacity—it is invoked only upon request. All other models feature at least some degree of idle capacity.

 

- Billing granularity and savings: Serverless is metered in units of 100 milliseconds. PaaS, containers and VMs are typically metered by the hour or the minute.
# How can one get started with Vercel, and what are the main steps involved in deploying a serverless function using Vercel?
- Sign up, install Vercel
- Develop your serverless function: Write your serverless function code in the language of your choice. Vercel supports various languages such as JavaScript, TypeScript, Python, Go, and more. Ensure that your function is properly structured and ready to be deployed.

- Test your serverless function: Before deploying, it's a good practice to test your serverless function locally to ensure it works as expected. You can use the Vercel CLI to run your function locally and perform tests.

# What are APIs, and how can they be utilized in Python applications to access and manipulate data from external sources?
- APIs (Application Programming Interfaces) are sets of rules and protocols that allow different software applications to communicate and interact with each other. They define how different components of software systems should interact, enabling developers to access and manipulate data from external sources.

- In Python, APIs can be utilized to access and manipulate data from external sources by making HTTP requests to the API endpoints and processing the responses.

# What is the Requests library in Python, and how can it be used to interact with APIs by sending HTTP requests? Can you provide an example of a basic GET request using the Requests library?
- The Requests library is a popular Python library for making HTTP requests. It provides a user-friendly and intuitive API that simplifies interacting with APIs by sending HTTP requests and handling responses. The library abstracts away the complexities of making HTTP requests and offers convenient methods for common HTTP methods like GET, POST, PUT, DELETE, etc.
    ```import requests

    # Make a GET request
    response = requests.get('https://api.example.com/data')

    # Check the response status code
    if response.status_code == 200:
        # Request was successful
        data = response.json()  # Convert response to JSON format
        print(data)
    else:
        # Request was not successful
        print('Error:', response.status_code)
    ```

    ## Things I want to learn more about
  - Kubernetes
