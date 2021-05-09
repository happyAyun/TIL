- Kubernetes Cluster 시작
  
  - launch.sh
  - 클러스터 구성 요소를 시작, Kubectl CLI를 다운로드.
  
- Create Deployment - 배포 생성하기
  
  - yaml 파일을 통해 cluster에 배치한다.
    - `kubectl create -f x.yaml`
  - deployment 리스트 확인
    - `kubectl get deployment`
  - 각각의 deployment 의 세부사항 detail 확인
  - `kubectl describe deployment [deployment name]`
  
- Create Service - 서비스 배포

  