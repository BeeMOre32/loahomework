1. 개요

이 문서는 현재 개인적으로 진행하고 있는 프로젝트의 기획안이며, 챈럼들에게 지금 진행하고 있는 개인 프로젝트가 어떤 것 인지를 설명하는 기획안입니다.

2.이걸 만들게 된 이유

현재 로스트아크 라는 게임 자체에서 지원하고 있는 일일에포나, 카던, 가디언 토벌, 군단장, 및 기타 등등 여하 숙제라고 불리는 것들을 표시하는 기능이 있기는 하지만 생각보다 보여지는 정보의 양이 적기 때문에 별도의 사이트를 이용하는 이용자들이 많다. 그렇기 때문에 포트폴리오 용도로 만들 예정이며, 추후 업데이트 및 사후지원은 있을 예정이고 깃헙에 호스팅을 맏기고 유저의 데이터는 브라우저 자체의 데이터 베이스를 이용하여 별도의 서버 없이도 상태를 저장 할 수 있도록 구상을 할 예정임.

3. 대략적인 형태

여기에 아래와 같이 캐릭터 박스를 드래그 앤 드롭 할 수 있도록 외부 라이브러리를 사용하여 제작을 할 예정.

대신에 캐릭터를 클릭을 하면 별도의 모달창을 열게 되며 이 모달창을 이용해 일일 숙제 및 주간 숙제 완료를 체크 할 수 있으며, 체크를 모두 마쳐야 위의 사진 처럼 움직이게 할 예정

(그 외에도 추가적인 기능 추가 및 이루어 질 수도 있으며 디자인 및 형태가 달라질수도 있음을 알림)

4. 제작을 하는 데 필요한 것(메모용)

React-app(프레임 워크)

(라이브러리)

 ReactRouter, beautiful dnd, Framer motion, Recoil, react form hook, gh-pages, moment.js, React-hook-form

5. 예상되는 문제점

5.1 다른 컴퓨터 간의 이동이 불가능: 위는 앞에서 말 했던 별도의 서버 없이 브라우저에서 지원하는 데이터베이스를 이용을 하기 때문에 이는 곧 다른 브라우저 또는 다른 컴퓨터 또는 다른 환경에서도 같은 데이터를 공유 할 수도 없고, 브라우저에서 지원하는 데이터베이스에 오류가 생길시 페이지 전반적인 오류를 불러올 수도 있기 때문에 이는 유저의 사용자 경험을 안 좋게 만들수도 있음. 이 문제는 근본적으로 서버를 두지 않기 때문에 발생하는 오류 이므로 잠정적으로 구글의 firebase를 이용해 유저간의 데이터를 따로 google서버에 호스팅을 하는 방식으로 데이터를 이전하는 일이 필요함, 하지만 이는 유저의 이동저항 그리고 브라우저와 서버간의 데이터 이동시 발생하는 오류에 대처하기가 힘들어짐. 하지만 지금 당장 firebase를 기반으로 하는 지식 부족 및 실력 부족으로 인한 한계 이므로 페이지를 런칭하고 어느 정도 기간 후에 firebase와 지식을 갖추고 천천히 이동을 할 예정. 하지만 그 때 동안 발생하는 오류 및 불편한 점은 유저의 좋지 않은 경험으로 남을 것이 예상이 됨.

5.2 매주 수요일 마다 초기화를 해야 함: 이 부분은 온전히 나의 코딩 실력의 부족이므로 상기의 문제점은 페이지 제작 완료후 빠른 시일내에 고칠 수 있도록 조치 하겠음.
