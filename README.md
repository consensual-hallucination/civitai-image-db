# civitai-image-db  

Part of collection of records for stable diffusion generated images from civitai.com  

`by_username`: csv files with image links/data in folders by username  
`all`: unsorted  

Sample in csv format with following fields:  
```
id: record id  
image_url: This is civitai's image UUID/GUID and it forms the image URL  
user_id: this is not civitai's user ID, it's a foreign key to other table that contains civitai's usernames
nsfw_level: nsfw_level  
created_at: timestamp of when image was created/uploaded at civitai.com  
published_at: when image was made public  
tag_ids: comma separated civitai image tag IDs  
image_id: civitai's image ID  
```


`image_id`: originally I had downloaded images with corresponding .txt file with its metadata/prompts but this took a lot of storage. Metadata for the most part is already in the image file and if any additional data is needed this is what the `image_id` is for, you can fetch it.  

`image_url`  
Full image URL can be constructed as follows:  
`https://image.civitai.com/xG1nkqKTMzGDvpLrqFT7WA/{image_url}/original=true/`  


Note: You will get `404` if an image was deleted.  
  
If you need links for any specific username or actual images/metadata feel free to ask as I likely already have them - saves downloading again.  

Mind that images may be NSFW or otherwise disturbing.   
