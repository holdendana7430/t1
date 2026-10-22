代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2twqlwhmj.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2bgthqgam.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2vcqwodtw.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2argyossd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2cohgbyvr.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2frtlslqx.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ixrmuhsk.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2hpuibvap.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2rprruiso.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2gmieatvv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2lweyaxwd.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2bejpmewt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2uhpwnjcj.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wwjtbuyk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2iucmmqkj.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2foicursi.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2gfmucour.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2mlirtzui.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2zvpvplbu.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2qyvjvoog.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2kusvbsps.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ftahqvdn.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2gvhrykdu.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2ftbylzrr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2abddzual.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2hxhtnzkj.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2euerpmua.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2znztjkli.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2cictfjjq.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2imapgjfj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ckkuuyxq.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2xsxacgdb.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2phaeaxti.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2zyauikam.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2adneedde.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jtixgcuv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2bkqgfaxx.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2vmxyzkgi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2hgrthrab.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2povagvbw.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2kxpvpmjl.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2fusgsuod.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2sobcdgqf.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ydsdapen.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2khpmbdpm.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2nhpcxhba.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2usfshirh.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2qpmeuagq.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2icrcisjf.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2ttuzyopp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2hxtwimct.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2zaouiejf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2dmudmabm.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2goizpoqs.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2zpsnmxjy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mdhomwhf.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2rpndvjda.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2txeggdmm.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cykwivry.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2gegnkckz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2nkwxhgxb.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2mnbeomha.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2voiucwgu.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2ikbayfzc.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2gsxkbjpu.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2efdiecrl.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2tkhlgsjl.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2jkevjrsj.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rnajuqxv.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2uxuzdxqs.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2prtveoza.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2znbsjrbg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2kpzkizse.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2rizlonox.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ucevouav.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2zcomuqra.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2bfofsbyr.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2abeydlcp.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2woisxmoj.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lirhtftg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2hsnobfxe.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ehjfxgwj.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ithepciv.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2qibsdmxs.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2uwqvegup.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2yjnmmksx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2fhdsuqzo.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2ncdiglxi.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2zshofidv.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2runfdzbd.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2znuexpqf.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2roxzmmgd.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2atbvtjev.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2malsnomu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2rmlalxki.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2uwepotgw.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2mckumsfa.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2zkttegyw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jcfulbzg.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2fktjtnlk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2wjxkjpsy.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2qtsxrzba.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2tcfhgsjr.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2olkzwone.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2xgghgonh.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2sswurcze.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2fosqcumy.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2szimlnct.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2yyllenqk.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2oomlehpf.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2xrmtanhv.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2ownjrwka.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2cztomzew.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2ikjgnvgw.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vimbxapr.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2cywtwnho.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2xkgvbmnj.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2fafmdjbo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2piggujgz.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2kpzshoey.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2zyptwjlf.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2pgphsdfx.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2vsjpmobc.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2licpujcm.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2dymmbsap.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2pestcqtz.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bffkuddw.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2fhzozqwy.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2vifcajsx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jxbvzoas.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2glhsdetv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2diyrdkdf.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2eecjgjoi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2izxjxufa.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2zygvguzs.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tnvcdjrz.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2qvxuejsf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vlcfugrz.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2fyjcdejl.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2zkbfanqv.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2nexzlceg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2dledsulc.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2pdqdxpxr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2uomdmmpi.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2bbnsnzmd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2vjystkfp.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2xvvltocv.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2txjwyuqj.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2xlghltfh.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2jseyyucs.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2fvzdtsif.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2lgpdrtor.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2okliyjqo.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2usuuczoq.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2xakvrojm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2cchllfzi.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ewqczbhj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2raujolhi.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2bdzhwrmq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2fhldvovr.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2zgiaxjwh.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2pgqphztp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2guqeprcy.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2iueicwfy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2isvrbzmv.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2evsacwux.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2enelppfx.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2hgxyfkka.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2mhkxfhjr.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2hdjtkcvv.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2cpxqxouq.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2oombyiqh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2jumnimtk.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2cblqkzek.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vmhsifac.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2vdvvoaxr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwskgxqo.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2oypwvvsi.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2gwdinont.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2rpqdbxui.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2jkgvkdbe.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2vzoywgay.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2ovguyzuj.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2ulgmqtau.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2atwbomxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2imdoekzx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2qccnebwr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xnzezpvt.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ngglafba.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nlbvrsyo.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2ltudfzhu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2rrsepahl.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ziedjrre.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2bfokfnkd.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2pjcfcemk.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2jcmezdsx.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hkuduvyo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2flvsznxv.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2wulvhpdg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yorhqguk.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kdrlsfys.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2fkbofpvs.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2xduljoqt.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2rorfenwj.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2vmctkthe.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2jnvtjngm.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2buoiciku.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2qhhpwvsx.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2szyowxik.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2ottbitgy.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2mgnylwod.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jlimmyjb.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2fluizlkv.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2akbkkmdr.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2fsrarltd.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2cndbnhpj.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2ezsjnbqq.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ijxrvemv.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pfctmgzj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vlpsxgob.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2dkemelie.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2wmsehofc.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2pxbbfowv.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2hqqoiupi.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2hqeajlgp.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2bewyppgl.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2qxjevbgq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2tzzbyava.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kytjfhab.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2hjbblkdt.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2hziugsdz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2flxlqqlb.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ztxiqyrh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2slprogry.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2qfgesqkf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rsqyujvt.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2kzlqxdlw.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2oaeabnlh.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2ajbkurgd.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2qwgyanie.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2wziildjy.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2rzowujag.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2wppxntxw.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2sqwwiuiq.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2bqkhiwfa.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2ecdijfqu.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2wsxrahmx.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2wqcivekh.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yqunfetk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2cscjwhjr.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2fqsbmqrv.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2mggwyqnf.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2lbhxfojh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2iumfhvna.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2ztbnvwhe.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2lqueoqxy.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2evkjfpkf.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2omxksuxt.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2gwslmaww.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2abyvdogp.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ftpipvfj.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2mmfppchm.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2sxzbxneu.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2ppizpwas.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2zcawarqm.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2ltimgfyj.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2bgtxwrxd.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2jhiozcjm.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wwmtvnqq.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2weucflwp.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2byjwpkzr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2itiyhsft.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rwvqjqyl.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2mnctbqne.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2rdskoldg.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2npxywala.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2njvvvfio.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2utsmvaip.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2etwajyhq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rehjevej.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2amrmlqqu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2bvdjhnyq.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2wwfoghtt.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2zbvdgdbu.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2ucceitfj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwbhjnxt.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ychzaxyb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2empjunil.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnuodydo.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gyxtuelx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ocddyzll.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2skxcwskd.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jtfwgulq.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gcvpjjoa.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ywuhccsq.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2sxrxeqhr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2rhzwpawh.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wifxxcpk.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lzxwyfcx.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2njbzyzxk.html


<!-- 参考信息 -->