Kontrol Düzlemi (Control Plane) Bileşenleri

etcd

OpenShift kümesinin dağıtık anahtar-değer deposudur. Küme durumu, yapılandırma bilgileri ve meta veriler etcd üzerinde saklanır.

kube-apiserver

Tüm API isteklerini kabul eden, doğrulayan ve yönlendiren ana bileşendir. Hem kullanıcı isteklerini hem de iç bileşenler arası iletişimi yönetir.

kube-controller-manager

Küme içindeki durum ile istenen durum arasındaki farkı gideren kontrol döngülerini çalıştırır. Örnek kontroller: ReplicationController, EndpointController.

kube-scheduler

Yeni oluşturulan Pod’ların hangi node üzerinde çalışacağına karar veren zamanlayıcıdır (scheduler).

Node (Düğüm) Bileşenleri

kubelet

Her node üzerinde çalışan ajan bileşendir. Pod manifestlerini kontrol eder, Docker/CRI-O ile containerları oluşturur ve durum bilgisini kontrol düzlemine iletir.

CRI-O

Kubernetes’in Container Runtime Interface (CRI) standardına uyumlu, hafif bir konteyner çalışma zamanı motorudur.

kube-proxy

Her node’da çalışır. Ağ kurallarını yönetir ve servisler (Service) üzerinden gelen trafiği ilgili Pod’lara yönlendirir.

OpenShift’e Özgü Bileşenler

OpenShift SDN (Network)

OpenShift’in varsayılan yazılım tanımlı ağ katmanıdır. Pod’lar arası iletişim için ağ izolasyonu ve çoklu ağ stratejilerini destekler.

Ingress Router (Önyüz Yönlendirici)

HTTP/HTTPS trafiğini küme içindeki servis ve Pod’lara yönlendiren HAProxy tabanlı yönlendiricidir.

Image Registry (Görüntü Kaydı)

Konteyner imajlarını saklayan dahili Docker kayıt deposudur.

OAuth Server

Küme erişimi için kimlik doğrulama ve yetkilendirme işlemlerini yürütür. OAuth 2.0 standartlarına dayanır.

Operator Lifecycle Manager (OLM)

Operator paketlerinin dağıtımı, güncellenmesi ve yaşam döngülerini yönetir.

Cluster Version Operator (CVO)

OpenShift sürüm yükseltmelerini ve bileşen güncellemelerini otomatikleştirir.

Kullanıcı ve CLI Araçları

kubeadmin Kullanıcısı

Kurulum esnasında oluşturulan varsayılan yönetici (admin) kullanıcıdır. Küme ayarlarına tam erişim hakkına sahiptir.

oc CLI

OpenShift’e özel komut satırı aracıdır. Pod yönetimi, proje oluşturma, imaj işlemleri ve birçok OpenShift işlevine erişim sağlar.# openshiftcomponents
