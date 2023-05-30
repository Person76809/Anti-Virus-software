# Anti-Virus-software
This code scans for viruses and deletes them. For more in depth info check the read me file.

how it works: 

the is_malicious() function checks the file extension of each file and compares it against a list of known malicious extensions (MALICIOUS_EXTENSIONS). If the file has a malicious extension, it is considered malicious, and the handle_malware() function is called to handle it. You can modify the is_malicious() function to implement more advanced malware detection  

Real-time scanning: The start_real_time_scanning() function starts a separate thread for continuously monitoring the specified 

Quarantine Directory: The detected malicious files are moved to a quarantine directory for isolation and further analysis.

The code includes a placeholder for implementing user experience improvements. You can customize this section to include features like real-time 

delete_viruses that allows you to delete the detected viruses and cure your computer of some viruses.

delete_viruses, should be called at the end of the main function. It will execute the code to delete viruses and cure the computer. 

Input Validation: Ensure that the directory_path provided by the user exists and is a valid directory before starting real-time scanning or performing a one-time scan.

Exception Handling: Handle exceptions that may occur during file operations, such as moving or deleting files. It's important to handle exceptions gracefully and provide appropriate error messages to the user.

Logging: Consider using a logging framework to log important events, errors, and actions taken during the scanning process. This can be helpful for debugging and monitoring purposes.

Fine-tune ClamAV Configuration: Review and configure the ClamAV antivirus settings according to your specific requirements, such as adjusting the sensitivity level or enabling specific scanning options
