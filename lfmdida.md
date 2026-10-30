代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gwzachvws.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftawhlhq.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gnipngdve.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gjordzrnu.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/glajyxxnp.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gjachvweu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gctvdymvi.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwqxzqbl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcmanewf.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gxypbhbis.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhzdelyr.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpkvmhqi.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gepadbrjn.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkorrjtig.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gargvuefk.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcntknkt.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/goewxmrju.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gcmrhzxek.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gxebeqrqq.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhekewzk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gqkdweogd.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guuuvrglt.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gzpkbztez.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/ginpzhwhs.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/girjnkzap.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/glwavgrmx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlzocgnw.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gehlertjq.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/ghyoplaze.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gkihtvpok.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gqdnyndhs.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gvfdyynai.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gwdwhvdft.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gqohtnclr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmsyhoim.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gwdsilvih.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gegjamgkq.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwgosylx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrlgyfwh.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gswrjquxo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwklnwpe.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gyjegoxgl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gsdecacsu.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvvjiclj.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/ggphilmml.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsfcvjrm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/ghlzzrhgq.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnskllfzn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrolcqqf.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gomkkwjjf.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvcctwfy.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecxnoojx.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gntnbnabw.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gjaqmcfup.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/glvcyedmk.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwllebxyh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqumrrcpn.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gullqpxae.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gncznousk.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfmygubg.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/geonamait.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gfxgzyjgb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gypoznfao.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggndiehzg.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gugfxhflp.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrphkkuw.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/glvvmefgd.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxyvsetn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gwskyfvwo.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/godndokiq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgechvvb.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gzehwfnqy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzmallnf.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcbdrinu.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gycitwidn.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrggyusx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gmifookvx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gyrjdtamm.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gynkdruao.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gybcwtaeb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/glgjrhftw.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gakvpdshp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrxqoetw.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gmvdpdcdz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gtpslyyqr.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/grpyycltp.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcolnfrar.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gidrclfhk.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrncmpre.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/guyijetms.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebektytq.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gwhgimawc.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gzvwgyveo.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gesccbiqc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gxcoublll.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gndaeblfg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/giysixfxk.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhbskyvj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/ggkvvtzsl.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxmuqxiq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxdhrnre.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpjivwto.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzltgqes.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnjbgwfn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gqexjegqg.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmblaakju.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcsktwbi.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssxtphmi.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjgxlubk.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/grgmcckai.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gugpjvwzi.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/growyglan.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkffuxow.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gvipctlmp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/grtsmqycl.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gbozfwnhb.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvfxfudj.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjykhivi.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gantngeao.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gekgdxxor.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gciikjsim.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxmudovb.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmopubrqz.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gcducwwgg.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gibhamdga.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjvlzcrc.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gzzrrreyc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/giwmeqyjj.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdmdghik.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gmlwpjoex.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvjsqnku.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/guniebmfo.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gstydymrg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gexyzrcxd.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkgnavfo.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyyukfza.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuxhbffo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gkirncaoz.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gsycpdgdd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gaqcumnrm.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvumhumw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gtkmnlbwx.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhstsein.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbldnbjn.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwvzqjyl.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjianhoyr.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gcaacpwpv.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/guxnaxwgc.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gcracsbhk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gkkhtwoig.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gjfvmdouc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/goemylfrx.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgbtvvty.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gufncibbl.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcgoglfo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwehksnlz.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gndquieez.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gethgfpak.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gfaanbfhr.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcnkwqox.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfccczsk.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/goazqfknu.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfodhzcf.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/goguqtjsk.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grlokaykf.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/guwwaqhqw.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbfrprps.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gackeqozw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gugdtuerv.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskshzmlw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/geydqjech.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfoarkwhg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygmgolba.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gthtyrhwx.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gqfnwkmhv.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/goateognm.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtinfkpii.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gnabdmlvq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gpqfjwjwj.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gkfemmbuc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnvwkyfh.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvsnxhse.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gzvnjzlek.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gseuwveow.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmzlnpfe.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvarvkje.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwrjrqpc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gaijbxtya.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/gtzsppxth.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzttovfw.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvbzhcwv.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gaskzuyos.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gicdqlwbf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gobliuusb.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/grxjxqahx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/goqwopjgh.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gctnrjnxx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gstojcwct.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gfszftarn.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/groqfiant.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gskvkcgna.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/guoaeicfi.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gmfjgbodb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/gifrrhcnl.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrsirlhh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkaaukdj.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gkikatdyj.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfpwnwvc.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfcvvssu.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/glzfzjsdg.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqbwlpxm.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glguadxkn.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gydkmtjmh.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gvwfjhsiu.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gxzqepneo.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdabowhii.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/glqntlhcu.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/ginmlpyaq.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/garmgsabj.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnoxanvf.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/geascfxox.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gadtlsuqu.sHtML

[T20] Swift：数组操作
来源：http://m.share.fanxiaobao.xyz/Article/details/ghaerjeeb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/grlpjffwg.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqaddutyg.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnekpygw.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/geqtxzjlu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtxywvdv.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmhizkeu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyxqzdle.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gizztxoqi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gkwsnowdd.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtdfjrsl.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaykpxhte.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafsfaxko.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/grtmvdxmn.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gegagfkdf.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzcyfzfq.sHtML

[T28] Swift：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gevdpmaoh.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/ghzblipjo.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gzirserfl.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gocwqkslp.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/gtperzlza.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/glgqzutrv.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpgpbkvr.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gtatornyi.sHtML

[T32] Lua：局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/goiqbzjgq.sHtML

local a = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gfycrokhm.sHtML

[T33] Lua：表（数组）
来源：http://blog.fanxiaobao.xyz/Article/details/gdyhodjcw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/gzvwtzhlo.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/gkupevabm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fanxiaobao.xyz/Article/details/gkautpsot.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqysnxiy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gntrsvaxq.sHtML

[T36] Lua：函数
来源：http://blog.fanxiaobao.xyz/Article/details/ggpqvvqzv.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/gvjeogcko.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqplmvdc.sHtML

"a" .. "b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrapiwmp.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbywbovwc.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/gvxbpujkv.sHtML

[T39] Lua：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gkkdinqev.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmykbbgvj.sHtML

[T40] Lua：元表
来源：http://mobile.fanxiaobao.xyz/Article/details/glwbejoic.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fanxiaobao.xyz/Article/details/ghcgdsahk.sHtML

[T41] Perl：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gmctvdjne.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzjtiiki.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfursktfj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijdkncjj.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsukpjngc.sHtML

"值: $a"
来源：http://3g.fanxiaobao.xyz/Article/details/gfeulhwbd.sHtML

[T44] Perl：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkrbdibf.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewjtsjxd.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gqangimrx.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gipniaqon.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gckhmwqgg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gszekpiho.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fanxiaobao.xyz/Article/details/gboldjszs.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqddiiqtt.sHtML

[T48] Perl：正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpuvxset.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspnddyow.sHtML

[T49] Perl：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gztzyokmo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/giurukbpk.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/guhdncqfk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/gapovxnek.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskofoldz.sHtML

[T51] Scala：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/guaibtzbw.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/ggscvhbvn.sHtML

[T52] Scala：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgawtksr.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guauvjbze.sHtML

[T53] Scala：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gpwbtvuxd.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gubyjvjth.sHtML

[T54] Scala：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gutkllkje.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfykymjds.sHtML

[T55] Scala：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gremmtkyp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gyuyseaqw.sHtML

[T56] Scala：样例类
来源：http://www.share.fanxiaobao.xyz/Article/details/getphhqcc.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxrxxhis.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gilrkvwac.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxsslhuy.sHtML

[T58] Scala：函数定义
来源：http://baike.fanxiaobao.xyz/Article/details/gsxumjynw.sHtML


<!-- 参考信息 -->