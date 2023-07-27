# Digital-library
Digital library design using Python 


import JSON

def create_My_Digital_library():
  library = {}
  library["books"] = [ ]
  library["articles"] = [ ]
  return library

def add_book(library, book):
  library["books"].append(book)

def add_article(library, article):
  library["articles"].append(article)

def get_books(library):
  return library["books"]

def get_articles(library):
  return library["articles"]

def main():
  library = create_library()
  add_book(library, {"title": "Things Fall Apart", "author": "Chinua Achebe"})
Add_book(library, {"title": "A political satire", "author": "Chinua Achebe"})
Add_book(library,  {"title": "The Trouble with Nigeria", "author": "Chinua Achebe"}) 
  add_article(library, {"title": "The Trouble with Nigeria", "author": "Chinua Achebe"})
  print(get_books(library))
  print(get_articles(library))

if __name__ == "__main__":
  main()
