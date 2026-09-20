# k8s-postgrest-postgres-challenge

Pod é a menor unidade do Kubernetes, agrupando um ou mais containers que compartilham rede e armazenamento. Um Pod criado sozinho não tem autocura: se for deletado ou falhar, nada o recria, pois não há um controlador responsável por ele. É por isso que raramente criamos Pods diretamente — usamos Deployments, que gerenciam um ReplicaSet por baixo dos panos. O ReplicaSet garante que sempre exista o número desejado de réplicas rodando, recriando Pods automaticamente quando necessário. O Deployment vai além disso, adicionando controle de rollout: atualizações graduais (rolling update) e a capacidade de reverter (rollback) para uma versão anterior caso algo dê errado.


