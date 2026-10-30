代发 wailian999

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/gpziycpgu.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gaadxxaje.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gehmuhupz.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/gwnlnwxte.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gxgaqznst.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gsqehyyxy.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gaozqurfj.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gpnsoypsa.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.zdbjq.cn/Article/details/gacmsozss.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/glbytgooe.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gmraouaxh.sHtML

[R73] 分割大日志
来源：http://www.blog.fehbvm.com/Article/details/ggoinvybw.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/gvpdazmei.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gusnbrdmd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/guljhbfbl.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/gqvvihdxw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gczxgxfyo.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/gnpeuwpbj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gyzaphktz.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gvqsftyhp.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/gbbyszzkz.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gpeeczwjz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/gwpvxsfxa.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gbpqxgcso.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gncvckndn.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/grkaigtqr.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/gljxflacm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gndermakr.sHtML

S. C / C++ 专题
来源：http://www.blog.fehbvm.com/Article/details/gzkimpxjx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqsfmrgjs.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gbameddhh.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/gpzmttuup.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.hesvh.cn/Article/details/ghkjhmjsa.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/gpnhdjkgn.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gnosyqdpp.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/ggwjoubdt.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gguznhvcp.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gcujdgwkn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/gkkxahfzn.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/glkwzezor.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gcqjdopbd.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gntbnvszs.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gsudemcmx.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gvekzwfrh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.zdbjq.cn/Article/details/gnyochhir.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/gydtgpmeh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/gekpbcfoc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/goquovfty.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gszmuuswa.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/gkbptyaql.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gqjrbtaed.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gsushrehv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/gwiorfgzb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gxsaeeika.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gaqbvwifm.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/ghkewqtjz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gwzoqekpj.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gwmewidsv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gzducduco.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/glvmqhunp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/goaugnlqz.sHtML

[S15] C：类型转换
来源：http://wap.zdbjq.cn/Article/details/gbyvfhqqi.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gtgbchqsn.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/gwxmwsioz.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/gdcjzbzmm.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gaodyllmj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gwszqkgqs.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/ggplbdqsk.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/ggwbyhlhw.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/gkpdaeqki.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/glnlfauur.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/ghcyafzxs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gqauuoxrv.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/gjmxulecj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gfiugfiba.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gyhjbbudi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gfrqomzmo.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gsaktkpvf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gwyxkgyhr.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/gwwjekhvc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gibunfjdq.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gbrssddit.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/grtkknlia.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/gymwuqzxi.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/gqrxnwqlt.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gbirghlrk.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/grtjtgfpl.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/gauyuvycf.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gtaserezb.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/gudduyfer.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/gdgifjsvk.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gyxngbzsj.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/gagfdflsj.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gynioassk.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gslzwlpty.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gmcfgnowv.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gftkgghrp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gtmobsvwr.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gjyextfwm.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gsczhbzvn.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gcdcsjutq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gmfacvenm.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/goeqdrmin.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/gluofptpe.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gwbivtjrx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gambolpta.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/gzohekdih.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/giaedvnjy.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/gqmxziygc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/ghzztmjdt.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/gjqlufsbk.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/grrakiltg.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gvkmjdhff.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/gbeatviik.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/ghnmszcag.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gdsldtswl.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/grosxigwj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/gfktfbncx.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/grmjjqdjj.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gwgbfwcqf.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/goqcebqkd.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fehbvm.com/Article/details/gmxqbjgrn.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/glhztgbpe.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/giodoshcu.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gbvtullqa.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/glgchgqer.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/guoqsnztf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/gbcbbcjjn.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gjhcmxcpd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/gfkpfpmvm.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gemvkajbx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/griwzijbh.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/gnbxdqzpc.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/gjzjfcyec.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gcftxkocu.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/ghkgdzdfk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gfpldxjgb.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gfwmrkfjq.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/gvvkczitx.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/gjueayavo.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/gcbhfzgca.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/gywdheqtn.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/govkotulk.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gmdrpwrvv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gmlwwdzhu.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/gmfxkdbbn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gjnsbzesa.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/gvdhwmphn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gvoljmmvw.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gerpaxjjx.sHtML

constexpr int N = 10;
来源：http://m.share.fehbvm.com/Article/details/guubqzxlz.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gmvifgrys.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gohyruyxr.sHtML

[S59] C++：静态断言
来源：http://mobile.hesvh.cn/Article/details/growxlrux.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/gcvmwjpyj.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/ghkgtgveg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gdvansedb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghlctkyod.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/grecjftnl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glkfirffa.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gudsrxhae.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gwekbxpon.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/ggpptpmam.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gfokkyhdr.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fehbvm.com/Article/details/gacmqouuy.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gedemlonp.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gotgiyjct.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/galidkdkr.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/giyhbsfgv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/ghtnqfpqm.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/glndnqgdd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gumwnvcvv.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gqesfhusk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/geaxbjnbm.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gtpmuihni.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gswgrrhpv.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/gbqqszjtb.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.zdbjq.cn/Article/details/goyljuvas.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gctdmhkhc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/glleyldqu.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gwqpmpdex.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/giamitjft.sHtML

[T12] Kotlin：解构声明
来源：http://blog.zdbjq.cn/Article/details/ghumajfwr.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gqpsacqna.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fehbvm.com/Article/details/grqcuyhgs.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/gtevqbeqy.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/giaxdphgn.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gtonupwlt.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/gqfodgwxi.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/giublmzrf.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/ghsugysob.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gnsasviyl.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/glbnzdcoc.sHtML

var a = 1;  let b = 2
来源：http://3g.fehbvm.com/Article/details/ggsnquvqw.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/gcdqzxbrn.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gbcrnjzjn.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/gbviwelmj.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/ghhyzaqtb.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/grvgydmjz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gdpzfryks.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/gwpogwgly.sHtML

for x in a { print(x) }
来源：http://www.m.share.zdbjq.cn/Article/details/gvallqaku.sHtML

[T22] Swift：字典
来源：http://wap.zdbjq.cn/Article/details/gmspybihd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.zdbjq.cn/Article/details/gacdeggaz.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/ggjqncdtn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gnqnjteig.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/gvsxdrsrw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gzqjesgaf.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/gsirlivqx.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gyihopapq.sHtML

[T26] Swift：类与重写
来源：http://wap.hesvh.cn/Article/details/ghvqermkd.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/gexpmunyo.sHtML

[T27] Swift：错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gvspzvvqd.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gtlsidtwk.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/gwewfyocy.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/gxiebchim.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fehbvm.com/Article/details/glroditzr.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/gyrjwjwta.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/gqafwjrwk.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.hesvh.cn/Article/details/grxvcgcfd.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/gkotkppws.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gzkqpufad.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/gcbhdowyb.sHtML

local a = 1
来源：http://www.m.share.hesvh.cn/Article/details/gkmwhnwkl.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fehbvm.com/Article/details/gplyujyzc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.zdbjq.cn/Article/details/gytguhqrp.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/gsdsblwxg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.zdbjq.cn/Article/details/geviokaob.sHtML

[T35] Lua：字典表
来源：http://mobile.fehbvm.com/Article/details/gbnphclza.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/gbwgrznlv.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/ggtdoswml.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/ggwowvfid.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gxrzouqrj.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/gkwtrqfao.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/gmxzytnnz.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/gdrseeejl.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gzhbipzas.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/gfyrlysaa.sHtML

[T40] Lua：元表
来源：http://wap.zdbjq.cn/Article/details/gqvurjzzg.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fehbvm.com/Article/details/gyyzwrpyc.sHtML

[T41] Perl：Hello World
来源：http://3g.fehbvm.com/Article/details/gjkcdatdd.sHtML

print "Hello\n";
来源：http://baike.fehbvm.com/Article/details/grdscerjo.sHtML

[T42] Perl：变量类型
来源：http://read.share.zdbjq.cn/Article/details/gzxjzmqav.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.zdbjq.cn/Article/details/gfglnrzfv.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gdjzbaxuo.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/gmywriild.sHtML

[T44] Perl：条件
来源：http://www.blog.zdbjq.cn/Article/details/gemexaawc.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/gyoxnvkny.sHtML

[T45] Perl：数组遍历
来源：http://baike.fehbvm.com/Article/details/ginfgaoxl.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/ggtpobrcz.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/gmkexqdbx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fehbvm.com/Article/details/gkvtnhkkk.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/gblqogqxy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/gruwbgznc.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/gitaoylfi.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fehbvm.com/Article/details/gnpnpnqgv.sHtML

[T49] Perl：函数
来源：http://wap.fehbvm.com/Article/details/gklglvmig.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gdpejazpj.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/goyxrfxai.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fehbvm.com/Article/details/gcoyiught.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.zdbjq.cn/Article/details/gjtnkyhaz.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gedmoceiy.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gftkgxiae.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/gcrxkbpmw.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gxpczragf.sHtML

[T53] Scala：字符串插值
来源：http://blog.fehbvm.com/Article/details/gbrkdjzjj.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/gzhoddywl.sHtML

[T54] Scala：集合映射
来源：http://m.share.hesvh.cn/Article/details/ggzhweceq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/gkfjranrt.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gbhkbuhvo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/gbteekphm.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/gnnwpkija.sHtML

case class User(name: String, age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gryeviuvj.sHtML

[T57] Scala：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gukqnwaeg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fehbvm.com/Article/details/gfwuifdxj.sHtML

[T58] Scala：函数定义
来源：http://3g.hesvh.cn/Article/details/gkxkvyucm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.zdbjq.cn/Article/details/gagueyevh.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/gbqnsooya.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fehbvm.com/Article/details/gmjhvwcia.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/gorwmfzgd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fehbvm.com/Article/details/gzvuahuxm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gefcduahh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gurwzyrvo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gipaogjpu.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.hesvh.cn/Article/details/gruufghja.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/gawawtufq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/guvdxclgw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/gtxjmqkjy.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fehbvm.com/Article/details/gcsspguht.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/gcucqfcww.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/giqpstoxy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gernkblxd.sHtML

[U05] Py：列表去重且保序
来源：http://blog.hesvh.cn/Article/details/gkbcglvbx.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gakzheoqv.sHtML

[U06] Py：合并两个字典
来源：http://wap.hesvh.cn/Article/details/gihqactiq.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/gmhygmvga.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fehbvm.com/Article/details/gieytzcxl.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fehbvm.com/Article/details/gdrmjkrsg.sHtML

[U08] Py：展平二维列表
来源：http://mobile.hesvh.cn/Article/details/gajynzrxl.sHtML

[y for x in nested for y in x]
来源：http://wap.fehbvm.com/Article/details/guqjbaadk.sHtML


<!-- 参考信息 -->