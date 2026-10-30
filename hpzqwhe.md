代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gxwaasrao.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/glkuhopqk.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/gbszptnhx.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/gafbfblcz.sHtML

ssh user@host 'uptime'
来源：http://baike.fehbvm.com/Article/details/gxbgquvjq.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/glmgcswgy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/gcfqeizmg.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gwgcslbmx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/grhmbnlmf.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gxqzwapkg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/glkjcdaze.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/gguvvsagy.sHtML

df -h;  du -sh *
来源：http://www.m.share.fehbvm.com/Article/details/gqhhxykwp.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/gketysxbj.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/gtafyorbi.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/gmkymrrtk.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/gniknjuzj.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gxfyiibut.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gyqjirpbz.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/gqctnwqsj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gemjsjojy.sHtML

[R66] 定时任务
来源：http://baike.fehbvm.com/Article/details/glsiphcyd.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/gzutgslec.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gdcstghek.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gvzrhgzjz.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gwojznjfg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/gjvxwozjg.sHtML

[R69] 生成随机密码
来源：http://www.share.fehbvm.com/Article/details/gpmenwmxn.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/gcmhelyaa.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gzfesztuf.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/gtquaveos.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/glvtsybdz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/grfvobcgo.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gvsyurxso.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gjklftdfa.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/gmeuzscmv.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gigzyjtsp.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/gdpvpfuez.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/ggphbyhjq.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gjbgksihn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gjwxlifrb.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/ghmihpcfp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gyvxodqan.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/gyqgnpsqm.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gsrohgshu.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gycfdtogq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gkbkkiusp.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/gybrtzrvr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gjoeiztlv.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gvcgzzyjk.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/guqokdujr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gckzjaaet.sHtML

S. C / C++ 专题
来源：http://wap.fehbvm.com/Article/details/gvgiosfhb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtotcgokw.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gfectxgzq.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/grrmxbayp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/gwsvxubzw.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/gcmgnmngu.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/ggwjjvsir.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gosdepmht.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/goxvuvkco.sHtML

[S04] C：字符串复制
来源：http://mobile.fehbvm.com/Article/details/gbfbxrsid.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gmeoidmhp.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gptceejik.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gjusostyq.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gzepuhsrp.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/gzaagbleg.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/gqtwinzat.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.hesvh.cn/Article/details/ghtpzralo.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gvwupgfgv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/gxleqabmy.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gsjsoysri.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gjipyzwyf.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/ghepgnbhm.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gzuydfnma.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gybhtvcum.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/gbykjtevh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/ghhnfezpl.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gcohsurgn.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/gudvlsnee.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gkijxcqlf.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gbmufqxak.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/gmvnsaivs.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/gdzpkavsb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/gvaoluhub.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gwhntjmxm.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/gcsisabqw.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gtkipbial.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gchcuvyak.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gtdinecju.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/ghqfgadsb.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/ggtuvoiyu.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gepngaamd.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gdqhmxdxx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gfapimugk.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/gvebtaaxo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gjqvzvgth.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/gtscvjftr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gzggxhmuh.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gejejsdrh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gpauyhrjd.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gvprybjua.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/glzupuspd.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gytobsvrh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/grzpnyuvf.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gvcoiemkb.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gsrhwsotk.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/geopplpkt.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/gvenvzcst.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gjgcjsgqr.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gvypxeptk.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/gkywaferz.sHtML

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/gsnyssdad.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/glqpzbjpn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gbrwcnoxy.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/grsckhqnx.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gtkqndybj.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gabasktae.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/gyzjiyciv.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gzjwcoenk.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gokmbezgd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gfvymxrhd.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/guxawtnsc.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/gaaufefgj.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/gmdohzvoy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/gefdrxfda.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/gisumtikg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gfslblovw.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gsdlyhtvn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gtohedkik.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gwopwwwjz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gyuuxdkcw.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gnmbfeybk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/gjrxpevuu.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gofxvtovb.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gjjgoedwz.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gvnbvryqp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/golycvemj.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gzbvhhozj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gqvsyixjd.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/gpfzslnuw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gehrpzodg.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/grxwtkulk.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gxaouvqlb.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gatcxkmjp.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gqtfvnfeq.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/ghwhvdrxy.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/gkdxeifri.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/gviqtfwyk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gkwpmdqaz.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/gdebjghab.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gpugjtsez.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/glweahrri.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gtsjauukf.sHtML

[S48] C++：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gjumsdjdr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/gwliqudbz.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/grpcozgnl.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/gcngbkkwu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gnjtozaun.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/gzwzbnpbx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/gpbqdoinr.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/ggceuypwd.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/gioshyevi.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gqnicflhj.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gkyxdievy.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gcduqcsec.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/ggdszjpvm.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/ggezwagpu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/gzxsnkggp.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/gjoolhirn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/glvvkmpex.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/gkeeleqih.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/goqripkhw.sHtML

[S57] C++：编译期常量
来源：http://blog.hesvh.cn/Article/details/gjmnxyoyi.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gcudbliru.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gfojdhqpg.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gzvijatdq.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/ggzfqkqvq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/gezneeqjb.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gamqackgt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gnzzeqpud.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwundwcnr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gedzgeopv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnlniqoru.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gtrkrntsc.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gicadqzhn.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gwtfcfzxu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.zdbjq.cn/Article/details/gaecbvgru.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gwfjtuitt.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gizynzwsq.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/gexqltemp.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/gjcvguytw.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/gzwoouwtg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/ghostyyys.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gxuccdwlm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gpgqlxczj.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gzmhyoxzl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/ggnpcxygo.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/gfrdygvxr.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gjykwfzhg.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/gitiqqzya.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gfdhfkjpt.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/gtqzvqhsy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/gsxqiwcdu.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gxpjnnhrh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/gpyushmeo.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gtqkqghuk.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/gvinieqrz.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/goieitfly.sHtML

val m = mapOf("a" to 1)
来源：http://baike.hesvh.cn/Article/details/glkslbzls.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gsikzzcxj.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gtemfioai.sHtML

[T15] Kotlin：接口
来源：http://m.share.hesvh.cn/Article/details/gspduhezd.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/gkcrgavxu.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gnasidytz.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/glfgditnj.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/gtgnneych.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gzxezykqt.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gvpgidalg.sHtML

"值: \(b)"
来源：http://read.share.hesvh.cn/Article/details/gzjelbyyu.sHtML

[T19] Swift：可选绑定
来源：http://3g.hesvh.cn/Article/details/govjjgufv.sHtML

if let n = opt { print(n) }
来源：http://mobile.zdbjq.cn/Article/details/gaaogxqlb.sHtML

[T20] Swift：数组操作
来源：http://www.blog.hesvh.cn/Article/details/gvqihxrfn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/gcpravvco.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/geqgptqvh.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/gappdnopt.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/gntomdwge.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gtupiscmv.sHtML

[T23] Swift：函数
来源：http://3g.zdbjq.cn/Article/details/gvzmizesw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gvfguugmh.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/gvcrcajfw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/gvgbmwudx.sHtML

[T25] Swift：结构体
来源：http://3g.zdbjq.cn/Article/details/ghozdfbnz.sHtML

struct P { var x: Int }
来源：http://3g.zdbjq.cn/Article/details/glfsamfil.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/gmlpowqqh.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/gtwxjrjce.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/gelgczrmj.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/gyyzvtvaa.sHtML

[T28] Swift：枚举
来源：http://wap.hesvh.cn/Article/details/grojsclvp.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/gxovfrufp.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/gsjuyciwz.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/gcsphmobb.sHtML

[T30] Swift：协议
来源：http://www.share.fehbvm.com/Article/details/gxtbxaphz.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.zdbjq.cn/Article/details/gdpjqcpwg.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/gyxpytvxx.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gxpxcddwn.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/grwdymvho.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gnusdkavu.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.hesvh.cn/Article/details/ggpwkzvty.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/grvqkormm.sHtML

[T34] Lua：遍历表
来源：http://blog.fehbvm.com/Article/details/gnxyihrlh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/ggagavpud.sHtML

[T35] Lua：字典表
来源：http://baike.fehbvm.com/Article/details/gklsgyibb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/gaekcgdxv.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/ggpskqurg.sHtML

function add(a, b) return a + b end
来源：http://read.share.zdbjq.cn/Article/details/gbwxkaqbi.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gkwljrxbl.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/gbgbwdtqr.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/grzkujecs.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/gofmcchpz.sHtML

[T39] Lua：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gxdukrmaa.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/gvzghinig.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/gykemefjq.sHtML

setmetatable({}, { __index = base })
来源：http://baike.hesvh.cn/Article/details/gdfwixdqk.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/glnwasvjp.sHtML

print "Hello\n";
来源：http://m.share.zdbjq.cn/Article/details/ggosalwly.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/gfwjwkaau.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fehbvm.com/Article/details/ggzdpibfr.sHtML

[T43] Perl：字符串插值
来源：http://blog.fehbvm.com/Article/details/gwzcttquz.sHtML

"值: $a"
来源：http://www.m.share.fehbvm.com/Article/details/gghrwlaay.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/grhhdtnmh.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.hesvh.cn/Article/details/ggccmmqpu.sHtML

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/gjluulnlh.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/griedzkrb.sHtML

[T46] Perl：哈希操作
来源：http://www.share.hesvh.cn/Article/details/giratxiyt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fehbvm.com/Article/details/gctrdojke.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/gntnyndrq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/gxlmlpwxl.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/gzzcelqgk.sHtML

$s =~ s/old/new/g;
来源：http://www.share.hesvh.cn/Article/details/gvizirdlu.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/gkioltdcd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gbvtrehkq.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/ggvmwyqbr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/gdnctnddv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fehbvm.com/Article/details/gnuvezzkg.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gapdwimjz.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gkfshexgq.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/gkbafvubt.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/gydoimsnp.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gngtzbyby.sHtML

s"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gpbnfveph.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gtzoibqzm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.hesvh.cn/Article/details/gekwaqvgr.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/gqwcnhhmk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.hesvh.cn/Article/details/gvrdexboj.sHtML

[T56] Scala：样例类
来源：http://3g.zdbjq.cn/Article/details/gykpcpueh.sHtML

case class User(name: String, age: Int)
来源：http://3g.fehbvm.com/Article/details/gpwhvosqc.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gzicfhbpm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/goygyweaj.sHtML

[T58] Scala：函数定义
来源：http://read.share.fehbvm.com/Article/details/gxnqyvmdp.sHtML


<!-- 参考信息 -->