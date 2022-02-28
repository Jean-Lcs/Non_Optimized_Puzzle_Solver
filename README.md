# Non_Optimized_Puzzle_Solver

The objective of this project is to solve a puzzle, following these steps
  -  Take any initial image
  - Cut it into a certain number of pieces (this number being modifiable)
  - Shuffle it randomly
  - Find, among all the permutations, the one minimizing the discontinuity of the RGB pixels
  - Reassemble the image thanks to the permutation that is now known 

This method is not very optimized because we calculate the discontinuity for each combination. As an example, for a puzzle having for 4 three and for length the same number (16 pieces), we must calculate the discontinuity for 16 ! = 2.1 billion permutations.
The algorithm is therefore very slow, but works well.

However, this algorithm has an advantage, it does not require to be given a piece of the puzzle as a corner or an edge. This means that the cut image alone is sufficient to find the original image.
