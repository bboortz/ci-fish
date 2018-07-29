# ci-fish
CI system which is trying to solve different problems for developers using simplifying and swimming in docker bowl


## Project Status
Currently only a collection of ideas.
In case you want to provide any feedback no not hesitate to do so!


## Problems

### The Problems ci-fish is trying to solve
* Many CI systems are hard to install 
* Many CI systems are hard to maintain over the time
* Many CI systems are not supporting developer with their development and delivery process
* Many CI systems are not helping developer to get rid of manual tasks like maintaining changelogs, release notes, etc.
* Many CI systems are becoming a vendor-lock-in
* Many CI systems are hard to run locally 
* Many CI systems are not seperating very well so that pipelines can read other pipelines data
* Mnay CI systems are dealing this secrets not in a secure manner


### Ideas how to solve the Problems?
* Using docker to ship the ship the product to ensure it can be easily downloaded, installed and run
* Using docker to seperate pipelines in a secure manner to ensure the processed data cannot be read by other pipelines
* Using yaml files for configuration to ensure it is easy to maintain.
* Using no database to ensure it is simple to restore and behaving as a self contained service.
* Using REST interfaces to ensure it can be easily interfaces and integrated into other tooling
* Using json payload for all interaces to ensure the input/output can be easily processed
* Using (web) hooks to provide information/data to other systems like chatbots, other build systems, etc.
* Using strong encryption to ensure secret, confidential or personal data stay safe.
* Building a system around common development and delivery processes that automates all manual work to ensure the system fits to your process
* Avoiding all kind of non open source components to ensure we are avoiding a vendor-lock-in


## Developer and Delivery Processes

### Common Developer and Delivery Process

![Common Developer and Delivery Process](https://www.draw.io/?lightbox=1&highlight=0000ff&edit=_blank&layers=1&nav=1&title=developer_process.xml#R7Vvvk7I2EP5r%2FNgbSBDhoz%2FOt%2Fehnc7c2%2BnnHERgDgiN8dT%2B9d1AUDCcMh0UrDpzJ9mEjdlnd5Nn0RGeJ7sfnGThb8yn8QgZ%2Fm6EFyOETAvZ8CYl%2B0IywU4hCHjkq0FHwXv0D1VCQ0k3kU%2FXtYGCsVhEWV3osTSlnqjJCOdsWx%2B2YnF91owEVBO8eyQupS%2Fjo%2FyvyBehkpu2e%2Bz4lUZBqCZ3yiV%2FEO8z4GyTqhlHCK%2FyV9GdkFKXWuo6JD7bVkT4dYTnnDFRXCW7OY2ldUvDFfctv%2Bk9rIfTVLS5wTZ84ny4K8DMsnxMfkGFhi8Sb2i5hPyDin1pnm0YCfqeEU%2B2t%2BACIzwLRRJDy4TLfPXUV63DAg3ZEJx9HizqgGTFUqEcAMkRJI6CFBoefH7K5YAojucsZjyfGy9fF8icHFRVe%2FIX9OgmUFb5olzQXUWkTPKDsoQKvochqhe5bukCyoUtpWN79AbkKAzDiiNYWAmJ8sHgoPyIAlwoIFqCgjVQfpLPKA1AxmBVcjr4%2B0nWnxpYsGJRx6duuZSl9MTMSqRBIe0XQZRMVUcS%2Bb6cZtbkEEcvME69oIr5RLWbgMzHqZU0OHYHqNotUbWvAarVEGl2LMHyoy%2B4DOSlNCJfC5L6BdwipPA%2FpVt5neNd3AKzV%2B5qUOTFhEerfaGFeB7NQKknlXkc0OMRaa%2BKUyKUIpmtIyETHwd1YTn6g5%2Fef6r1rtzUtM646VU8E7d1Tfcarmlf3gTiKLd%2BPaOj73aCizngbN5XSF815WPzFAITNUBgNUBgXgOCyRMCkDRtuzeDwNEg%2BD3Pu437LOiC4%2Bl3aaYdInUk7YYcdOl4NFvOrKl7FqhrpjELncaQowNomuMGAEthpwi6l4OouuNUsfDJOjyg1H6PAR2Z1JzsAsmNXgo6gl7kjNGa%2BlPZluqlgYwXiXHOmyw5TcqEJ40EtgCcYJMN5WQwzNL9puYqZkM4X9w%2FC2qCPK%2Bj6HVOoxcZrg6%2Bcavjldkig%2FbKZJZzw9APOh2H5HgyLCZj6kl1Qb9ozLJELvK%2BjoU3ZS86kr2yF7Mpt2pUwWdV2uJXkW5JNvgmTQsd87dCBdwi6FpyjizKqDwErZ%2B0oyOX6pd2lEWxRzr0jjXq1y%2FvOKzgoTHol3iUJq9gUC%2ByDJJ7YHeymE774h5jNDDugfSirQbck3x0RD5se1jkAzUVdwdFPmY3IB%2FOeFjkA401VN7APhAsgt7Z0fCm1EPHsVfqgZrK0%2BeeUmSbXCGnf29y4vDfqEfJNp5koyMn6plsPGCF3dEIX89kQ68GPSAGPZMNvZDzlmQxTWgK%2BZOlGiDDYBuvSxePcV9swzEGxjZwi9LJk210xDZca1hsA7eo2fT7pS3XNYyzsdoBKqaJh0U3sF7GWcAJEla0v7Oz4U3ZRgOOvdINrBdyfJrFTH7k4rlGxpm%2F8WSBTrBR8aUoQXhA7%2B151rUpQAOy%2FXIA3KJM8387f8L5Y1gkAOtVmUcEoV8WgFvVVP5cU%2FIRy5TXvgiiKfmjzJatiibDYBu2M3PG877Yhmk4Q6MbLYonT7rREd0wYfcbFt9o%2BhJPfrAFKyLjEOCDDOXZ0sZub48pTWzfNJShefwxUd5X%2Bc0Wfv0X)


### Common Problems with this Process
* The process often missing testing
* The process often also contains manual testing
* The process often is very slow. E.g. integration takes long
* The process is hiding some work. E.g. maintaning changelog and release notes

### Ideas How to solve the Process Problems?
* Enforcing testing
* Enforcing that only small changes can be done to the system
* Enforcing that every successfull build becomes a new built product
* The CI system has to maintain the versioning, changelog and release notes for the developer
** the developer only has to decide if it is a major, minor and patch update



## Implementation Ideas

