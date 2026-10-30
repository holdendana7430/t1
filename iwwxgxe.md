代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydghshie.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gknmkftrp.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gaftakyic.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxnpldzg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gvzqzwecp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdkxoqzu.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggojfjpex.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfhttpba.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnjkgnwl.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gltjluzth.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpvdjlfy.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gtyconcqj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/grkhrfqhs.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gbqyehlau.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/garticpav.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgujpoks.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/ghlyiorpd.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkvvhrwl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmipuwar.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/geotfffmq.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzozqymcq.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gktpqdknr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykxriigm.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/glcrrlozr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/ggutrggxi.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gktqwvgsw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gbdslwuyg.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjwzvyqs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjmktegq.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gknswkuch.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyoxbxmig.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/ginxcavog.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmtqsqwg.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gpynzgohv.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdtdfpky.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/guzrctdxt.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gbaqptmlz.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjahjmhiu.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlzjxfqt.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/ghlncicvz.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrrroczj.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmejknvhx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gepcjyaai.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gesivrewq.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gvvzysumd.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gkgoddvrn.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmachnya.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gnoywbhtv.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/girafrtwn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gliarwdsu.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/guuwlghpl.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gengqcgbc.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtegtiiip.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghaueukrt.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/ggydmngev.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gyidkxcxd.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlwjyoay.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gutoojliz.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gxowgscnj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghthswohy.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzfjexqf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxmnvsio.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gntknjsee.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnoamcyb.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbzjpztw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfvrfpuh.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gegwkndzz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gohfetcin.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjahlaphn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gybnsrohd.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqmgvcmn.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxexryke.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gangzwprx.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gmdlkzhuu.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzdmitzt.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxucogcp.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkbfitvi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwewaccvv.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbgijatr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkafgeomn.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzgsaxjo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgrkriup.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gfrjvxuet.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxdiebdh.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepwzymxj.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gtvojxfvy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gvlvgkqed.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/glsqzyzog.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gxtemmium.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhnfzdsp.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gdunlqkmy.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwoduvge.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpbmxbgp.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gpytltgxk.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfrqtmse.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/grikokwor.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gfawmfeli.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gjphywlcc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhdhfmyg.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gjrtzxjyk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gczlhgfee.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gykjbpvop.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxxczxjr.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gqylwjlpk.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgdsvshn.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gngwfajch.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gzsqnfbul.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gssscnmbl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkztvfypp.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpyhkrlc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfesuiaa.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/guftedutz.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/ggcoldccf.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gyuiqibdi.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbjhsapa.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gscppobus.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gltvihnwi.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gokdbyili.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkgcxeww.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxmfocip.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gadagbsed.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnjizwcl.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gmnfgtlbu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gdlcriupn.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gxlpiralc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnwyvccb.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gpyezygmj.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqvvwgam.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtqpfpll.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/gatuukrxy.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gbzprsmpz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/gargqsjhk.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkkltzel.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxocedfr.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/geybpqqgi.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gxhvqqskx.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/ggctjjepp.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gjaomytrj.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/ggftjtzir.sHtML

for (i in 1..10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gjtczwohv.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkbrbtvf.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqmmjayq.sHtML

[T16] Swift：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gwowwmycn.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/guhykihmm.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gmaptpjdb.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gickjphxp.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsczmkoax.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gtchqzlbe.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/goryimhzq.sHtML

if let n = opt { print(n) }
来源：http://3g.fanxiaobao.xyz/Article/details/ggjnraaub.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkdxslhw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gxbfaxfly.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gehvqnbqp.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/gjfvgcloc.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpicqrtc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giskkyqjx.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpoaxzpv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gscasckgu.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gybyahwgt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gkjyjnthz.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxvvvwvs.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzojcmjwe.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/ghkkxlwzv.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkuikstz.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrsblddi.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/gobuvtntu.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfoowmsue.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/guwyvdnrd.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/gxmhfbmmp.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gixcmscru.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/ggaizjkbi.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gvjtuatly.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gbvpjwmvj.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdoswgbyu.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcjvvoap.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gplensmys.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqdbpxhr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgzglrtp.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/gfkeammtb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fanxiaobao.xyz/Article/details/gephryqtn.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxpykemu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gnbwatsdf.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcherxxy.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gbgspbgms.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gbmxrgytk.sHtML

"a" .. "b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcchcnos.sHtML

[T38] Lua：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gcubwzhzo.sHtML

if x > 0 then print("正") end
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbwwyyoo.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gnkkagiff.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/guogdoydu.sHtML

[T40] Lua：元表
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmaqucig.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyfwtjow.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzbdwqsu.sHtML

print "Hello\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grucrsorx.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxzegtcn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gaowagsgs.sHtML

[T43] Perl：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gfmskelgq.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/giqlhfywj.sHtML

[T44] Perl：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gwqtnoann.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhntjvhh.sHtML

[T45] Perl：数组遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gkuyqplpw.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzhfydid.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/gnaabagon.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkvrgqqtr.sHtML

[T47] Perl：正则捕获
来源：http://3g.fanxiaobao.xyz/Article/details/gtwglrpfs.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpehvaupj.sHtML

[T48] Perl：正则替换
来源：http://m.share.fanxiaobao.xyz/Article/details/giqrqvfxc.sHtML

$s =~ s/old/new/g;
来源：http://wap.fanxiaobao.xyz/Article/details/gwxynzkzs.sHtML

[T49] Perl：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gailgcnew.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsjyaozbz.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/glfjylmrh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpfdmled.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fanxiaobao.xyz/Article/details/gykvfqtux.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvybgfjl.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gzvsptdwm.sHtML

[T52] Scala：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqwsxula.sHtML

val a = 1;  var b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkrcdorn.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggabyjvtr.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/ggchvsoqo.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwfugjws.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvgyztwo.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gplgufbbe.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/govehogpk.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/gurboeeqa.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/glvzykhhl.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gnxqgsmne.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/gduwjsacf.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/gsvwzcgxo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvbmwjyy.sHtML

[T59] Scala：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gzqpbnnsd.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbdslssm.sHtML

[T60] Scala：折叠
来源：http://blog.fanxiaobao.xyz/Article/details/ggrxyhbhu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fanxiaobao.xyz/Article/details/gafmbskdd.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxknmbabk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gybtcdauc.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ghohftrdt.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fanxiaobao.xyz/Article/details/guqeuvgbb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclqdeqeq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fanxiaobao.xyz/Article/details/gctruirxa.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gcrfxlpzw.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpujznxr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsdgspfz.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fanxiaobao.xyz/Article/details/gnryqbyep.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fanxiaobao.xyz/Article/details/gbhphecug.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/gnihcrgma.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/geosbdujo.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdrtfxhm.sHtML

{**a, **b}
来源：http://baike.fanxiaobao.xyz/Article/details/gwmvevfdi.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fanxiaobao.xyz/Article/details/geiqsztht.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/gwgqyslro.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuxhmdqs.sHtML

[y for x in nested for y in x]
来源：http://wap.fanxiaobao.xyz/Article/details/gyebtequp.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fanxiaobao.xyz/Article/details/gobbnvtfq.sHtML

max(d, key=d.get)
来源：http://baike.fanxiaobao.xyz/Article/details/gjnhzgmho.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fanxiaobao.xyz/Article/details/grjpjphuy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fanxiaobao.xyz/Article/details/geolwgwmf.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxftvlhw.sHtML

(x * 2 for x in arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gxlmogaos.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fanxiaobao.xyz/Article/details/gctybmopm.sHtML

Counter(arr).most_common(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gdzcgupvr.sHtML

[U13] Py：固定长度队列
来源：http://baike.fanxiaobao.xyz/Article/details/gutzcbocf.sHtML

deque(maxlen=10)
来源：http://blog.fanxiaobao.xyz/Article/details/gjhkztfhp.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhtinvoc.sHtML

defaultdict(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhqzrfut.sHtML

[U15] Py：高精度计时
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfxyhsqi.sHtML

t = time.perf_counter()
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfqzffae.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwbwovjr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzcofjtv.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/guebawohj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fanxiaobao.xyz/Article/details/gittmyyph.sHtML

[U18] Py：预编译正则
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmwpexlc.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gyhctphhg.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpvrfwcq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggifusflp.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fanxiaobao.xyz/Article/details/gisztfdwh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fanxiaobao.xyz/Article/details/gyzeaxcgu.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fanxiaobao.xyz/Article/details/gsmgjybht.sHtML

@contextlib.contextmanager
来源：http://baike.fanxiaobao.xyz/Article/details/ggstcwhuj.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzofzquz.sHtML

list(zip(*m))
来源：http://blog.fanxiaobao.xyz/Article/details/gotzfkysp.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtoiupoy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fanxiaobao.xyz/Article/details/gfppxlfiq.sHtML

[U24] Py：路径操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gckxdlpjs.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gvvwueuql.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fanxiaobao.xyz/Article/details/gpheedivx.sHtML

csv.DictReader(f)
来源：http://baike.fanxiaobao.xyz/Article/details/gxfemyunz.sHtML

[U26] Py：并发下载
来源：http://baike.fanxiaobao.xyz/Article/details/gwuffidao.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fanxiaobao.xyz/Article/details/gvxsqozep.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fanxiaobao.xyz/Article/details/gqanumpef.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnggjfpz.sHtML

[U28] Py：类型别名
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtdzrebo.sHtML

UserId = int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagntpzdr.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpbzrunn.sHtML

@property 与 @x.setter 配合
来源：http://baike.fanxiaobao.xyz/Article/details/gyxczdnzz.sHtML

[U30] Py：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gudgkkeuv.sHtML

@dataclass(slots=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgxwjinv.sHtML

[U31] Py：单测
来源：http://mobile.fanxiaobao.xyz/Article/details/gofwvbzas.sHtML

python -m pytest -q
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvcmavvw.sHtML

[U32] Py：代码格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gtawleqju.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzpelaap.sHtML


<!-- 参考信息 -->