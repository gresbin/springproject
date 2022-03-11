# Megabox

## 개발 준비 단계

#### 1) ER-Diagram

![image-20220311205621457](README.assets/image-20220311205621457.png)



#### 2) UML 클래스 다이어그램

1. Model

   | USER                                                         |
   | ------------------------------------------------------------ |
   | int user_id<br />String password<br />String email<br />String userName<br />int age<br />boolean sex<br />String phoneNum<br />String userNickname<br />String img_url<br />Date createdAt<br />Date updatedAt<br />int point |
   | public User()                                                |

   | MOVIE                                                        |
   | ------------------------------------------------------------ |
   | int movie_id<br />String movie_title<br />String ori_title<br />boolean adult<br />String poster_path<br />float popularity<br />Date release_date<br />String director<br />Strinor<br />int genre<br />int runtime <br />String overview<br />float voteaverage<br />String trailer<br />String spoken_lang<br />String status<br />String pro_comp<br />String pro_cont<br />int revenue<br />int people |
   | public movie()                                               |

   | GENRE                               |
   | ----------------------------------- |
   | int genre_id<br />String genre_name |
   | public genre()                      |

   | MOVIE_GENRE                                   |
   | --------------------------------------------- |
   | int mg_id<br />int movie_id<br />int genre_id |
   | public Movie_genre()                          |

   | TICKETING                                                    |
   | ------------------------------------------------------------ |
   | int ticket_id<br />int user_id<br />int movie_id<br />String location<br />Datetime onscreenTime<br />int noPeople<br />String seats<br />int usedPoint<br />int earnedPoint<br />String couponType<br />float discountRate<br />String paymentMethod |
   | public Ticketing()                                           |

   | REVIEW                                                       |
   | ------------------------------------------------------------ |
   | int review_id<br />int user_id<br />int movie_id<br />float score<br />String review<br />Datetime createdAt |
   | public Review()                                              |

   | INQUIRY                                                      |
   | ------------------------------------------------------------ |
   | int inquiry_id<br />int user_id<br />String inquiryTitle<br />String inquiryContent<br />Datetime createdAt |
   | public Inquiry()                                             |

   | LIKE                          |
   | ----------------------------- |
   | int user_id<br />int movie_id |
   | public Like()                 |

   