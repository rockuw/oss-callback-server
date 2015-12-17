# A simple callback server for OSS

Callback Server用于接收OSS的上传回调请求（HTTP POST）。如果在上传文件
时指定了Callback，当文件成功上传到OSS时，OSS会向用户指定的callback
server发起一个HTTP POST请求，以通知本次上传成功。

https://help.aliyun.com/document_detail/oss/api-reference/object/Callback.html

## Run

### Install dependencies

    bundle install

### Start server

    ruby server.rb

默认会监听本机的`4567`端口，可以通过`ruby server.rb -p xxxx`来指定监听
的端口。
