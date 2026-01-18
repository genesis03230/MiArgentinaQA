# Bug Reports – Mi Argentina

---

## BUG-01: Province Can Be Lost Outside the Playable Area

### Environment
- Engine: Unity 2021.3.12f1
- Platform: PC
- Build: Playable version

### Severity
High

### Priority
High

### Description
During gameplay, collectible province objects can be dropped outside the intended playable area.  
Once lost, the province does not respawn or return to a valid location, making it impossible to complete the game without restarting.

### Steps to Reproduce
1. Start the game and enter the main puzzle room
2. Pick up a province using the raycast interaction
3. Move close to a wall or boundary of the playable area
4. Drop the province outside the map limits

### Expected Result
- The province should not be allowed to leave the playable area  
OR  
- The province should respawn after a short time in a valid position

### Actual Result
- The province falls outside the map
- The object becomes unrecoverable
- Game progression is blocked

### Impact
- Prevents game completion
- Forces the player to restart the game
- Negatively affects user experience

### Evidence
- Video and visual evidence available in the `Evidence` folder
