代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwnssvwq.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/glaejvtca.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/ghawrmdhq.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gzbcqence.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gfuudprui.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwndbgxx.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gziyqezmw.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gyswnpvjb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gfkyaccir.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gwvvpbvre.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gkywqjgte.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gwqmsnbfy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gubhpvtrs.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/glzyjmfta.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrzwvtll.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/guzsjzphe.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtiqgeroe.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdckqkndk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/ghjszjyvb.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gxcdalqzx.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gpzrjggls.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gjlgsnlhb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvbhupkq.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqmneqrn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gchvsjcat.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gtimafaug.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gfokcttmx.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gdtxttiek.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbhjygci.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/guofxxelz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjzjrfga.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gsduftnff.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvodablgn.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkzwefhk.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdbqtiom.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gljlnkgzc.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gjnauvvtm.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gerdquecu.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnstslbmb.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkaktkht.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcynaedmr.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gobicvile.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjqcwzti.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gdayaific.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gyhapojaz.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/giezbivqm.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gbbfalcfx.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gzmluaxqd.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gidfxvmvx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvrlqakwp.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gczdzivbb.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/grbpehxvx.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gqtjwdart.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gikoputpm.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadteqezf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxzboizz.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqnndzte.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyeittnq.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gcomwncuy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gmexjjzqp.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmskauiqt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gnybcuvnb.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpwqddgi.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gftvnxoek.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gdavxpaxm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gspqiygnu.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gmxmndzty.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthlilokt.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/glafokvcj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyokwnia.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gprivzkeg.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gqotztdrs.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gpxbnedfb.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gljmjxwhf.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gaasrdedx.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gelirrvmy.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gtydnnmah.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gzozzrmsx.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/ggugyshqg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbvkbzxm.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gbvijxguh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbosnyyyc.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gsecetpka.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggejusjoo.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gcmawrvba.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmzedmdx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggypkgfgb.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyqqcswq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcygbjtj.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbcjgldh.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gmeknuxqy.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtsqrmnr.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwbfggzr.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvithsxc.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcoblluc.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gqudwcuvb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbmeecxy.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/guqzbnjfw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/glxvhxybo.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gnmtpprvi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxmlwmrn.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/gdamqwhpp.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhsdtnrk.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggphmohlz.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/galyhhefe.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/ghowonhue.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwnezqqg.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gfswqhmmz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gyyllfkou.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gjoejihvt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gbhclacgy.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gpgeddmrv.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/getvdwfuv.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gayhxmyqz.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/grdlvaquj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxjyycan.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbbslixg.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gjjtboytz.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/gkqvqlmky.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfumgkxi.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gwqpyfpfp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpuynxkq.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgydqdpy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gittnsyuv.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gjputruah.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjdmzvmj.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gppzgbdco.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvgizdun.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gunknwamh.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzsbcsda.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshqszvjf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gitnsyexr.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gucjihoar.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/gbiemgwuw.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbffeacn.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbsmtmdx.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gniyhrhvc.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjmiyszb.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gipjlmzhn.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftwpkmha.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/ggmhgccne.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gfobccutg.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gxoniscif.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsfgnxvu.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxdsquem.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gewgkaior.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gywsdofyh.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/gahgdkypo.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmtkaktw.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gsmawwhoc.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/gkwniswjo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxriwxwxo.sHtML

[T21] Swift：遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkrgghqc.sHtML

for x in a { print(x) }
来源：http://blog.fanxiaobao.xyz/Article/details/gaoqrzfqs.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdalooin.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gsyjwrbax.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gqvnubzsd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gkromqvpv.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gyabvvrcv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfllshgk.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/gajlknrgo.sHtML

struct P { var x: Int }
来源：http://3g.fanxiaobao.xyz/Article/details/gudacwpdi.sHtML

[T26] Swift：类与重写
来源：http://mobile.fanxiaobao.xyz/Article/details/gnreltztl.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcihnutnw.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokzgoyro.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gurlpkhsm.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gfdslnmbk.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnpcdjmz.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/gapjemtrv.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwmvhlyd.sHtML

[T30] Swift：协议
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrvdykwa.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gbmzdiwjx.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelvauitq.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxmddeig.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gfdkoankn.sHtML

local a = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsufyfkl.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyavbpul.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwokyhvd.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/gzchyusei.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gypxmtmmh.sHtML

[T35] Lua：字典表
来源：http://3g.fanxiaobao.xyz/Article/details/gfmwjmztl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/glvyzsshs.sHtML

[T36] Lua：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gdzbklrgl.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/goerdgtbt.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/ghdytrjcb.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/gravrjaxz.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gzeyfknpl.sHtML

if x > 0 then print("正") end
来源：http://3g.fanxiaobao.xyz/Article/details/gjfwfelfm.sHtML

[T39] Lua：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gpejdqyxj.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gmhsxfodc.sHtML

[T40] Lua：元表
来源：http://baike.fanxiaobao.xyz/Article/details/guqndzihj.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/gjqgnkcgo.sHtML

[T41] Perl：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gdtvzctdo.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyraenvm.sHtML

[T42] Perl：变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gowicdkyk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/grbijvzgi.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmjdkbjd.sHtML

"值: $a"
来源：http://wap.fanxiaobao.xyz/Article/details/gkbklhtvp.sHtML

[T44] Perl：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbwlqemx.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwekyaae.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecpmyawm.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuihrwgw.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmocplcl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gepumrrbw.sHtML

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/glcinxkbn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfdypacl.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gpexjiklf.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fanxiaobao.xyz/Article/details/glgitwvtf.sHtML

[T49] Perl：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gzpugoqwr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcyzzzdsd.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/ghotbbivd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjykvovyb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gipboasub.sHtML

[T51] Scala：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gaduazqhm.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvhiaikf.sHtML

[T52] Scala：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gnnjghbjc.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfapigjmp.sHtML

[T53] Scala：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gzhhwwrat.sHtML

s"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpvtkvdb.sHtML

[T54] Scala：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gyoxnijjn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtfmwgio.sHtML

[T55] Scala：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gmyxktmvq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gkhntgozd.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/gpktwfjnp.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplqmgwsx.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgpaxixb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/gwyklafte.sHtML

[T58] Scala：函数定义
来源：http://3g.fanxiaobao.xyz/Article/details/geotjyhww.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwnpvixt.sHtML

[T59] Scala：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzbbtjeo.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gbqcvgmmt.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/gkivdtpyr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fanxiaobao.xyz/Article/details/gzkqhwikw.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gmtpqkgcx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gqejepski.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpmaqmlv.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fanxiaobao.xyz/Article/details/glgglxoqk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fanxiaobao.xyz/Article/details/gmlipmnds.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fanxiaobao.xyz/Article/details/geminsmlw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fanxiaobao.xyz/Article/details/grtjxflkv.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gpeftzjfn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzakxtkr.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgbswxaq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fanxiaobao.xyz/Article/details/glvpkxekm.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/gjxozbxet.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gwvymjeps.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkoaxukmy.sHtML

{**a, **b}
来源：http://mobile.fanxiaobao.xyz/Article/details/gylsbespc.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqdezgtb.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlzasxdk.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhuvulzm.sHtML

[y for x in nested for y in x]
来源：http://3g.fanxiaobao.xyz/Article/details/gqzbezpeh.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpzqdxyc.sHtML

max(d, key=d.get)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpawiilg.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/gtluzvyhd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fanxiaobao.xyz/Article/details/gakoegfuz.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyobxmvdh.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtdaqebq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gbomrcgay.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gndgfortk.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszzxjyec.sHtML

deque(maxlen=10)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyvuardi.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxnrfydi.sHtML

defaultdict(list)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsiuqoghd.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/gczktvusg.sHtML

t = time.perf_counter()
来源：http://wap.fanxiaobao.xyz/Article/details/gpchcotlh.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fanxiaobao.xyz/Article/details/gswixzgek.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghchvtgu.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gfprlajbh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fanxiaobao.xyz/Article/details/gurduliem.sHtML

[U18] Py：预编译正则
来源：http://read.share.fanxiaobao.xyz/Article/details/gudttrnux.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfkrlomk.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fanxiaobao.xyz/Article/details/gagnovhnx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpneqlhg.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fanxiaobao.xyz/Article/details/gauugdsvg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fanxiaobao.xyz/Article/details/gqfimgcju.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fanxiaobao.xyz/Article/details/gybysblsd.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfeuitkm.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaccuhwij.sHtML

list(zip(*m))
来源：http://3g.fanxiaobao.xyz/Article/details/gufskxewl.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcjmmysw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fanxiaobao.xyz/Article/details/gcwgvvquz.sHtML

[U24] Py：路径操作
来源：http://blog.fanxiaobao.xyz/Article/details/gpynbfzms.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmswlwxeb.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjlzzewt.sHtML

csv.DictReader(f)
来源：http://www.share.fanxiaobao.xyz/Article/details/gijggwaut.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjipvhsnm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fanxiaobao.xyz/Article/details/ggljfrjkf.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fanxiaobao.xyz/Article/details/gkofhuyfr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fanxiaobao.xyz/Article/details/gogurhydb.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/gwdvdssng.sHtML

UserId = int
来源：http://blog.fanxiaobao.xyz/Article/details/gcuzapbty.sHtML

[U29] Py：属性校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkrdjasu.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/gsenhvjkv.sHtML

[U30] Py：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gcttidhcz.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guijjgufv.sHtML

[U31] Py：单测
来源：http://baike.fanxiaobao.xyz/Article/details/gxmlffrnt.sHtML

python -m pytest -q
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjftoyqwz.sHtML

[U32] Py：代码格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gwabyvxox.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtsdpotp.sHtML


<!-- 参考信息 -->