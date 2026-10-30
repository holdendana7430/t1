代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gbvonccgy.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylpwdtvh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogkxodbv.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxbvuxzh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqouiklxu.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gqrciayoe.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwenykjw.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ganphiriy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/glxujzyjl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gsnvxyvxn.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gokwdpdhe.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvxechmxv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/glvnxfgns.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gwqodklai.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gnloicija.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/grybpyncx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtegduuep.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gwvozbihh.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/geziufbyy.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgqsspqz.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gsvuaoxso.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamepgjyo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/geftvttlp.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/geslyakrw.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gnlohndux.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gthywmvww.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/glytgdzdn.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzknwlpp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gfejcksdu.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvoclohz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyrjgjus.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gjyucqbju.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gbdcnfmik.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwecwouq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gackqmzsi.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gkpmnzfbg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gyewotzgo.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqvusmoz.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojumhhib.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/govxcmdwp.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/glfopkuyz.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcqaftuf.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/galspbvor.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gopxqhwwt.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuawvorq.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnhlcibw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gumawnthw.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gytravysx.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gfelqmxvs.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gptlscihe.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrkayyuo.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gtvsepabk.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyykvfit.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdoblwwh.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gybbbvicd.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gasfhyash.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnkmotyi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyaxwmah.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbkwokdu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gsxnkjmat.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gwwsnytzu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmfiyige.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/grjvqevty.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpumtcqh.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfgljosy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyhyonlr.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gxiidbwxg.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gqsfrzugk.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gfnpzspnt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gwirrittd.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbndcxyk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjkqfxwf.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/guealnmln.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gfhucmqio.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gghjdgqpc.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrsgyxrw.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gapgvldmq.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gygnbzktr.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnrzlomr.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyaezydce.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzcxbiir.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gicvylzez.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkavswvh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gihkdjxau.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gmrfmkgpr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnoalvzfi.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgmjmxym.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gifufzpum.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyeclwwfl.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxbywvxw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/geukezimv.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gkyjgdxqe.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfoulstqc.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gtpcfrmfl.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gunzbwihi.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/gmmrnxhoy.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwimrhiu.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdznoeogl.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gvldjvisg.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gstwwjlib.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gwwpxpefv.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gotlhabcq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbxtvxek.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkaqyxugj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gokdnladg.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gpisrqckc.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/guviqcijb.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfpmopvs.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gstsklyur.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gofsjrzam.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrbotocz.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqoblckg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gkpilpwvt.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gqfdogqbk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsqdodar.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gortzozrq.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gxarmortq.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/goflspshi.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gqdhqnxrm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqgfvzgv.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gvidoogkb.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyubhiws.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gsohrufds.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/girwumepa.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/guspuksao.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/gepcknqdv.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwyciygi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/geyttmfun.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gajlgsklb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gklxsbsef.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gueqgykec.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtauavab.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gepluzegu.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgcpcfvs.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvrjoxci.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyanwrimn.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gxzyqbmob.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/gpxviaxxr.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gemqlzrku.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gtmhoywmo.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmrigrac.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzawrdgf.sHtML

[T14] Kotlin：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgxueumi.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsvnsumn.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/gxtntxgvs.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/geejainog.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvugtodz.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwigjbqph.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gxbkgolez.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gevfbkqnz.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gbtrjndnu.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/gyleqaezg.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/ggetrzshq.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/gezeivjbd.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gaehjzbbd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/glkeumxzb.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/glrqosspe.sHtML

for x in a { print(x) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgrasvfr.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gzivebffp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmoyaoap.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gxqmpqhdu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/guwbvxamm.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmpxhskr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/ghzjodgtg.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/ggwgmnkkj.sHtML

struct P { var x: Int }
来源：http://3g.fanxiaobao.xyz/Article/details/gspnhllbd.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/gcmyzktos.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvirfrgqd.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/guxvhhwrs.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gobkpurmk.sHtML

[T28] Swift：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/glpydsyxr.sHtML

enum Color { case red, green }
来源：http://mobile.fanxiaobao.xyz/Article/details/gltwvhupd.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gpluwplko.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gvseejttc.sHtML

[T30] Swift：协议
来源：http://wap.fanxiaobao.xyz/Article/details/giepgdcnh.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gszrnaoog.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gnccplscj.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gimwpokdv.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gfjuvofbu.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqasyoav.sHtML

[T33] Lua：表（数组）
来源：http://blog.fanxiaobao.xyz/Article/details/gquuhkdco.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fanxiaobao.xyz/Article/details/gdslahatc.sHtML

[T34] Lua：遍历表
来源：http://m.share.fanxiaobao.xyz/Article/details/gzculyvjs.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/gfpbnnejw.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/gffccojbp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/glxuumehi.sHtML

[T36] Lua：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqjwtjis.sHtML

function add(a, b) return a + b end
来源：http://baike.fanxiaobao.xyz/Article/details/gzlhbtcwg.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunkshlir.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gphtkmjcf.sHtML

[T38] Lua：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gbshqzfwg.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbmvtuaj.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgpeoazj.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhldwqtp.sHtML

[T40] Lua：元表
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjkqyzqj.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/ggiezuaci.sHtML

[T41] Perl：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gvleimhkq.sHtML

print "Hello\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekqehxeb.sHtML

[T42] Perl：变量类型
来源：http://wap.fanxiaobao.xyz/Article/details/giqjctgnc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnowpvolt.sHtML

[T43] Perl：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gjoevgcxh.sHtML

"值: $a"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsaszelis.sHtML

[T44] Perl：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gspyfkvja.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtrizhkq.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gfyfifpbf.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfucxilo.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzxpcdwe.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdkjdwlyg.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmimfyaf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkucwfxve.sHtML

[T48] Perl：正则替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzyutmyz.sHtML

$s =~ s/old/new/g;
来源：http://baike.fanxiaobao.xyz/Article/details/goxkqqcis.sHtML

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjznuwvii.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbuiqmzsz.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwezijjy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvkagjrd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwrgwywjb.sHtML

[T51] Scala：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwmehfmd.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvonnalur.sHtML

[T52] Scala：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmuywjcxm.sHtML

val a = 1;  var b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gkdbqeqwg.sHtML

[T53] Scala：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gzvniggog.sHtML

s"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gawmlulwc.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/glaucmkas.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuhtlzan.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzwhuucs.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzqsdzce.sHtML

[T56] Scala：样例类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlmaetfq.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gsceqjkpu.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvfuuugw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginzuhjlp.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/genhkcpgt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdussrtbm.sHtML

[T59] Scala：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gqcgbblic.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gdvyamopi.sHtML

[T60] Scala：折叠
来源：http://wap.fanxiaobao.xyz/Article/details/gnixaiyut.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fanxiaobao.xyz/Article/details/gtctsxakq.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gyfxxdsiu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gwuwjessu.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gmsmzaqem.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmuynpec.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fanxiaobao.xyz/Article/details/gylrztqxr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fanxiaobao.xyz/Article/details/gznafvgdl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gyqlxqizq.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/glpsqqwrx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmqsrinb.sHtML

[U04] Py：变量调试打印
来源：http://blog.fanxiaobao.xyz/Article/details/ggggjftnk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fanxiaobao.xyz/Article/details/gnqgdklpf.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fanxiaobao.xyz/Article/details/gxazuwjvk.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gcutzohel.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gigendccs.sHtML

{**a, **b}
来源：http://wap.fanxiaobao.xyz/Article/details/gscrgyulg.sHtML

[U07] Py：反转字典键值
来源：http://blog.fanxiaobao.xyz/Article/details/ghoxfzmqi.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixyrmdzg.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/gzpteneef.sHtML

[y for x in nested for y in x]
来源：http://read.share.fanxiaobao.xyz/Article/details/gidcviexq.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fanxiaobao.xyz/Article/details/ghrwuoscq.sHtML

max(d, key=d.get)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcmwwcri.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpqujdzb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbbgizrc.sHtML

[U11] Py：生成器表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gifszkkuq.sHtML

(x * 2 for x in arr)
来源：http://wap.fanxiaobao.xyz/Article/details/ghjovlgqs.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gfeixcbst.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfivxivoc.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gledfqgqc.sHtML

deque(maxlen=10)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqoxjqwc.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvgrzerf.sHtML

defaultdict(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzpokdkc.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrisvvdg.sHtML

t = time.perf_counter()
来源：http://blog.fanxiaobao.xyz/Article/details/gcjmtouic.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fanxiaobao.xyz/Article/details/glrhmzoys.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fanxiaobao.xyz/Article/details/guuqigdlz.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gjcfpbgle.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fanxiaobao.xyz/Article/details/ggokxqpqd.sHtML

[U18] Py：预编译正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkfetdsd.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/goizxaeyo.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fanxiaobao.xyz/Article/details/grmlowrsk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrsxlgrl.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fanxiaobao.xyz/Article/details/gzewewyzn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjawhinhn.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fanxiaobao.xyz/Article/details/ghjurdkrq.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/ghznvzgps.sHtML

[U22] Py：矩阵转置
来源：http://3g.fanxiaobao.xyz/Article/details/gljkbfgbb.sHtML

list(zip(*m))
来源：http://wap.fanxiaobao.xyz/Article/details/gwrshobjk.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedffoass.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fanxiaobao.xyz/Article/details/grvsfyjvc.sHtML

[U24] Py：路径操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdmwtxcn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gfuiaomhf.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fanxiaobao.xyz/Article/details/galtnuqqe.sHtML

csv.DictReader(f)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhwjgfbd.sHtML

[U26] Py：并发下载
来源：http://3g.fanxiaobao.xyz/Article/details/gyafwniam.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fanxiaobao.xyz/Article/details/gceftqozf.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fanxiaobao.xyz/Article/details/grtxbypjy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fanxiaobao.xyz/Article/details/gryndqmtc.sHtML

[U28] Py：类型别名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjozommn.sHtML

UserId = int
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgyufrxb.sHtML

[U29] Py：属性校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gamwiffcw.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgnncbfo.sHtML

[U30] Py：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gchhokjwy.sHtML

@dataclass(slots=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gvuhosmep.sHtML


<!-- 参考信息 -->