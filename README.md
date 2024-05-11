# civitai-image-db  

**Over 4 million image URLs** - updated weekly.  

Links were not filtered so expect nsfw/18+ images - use at your own risk etc. etc. ...  

Part of collection of records for stable diffusion generated images from civitai.com  

**Directories:**  
`by_username`: csv files with image links/data in folders by username  
`all`: unsorted  

**CSV fields:**  
| Field Name   | Description                                                                                       |
|--------------|---------------------------------------------------------------------------------------------------|
| id           | record id                                                                                        |
| image_url    | This is civitai image UUID/GUID and it forms the image URL                                       |
| user_id      | this is not civitai user ID, it's a foreign key to other table when I keep track of usernames    |
| nsfw_level   | nsfw level, I think possible values are from 1 to 16                                             |
| created_at   | timestamp of when image was created/uploaded at civitai.com                                      |
| published_at | when image was made public/posted                                                                |
| tag_ids      | comma separated civitai image tag IDs                                                            |
| image_id     | civitai image ID                                                                                 |



`image_id`: originally I was downloading images and saving corresponding .txt files with its metadata/prompts but this took a lot of storage.  
Metadata for the most part is already in the image file itself and if any additional data is needed this is what the `image_id` is for, you can fetch it.  

**image_url**  
Full image URL can be constructed as follows:  
`https://image.civitai.com/xG1nkqKTMzGDvpLrqFT7WA/{image_url}/original=true/`  


**Note:** You will get `404` if an image was deleted.  
  
If you need links for any specific username or actual images/metadata feel free to ask as I likely already have them - saves downloading again.  

Mind that images may be NSFW or otherwise disturbing.   
