• Objects (files) have a Key
• The key is the FULL path:
	• s3://my-bucket/==my_file.txt==
	• s3://my-bucket/==my_folder1/another_folder/my_file.txt==
• The key is composed of prefix + object name
	• s3://my-bucket/==my_folder1/another_folder/==my_file.txt
• **There’s no concept of “directories” within buckets (although the UI will trick you to think otherwise)**
• Just keys with very long names that contain slashes (“/”)
• Object values are the content of the body:
	• Max. Object Size is 5TB (5000GB)
	• If uploading more than 5GB, must use “multi-part upload”
• Metadata (list of text key / value pairs – system or user metadata)
• Tags (Unicode key / value pair – up to 10) – useful for security / lifecycle
• Version ID (if versioning is enabled)