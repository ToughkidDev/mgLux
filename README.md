# mgLux
mgLux - MSX Megarom Loader for LuxuryBox - Written by ToughkidCST 


## 개요

### mgLux       
	mgLux는 2013년 9월 MSX천국동의 프로젝트인 일명 "메가램카드 복각" 프로젝트의 결과물로 
	최종 출시한 "럭셔리박스"를 기반으로 만들어진 전용 롬파일 실행기입니다. 
  
### LuxuryBox
![LuxuryBox](mgLux.jpg)


### 사용방법
	
	mgLux.com [filename.rom] /opts

  mgLux는 대부분의 롬파일에 대하여 특별한 옵션없이 안전하게 실행됩니다. 
   

###  1. mgLux.com [filename.rom] 
  
  기본적인 사용방법은 도스프롬프트에서 위와 같이 mglUx과 파일이름을 입력하는 것 뿐입니다. 
  mgLux는 실행되는 순간 짧은 시간을 통해 롬파일 방식을 파악하고 실행하도록 합니다. 
  전반적으로 이 방법은 대부분의 게임을 실행하는데에 문제가 없는 방법입니다. 

   	예) mgLux gradius.rom  

###  2. mgLux.com  [filename.rom] /opt
  
   그럼에도 불구하고 
   mgLux로 롬의 실행이 적절하게 이루어지지 않은 경우. 
   mgLux가 롬의 mapper를 분석하는 시간을 생략하고 좀더 빠른 속도로 게임을 실행시키기 위하여. 
   이런 특별한 경우에 대하여 아래와 같이 최소한의 옵션을 사용하실 수 있습니다.

   /g - 만일 1번과 같은 방법으로 게임이 실행되지 않으면, /g 옵션을 사용하면
        게임파일을 분석해 정확한 매퍼와 실행방법을 알려줍니다. 
        거의 대부분의 게임은 이를 통해 실행 가능합니다. 

   /s - Konami, Konami-SCC 방식의 매퍼를 사용하는 메가롬 게임을 실행합니다. 
        '/g'옵션을 통해  Konami 방식인지 파악하실 수 있습니다. 

   /8 - ASCII8  방식의 매퍼를 사용하는 메가롬 게임을 실행합니다. 
        '/g'옵션을 통해 ASCII8 방식인지 파악하실 수 있습니다. 

   /f - ASCII16 방식의 매퍼를 사용하는 메가롬 게임을 실행합니다. 
        '/g'옵션을 통해 ASCII8 방식인지 파악하실 수 있습니다. 

   /r - 특별한 경우 이 옵션을 사용해야 실행되는 롬파일이 있을 수 있습니다. 
        이 옵션은 보통의 방법으로 실행되지 않는  롬파일에 대해 다른 형태의 롬파일 실행 방법을 제공합니다.  
        특정한 롬파일이 구동되지 않는 경우 이 옵션을 사용해 보십시요. 

   /q - 'MMC/SD'를 작동을 금지시키고 롬파일을 리셋해 실행합니다. 
   	이 옵션은 리셋이 필요한 게임의 실행시에 'MMC/SD'의 부팅초기화 프로세스를 금지시키고 
        즉각 롬파일을 실행해 실행호환성을 높입니다. 
        'MMC/SD'를 사용자 분들께 유효합니다. 

   /t - MSX로 Turbo-R을 사용하고 있다면 이 옵션을 통해 게임의 속도를 향상시키고, 
       게임에 따라 프레임레이트를 끌어올려 게임을 좀더 부드럽게 실행할 수도 있을 것입니다.
  
   /d - 사용자의 필요에 따라 로딩후 도스로 돌아오는 옵션이 필요할 수 있습니다. 
        이를 위해 사용하십시요. 

   /z - Zemina16K 매퍼방식의 메가롬 게임을 실행합니다. 
	초기 메가램팩(재미나 골든박스, 딜럭스박스등)들을 위해 릴리즈되었던 변형분할된 파일중에는  
        호환성을 위해 이 옵션이 필요한 경우가 있습니다. 
  
   /m - Sony에서 발매된 게임들에 댛 숨겨진 디버그 및 치트메뉴를 발생시키는 
        일명 Sony Inside-Magic Key  기능을 Enable 시킵니다. 
	GallForce, 雀聖, Replicart, 기기괴계, 패밀리복싱등의 게임들이 매직키 기능을 지원합니다. 

## Youtube Video Link - mglOcm,  "Sony Inside(裏) Magic Key" support
[![mglOcm, Sony Inside(裏) Magic Key support](https://yt-embed.herokuapp.com/embed?v=Vgrt5NiHgw0 )](https://youtu.be/Vgrt5NiHgw0 "Sony Inside(裏) Magic Key ")

   /k - "코나미10배로 즐기는 카트리지' 삽입 효과 발생

	  예) mgLux hinotori.rom /k
      	  불새를 실행하고, 슬롯2에 "코나미10배로 즐기는 카트리지" 를 삽입 효과 
     
   /k:keyword - keyword에 해당하는  카트리지를 슬롯2에 삽입 효과 발생 

          예) mgLux gradius.rom /k:twinbee
          그라디우스를 실행하고 슬롯2에 트윈비 카트리지를 삽입 효과 

           코나미 합성비기가 발생하는 각 키워드는 다음과 같습니다. 

               "kungfu",   이아쿵후
               "kungfu2",  이아쿵후 황제의 역습
               "kmare",    마성전설 
               "twinbee",  트윈비
               "gradius",  그라디우스
               "mong",     몽대륙
               "vampire",  악마성드라큘라
               "kingkong", 킹콩
               "qbert",    큐버트
               "hinotori", 불새
               "goemon",   간바레 고에몽
               "galious",  마성전설2 갈리오우스의 미궁
               "mgear",    메탈기어
               "gradius2", 그라디우스2
               "f1spirit", F1 스피리트
               "usas",     우사스
               "salamand", 사라만다.          

## Youtube Video Link - mglOcm, mgLux 코나미게임 합성 효과 즐기기 
 - https://www.youtube.com/watch?v=g5yTJ_7XwyQ&list=PLlD0W14KLTkpq5dnONr_U6fAUWuyGliEw&index=3


[![MSX mgLux mglOcm 코나미게임 합성 효과 즐기기](https://yt-embed.herokuapp.com/embed?v=g5yTJ_7XwyQ)](https://www.youtube.com/watch?v=g5yTJ_7XwyQ "MSX mgLux mglOcm 코나미게임 합성 효과 즐기기 ")

### 주의사항    -  

	0. 게임을 즐기신 후,  MSX의 전원을 끈 뒤 안전한 부팅을 위하여 3초이상 전원이 꺼진 상태를
	   유지해 주시기 바랍니다. 
	   럭셔리박스 메모리의 데이터가 충분히 지워지는 시간이 필요할 수 있습니다. 
	

	1. 기존 초기 메가램팩(재미나 골든박스, 딜럭스박스등)들을 위해 릴리즈되었던 변형분할된 파일이 
           에뮬레이터등을 위해 *.rom 파일로 다시금 단일파일로 만들어진 변형 롬파일들은  
           mglUx의 롬파일의 매퍼분석을 방해합니다. 
           대게의 경우 '/s', 'z' 옵션을 통해 이런 롬파일들이 실행 가능합니다. 
	     

	2. FDD가 주류이던 시대를 지나, MMC/SD나 SUNRISE-IDE등 대용량 고속매체를 사용함으로서, 
	   메모리부족으로 인한 호환성의 문제가 나타나는 게임이 있을 수 있습니다. 
	   이러한 경우 게임이 실행될 때까지 부팅하는 동안 각각 메모리를 확보할 수 있는 방법이 
	   필요할 수 있습니다. 
	   mmc/sd의 경우 '[CTRL]'키를, Sunrise-IDE는 '[INS]'키를 부팅하는 동안 눌러줌으로서
           게임을  실행하는데에 필요한 메모리를 확보하는데 도움을 줍니다.   
	   그 외의 경우에는 각각 매뉴얼을 통해 부팅 옵션을 확인해 보시기 바랍니다. 

	
	3. 오랜동안 다양한 하드웨어에서 실행되기 위해 변형된 롬파일들에 대해 mglUx는 비교적 
	   높은 안정성의 실행률을 자랑하고 있으나,  '/r'옵션의 사용으로도 실행되지 않거나, 
           오동작하는 롬파일이 발견되면 게시판을 통해 알려주시기 바랍니다.  
	    mglUx의 개선에 큰 도움이 됩니다. 


	4. dsk2rom으로 만들어진 롬들에 대하여 ASCII방식으로  만들어진 메가롬파일에 대응하고 있으나, 
           그외 호환성에 문제가 있을 수 있습니다.  참고하시기 바랍니다. 



### 사용환경 - 
	
	64KB이상,MSX-DOS2환경 이상의 모든 MSX
 
    
