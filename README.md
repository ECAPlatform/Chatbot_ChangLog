# Chatbot_ChangLog



####  admin portal
#####  2023-06-13
1.  db , chatmessage 添加2个字段

2.  更新数据库的基础数据

   	UPDATE chat_message  c
		INNER JOIN sys_user s
		ON c.custom_id=s.id
		SET c.custom_name=s.username
		
		UPDATE chat_message  c
		INNER JOIN sys_user s
		ON c.user_id=s.id
		SET c.user_name=s.username
