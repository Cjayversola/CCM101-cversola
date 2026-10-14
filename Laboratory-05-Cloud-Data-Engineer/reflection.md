# Mission 5 Reflection: The Cloud Data Engineer

In this laboratory activity, I learned about the three common types of cloud storage: block storage, file storage, and object storage. Each type has a different purpose. Block storage is commonly used for virtual machine disks and databases. File storage organizes data into files and folders, while object storage is useful for storing photos, videos, backups, and other unstructured data.

I learned that object storage is a good choice for a photo-sharing application because it can handle large amounts of images. As the number of users increases, the storage can grow to support more photos. Each object can also have its own metadata and unique identifier, which helps organize stored content.

Another important part of this activity was deploying MinIO using Docker. At first, I encountered an error when trying to download the original MinIO image from the laboratory instructions. I used the Chainguard MinIO image instead and was able to start the container. This taught me that troubleshooting is an important skill when working with cloud technologies.

I also learned how ports and environment variables are used when configuring a container. Port 9001 allowed me to access the MinIO web console, where I created the `client-photos` bucket. This helped me understand how an object storage service can be managed through a web interface.

For an enterprise application, I would improve the storage setup by using proper access permissions, regular backups, versioning, and redundancy. These measures can help protect photos from accidental deletion and reduce the risk of data loss. I would also avoid using simple laboratory credentials in a real production environment.

Overall, this activity helped me understand object storage and gave me more experience with Docker and Linux commands. I also learned that errors can be solved by checking the problem and finding a suitable alternative. These skills are useful for future cloud computing activities.
