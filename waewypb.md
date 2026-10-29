代发 wailian999

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/ggnqzeufl.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/grstjodje.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/gwzndpith.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gzeezjavv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/gdszsbckz.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gvcqrxmve.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/gndvzzrpp.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.zdbjq.cn/Article/details/gmjuffrqk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gdgeseoxv.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gtdnarhbg.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gqrrekkqo.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gsebjkqvj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gqamixqsp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/glzulldcb.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/ggbujiyma.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/gisjgflag.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/ggqfppets.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gsqaehwih.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gnpsufkds.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gfleemeyb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gnvzkvxno.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/gbtsjkyzo.sHtML

(double) a / b
来源：http://www.m.share.hesvh.cn/Article/details/guxrtrdca.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/ghitkaoce.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gzsunjosw.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/ggsyaqutk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.hesvh.cn/Article/details/gcyxbvivu.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gbvytuejj.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gmshfedgj.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/gpceqeffq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gkmbsjhti.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/guwwpjddd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gwhsbjpvn.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gqhaybncx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/ggmvmakfz.sHtML

[S22] C：字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gybytkwbd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/grdpuuqoc.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gvvzaueih.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gwkbrchst.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gjzznrfzt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/gntwahvsz.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/gdjlgpvua.sHtML

memcpy(dst, src, n);
来源：http://www.blog.zdbjq.cn/Article/details/gwwpwvyti.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/gfnztmfjc.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/grpauqwwv.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gqfrceuth.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gvtukcvor.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/ggdyugzfv.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/glvywngjx.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gyajvxukd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/gjhvvwtcy.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gfuncklwh.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gbdusgrzq.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/gscrjxtio.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/gfmrzblre.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gglgpijfm.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/gtukksljy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/gcrfpabka.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gaaoyavxf.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/gkhapviyf.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gkhnkkanp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/gbwivmavf.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/gqxxdkzbn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/ggguzabrk.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/gvowiqeva.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gacsbcwsj.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/geeblujpn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/ggfgkdqmu.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/giuntitvv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gevpxxozi.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/grtsapvqz.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/gikhvjkoo.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gecwuyzfz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gwidjffqd.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/gbsvztkcn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/ghwpofbqp.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/gttjjpfax.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gohtzqvbj.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/gvsdgbjav.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/gfogyceir.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gaishzqgy.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/gdaaldmcr.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/giemxbwur.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/gyzadvbth.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/grjdvwfqw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gojsfpckn.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/glkqwlmwg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gwpgkvpzx.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/gdpjzsnwe.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/gbkvhrzgi.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gtiyosqnf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/gnfjncxss.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gmuigddgy.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gcsfbrygb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/gdwfljmin.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gktncmapy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gamubazas.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gsyqtvwen.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/gdteufmce.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gruzzmpex.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/gxzjuxmsc.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/gkxmxdrhf.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gnkcmofhd.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/gzmkurrao.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gsquksxrb.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gesljynle.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gqtwccqqm.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/glxaicepl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/gacgrsrqn.sHtML

[S57] C++：编译期常量
来源：http://mobile.fehbvm.com/Article/details/gziedoygv.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/ghjxnqccr.sHtML

[S58] C++：命名空间
来源：http://wap.fehbvm.com/Article/details/gpdpsxslt.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/gfzefjfpw.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gfrncvktg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gmfbwnnke.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/ggdoccpvt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/gfyrqnlsq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/guillhmbd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/givomddjp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqyeplfmw.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/geleoufhb.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gyomqctnm.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/gxsgnsfyl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/gnoysxswq.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/grefpwjll.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gyqhgczzj.sHtML

[T04] Kotlin：空安全
来源：http://m.share.hesvh.cn/Article/details/griavvzvn.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/gnsaiybdg.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/gxwubdmoi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/gjrelfuoa.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gkhkdzwcr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/gpvzulpgw.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gqoyjovwz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gdepucdry.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/glfbcrplv.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/gzejgjoqw.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/grcwiiyjd.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gojteqsby.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gjkgahobv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gkwrhloxc.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gyjdmnmiv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/gdzygrapc.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gpkbamcwm.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gaepoxtve.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.hesvh.cn/Article/details/ggmvizbil.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/gzfdqigfh.sHtML

[T14] Kotlin：循环
来源：http://3g.hesvh.cn/Article/details/gqjkbrjuo.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gintpdomz.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/geyyittza.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gjxstwqfk.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/gdbihavsw.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gtnehxnwr.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/gmqyskshs.sHtML

var a = 1;  let b = 2
来源：http://blog.zdbjq.cn/Article/details/gticmiodn.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/glkotlwvh.sHtML

"值: \(b)"
来源：http://www.m.share.zdbjq.cn/Article/details/griaichmw.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/gfkxmtvsd.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gxwaeuece.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gpxqqblxk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/gznojroyu.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/grdkcitht.sHtML

for x in a { print(x) }
来源：http://www.m.share.fehbvm.com/Article/details/gtmqesmve.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/giqiqqzps.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.zdbjq.cn/Article/details/gtlxolzri.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/gidpnaepr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/gdjvdirms.sHtML

[T24] Swift：闭包
来源：http://wap.hesvh.cn/Article/details/gjboefzym.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gfcuetstl.sHtML

[T25] Swift：结构体
来源：http://blog.fehbvm.com/Article/details/gduzscgvw.sHtML

struct P { var x: Int }
来源：http://mobile.fehbvm.com/Article/details/gnbxofhqx.sHtML

[T26] Swift：类与重写
来源：http://www.share.hesvh.cn/Article/details/glczwnoxz.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/goksybxoz.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gsghpcjys.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.hesvh.cn/Article/details/giftcodli.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/glgnkuajy.sHtML

enum Color { case red, green }
来源：http://www.share.fehbvm.com/Article/details/grxhsaivj.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/gloqvwaka.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gsowndigd.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/gnpnzxpib.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/gnwflbrar.sHtML

[T31] Lua：Hello World
来源：http://www.blog.hesvh.cn/Article/details/grgwmuesd.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gcmaotwjs.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/ghufapdfc.sHtML

local a = 1
来源：http://baike.zdbjq.cn/Article/details/gpppqauqs.sHtML

[T33] Lua：表（数组）
来源：http://m.share.hesvh.cn/Article/details/gnvmxzmrn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.hesvh.cn/Article/details/gijavxvyf.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/gxuvddjru.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.hesvh.cn/Article/details/gxvocftuw.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gyedskvyp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/gtfudbnmq.sHtML

[T36] Lua：函数
来源：http://www.blog.zdbjq.cn/Article/details/gsuwpdjfy.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/glfdqwapq.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fehbvm.com/Article/details/gzzxsydhw.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/gtlxtlyzw.sHtML

[T38] Lua：条件
来源：http://www.blog.zdbjq.cn/Article/details/glklqjzhj.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/gczdmogqx.sHtML

[T39] Lua：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gtivydium.sHtML

string.find(s, "%d+")
来源：http://3g.fehbvm.com/Article/details/gqdmqvftq.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/gkupbbadf.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fehbvm.com/Article/details/ggeymggtb.sHtML

[T41] Perl：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gpcymvont.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/gtselavwl.sHtML

[T42] Perl：变量类型
来源：http://blog.zdbjq.cn/Article/details/goytiwmkw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.zdbjq.cn/Article/details/gmxxugjby.sHtML

[T43] Perl：字符串插值
来源：http://baike.fehbvm.com/Article/details/gwxxmwixq.sHtML

"值: $a"
来源：http://m.share.hesvh.cn/Article/details/grtmvdngr.sHtML

[T44] Perl：条件
来源：http://www.share.hesvh.cn/Article/details/gkhayuxpx.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fehbvm.com/Article/details/gsxnknwfc.sHtML

[T45] Perl：数组遍历
来源：http://www.share.zdbjq.cn/Article/details/gkkhbxtlx.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/gmsfizowv.sHtML

[T46] Perl：哈希操作
来源：http://mobile.hesvh.cn/Article/details/gvrkbiyek.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.zdbjq.cn/Article/details/gmcmnasjz.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.hesvh.cn/Article/details/geaaelprr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/guqsyxmzm.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/ggodwfjei.sHtML

$s =~ s/old/new/g;
来源：http://read.share.hesvh.cn/Article/details/gjuipyics.sHtML

[T49] Perl：函数
来源：http://wap.fehbvm.com/Article/details/gkshuglqn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gwursirga.sHtML

[T50] Perl：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gcmmltobh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.zdbjq.cn/Article/details/gqwspoxsd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/gwvsdylyr.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gbhxluybd.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gkgzcwdhk.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/gmvgarjif.sHtML

val a = 1;  var b = 2
来源：http://baike.zdbjq.cn/Article/details/gdzcrucun.sHtML

[T53] Scala：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gyzpwomwu.sHtML

s"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gpxkqnhmj.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gprffcbct.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/gpvahrzjo.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gyuvlmyuo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.zdbjq.cn/Article/details/gjzgphtbb.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fehbvm.com/Article/details/grfhgblwl.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fehbvm.com/Article/details/gaindbanv.sHtML

[T57] Scala：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gsokfvrzn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.hesvh.cn/Article/details/gjoaewweu.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/gwpxaxljx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.zdbjq.cn/Article/details/goelxvnhi.sHtML

[T59] Scala：循环
来源：http://www.share.zdbjq.cn/Article/details/ggteamowe.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/grzlkvqwv.sHtML

[T60] Scala：折叠
来源：http://www.blog.zdbjq.cn/Article/details/ghgbzzvmt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fehbvm.com/Article/details/giwcmsvhv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxkxlduyj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gbfuimxgh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gldazznix.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fehbvm.com/Article/details/gcfpkvfaz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/ghvtztugu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/ghtqquoyd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/ghpxlnlpg.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.zdbjq.cn/Article/details/gxftnmxxt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.hesvh.cn/Article/details/gtldlcpdz.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.zdbjq.cn/Article/details/gtmbmrdix.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/gwbdsbdtc.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/gboyzalbx.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gxvvyrxnh.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fehbvm.com/Article/details/gaheiwgvb.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/gxhwecbnk.sHtML

[U07] Py：反转字典键值
来源：http://blog.hesvh.cn/Article/details/ghtforapo.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/gegpbtcjg.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/gvxhxtykd.sHtML

[y for x in nested for y in x]
来源：http://3g.fehbvm.com/Article/details/gdfozbrwd.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.zdbjq.cn/Article/details/ghkmdrspc.sHtML

max(d, key=d.get)
来源：http://3g.hesvh.cn/Article/details/gsgevziti.sHtML

[U10] Py：按值排序字典
来源：http://baike.fehbvm.com/Article/details/gnzelyzsb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/ghwxeitns.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fehbvm.com/Article/details/gkdcfnqjp.sHtML

(x * 2 for x in arr)
来源：http://wap.zdbjq.cn/Article/details/grgxrqniw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/gsepxjpfc.sHtML

Counter(arr).most_common(3)
来源：http://m.share.zdbjq.cn/Article/details/gfslfhbvl.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fehbvm.com/Article/details/gaklxgkjb.sHtML

deque(maxlen=10)
来源：http://wap.hesvh.cn/Article/details/geipkuuva.sHtML

[U14] Py：分组收集到列表
来源：http://blog.zdbjq.cn/Article/details/gtumqannz.sHtML

defaultdict(list)
来源：http://www.m.share.hesvh.cn/Article/details/gtdkpbljf.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/gdfcirvrl.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/gxvncnuwr.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fehbvm.com/Article/details/gtrzoroyc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fehbvm.com/Article/details/gocxpzvlg.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/ggyrfpvvf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fehbvm.com/Article/details/gqqcirnny.sHtML

[U18] Py：预编译正则
来源：http://mobile.zdbjq.cn/Article/details/gpkxqjdgw.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gijnpkhqu.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.hesvh.cn/Article/details/goqmoiwor.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.hesvh.cn/Article/details/gyoiczlqn.sHtML

[U20] Py：缓存函数结果
来源：http://wap.hesvh.cn/Article/details/ggvyqwrhm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.hesvh.cn/Article/details/gyljwtohf.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.hesvh.cn/Article/details/goapxbxan.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fehbvm.com/Article/details/gkihezqaq.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/gmllhscfn.sHtML

list(zip(*m))
来源：http://blog.zdbjq.cn/Article/details/gtpjhboov.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fehbvm.com/Article/details/gpwjbjphi.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/gdogglbrw.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/gxibdywtb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gtqqtqcom.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.zdbjq.cn/Article/details/gacnflyqg.sHtML

csv.DictReader(f)
来源：http://read.share.fehbvm.com/Article/details/gumqbaasr.sHtML

[U26] Py：并发下载
来源：http://m.share.zdbjq.cn/Article/details/gqmvqqjuw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.hesvh.cn/Article/details/gvbvcwkuz.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/gmrwrdigw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fehbvm.com/Article/details/glwhbhyhe.sHtML

[U28] Py：类型别名
来源：http://mobile.zdbjq.cn/Article/details/gtsynpczu.sHtML

UserId = int
来源：http://m.share.fehbvm.com/Article/details/gicrhhdtb.sHtML


<!-- 参考信息 -->