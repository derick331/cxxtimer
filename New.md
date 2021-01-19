# Requirement
1. deletePlaylistSong() - (*head_ref)->length need to delete twice? Why?


<= userSong instead of < userSong? because when length = 1 and userSong = 1, then how?
<= userPlaylist instead of < userPlaylist?

deletePlaylistSong() no need traverse the playlist? SongCollection* selectedSong 没有用到?


addPlaylistSong() if (selectedPlaylistSong->song == selectedSong) move in front of 
while (selectedPlaylistSong->next != NULL) ? 
ANS: Nonid. Because we put the if statement behind is because the while loop cannot check whether the last song in playlist
     is the same as the song to be added by user.


deletePlaylistSong() got error because of this (?):
addPlaylistSong() no 'newSong->length++' for else{} only if{}


addPlaylist() - if using while(last->next != NULL) cannot check for the last node whether
the playlist exist or not because last node 的 next is NULL, it will break from the loop before
checking the last node.


displayPlaylist() - why i < 3 in the for loop?

deleteSong() - if(userSong == 1) // if user choose the first song

PlaylistMenu(), case 5:
why using SongCollection* selectedSong since it is not use in deletePlaylistSong()?

playlistSearch() - can straight use head to traverse? no need to create another pointer?
