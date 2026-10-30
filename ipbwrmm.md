代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.hesvh.cn/Article/details/gigufjwrz.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/gjmvabwcx.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/gngvsjmcb.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gmoorxfig.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.hesvh.cn/Article/details/gsemxueue.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/gijhhrddk.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gssfssaga.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gcnpynvie.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/gqbodlsrb.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gsgtqjcne.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gpiijyzhl.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gqbviyowp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/gisiutpbq.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gnzkjfbku.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/gfzkeqhxq.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/gkduocrrr.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gbjkpjhpd.sHtML

[R62] 找最占空间的文件
来源：http://3g.fehbvm.com/Article/details/gtkmqbnrs.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gvzryblhe.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/gzhgtbybq.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gmenykqte.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gbuvrmckn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/ghjfgjhqh.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/gzkvsdczo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/gvbqpcwgg.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gtmokomlu.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/geoecqram.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/gduqbdcoz.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gtensfcrs.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/ghhhazpid.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gotbanrff.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gpnpsfvey.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/gzoydrtaa.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/gznikheqj.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/ghepcvkun.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gnfacycwi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gojnxcuzd.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/gmvmznouh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gobovttrt.sHtML

[R73] 分割大日志
来源：http://baike.hesvh.cn/Article/details/gzyfywzrk.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gytuywdza.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gyjjguyla.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/gfehlqpuk.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gwvyotrtq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/gjlsmajuw.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gkevsdkcs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gyzkikewb.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/geofinrwe.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gmuqtfjye.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/gcnvcxypu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/gfchlpycg.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/gipnubmam.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/grpnommem.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/gfxfyjlho.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/ggrvopohs.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtkvijjlq.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/gkysdczvs.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmmyxwfur.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gobquppne.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/gsxrdwdpz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gogfgluvh.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gjdtxcfju.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gavhdsewm.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gpqaruixa.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/gthrpeesi.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/gzejkicfe.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gpnfldcxt.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gdblnoafb.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gejsvudlg.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/geebgayck.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gxsbptxlr.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/gejxkcctm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/gfqyqdxyc.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/guhzjvicw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gclrvwqut.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gmatjjpad.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/gdzvvjnlo.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gquebyxgw.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gxgeqkmsd.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gcriqyuco.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gjlmytszj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/gpurxnlrb.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gkmjdeggz.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gdseogclp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gyybfjizw.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gwcrhlirw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gorowqjbb.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gpbmjynrg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/gsnhmkoyl.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gjkwphiyb.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/ggpbkuyfc.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/gwbxtxnja.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/gblqsraqi.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/ggrvmdsdg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/gluqpxpyk.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gziejuuga.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gkhygzpul.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/gtlcjbrzv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gftrlwwql.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gbccrptwe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gnsscuhso.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/ggznwxghy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gurbhxnvf.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gfcmbkhlg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gdayehrma.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gmuvknjgf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/ggceesstp.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/giyrbyfgg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/gliimskdj.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/giupidfut.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/gffcupyzd.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gnnquuble.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gpdjvygjh.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gfpoqpnly.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gvewaolcy.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gwxwsmjih.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/glnplkfbo.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/gwreohucc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gpcigchny.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/goilrzmit.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/ghompzbux.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gaxzarpsq.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gvpspfgnl.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/gtdbuyriw.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/gzhgvyrva.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gosanpwzc.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gusaoloff.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/gfsnxerhu.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gzwkwhehf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/grycxpjyl.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/grkcfizec.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/gmyjkcbef.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gzenolzyv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gauvbavjt.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gzitegayi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gtiknkaed.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gzakcnkyz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gdhmnmcnq.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gjhhbxbyl.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gmikerqme.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/geywxovzf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gitdalfxk.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gtxhauuyx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gqtkafmiw.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/gqbkqdeqw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.zdbjq.cn/Article/details/gfzffwhbd.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/gjaazbtiz.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/gpztnujgg.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gjciokxfr.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/gyfnhwkdn.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gqdyyrbeh.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/gtttbzdez.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/ggqjxesmg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/grjwcbgqh.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/grtlsaglm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gnzpthazw.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gfwwxwdrz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gnndxddei.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/geknljcqq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/ganplqtea.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/gsraycnqr.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gnpcnrvir.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fehbvm.com/Article/details/gpfeyzbpb.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gykcizgum.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/grfxrnsyz.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gltdehxbg.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/gnmlubpob.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/gqfzjjifa.sHtML

int size() const noexcept { return n_; }
来源：http://baike.hesvh.cn/Article/details/gpaokfslj.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/gfvcwyvbs.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.zdbjq.cn/Article/details/gymrqkefk.sHtML

[S54] C++：异常处理
来源：http://read.share.hesvh.cn/Article/details/gzdodupxo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fehbvm.com/Article/details/gpumgflbv.sHtML

[S55] C++：结构化绑定
来源：http://m.share.zdbjq.cn/Article/details/gorapjutr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.hesvh.cn/Article/details/gjtjdcofa.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gakbrmgfy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/gllvgoifq.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/gbkdssmlt.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gomfoiqmy.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/glhebdojg.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/gkepqyhir.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gznjkbhcx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gatunlqvp.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/gkmdxuocd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/gqzazbxdm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/geokohyyf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gjjfbmuvt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/guvkeoyxz.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/guzjjffdk.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/ghpynejkt.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/giksthvle.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/gefrgnqiu.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gxknqldba.sHtML

"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gvyggoylm.sHtML

[T04] Kotlin：空安全
来源：http://baike.zdbjq.cn/Article/details/gzqgdfzcl.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gcsmunqid.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gazbqtbzq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/gcpobamxr.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/gifpmfsmt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gxaondgsl.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gwazvtwws.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/gtminljlv.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/gyqxdccum.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gtwndwttt.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/gbbpvjori.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/ghwxwigvd.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/grjfvhdzg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/gfnswaxrg.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/ggwgldbqt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/gfrphiqvp.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/grjzfkhlx.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gcdudtcla.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/ghyonmise.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/gzxvrcfse.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/gohpezcay.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gwvxdeibo.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/gedhxyvpe.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/grcryasjz.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gidxlhxeu.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gzobbkoiy.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/gctbthaoa.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/gjciuxfzi.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gukzpvfyu.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/gyinugbwx.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fehbvm.com/Article/details/gtqhjywpv.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gfnemhdsn.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/geggofejt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/gmdpgasci.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/grulsvqwa.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/gfgaflojd.sHtML

[T22] Swift：字典
来源：http://baike.fehbvm.com/Article/details/gynqmtfyo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/gobamwpgw.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/giqdpfoid.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.zdbjq.cn/Article/details/gkhcqgcjo.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/gbdwdloxg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fehbvm.com/Article/details/gmpfcfvyp.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/gdnhqgtxy.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gyfgmupys.sHtML

[T26] Swift：类与重写
来源：http://3g.hesvh.cn/Article/details/gkqvwtzfo.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/gsnqyhemh.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/gnszrqaiv.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/gkmelnzkq.sHtML

[T28] Swift：枚举
来源：http://blog.fehbvm.com/Article/details/gzcwgypfg.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/gjsbconon.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.hesvh.cn/Article/details/gxotzjthq.sHtML

guard let x = opt else { return }
来源：http://3g.zdbjq.cn/Article/details/gpjbntymp.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/gkqgwnzen.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gwsdctxxi.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gnkcctqga.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gyclxeabo.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/gkhkpwcuj.sHtML

local a = 1
来源：http://read.share.zdbjq.cn/Article/details/gtlgpwqqp.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gdrwdcfyi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fehbvm.com/Article/details/gbdgcypge.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gjaovnhgv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.hesvh.cn/Article/details/gmremvnmx.sHtML

[T35] Lua：字典表
来源：http://read.share.fehbvm.com/Article/details/ghjbucoph.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gxcftezns.sHtML

[T36] Lua：函数
来源：http://m.share.zdbjq.cn/Article/details/gnpugfjzf.sHtML

function add(a, b) return a + b end
来源：http://read.share.zdbjq.cn/Article/details/gohnyfqwm.sHtML

[T37] Lua：字符串拼接
来源：http://wap.hesvh.cn/Article/details/gheqdjaob.sHtML

"a" .. "b"
来源：http://www.m.share.fehbvm.com/Article/details/gcxdsoyui.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/gejtkmkpw.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/gyuuvkmnb.sHtML

[T39] Lua：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gxbnhtzjq.sHtML

string.find(s, "%d+")
来源：http://mobile.hesvh.cn/Article/details/gomnizfti.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/ggxssgckl.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/gpzhjjfyf.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gxkjtvmhl.sHtML

print "Hello\n";
来源：http://baike.hesvh.cn/Article/details/gyrlsdamc.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gkqizoptr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/geshsdxgj.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gwtjiexka.sHtML

"值: $a"
来源：http://wap.fehbvm.com/Article/details/glgbeyrfw.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/gbsfiljor.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpkqadssq.sHtML

[T45] Perl：数组遍历
来源：http://read.share.hesvh.cn/Article/details/gjloaowhh.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.hesvh.cn/Article/details/gsdjovxuh.sHtML

[T46] Perl：哈希操作
来源：http://read.share.zdbjq.cn/Article/details/gvtjnbkas.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/gfzpoylcr.sHtML

[T47] Perl：正则捕获
来源：http://read.share.zdbjq.cn/Article/details/gxrhvymwn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fehbvm.com/Article/details/gzpwvtmkl.sHtML

[T48] Perl：正则替换
来源：http://www.share.zdbjq.cn/Article/details/gfqhmicvz.sHtML

$s =~ s/old/new/g;
来源：http://baike.fehbvm.com/Article/details/gthzjaznm.sHtML

[T49] Perl：函数
来源：http://m.share.fehbvm.com/Article/details/gvzdmwipl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gajvsqnhp.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/giylwkydq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.zdbjq.cn/Article/details/gyyofeybr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.hesvh.cn/Article/details/grgccgpse.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gqjxslzlo.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/grsdzhttl.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gbtyienlx.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gsxwsqkdv.sHtML

[T53] Scala：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gdgqjhrxp.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/geyxqbnpo.sHtML

[T54] Scala：集合映射
来源：http://blog.fehbvm.com/Article/details/gconbyobm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fehbvm.com/Article/details/gzrcqavkf.sHtML

[T55] Scala：集合过滤
来源：http://blog.hesvh.cn/Article/details/gmphkknoj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fehbvm.com/Article/details/gicofjpyx.sHtML

[T56] Scala：样例类
来源：http://wap.zdbjq.cn/Article/details/gwivheffz.sHtML


<!-- 参考信息 -->