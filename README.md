# POST-TEST

# 서버 사용방법

## 회원가입
신규유저 등록
### 요청
> [POST] /users/signup

전달값
<pre>
{
  'username':'hongildong',
  'password':'hong1234',
  'name':'홍길동A'
}
</pre>

### 결과
#### 성공
<pre>
{
  '_id':'1234567890',
  'username':'hongildong',
  'name':'홍길동A'
}
</pre>
#### 실패
<pre>
{
  'message':'400 Bad Request'
}
</pre>


### 로그인
>[post] /users/signin

전달값
<pre>
{
  '_id':'1234567890',
  '_password':'123456789abc',
  'name':'홍길동'
  }
 </pre>
 
 ### 결과
 #### 성공
 <pre>
 {
   'message':''
 }
 </pre>
 
 #### 실패 
 <pre>
 {
  'message':'400 Bad Request'
 }
 
 </pre>
