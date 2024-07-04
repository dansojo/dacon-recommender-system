## Dataset Info.

### view_log.csv [파일] - train 데이터
- 유저가 기사를 조회한 로그 데이터
- 학습 데이터이며 해당 데이터에 존재하는 유저만 추천의 대상이 됨

  
userID : 유저 고유 ID


articleID : 기사 고유 ID


userRegion : 유저가 속한 지역


userCountry : 유저가 속한 국가




### article_info.csv [파일] - meta 데이터
- 기사에 대한 정보

  
articleID : 기사 고유 ID


Title : 기사의 제목


Content : 기사의 본문


Format : 기사의 형식


Language : 기사가 작성된 언어


userID : 기사를 작성한 유저 고유 ID


view_log에 포함되지 않은 유저가 존재할 수 있으며, 해당 유저는 추천의 대상이 되지 않음


userCountry : 기사를 작성한 유저가 속한 국가


userRegion : 기사를 작성한 유저가 속한 지역




### sample_submission.csv [파일] - 제출 양식
userID : 유저 고유 ID
추천의 대상이 되는 유저의 ID


articleID : 기사 고유 ID
해당되는 유저에게 추천할 기사의 ID


한 유저에게 5개의 기사를 추천하게 되며, 유저가 기존에 조회한 기사 추천 가능



### article_nouns_df.csv [파일] 
- article_info.csv 에서 작업
- 불필요한 컬럼 제거 (userRegion, userCountry, userID)
- article_info.csv 파일의 Title, Content 칼럼을 불용어 제거 및 명사만 추출
