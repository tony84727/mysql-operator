load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name = "io_bazel_rules_go",
    urls = [
        "https://storage.googleapis.com/bazel-mirror/github.com/bazelbuild/rules_go/releases/download/v0.20.3/rules_go-v0.20.3.tar.gz",
        "https://github.com/bazelbuild/rules_go/releases/download/v0.20.3/rules_go-v0.20.3.tar.gz",
    ],
    sha256 = "e88471aea3a3a4f19ec1310a55ba94772d087e9ce46e41ae38ecebe17935de7b",
)

http_archive(
    name = "bazel_gazelle",
    urls = [
        "https://storage.googleapis.com/bazel-mirror/github.com/bazelbuild/bazel-gazelle/releases/download/v0.19.1/bazel-gazelle-v0.19.1.tar.gz",
        "https://github.com/bazelbuild/bazel-gazelle/releases/download/v0.19.1/bazel-gazelle-v0.19.1.tar.gz",
    ],
    sha256 = "86c6d481b3f7aedc1d60c1c211c6f76da282ae197c3b3160f54bd3a8f847896f",
)



load("@io_bazel_rules_go//go:deps.bzl", "go_rules_dependencies", "go_register_toolchains")

go_rules_dependencies()

go_register_toolchains()

load("@bazel_gazelle//:deps.bzl", "gazelle_dependencies", "go_repository")

gazelle_dependencies()

http_archive(
    name = "com_google_protobuf",
    urls = [
        "https://github.com/protocolbuffers/protobuf/archive/v3.11.2.tar.gz",
    ],
    strip_prefix = "protobuf-3.11.2",
)

load("@com_google_protobuf//:protobuf_deps.bzl", "protobuf_deps")

protobuf_deps()

go_repository(
    name = "com_github_aws_aws_sdk_go",
    importpath = "github.com/aws/aws-sdk-go",
    sum = "h1:cOVt6EaBps0ax+uFGyzsTjMFkMktForcp0GQ0CM0cMU=",
    version = "v1.12.41",
)

go_repository(
    name = "com_github_beorn7_perks",
    importpath = "github.com/beorn7/perks",
    sum = "h1:BtpsbiV638WQZwhA98cEZw2BsbnQJrbd0BI7tsy0W1c=",
    version = "v0.0.0-20160804104726-4c0e84591b9a",
)

go_repository(
    name = "com_github_coreos_go_semver",
    importpath = "github.com/coreos/go-semver",
    sum = "h1:wkHLiw0WNATZnSG7epLsujiMCgPAc9xhjJ4tgnAxmfM=",
    version = "v0.3.0",
)

go_repository(
    name = "com_github_davecgh_go_spew",
    importpath = "github.com/davecgh/go-spew",
    sum = "h1:vj9j/u1bqnvCEfJOwUhtlOARqs3+rkHYY13jYWTU97c=",
    version = "v1.1.1",
)

go_repository(
    name = "com_github_docker_spdystream",
    importpath = "github.com/docker/spdystream",
    sum = "h1:cenwrSVm+Z7QLSV/BsnenAOcDXdX4cMv4wP0B/5QbPg=",
    version = "v0.0.0-20160310174837-449fdfce4d96",
)

go_repository(
    name = "com_github_elazarl_goproxy",
    importpath = "github.com/elazarl/goproxy",
    sum = "h1:p1yVGRW3nmb85p1Sh1ZJSDm4A4iKLS5QNbvUHMgGu/M=",
    version = "v0.0.0-20170405201442-c4fc26588b6e",
)

go_repository(
    name = "com_github_emicklei_go_restful",
    importpath = "github.com/emicklei/go-restful",
    sum = "h1:1MGKWTwW+rqKPXlCs0T+6UMYBNp8Hwl+gMQ6hmf/GaQ=",
    version = "v1.1.4-0.20170410110728-ff4f55a20633",
)

go_repository(
    name = "com_github_evanphx_json_patch",
    importpath = "github.com/evanphx/json-patch",
    sum = "h1:fUDGZCv/7iAN7u0puUVhvKCcsR6vRfwrJatElLBEf0I=",
    version = "v4.2.0+incompatible",
)

go_repository(
    name = "com_github_fsnotify_fsnotify",
    importpath = "github.com/fsnotify/fsnotify",
    sum = "h1:IXs+QLmnXW2CcXuY+8Mzv/fWEsPGWxqefPtCP5CnV9I=",
    version = "v1.4.7",
)

go_repository(
    name = "com_github_ghodss_yaml",
    importpath = "github.com/ghodss/yaml",
    sum = "h1:ZktWZesgun21uEDrwW7iEV1zPCGQldM2atlJZ3TdvVM=",
    version = "v0.0.0-20150909031657-73d445a93680",
)

go_repository(
    name = "com_github_go_ini_ini",
    importpath = "github.com/go-ini/ini",
    sum = "h1:/MArBHSS0TFR28yPPDK1vPIjt4wUnPBfb81i6iiyKvA=",
    version = "v1.32.0",
)

go_repository(
    name = "com_github_go_logr_logr",
    importpath = "github.com/go-logr/logr",
    sum = "h1:M1Tv3VzNlEHg6uyACnRdtrploV2P7wZqH8BoQMtz0cg=",
    version = "v0.1.0",
)

go_repository(
    name = "com_github_go_openapi_jsonpointer",
    importpath = "github.com/go-openapi/jsonpointer",
    sum = "h1:wSt/4CYxs70xbATrGXhokKF1i0tZjENLOo1ioIO13zk=",
    version = "v0.0.0-20160704185906-46af16f9f7b1",
)

go_repository(
    name = "com_github_go_openapi_jsonreference",
    importpath = "github.com/go-openapi/jsonreference",
    sum = "h1:tF+augKRWlWx0J0B7ZyyKSiTyV6E1zZe+7b3qQlcEf8=",
    version = "v0.0.0-20160704190145-13c6e3589ad9",
)

go_repository(
    name = "com_github_go_openapi_spec",
    importpath = "github.com/go-openapi/spec",
    sum = "h1:C1JKChikHGpXwT5UQDFaryIpDtyyGL/CR6C2kB7F1oc=",
    version = "v0.0.0-20160808142527-6aced65f8501",
)

go_repository(
    name = "com_github_go_openapi_swag",
    importpath = "github.com/go-openapi/swag",
    sum = "h1:zP3nY8Tk2E6RTkqGYrarZXuzh+ffyLDljLxCy1iJw80=",
    version = "v0.0.0-20160704191624-1d0bd113de87",
)

go_repository(
    name = "com_github_gogo_protobuf",
    importpath = "github.com/gogo/protobuf",
    sum = "h1:3PaI8p3seN09VjbTYC/QWlUZdZ1qS1zGjy7LH2Wt07I=",
    version = "v1.2.2-0.20190723190241-65acae22fc9d",
)

go_repository(
    name = "com_github_golang_glog",
    importpath = "github.com/golang/glog",
    sum = "h1:VKtxabqXZkF25pY9ekfRL6a582T4P37/31XEstQ5p58=",
    version = "v0.0.0-20160126235308-23def4e6c14b",
)

go_repository(
    name = "com_github_golang_groupcache",
    importpath = "github.com/golang/groupcache",
    sum = "h1:6o8aP0LGMKzo3NzwhhX6EJsiJ3ejmj+9yA/3p8Fjjlw=",
    version = "v0.0.0-20171101203131-84a468cf14b4",
)

go_repository(
    name = "com_github_golang_protobuf",
    importpath = "github.com/golang/protobuf",
    sum = "h1:6nsPYzhq5kReh6QImI3k5qWzO4PEbvbIW2cwSfR/6xs=",
    version = "v1.3.2",
)

go_repository(
    name = "com_github_google_go_cmp",
    importpath = "github.com/google/go-cmp",
    sum = "h1:crn/baboCvb5fXaQ0IJ1SGTsTVrWpDsCWC8EGETZijY=",
    version = "v0.3.0",
)

go_repository(
    name = "com_github_google_gofuzz",
    importpath = "github.com/google/gofuzz",
    sum = "h1:A8PeW59pxE9IoFRqBp37U+mSNaQoZ46F1f0f863XSXw=",
    version = "v1.0.0",
)

go_repository(
    name = "com_github_google_uuid",
    importpath = "github.com/google/uuid",
    sum = "h1:Gkbcsh/GbpXz7lPftLA3P6TYMwjCLYm83jiFQZF/3gY=",
    version = "v1.1.1",
)

go_repository(
    name = "com_github_googleapis_gnostic",
    importpath = "github.com/googleapis/gnostic",
    sum = "h1:7XGaL1e6bYS1yIonGp9761ExpPPV1ui0SAC59Yube9k=",
    version = "v0.0.0-20170729233727-0c5108395e2d",
)

go_repository(
    name = "com_github_gopherjs_gopherjs",
    importpath = "github.com/gopherjs/gopherjs",
    sum = "h1:EGx4pi6eqNxGaHF6qqu48+N2wcFQ5qg5FXgOdqsJ5d8=",
    version = "v0.0.0-20181017120253-0766667cb4d1",
)

go_repository(
    name = "com_github_hashicorp_golang_lru",
    importpath = "github.com/hashicorp/golang-lru",
    sum = "h1:0hERBMJE1eitiLkihrMvRVBYAkpHzc/J3QdDN+dAcgU=",
    version = "v0.5.1",
)

go_repository(
    name = "com_github_heptiolabs_healthcheck",
    importpath = "github.com/heptiolabs/healthcheck",
    sum = "h1:a39puQSX8A1O2aJS0ujECju+f2dlGoucVhIZaakwrbk=",
    version = "v0.0.0-20171103213001-9926c14869d1",
)

go_repository(
    name = "com_github_howeyc_gopass",
    importpath = "github.com/howeyc/gopass",
    sum = "h1:kQWxfPIHVLbgLzphqk3QUflDy9QdksZR4ygR807bpy0=",
    version = "v0.0.0-20170109162249-bf9dde6d0d2c",
)

go_repository(
    name = "com_github_hpcloud_tail",
    importpath = "github.com/hpcloud/tail",
    sum = "h1:nfCOvKYfkgYP8hkirhJocXT2+zOD8yUNjXaWfTlyFKI=",
    version = "v1.0.0",
)

go_repository(
    name = "com_github_imdario_mergo",
    importpath = "github.com/imdario/mergo",
    sum = "h1:FeeCi0I2Fu8kA8IXrdVPtGzym+mW9bzfj9f26EaES9k=",
    version = "v0.0.0-20141206190957-6633656539c1",
)

go_repository(
    name = "com_github_jmespath_go_jmespath",
    importpath = "github.com/jmespath/go-jmespath",
    sum = "h1:12VvqtR6Aowv3l/EQUlocDHW2Cp4G9WJVH7uyH8QFJE=",
    version = "v0.0.0-20160202185014-0b12d6b521d8",
)

go_repository(
    name = "com_github_json_iterator_go",
    importpath = "github.com/json-iterator/go",
    sum = "h1:QiWkFLKq0T7mpzwOTu6BzNDbfTE8OLrYhVKYMLF46Ok=",
    version = "v1.1.8",
)

go_repository(
    name = "com_github_jtolds_gls",
    importpath = "github.com/jtolds/gls",
    sum = "h1:xdiiI2gbIgH/gLH7ADydsJ1uDOEzR8yvV7C0MuV77Wo=",
    version = "v4.20.0+incompatible",
)

go_repository(
    name = "com_github_kisielk_errcheck",
    importpath = "github.com/kisielk/errcheck",
    sum = "h1:reN85Pxc5larApoH1keMBiu2GWtPqXQ1nc9gx+jOU+E=",
    version = "v1.2.0",
)

go_repository(
    name = "com_github_kisielk_gotool",
    importpath = "github.com/kisielk/gotool",
    sum = "h1:AV2c/EiW3KqPNT9ZKl07ehoAGi4C5/01Cfbblndcapg=",
    version = "v1.0.0",
)

go_repository(
    name = "com_github_kr_pretty",
    importpath = "github.com/kr/pretty",
    sum = "h1:L/CwN0zerZDmRFUapSPitk6f+Q3+0za1rQkzVuMiMFI=",
    version = "v0.1.0",
)

go_repository(
    name = "com_github_kr_pty",
    importpath = "github.com/kr/pty",
    sum = "h1:VkoXIwSboBpnk99O/KFauAEILuNHv5DVFKZMBN/gUgw=",
    version = "v1.1.1",
)

go_repository(
    name = "com_github_kr_text",
    importpath = "github.com/kr/text",
    sum = "h1:45sCR5RtlFHMR4UwH9sdQ5TC8v0qDQCHnXt+kaKSTVE=",
    version = "v0.1.0",
)

go_repository(
    name = "com_github_mailru_easyjson",
    importpath = "github.com/mailru/easyjson",
    sum = "h1:TpvdAwDAt1K4ANVOfcihouRdvP+MgAfDWwBuct4l6ZY=",
    version = "v0.0.0-20160728113105-d5b7844b561a",
)

go_repository(
    name = "com_github_matttproud_golang_protobuf_extensions",
    importpath = "github.com/matttproud/golang_protobuf_extensions",
    sum = "h1:YNOwxxSJzSUARoD9KRZLzM9Y858MNGCOACTvCW9TSAc=",
    version = "v1.0.0",
)

go_repository(
    name = "com_github_modern_go_concurrent",
    importpath = "github.com/modern-go/concurrent",
    sum = "h1:TRLaZ9cD/w8PVh93nsPXa1VrQ6jlwL5oN8l14QlcNfg=",
    version = "v0.0.0-20180306012644-bacd9c7ef1dd",
)

go_repository(
    name = "com_github_modern_go_reflect2",
    importpath = "github.com/modern-go/reflect2",
    sum = "h1:9f412s+6RmYXLWZSEzVVgPGK7C2PphHj5RJrvfx9AWI=",
    version = "v1.0.1",
)

go_repository(
    name = "com_github_munnerz_goautoneg",
    importpath = "github.com/munnerz/goautoneg",
    sum = "h1:7PxY7LVfSZm7PEeBTyK1rj1gABdCO2mbri6GKO1cMDs=",
    version = "v0.0.0-20120707110453-a547fc61f48d",
)

go_repository(
    name = "com_github_mxk_go_flowrate",
    importpath = "github.com/mxk/go-flowrate",
    sum = "h1:y5//uYreIhSUg3J1GEMiLbxo1LJaP8RfCpH6pymGZus=",
    version = "v0.0.0-20140419014527-cca7078d478f",
)

go_repository(
    name = "com_github_nytimes_gziphandler",
    importpath = "github.com/NYTimes/gziphandler",
    sum = "h1:lsxEuwrXEAokXB9qhlbKWPpo3KMLZQ5WB5WLQRW1uq0=",
    version = "v0.0.0-20170623195520-56545f4a5d46",
)

go_repository(
    name = "com_github_onsi_ginkgo",
    importpath = "github.com/onsi/ginkgo",
    sum = "h1:q/mM8GF/n0shIN8SaAZ0V+jnLPzen6WIVZdiwrRlMlo=",
    version = "v1.10.1",
)

go_repository(
    name = "com_github_onsi_gomega",
    importpath = "github.com/onsi/gomega",
    sum = "h1:XPnZz8VVBHjVsy1vzJmRwIcSwiUO+JFfrv/xGiigmME=",
    version = "v1.7.0",
)

go_repository(
    name = "com_github_pborman_uuid",
    importpath = "github.com/pborman/uuid",
    sum = "h1:MUyE44mTvnI5A0xrxIxaMqoWFzPfQvtE2IWUollMDMs=",
    version = "v0.0.0-20170612153648-e790cca94e6c",
)

go_repository(
    name = "com_github_pkg_errors",
    importpath = "github.com/pkg/errors",
    sum = "h1:WdK/asTD0HN+q6hsWO3/vpuAkAr+tw6aNJNDFFf0+qw=",
    version = "v0.8.0",
)

go_repository(
    name = "com_github_pmezard_go_difflib",
    importpath = "github.com/pmezard/go-difflib",
    sum = "h1:4DBwDE0NGyQoBHbLQYPwSUPoCMWR5BEzIk/f1lZbAQM=",
    version = "v1.0.0",
)

go_repository(
    name = "com_github_prometheus_client_golang",
    importpath = "github.com/prometheus/client_golang",
    sum = "h1:1921Yw9Gc3iSc4VQh3PIoOqgPCZS7G/4xQNVUp8Mda8=",
    version = "v0.8.0",
)

go_repository(
    name = "com_github_prometheus_client_model",
    importpath = "github.com/prometheus/client_model",
    sum = "h1:cLL6NowurKLMfCeQy4tIeph12XNQWgANCNvdyrOYKV4=",
    version = "v0.0.0-20171117100541-99fa1f4be8e5",
)

go_repository(
    name = "com_github_prometheus_common",
    importpath = "github.com/prometheus/common",
    sum = "h1:/MUKoJbk4oXV3uxkpfHVkmVfL+wzWW6dttaW26s07Gg=",
    version = "v0.0.0-20171117163051-2e54d0b93cba",
)

go_repository(
    name = "com_github_prometheus_procfs",
    importpath = "github.com/prometheus/procfs",
    sum = "h1:leRfx9kcgnSDkqAFhaaUcRqpAZgnFdwZkZcdRcea1h0=",
    version = "v0.0.0-20171017214025-a6e9df898b13",
)

go_repository(
    name = "com_github_puerkitobio_purell",
    importpath = "github.com/PuerkitoBio/purell",
    sum = "h1:0GoNN3taZV6QI81IXgCbxMyEaJDXMSIjArYBCYzVVvs=",
    version = "v1.0.0",
)

go_repository(
    name = "com_github_puerkitobio_urlesc",
    importpath = "github.com/PuerkitoBio/urlesc",
    sum = "h1:JCHLVE3B+kJde7bIEo5N4J+ZbLhp0J1Fs+ulyRws4gE=",
    version = "v0.0.0-20160726150825-5bd2802263f2",
)

go_repository(
    name = "com_github_robfig_cron",
    importpath = "github.com/robfig/cron",
    sum = "h1:70QTOM3skvDpJG6xz4AVSU2l91+lu1nAP5qvZU7NhRc=",
    version = "v1.0.1-0.20170309132418-df38d32658d8",
)

go_repository(
    name = "com_github_smartystreets_assertions",
    importpath = "github.com/smartystreets/assertions",
    sum = "h1:zE9ykElWQ6/NYmHa3jpm/yHnI4xSofP+UP6SpjHcSeM=",
    version = "v0.0.0-20180927180507-b2de0cb4f26d",
)

go_repository(
    name = "com_github_smartystreets_goconvey",
    importpath = "github.com/smartystreets/goconvey",
    sum = "h1:fv0U8FUIMPNf1L9lnHLvLhgicrIVChEkdzIKYqbNC9s=",
    version = "v1.6.4",
)

go_repository(
    name = "com_github_spf13_pflag",
    importpath = "github.com/spf13/pflag",
    sum = "h1:iy+VFUOCP1a+8yFto/drg2CJ5u0yRoB7fZw3DKv/JXA=",
    version = "v1.0.5",
)

go_repository(
    name = "com_github_stretchr_objx",
    importpath = "github.com/stretchr/objx",
    sum = "h1:4G4v2dO3VZwixGIRoQ5Lfboy6nUhCyYzaqnIAPPhYs4=",
    version = "v0.1.0",
)

go_repository(
    name = "com_github_stretchr_testify",
    importpath = "github.com/stretchr/testify",
    sum = "h1:2E4SXV/wtOkTonXsotYi4li6zVWxYlZuYNCXe9XRJyk=",
    version = "v1.4.0",
)

go_repository(
    name = "in_gopkg_check_v1",
    importpath = "gopkg.in/check.v1",
    sum = "h1:qIbj1fsPNlZgppZ+VLlY7N33q108Sa+fhmuc+sWQYwY=",
    version = "v1.0.0-20180628173108-788fd7840127",
)

go_repository(
    name = "in_gopkg_fsnotify_v1",
    importpath = "gopkg.in/fsnotify.v1",
    sum = "h1:xOHLXZwVvI9hhs+cLKq5+I5onOuwQLhQwiu63xxlHs4=",
    version = "v1.4.7",
)

go_repository(
    name = "in_gopkg_inf_v0",
    importpath = "gopkg.in/inf.v0",
    sum = "h1:73M5CoZyi3ZLMOyDlQh031Cx6N9NDJ2Vvfl76EDAgDc=",
    version = "v0.9.1",
)

go_repository(
    name = "in_gopkg_ini_v1",
    importpath = "gopkg.in/ini.v1",
    sum = "h1:GyboHr4UqMiLUybYjd22ZjQIKEJEpgtLXtuGbR21Oho=",
    version = "v1.51.1",
)

go_repository(
    name = "in_gopkg_tomb_v1",
    importpath = "gopkg.in/tomb.v1",
    sum = "h1:uRGJdciOHaEIrze2W8Q3AKkepLTh2hOroT7a+7czfdQ=",
    version = "v1.0.0-20141024135613-dd632973f1e7",
)

go_repository(
    name = "in_gopkg_yaml_v1",
    importpath = "gopkg.in/yaml.v1",
    sum = "h1:POO/ycCATvegFmVuPpQzZFJ+pGZeX22Ufu6fibxDVjU=",
    version = "v1.0.0-20140924161607-9f9df34309c0",
)

go_repository(
    name = "in_gopkg_yaml_v2",
    importpath = "gopkg.in/yaml.v2",
    sum = "h1:/eiJrUcujPVeJ3xlSWaiNi3uSVmDGBK1pDHUHAnao1I=",
    version = "v2.2.4",
)

go_repository(
    name = "io_k8s_api",
    importpath = "k8s.io/api",
    sum = "h1:5Z+PFfTIOXwKmOhQtZ0WBykbpGBBOuvbDx2YNAqIoYc=",
    version = "v0.0.0-20180308224125-73d903622b73",
)

go_repository(
    name = "io_k8s_apimachinery",
    importpath = "k8s.io/apimachinery",
    sum = "h1:xRBnuie9rXcPxUkDizUsGvPf1cnlZCFu210op7J7LJo=",
    version = "v0.17.0",
)

go_repository(
    name = "io_k8s_apiserver",
    importpath = "k8s.io/apiserver",
    sum = "h1:aJTDWEWWRYWfbW8Z6Mk//pNHFnHlHZnzkQAhwOoUtzI=",
    version = "v0.0.0-20180327025904-5ae41ac86efd",
)

go_repository(
    name = "io_k8s_client_go",
    importpath = "k8s.io/client-go",
    sum = "h1:kiH+Y6hn+pc78QS/mtBfMJAMIIaWevHi++JvOGEEQp4=",
    version = "v7.0.0+incompatible",
)

go_repository(
    name = "io_k8s_code_generator",
    importpath = "k8s.io/code-generator",
    sum = "h1:tpq+nvY9+2K8qRsOIUzJY8Mq7sNrfisNwQLc4/Xw76o=",
    version = "v0.0.0-20180228050103-7ead8f38b01c",
)

go_repository(
    name = "io_k8s_gengo",
    importpath = "k8s.io/gengo",
    sum = "h1:4s3/R4+OYYYUKptXPhZKjQ04WJ6EhQQVFdjOFvCazDk=",
    version = "v0.0.0-20190128074634-0689ccc1d7d6",
)

go_repository(
    name = "io_k8s_klog",
    importpath = "k8s.io/klog",
    sum = "h1:Pt+yjF5aB1xDSVbau4VsWe+dQNzA0qv1LlXdC2dF6Q8=",
    version = "v1.0.0",
)

go_repository(
    name = "io_k8s_kube_openapi",
    importpath = "k8s.io/kube-openapi",
    sum = "h1:UcxjrRMyNx/i/y8G7kPvLyy7rfbeuf1PYyBf973pgyU=",
    version = "v0.0.0-20191107075043-30be4d16710a",
)

go_repository(
    name = "io_k8s_sigs_structured_merge_diff",
    importpath = "sigs.k8s.io/structured-merge-diff",
    sum = "h1:4Z09Hglb792X0kfOBBJUPFEyvVfQWrYT/l8h5EKA6JQ=",
    version = "v0.0.0-20190525122527-15d366b2352e",
)

go_repository(
    name = "io_k8s_sigs_yaml",
    importpath = "sigs.k8s.io/yaml",
    sum = "h1:4A07+ZFc2wgJwo8YNlQpr1rVlgUDlxXHhPJciaPY5gs=",
    version = "v1.1.0",
)

go_repository(
    name = "io_k8s_utils",
    importpath = "k8s.io/utils",
    sum = "h1:0B4CPoGpLUgKc/u8nMxKFYl00WpWI6dhATdivCVNjP4=",
    version = "v0.0.0-20171219162953-0ab3217ce272",
)

go_repository(
    name = "org_golang_x_crypto",
    importpath = "golang.org/x/crypto",
    sum = "h1:VklqNMn3ovrHsnt90PveolxSbWFaJdECFbxSq0Mqo2M=",
    version = "v0.0.0-20190308221718-c2843e01d9a2",
)

go_repository(
    name = "org_golang_x_net",
    importpath = "golang.org/x/net",
    sum = "h1:rjwSpXsdiK0dV8/Naq3kAw9ymfAeJIyd0upUIElB+lI=",
    version = "v0.0.0-20191004110552-13f9640d40b9",
)

go_repository(
    name = "org_golang_x_sync",
    importpath = "golang.org/x/sync",
    sum = "h1:wMNYb4v58l5UBM7MYRLPG6ZhfOqbKu7X5eyFl8ZhKvA=",
    version = "v0.0.0-20180314180146-1d60e4601c6f",
)

go_repository(
    name = "org_golang_x_sys",
    importpath = "golang.org/x/sys",
    sum = "h1:ng0gs1AKnRRuEMZoTLLlbOd+C17zUDepwGQBb/n+JVg=",
    version = "v0.0.0-20190826190057-c7b8b68b1456",
)

go_repository(
    name = "org_golang_x_text",
    importpath = "golang.org/x/text",
    sum = "h1:tW2bmiBqwgJj/UpqtC8EpXEZVYOwU0yG4iWbprSVAcs=",
    version = "v0.3.2",
)

go_repository(
    name = "org_golang_x_time",
    importpath = "golang.org/x/time",
    sum = "h1:+DCIGbF/swA92ohVg0//6X2IVY3KZs6p9mix0ziNYJM=",
    version = "v0.0.0-20180412165947-fbb02b2291d2",
)

go_repository(
    name = "org_golang_x_tools",
    importpath = "golang.org/x/tools",
    sum = "h1:TFlARGu6Czu1z7q93HTxcP1P+/ZFC/IKythI5RzrnRg=",
    version = "v0.0.0-20190328211700-ab21143f2384",
)
