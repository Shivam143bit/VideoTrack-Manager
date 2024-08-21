# VideoTrack-Manager-
Enhanced user interface and input validation features enable users to add, update, delete, search, and list videos with the YouTube Manager application, a command-line tool for managing a list of YouTube videos.
It is a command-line tool designed to help users manage a list of YouTube videos stored in a JSON file ('youtube.txt'). This tool allows users to perform various operations, including listing all videos, adding new videos, updating existing videos, deleting videos, searching for videos, and exiting the application. Below is a detailed description of each functionality, how it works, and the functions used to implement these features:
# 1. List All YouTube Videos
## Functionality: 
Displays a list of all YouTube videos currently stored in the JSON file.

## How It Works:
-> The list_all_videos(videos) function is called.
-> It prints a header and iterates over the list of videos, printing each video's name and duration in a formatted manner.
-> If there are no videos, it informs the user that no videos are available.

## Function Used: list_all_videos(videos)

![Screenshot 2024-05-27 233301](https://github.com/Shivam143bit/YouTube-Manager-Application-/assets/85752605/1c9802ae-979a-4d2d-a17e-4c89631be61f)
![image](https://github.com/Shivam143bit/YouTube-Manager-Application-/assets/85752605/8502d02b-f7a3-45ac-8d09-c0190bf17b36)

# 2. Add a YouTube Video
## Functionality:
Prompts the user to input a new video's name and duration, and then adds this video to the list.

## How It Works:
-> The add_video(videos) function is called.
-> It prompts the user to enter the video's name and duration.
-> The new video details are appended to the videos list as a dictionary.
-> The save_data_helper(videos) function is called to save the updated list to the JSON file and inform the user that the data has been saved.

## Function Used: add_video(videos), save_data_helper(videos)

![image](https://github.com/Shivam143bit/YouTube-Manager-Application-/assets/85752605/0f7b2175-14c0-48e9-abfb-0f764125a86b)
![image](https://github.com/Shivam143bit/YouTube-Manager-Application-/assets/85752605/1f4ff61b-a475-4b6a-b403-2d5f5e1094a0)

# 3. Update a YouTube Video
## Functionality: 
Allows the user to update the details of an existing video by selecting it from the list.

## How It Works:
-> The update_video(videos) function is called.
-> It calls list_all_videos(videos) to display the current videos.
-> It prompts the user to select the video number they wish to update.
-> If the input is valid, the user is prompted to enter the new video name and duration.
-> The selected video in the videos list is updated with the new details.
-> The save_data_helper(videos) function is called to save the changes.

## Function Used: update_video(videos), list_all_videos(videos), save_data_helper(videos)

![image](https://github.com/Shivam143bit/YouTube-Manager-Application-/assets/85752605/799fb030-2cba-4d3d-92d3-8999c9a6204d)
![image](https://github.com/Shivam143bit/YouTube-Manager-Application-/assets/85752605/daec61ec-8148-4caf-a963-ec495c7f4c17)
![image](https://github.com/Shivam143bit/YouTube-Manager-Application-/assets/85752605/08df80f2-8c16-41aa-8dac-d365a0a59bd9)

# 4. Delete a YouTube Video
## Functionality: 
Allows the user to delete a video by selecting it from the list.

## How It Works:
->The delete_video(videos) function is called.
->It calls list_all_videos(videos) to display the current videos.
->It prompts the user to select the video number they wish to delete.
->If the input is valid, the selected video is removed from the videos list.
->The save_data_helper(videos) function is called to save the updated list.

## Function Used: delete_video(videos), list_all_videos(videos), save_data_helper(videos)

![image](https://github.com/Shivam143bit/YouTube-Manager-Application-/assets/85752605/38bad0ad-6ce7-4c4b-bee5-e43317c1d75f)
![image](https://github.com/Shivam143bit/YouTube-Manager-Application-/assets/85752605/1e001c0a-9493-41c2-bda7-51a6185dfe33)
![image](https://github.com/Shivam143bit/YouTube-Manager-Application-/assets/85752605/4a03e97a-fcc3-4e56-a65a-162be139744a)

# 5. Search for a YouTube Video
## Functionality:
 Allows the user to search for videos by name.

 ## How It Works:
-> The search_video(videos) function is called.
-> It prompts the user to enter a search term.
-> It filters the videos list to find videos whose names contain the search term (case-insensitive).
-> The found videos are displayed in a formatted list. If no videos match the search term, it informs the user that no videos were found.

## Function Used: search_video(videos)

# 6. Exit the App
## Functionality:
Exits the application.

## How It Works:
-> The user selects the option to exit.
-> A goodbye message is printed, and the loop in the main() function breaks, terminating the application.

## Function Used: No specific function, handled in the main() function loop.

![image](https://github.com/Shivam143bit/YouTube-Manager-Application-/assets/85752605/0c6ed552-fb4b-4908-a77a-6526d81bca8e)


# Real-Time Problems and Motives Solved by the YouTube Manager Application
## Problems Solved:
## -> Organization of YouTube Content:
      Users often have a list of YouTube videos they want to manage, including videos they plan to watch, have watched, or want to keep track of for future reference. This application helps organize this list in one place.
      
## -> Simplified Management:
      Manually tracking YouTube videos, their titles, and durations can be cumbersome. The application simplifies this by providing an easy way to add, update, delete, and list videos.
      
## -> Quick Access to Video Information:
      By listing all videos in one place, users can quickly access and review their collection, saving time compared to searching through bookmarks or history.

## -> Search Functionality:
      With many videos in a list, finding a specific video can be difficult. The search feature allows users to quickly locate videos by name.

# Conclusion

The YouTube Manager application is a practical tool designed to streamline the management of personal YouTube video collections. By allowing users to add, update, delete, list, and search videos, it addresses common organizational challenges faced by frequent YouTube users. The application's clear interface and robust functionality make it a valuable resource for anyone looking to efficiently manage their video content.

The project demonstrates how basic programming concepts such as file handling, user input, and list operations can be combined to create a useful real-world application. It showcases the importance of data persistence, user feedback, and input validation, ensuring that the application is both reliable and user-friendly.

In conclusion, By following this structure, the YouTube Manager application provides a simple yet effective way to manage a list of YouTube videos, making it easy for users to perform CRUD (Create, Read, Update, Delete) operations with additional search functionality.
      











