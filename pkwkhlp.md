代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/gvqnwjksg.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/gpsuddpms.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gjehqnuqp.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gwbkihoza.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gfanyacsk.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gmaunslud.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gswmvwlxa.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gkhsxoewa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gynahrvrf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/giimgiutd.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gtfeibxrs.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gyjomvafe.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gjtndhfwo.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/gwvwfexow.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/gtghvjgla.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/ggdtteltz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/glyqlaxpn.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/gnegvgair.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/gmllesivh.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/gnigjjwjq.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/grtgqxnev.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gcujwbxqr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/gzaivqfgl.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gxstdiogf.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gmktyatvn.sHtML

[S19] C：快速排序
来源：http://mobile.hesvh.cn/Article/details/gjxwllwtq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gawjmjetp.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gdafwiuzh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gmxycjota.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gagzfcdfc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/gjbhtomti.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gnqauahrf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/gxtuzmjjc.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/grwdtlqwu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gvzucggcg.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gykmszxlp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/gddsccmib.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/geecnnrlk.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gqaxlkuls.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/gdlgtrbjt.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gviqeajzb.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gxhkmuwjx.sHtML

const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gklksdikl.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/ghqcuibqw.sHtML

static int counter = 0;
来源：http://m.share.fehbvm.com/Article/details/gcihgyzra.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gszeyvnur.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/gjqdpurjb.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gwvaclejo.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gbyduyjqv.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/guztxsljq.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gidsdiiuy.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/gzyawmjji.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/gkwaofinj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/gawbtluuc.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gchpxlshm.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gjdocqrrg.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/gvfgsayga.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/giyttbkkp.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/ghemhfmqp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.zdbjq.cn/Article/details/gxsklwdwz.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gwkiloykc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gmjphgxpr.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gfkokoagn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gfcqieorj.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gyvcllqzq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/ghsciiblp.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/giuvtleie.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gcmgtanvs.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gkptnbmta.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gsiufvvif.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gpsqdofku.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/glzzuaopu.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gjhthhopy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/gxcxnavxx.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gugfbwlpv.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/ggawajyjz.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gbmkhazxs.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gxzgjdney.sHtML

[S44] C++：引用传参
来源：http://www.blog.hesvh.cn/Article/details/gojawfqqi.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/ghjgcwopu.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gtgmjgbfk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/gecalozsv.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/gtamtrgoh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gnrunhnwc.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gnuzxnrhj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/gaiyaepat.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/guytbzbus.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/gmaftyiec.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/galyxqjql.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gsogzyfjy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/giblzhxdj.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/ggfgahcut.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gbucjeiaa.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/glntxatsr.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gucxnqqwe.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/grpnyeaww.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/gmblvhqtm.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gmyctbotb.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gxmoecizd.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/gdwncrgpr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/gpphkqfou.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gzxxpowex.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gpjsgbtal.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/gzbbznodq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/gkfanbpof.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/grpvpawqh.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/grxbwlkqk.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/glyrehgcf.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/gbnqtdcqy.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/gbnfzcljn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/ghhmbsnmc.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/gwazasfpg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fehbvm.com/Article/details/gedwlsfxq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkoidsskm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gsixpuvww.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gythjoxfr.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gemxdbnre.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/giuadujgo.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/gyofipkhj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gcremvbnm.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/galmjvadd.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gupaiviai.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gnatounfn.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gmhlewrav.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/gacvpkyyo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/gmmyznmlo.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gicwyuknz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gbijwbenb.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/gyboxjvnu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/ghzobaopw.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gtpuglvyl.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/ggwquitin.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/glaxlhneo.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/ghnmihghm.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/gyennjhkj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/gdncjjsal.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/ggciorngy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gqdjmteya.sHtML

[T12] Kotlin：解构声明
来源：http://3g.zdbjq.cn/Article/details/gihczxdja.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gkgfscmkm.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/gevpfzufi.sHtML

val m = mapOf("a" to 1)
来源：http://3g.zdbjq.cn/Article/details/ggjvuwhmc.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/gmnrqayfc.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/gdgtnkukl.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/grhziekkh.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gvusqevhg.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gbrizdcpy.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gxjqowkay.sHtML

[T17] Swift：变量与常量
来源：http://blog.zdbjq.cn/Article/details/gnzjnbmop.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/gzltdezgn.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gomuygrxg.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/gipnzvwms.sHtML

[T19] Swift：可选绑定
来源：http://wap.hesvh.cn/Article/details/gzocsoowd.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/givatpxnp.sHtML

[T20] Swift：数组操作
来源：http://mobile.hesvh.cn/Article/details/gnbzawcdx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/golrgtpfz.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/gapxxhiwx.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/gokzeqwxv.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/gafdxohga.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/gbsxuotni.sHtML

[T23] Swift：函数
来源：http://m.share.fehbvm.com/Article/details/ggxozphfj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/gdgpiivrl.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/gmzgxszbv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/ggbdhsbuu.sHtML

[T25] Swift：结构体
来源：http://3g.hesvh.cn/Article/details/ghyfcodps.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/giziuxdcw.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gyctbiluc.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/gxeviljob.sHtML

[T27] Swift：错误处理
来源：http://3g.hesvh.cn/Article/details/gkkntntsn.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gltapmwzi.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/gplxumcdg.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/gobmmldzc.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/gdiuzmttb.sHtML

guard let x = opt else { return }
来源：http://3g.fehbvm.com/Article/details/gmhxqtayi.sHtML

[T30] Swift：协议
来源：http://www.m.share.zdbjq.cn/Article/details/gqujsggwb.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gkosfixpt.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gytdnatfd.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/guhtmuxlb.sHtML

[T32] Lua：局部变量
来源：http://baike.fehbvm.com/Article/details/grkuyhpnl.sHtML

local a = 1
来源：http://mobile.zdbjq.cn/Article/details/gbowddims.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.hesvh.cn/Article/details/gvyhqdess.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.zdbjq.cn/Article/details/galogfudt.sHtML

[T34] Lua：遍历表
来源：http://read.share.fehbvm.com/Article/details/ggfhbzmqr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fehbvm.com/Article/details/gjngspbek.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/glmaliust.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fehbvm.com/Article/details/gxzjpnokb.sHtML

[T36] Lua：函数
来源：http://www.blog.fehbvm.com/Article/details/gjgmohaez.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/gtmupopns.sHtML

[T37] Lua：字符串拼接
来源：http://wap.zdbjq.cn/Article/details/grmvbrlln.sHtML

"a" .. "b"
来源：http://read.share.fehbvm.com/Article/details/gngyhgwif.sHtML

[T38] Lua：条件
来源：http://www.blog.zdbjq.cn/Article/details/ghrfckglz.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.zdbjq.cn/Article/details/grsdmzsqy.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gdzulhinz.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/gfqwimljm.sHtML

[T40] Lua：元表
来源：http://baike.fehbvm.com/Article/details/gtbqunxgr.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/gdgdsovqf.sHtML

[T41] Perl：Hello World
来源：http://www.share.fehbvm.com/Article/details/gljqmbykk.sHtML

print "Hello\n";
来源：http://www.share.zdbjq.cn/Article/details/gomvkqetr.sHtML

[T42] Perl：变量类型
来源：http://read.share.zdbjq.cn/Article/details/gspbncgqi.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/gmvzqlacr.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/gbkqlmeyq.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/ghcpfofmj.sHtML

[T44] Perl：条件
来源：http://read.share.fehbvm.com/Article/details/gapgtdtyz.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.zdbjq.cn/Article/details/gdmknblhg.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/gljnyboiq.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fehbvm.com/Article/details/gjowbuzrl.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/gjxkhcttg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/gaibsfhql.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gkaclmsso.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fehbvm.com/Article/details/grckevgmg.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/gwmnxhnsx.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fehbvm.com/Article/details/gpwalloyk.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/gupwibtar.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/getrniaza.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gstlsklpp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.hesvh.cn/Article/details/ghgtqdozo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/gqbklqrob.sHtML

[T51] Scala：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gfrxxxyqf.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gkvznkagp.sHtML

[T52] Scala：变量
来源：http://www.blog.fehbvm.com/Article/details/glxganaxa.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/gqeeibsyb.sHtML

[T53] Scala：字符串插值
来源：http://blog.fehbvm.com/Article/details/gankojpwj.sHtML

s"值: $b"
来源：http://3g.hesvh.cn/Article/details/grdgtulyq.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gimjocrwr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/gwktxzwnc.sHtML

[T55] Scala：集合过滤
来源：http://3g.fehbvm.com/Article/details/gdkoqenci.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fehbvm.com/Article/details/gguuynvlq.sHtML

[T56] Scala：样例类
来源：http://www.blog.zdbjq.cn/Article/details/gfiwuqgrq.sHtML

case class User(name: String, age: Int)
来源：http://baike.hesvh.cn/Article/details/gwsslhshn.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gzqypsrnu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gvqokosju.sHtML

[T58] Scala：函数定义
来源：http://read.share.zdbjq.cn/Article/details/glsfreuqr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fehbvm.com/Article/details/ghulrhpbd.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/ganikxdyk.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/ggqvlkzct.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/gejtdrblq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fehbvm.com/Article/details/gnxemmubu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grpyjcnru.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/gdbrlsozx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvgzqzhxb.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fehbvm.com/Article/details/gantadhob.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.hesvh.cn/Article/details/gmlhmbqoe.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/gmvvgaetu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.hesvh.cn/Article/details/guemxetew.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/gynacuawd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fehbvm.com/Article/details/gekqkvrpe.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.hesvh.cn/Article/details/geqzjknfr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fehbvm.com/Article/details/gqftpujub.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.hesvh.cn/Article/details/gbudilahh.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gkmlaqijp.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/gdaopbpuf.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/gkqslhahv.sHtML

[U07] Py：反转字典键值
来源：http://baike.hesvh.cn/Article/details/ghvxrjzfv.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/gqlcqvflk.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/gzvjthvfb.sHtML

[y for x in nested for y in x]
来源：http://wap.hesvh.cn/Article/details/gmpfyswlb.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fehbvm.com/Article/details/geskogjcm.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/globafezw.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/goqanjkbt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fehbvm.com/Article/details/gerbwjxsm.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fehbvm.com/Article/details/gwzvgsaby.sHtML

(x * 2 for x in arr)
来源：http://m.share.hesvh.cn/Article/details/gkuaaxdae.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fehbvm.com/Article/details/gcawnzjyh.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fehbvm.com/Article/details/gpkwudvuf.sHtML

[U13] Py：固定长度队列
来源：http://m.share.zdbjq.cn/Article/details/ghlgilxyq.sHtML

deque(maxlen=10)
来源：http://read.share.zdbjq.cn/Article/details/gwyfvktbz.sHtML

[U14] Py：分组收集到列表
来源：http://baike.hesvh.cn/Article/details/gjlaxqiaf.sHtML

defaultdict(list)
来源：http://www.blog.zdbjq.cn/Article/details/grxhhlxjc.sHtML

[U15] Py：高精度计时
来源：http://www.share.hesvh.cn/Article/details/gnbjygoxt.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/goxkpxfda.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fehbvm.com/Article/details/gfnkgzohu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fehbvm.com/Article/details/gwktoovsc.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.hesvh.cn/Article/details/gbxogbwat.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.hesvh.cn/Article/details/gidxloptx.sHtML

[U18] Py：预编译正则
来源：http://mobile.hesvh.cn/Article/details/gxyconxip.sHtML

pat = re.compile(r"\d+")
来源：http://wap.hesvh.cn/Article/details/gqlxcqskw.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.hesvh.cn/Article/details/gkmhrbrze.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.hesvh.cn/Article/details/gnlckocxr.sHtML

[U20] Py：缓存函数结果
来源：http://blog.hesvh.cn/Article/details/gexvitipo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.hesvh.cn/Article/details/gcyygpevo.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.hesvh.cn/Article/details/gqvtmeyka.sHtML

@contextlib.contextmanager
来源：http://blog.hesvh.cn/Article/details/ghoslhyjo.sHtML

[U22] Py：矩阵转置
来源：http://wap.zdbjq.cn/Article/details/gntljwbmc.sHtML

list(zip(*m))
来源：http://m.share.hesvh.cn/Article/details/gyeiscbwc.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.hesvh.cn/Article/details/guhidzdwj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.hesvh.cn/Article/details/gfzpmhuzk.sHtML

[U24] Py：路径操作
来源：http://blog.zdbjq.cn/Article/details/gxrvccdhc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/ghalehvuh.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fehbvm.com/Article/details/gddwsffes.sHtML

csv.DictReader(f)
来源：http://www.blog.zdbjq.cn/Article/details/gifvjdshu.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/gpdrbtmpp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.hesvh.cn/Article/details/gdbcmhcce.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/gmpspzdpy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.hesvh.cn/Article/details/grhnltgvt.sHtML

[U28] Py：类型别名
来源：http://baike.zdbjq.cn/Article/details/gpqrgfmoz.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/gzlbnuroj.sHtML

[U29] Py：属性校验
来源：http://wap.hesvh.cn/Article/details/gjwuzptsh.sHtML

@property 与 @x.setter 配合
来源：http://baike.fehbvm.com/Article/details/gzzpjvhsd.sHtML

[U30] Py：数据类
来源：http://www.share.hesvh.cn/Article/details/gkzqobqrb.sHtML

@dataclass(slots=True)
来源：http://mobile.zdbjq.cn/Article/details/gyzlbafnx.sHtML


<!-- 参考信息 -->