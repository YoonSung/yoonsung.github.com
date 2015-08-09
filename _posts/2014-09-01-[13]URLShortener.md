---
layout: entry
type: "Tags"
title: "URLShortener"
author: Yoonsung
author-email: estrella@nhnnext.org
description: URL축약 서비스
tags: [Servlet, Mysql, Redis]
publish: true
---

> Redis 및 Mysql Dump BackUp을 이용한 URL 축약 웹서비스입니다. URL을 입력하면, 짧은 버전의 URL을 반환하고, 해당 URL접근시 원본 URL로 리다이렉트 시켜 주는 기능을 합니다. Redis에 저장된 데이터는 Linux Cron Job을 통해 주기적으로 RDBMS (Mysql)로 백업됩니다.
Python을 이용해서 for문을 돌며 redis의 데이터를 mysql로 옮기는 기능을 구현 했으나, 성능상 좋아보이지 않아 redis의 dump파일을 mysql에 dump insert하기 위한 기능을 구현했습니다. redis에서 csv로 백업해 주는 기능이 없어서 redis-client.c 파일을 수정해서 원하는 기능을 구현했습니다

***

<br/>
<a href="https://github.com/YoonSung/URLShortener">소스저장소</a>
<div class="youtube">
	<iframe src="http://www.youtube.com/embed/SnDClysgZrk?autoplay=1" class="video"></iframe>	
</div>