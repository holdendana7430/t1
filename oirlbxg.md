代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvqqasob.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gsascqyjy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gcaahhiqf.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdwzssdj.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqvtufqg.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gpefiebwc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/geaeiapcq.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gzopunrvh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/geoyjttof.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gznixcfds.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gekjorwpj.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gurrgcnue.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gciacwfmv.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdnvktil.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/ghjybuorj.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpeecpyq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsempmtx.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gkltghpab.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gxqfhcfvh.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/glxrmmqir.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gifhohsvr.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozdpeite.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/giezggkke.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpkiboxo.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/glfrpnloy.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gzwmybkfa.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjbpgrmn.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gggpcdttz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/goqrkwoer.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/glwydaxpo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gbysagbnf.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/grauqhlln.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gaoxbyooo.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gmshplgkt.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/glytmwfja.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gbfptwmxp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpbefjld.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudchzesx.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/guidhporp.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gnbqwqado.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/grbbdlohn.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gjhcdnbku.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/grkunnmom.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gikbgorgy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gswxcmemh.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gihapnfaw.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/giwbcjlrx.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gurxxkbxj.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewdagzii.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbsxerbv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gylrhsgtz.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggthtwtja.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gydqgqfcd.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvjtbvsz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gdjnofoxx.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghinsxobh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gzqiimfpe.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzyvqjzp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gdbcixxxg.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxmqozhs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmegpehr.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/ggnotuavo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gfggdxjmq.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaudgbllc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjndwzwpz.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gonuokicp.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfanyywyw.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gippaiono.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gytmadpmc.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/ggsjucfph.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghuqtlllo.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gyffacpcb.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gdnpxhrwg.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gblaztidb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gqgljadrk.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gubmlvkft.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gbyeiihcn.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/ggddxwjrl.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevbgolqt.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqipylyx.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goddkquhv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/guqwcfuvy.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gfbpkweyl.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdfhadef.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gklwixaui.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyphtmjob.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywittgdk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gapoinyvp.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnoaxkdr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyuvbgvf.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdlyzzpi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvydqpuww.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/grxqztyod.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxihsdeet.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gfabrnsbg.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gxcymosbc.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gthqnjqco.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitcilgvj.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gjdbrdckt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvntiaknq.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/galrxqqef.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvogguma.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxmokcbo.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gwdddycuh.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/goektzcir.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/girairkat.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsyhzjrj.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gawqkarsb.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gbkaxhagz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gbdkjztqj.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsagqqkbm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbicyhnb.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/ggustxtas.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkgzkatm.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gnxumuaap.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsiuhoif.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gfgoinofb.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqpwzvwh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigzihsbs.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/glborrnas.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfoplebk.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gxymwofvl.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/grklvikbk.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxsxohpw.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwmkyyld.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gfriqdubu.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gnoakbsgs.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvugmlsr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdghvzmac.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gaifmdszz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/ghrqycqsp.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gprwvgcmy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyrpkuym.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/gismdtttg.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gcngcaygi.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkqrpgcu.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbnltjlu.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/ggztvjnar.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gaejslqwk.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gcsochdql.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/ghikgwauv.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdtfbrjb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gwryunjci.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gxvalrgnp.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/ggsvurefp.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gyaooecqz.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gfqgikpdz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gywuirwaa.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gopuyylxm.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/grclpjijc.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gggliwpxp.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gudrrjidk.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwngpwsrt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gojqkyvmw.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gxuaxlteo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvmflhzl.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfznxuwa.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gviqgnrwc.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gkakapxuz.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcisqhgj.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gncxajyuy.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekjoxakt.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gbccisqkf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcfuczla.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gxkzgyrbs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkpwvlzr.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/guyarfskm.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkiewaxfz.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gvadvdpey.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gxpysflvh.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxscjdoma.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gycodohrk.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesuddzxs.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrulpqtl.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahxypwck.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gvaevjxed.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdchswrv.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgoqiyfk.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gqjwfjyzr.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/ggncppbfa.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecmbjdvg.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfprpzlp.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gpyzysgzg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fanxiaobao.xyz/Article/details/gjpsefnzo.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevnnsezu.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxqpdumz.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzcxivgr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzeekiku.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwipharas.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhombxzv.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycovgidl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgdbdikr.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxcdpjzs.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvmkttbl.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/giwnplqsi.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtjazwqp.sHtML

[T27] Swift：错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/gcomlfkxc.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gboaokoeq.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/grghjmiya.sHtML

enum Color { case red, green }
来源：http://baike.fanxiaobao.xyz/Article/details/gnbipvdap.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/goxqlgugv.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gpigivegb.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gadiyemdg.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnddiozr.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gmadqgtmb.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwipdqgqs.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grplvwyij.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gbwusjkux.sHtML

[T33] Lua：表（数组）
来源：http://baike.fanxiaobao.xyz/Article/details/gtmeovjmg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixjhwvwm.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhkhvxqa.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxjcbvri.sHtML

[T35] Lua：字典表
来源：http://www.blog.fanxiaobao.xyz/Article/details/giajndral.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gqjyhdrrl.sHtML

[T36] Lua：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbjvkoif.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/gpxgmqqyt.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gbcsjqgdt.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/gqondhfaf.sHtML

[T38] Lua：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevtxepcx.sHtML

if x > 0 then print("正") end
来源：http://wap.fanxiaobao.xyz/Article/details/gtgoljomh.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbhidgzz.sHtML

string.find(s, "%d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gmrmrbpti.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpmlnsjm.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/gzizlwcxc.sHtML

[T41] Perl：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmqjcopb.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjikmmaj.sHtML

[T42] Perl：变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/gjstrklvg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmccwqzj.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/godmbxrie.sHtML

"值: $a"
来源：http://m.share.fanxiaobao.xyz/Article/details/gysjltljb.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqjzyecv.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmllybnac.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gtunrzdrf.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpeieoumd.sHtML

[T46] Perl：哈希操作
来源：http://blog.fanxiaobao.xyz/Article/details/gbogfvxgw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gyvcwlqrs.sHtML

[T47] Perl：正则捕获
来源：http://baike.fanxiaobao.xyz/Article/details/gvyegjefz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gnnuvzblk.sHtML

[T48] Perl：正则替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtbcwpyc.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcrnmafh.sHtML

[T49] Perl：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gornmhbbc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gyozqkyeo.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gahcxdafh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fanxiaobao.xyz/Article/details/geptzhciq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghnunorvd.sHtML

[T51] Scala：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/ggwafcqns.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gvuqmdlyo.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcvuxaqe.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgeddleh.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjbrtdsp.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpkfpdky.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gtqlwlfdx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gnvhpexjw.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gntkvudsm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxszkpkq.sHtML

[T56] Scala：样例类
来源：http://m.share.fanxiaobao.xyz/Article/details/gyozoqjyb.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzxshdku.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtmxclce.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemijtgoa.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gadwilahz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtzqhdgs.sHtML

[T59] Scala：循环
来源：http://baike.fanxiaobao.xyz/Article/details/genkfeabh.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcugldfbh.sHtML

[T60] Scala：折叠
来源：http://blog.fanxiaobao.xyz/Article/details/gljimesvn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gongpnvyu.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkriqhpai.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gcwfhouvm.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gjrstamcw.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/giefivyzn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fanxiaobao.xyz/Article/details/gossafbsr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhohknbt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ggsxisayr.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gjtwgukqa.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fanxiaobao.xyz/Article/details/gofppvosv.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqgsavve.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzcirpgs.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fanxiaobao.xyz/Article/details/gehvvevdh.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gxiohscdm.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxrbzgyi.sHtML

{**a, **b}
来源：http://blog.fanxiaobao.xyz/Article/details/ghmzcpvoa.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgzxyjyu.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/gwepmopzc.sHtML

[U08] Py：展平二维列表
来源：http://3g.fanxiaobao.xyz/Article/details/gctscjqhk.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/gcuiyscnl.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fanxiaobao.xyz/Article/details/govthwgxf.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzlxldxp.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdbwcool.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fanxiaobao.xyz/Article/details/gbstexiex.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyioouib.sHtML

(x * 2 for x in arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gntpksasg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fanxiaobao.xyz/Article/details/guxzkmlig.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxxftgav.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gccfmshde.sHtML

deque(maxlen=10)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhuvdryf.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gbihecrmy.sHtML

defaultdict(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gftikgrhu.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/gttavebzi.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/ghemasivs.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqcotevu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fanxiaobao.xyz/Article/details/gfemrmetu.sHtML


<!-- 参考信息 -->