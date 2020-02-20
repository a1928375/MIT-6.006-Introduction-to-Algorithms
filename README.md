# MIT-6.006-Introduction-to-Algorithms

1. docdist1:
      
      This program computes the "distance" between two text files as the angle between their word frequency vectors (in radians).

      For each input file, a word-frequency vector is computed as follows:
      
          (1) the specified file is read in
          
          (2) it is converted into a list of alphanumeric "words". Here a "word" is a sequence of consecutive alphanumeric characters.
          Non-alphanumeric characters are treated as blanks. Case is not significant.
          
          (3) for each word, its frequency of occurrence is determined
          
          (4) the word/frequency lists are sorted into order alphabetically

          The "distance" between two vectors is the angle between them. If x = (x1, x2, ..., xn) is the first vector (xi = freq of word i) and  y = (y1, y2, ..., yn) is the second vector, then the angle between them is defined as: 
          
          d(x,y) = arccos(inner_product(x,y) / (norm(x)*norm(y))) where: inner_product(x,y) = x1*y1 + x2*y2 + ... xn*yn
          
          norm(x) = sqrt(inner_product(x,x))

2. docdist2:

      Changed concatenate to extend in get_words_from_line_list，其餘都與docdist1相同

3. docdist3:
      
      Improved inner_product to exploit sorted order and achieve linear instead of quadratic time，其餘都與docdist2相同

4. docdist4:

      Changed count_frequency to use dictionaries instead of lists，其餘都與docdist3相同
      
5. docdist5:

      Change get_words_from_string to use string translate and split，其餘都與docdist4相同
      
6. docdist6:

      Changed sorting from insertion sort to merge sort，其餘都與docdist5相同
      
7. docdist7:

      Remove sorting altogether via more hashing，其餘都與docdist6相同

8. docdist8:

      Treat whole file as a single "line"，如Fig. 1，其餘都與docdist7相同
      
