代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcgpokrx.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrupafpy.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjrftcwm.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdafgmzeg.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpdfqnwo.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gctmgbpbr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gyooupvjl.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/ggmowtjfu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gzencylzx.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjqidnhm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gnusbjcbe.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvemvhsc.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gcckwjany.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gpfbhzgms.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guadlrxao.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gewgkcfjx.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkqqzrqi.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/ggxkvxjgb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmkwywtz.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiziuhzv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/goikahopp.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gcizfzjfl.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/guucezhfu.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gsphjnfoy.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmtehtxy.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gtokudyhd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqfyseue.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gyenfcjrv.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gzinumdrd.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkberddk.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gdakzfrla.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzdxfozf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/glovbuhps.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gyjdlpncg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcqepzky.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcfpwnvz.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmgknjfw.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gjygmcpnl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gkohkecjs.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfgrtizn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/githwsygy.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/guktsjixg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvhxcooa.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/grjhesxai.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwjhwfjl.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gayqexikj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gqznlopnt.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcdjbksc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gtahbrhog.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/ghftyfnjm.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gouznkfgs.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyxiuhhx.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/guohujzvu.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gbusxrdid.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotoshjbx.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwltpngp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gacdeznvx.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gbceufixy.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gyjqhliuu.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gjgjxwepu.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzskxydfg.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/ggobbfrdz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gsqnhxdhf.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gcpfiurcq.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geytllzhe.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gceqyzgba.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuxfllro.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbnftvbu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/guttlbjyi.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gkkjnokey.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfcciokv.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/ggpwkhopk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/ghfkjkqse.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gekgxpeic.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdrbnzmd.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghuauqupn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxonwpzf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmaqxozpb.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzimmuxvw.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/geeonyqyg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjvsvted.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gnrdpfnru.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogzksolx.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gzujztnmz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/giknydbvt.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnyhdjka.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gjgqviqkc.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gysqwphjc.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/grisswynq.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnymticnu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrlojeuk.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gctmpbwfd.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gjknmkbbg.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gzcdhnyan.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gomjwwovj.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gtdposcur.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcqdhunc.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqnhefwd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlwutsvn.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/ghiduruzz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gdaxlwvhb.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwvvafiq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gcpisdmzz.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/grrnvobyb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gamfpwjyh.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/goizjpyou.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gpkrkesik.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gjuccmsaj.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgxuthjc.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gbemfmfmy.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gftjeuvcr.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/ghcavbxsk.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gncqeycpx.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gutalxqbf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gqrnkmaew.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gkcfcnfhk.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gcevhjvlo.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/giehabmoz.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gvexmqlop.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gfodbfnfj.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gybzetixw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grevfbuwg.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbeadxfd.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytxefyir.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/guyvpicgt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghagmkymw.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjytlxoet.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfgkljaj.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gffzzejou.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gzrnublao.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gkggkyupb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gkafwutdx.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gucxzytxr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gaytpsqhc.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gzniqyjjy.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/ghtsczaxq.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gjueptvuo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwyzytacn.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvdrvgxt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtspetyrf.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjuksgxo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqslupsl.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gmmbnfsmq.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/guvdtdnft.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkwhiyci.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gdycnhmew.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gfxqleydz.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gazkhhvjq.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxwnkbbq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gnvbazduw.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhvesbsw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpvqcoup.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknkqmytl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gluvoqhkj.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsdrnwyr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpunwgfjm.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gugxxieae.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gulzulzsn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gyccszzcz.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrzltrgl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfdpsvgv.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwnypgoi.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gurkcfjcm.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gmkbhpovd.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrlczlyk.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gvytrpkcn.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrojmhvd.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gnhdvwtcr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/goixmbjkk.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/ginkgoofd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxygqvnqi.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/grjtxyfsn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gadbusnkl.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxganxrz.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkluuqama.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gbsqoyyvf.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdggsktob.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpuaxcav.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gcagjxpem.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gvjsjmcuh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqaxxcqr.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gesokhxbs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjmcvgcv.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gooxxzvgb.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmfggisa.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgzxitcc.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gaznqqhhj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gesnfzymy.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/grzavkrnc.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwgwejve.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvzjribq.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxttivsl.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/golbovhuo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxvbxygu.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gdaidfqek.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gekmpsmbl.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakobekth.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geckeguhp.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gultqirbv.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gdvijhaoe.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gdzaraimk.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqzquniz.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gakqojmxw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/geqpduxyq.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrrdvosc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gclqpanro.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtnibfsk.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzktfrun.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/giwkzjmyz.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gdwiysnqp.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gwqqgoofq.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/glzoynkyp.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/gmqhrgyxs.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhbvtsuc.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gevmabkaa.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvftsbjow.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/gljuxrudn.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gvbdthjkr.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gplchjrzx.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlgrvcek.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gbywndzph.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/guqyfobqw.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhsubbia.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gujysglmt.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzlehrxs.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclixmmew.sHtML

[T22] Swift：字典
来源：http://baike.fanxiaobao.xyz/Article/details/gssbcfogu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gxqhtkgeq.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzbwprtl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjhglioh.sHtML

[T24] Swift：闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/gccasrpyo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gsgpxiplu.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/guchaqthg.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gninhoyzc.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/gglbclwah.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gmovqipwy.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gecjfqyna.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gloaelznl.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gyzwuahdi.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqczowmgx.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/govppgnxq.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gqzfuipcs.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvupszoi.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjowmxal.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gvaijruev.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gtytyeehi.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/giujyfpcu.sHtML

local a = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/greyeqivm.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fanxiaobao.xyz/Article/details/gslektmpr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fanxiaobao.xyz/Article/details/gknwmdhmz.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/gwstdxfqw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusclklqm.sHtML

[T35] Lua：字典表
来源：http://mobile.fanxiaobao.xyz/Article/details/gszdqgtdx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsdnangd.sHtML

[T36] Lua：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmxlwvym.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtmgylwk.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcgguajc.sHtML

"a" .. "b"
来源：http://wap.fanxiaobao.xyz/Article/details/gzzqdprut.sHtML

[T38] Lua：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcclhdlh.sHtML

if x > 0 then print("正") end
来源：http://read.share.fanxiaobao.xyz/Article/details/gewjiuivt.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/glbacwjzi.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjvslwyw.sHtML

[T40] Lua：元表
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwicqbon.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/gmqazqofo.sHtML

[T41] Perl：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgjprcqe.sHtML

print "Hello\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gthjdgmzz.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gedrxenig.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfwrwpif.sHtML

[T43] Perl：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gpucbgsoy.sHtML

"值: $a"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahenyqdz.sHtML

[T44] Perl：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsqhekgh.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzzrbacfn.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gkgjpxgxy.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmqeuwrft.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gatwxrbam.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzbuemspi.sHtML

[T47] Perl：正则捕获
来源：http://blog.fanxiaobao.xyz/Article/details/gvwiwgrzq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golptxelg.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gnxgolbkm.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fanxiaobao.xyz/Article/details/glsdutymg.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gzrevjvoq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gyfyaftcs.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/ggluzcabm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fanxiaobao.xyz/Article/details/gcjzslohi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gizupudqj.sHtML

[T51] Scala：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/goshkdnss.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gujnchqos.sHtML

[T52] Scala：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gawynnarv.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbjandep.sHtML

[T53] Scala：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gpfvrujxv.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/ghnfreeek.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvxkcsma.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnefwsgy.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gvudpkgfh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gipvpcrle.sHtML

[T56] Scala：样例类
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmidsfgw.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glulyacig.sHtML

[T57] Scala：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gadswowax.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fanxiaobao.xyz/Article/details/ghqzhlwro.sHtML

[T58] Scala：函数定义
来源：http://www.share.fanxiaobao.xyz/Article/details/goicjjqzn.sHtML


<!-- 参考信息 -->