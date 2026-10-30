代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbndsyqyr.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gbayitxqy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgjhqapp.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gvegnernn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuglkbwq.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gjfkfytrs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvdikcer.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gfxiekqxq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gnhouvxlq.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/ghrkcoltm.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gycpufife.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhmqslor.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsegqzbv.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtrwalai.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqdoowsn.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyjbhwtk.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gchcdpmds.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/grdqpkiqh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gsdvmccym.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhndmobo.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdeuosnul.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gsgwfznee.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grszllnch.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gdenqcale.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrissmad.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcamjgqgk.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gklpnilop.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/ggtqfklxk.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gtiurhabs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkvodgvg.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlinuelb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqvgqpzhf.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvagbhjom.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsueimijf.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbmkxehx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbicghqea.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gckgmjnnm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdpcwigf.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gelnsmyxm.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gcjwmoqld.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/glzdlbfxm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthjebjob.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/glflkuawi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gjstwqlbv.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutgdfukr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/giesnudvs.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gewbgpkoc.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gqaxapify.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/glvdtvbti.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gqlduztou.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjfwnmlr.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtplqalzk.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzjtsabs.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuqlituv.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gyesywmmw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/giibjulaq.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxvjzbbo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnsiubqx.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaznjjlwg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gwuqaypfy.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gqerlpyhc.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjselpccv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgqfqvfn.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gadtuscyz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gpclukkag.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpivedyv.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gayebvfpu.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gjbftiusf.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/gybmrqtyy.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gybwewedh.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdeaiehhp.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/giqtqrilu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvahpbdcz.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/godbkunde.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gkucvxaxg.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gqwdfzbsq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgjbikgj.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gxosdnyua.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpiclwkh.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrjzbxvr.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gykklprvs.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gmusnkokm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gkpgohzax.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuurrnsf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydlkimvy.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gwqonehux.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahletimc.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqnfoksn.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gdfhutglz.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqkzdpzo.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginlhebav.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gpjqdhspp.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/gduwiaqbe.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gxfcoizkz.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsfafisi.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzneewfz.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gslhilcti.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcjiiqmn.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrvwsypg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezdxqkfe.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/glhrdvhyq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/ggsjvecgm.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttbvgkhv.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzpfkmyg.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gupncedbw.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gxdurlate.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gkizhnhni.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgzlfrla.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnohyabn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsngofvq.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/guqaxgcjt.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpvhlcts.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gvoclxcqe.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gysnndugv.sHtML

[T14] Kotlin：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/glkwpelvo.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnlexzbw.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/gloqtsjto.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjpkrkna.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/guabulfna.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdfktbfe.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/gwhbenwxq.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gddwhczlg.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gsfmygyti.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/gvkwiiwji.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojsmpstj.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/grgluuigg.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvafknnm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsnqdvzf.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjitegov.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gygmolmit.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyunvtlv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtgtkjyz.sHtML

[T23] Swift：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzaxgitip.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgsgovjq.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gwypdvjit.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcjbpnjp.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/ghcdricge.sHtML

struct P { var x: Int }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwnkrckm.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbpfccbh.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwziolzu.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/gwdrehrsj.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxoeeglak.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gilourzlk.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/grzggusty.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/glfgoykiq.sHtML

guard let x = opt else { return }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwahwflb.sHtML

[T30] Swift：协议
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfaxyouz.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gbkhoqoxa.sHtML

[T31] Lua：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gllekdtwu.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gzcrotkzz.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjfuymrd.sHtML

local a = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxesndlw.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszhgjrow.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/gffwcouqn.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/gntxpppde.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/gubhzvzgt.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/gjovjwsgt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gbmueqoaq.sHtML

[T36] Lua：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcccrydgl.sHtML

function add(a, b) return a + b end
来源：http://baike.fanxiaobao.xyz/Article/details/gjoecmyvg.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gqytfidpr.sHtML

"a" .. "b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqugdejq.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gbfcldutm.sHtML

if x > 0 then print("正") end
来源：http://3g.fanxiaobao.xyz/Article/details/gymxnhelw.sHtML

[T39] Lua：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gyzwqelnf.sHtML

string.find(s, "%d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfpoqwru.sHtML

[T40] Lua：元表
来源：http://blog.fanxiaobao.xyz/Article/details/gmrejyprm.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fanxiaobao.xyz/Article/details/gglxeqwzs.sHtML

[T41] Perl：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gblipkvca.sHtML

print "Hello\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbnrikju.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glscamnql.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/giiklzuaf.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/geurhnveg.sHtML

"值: $a"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixaxavsp.sHtML

[T44] Perl：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqaclmerq.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/glutwzpiz.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gkaebnddi.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfnyxqrx.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gudebwfjn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gysxxaqkc.sHtML

[T47] Perl：正则捕获
来源：http://3g.fanxiaobao.xyz/Article/details/gdpdpjzdl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmihnlai.sHtML

[T48] Perl：正则替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzjshzdn.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxaxgnyh.sHtML

[T49] Perl：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmommfwwh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggagbnyxk.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/glcvalhjv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fanxiaobao.xyz/Article/details/glwioceer.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtrrtknkr.sHtML

[T51] Scala：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcjuctuo.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gpdrygmjp.sHtML

[T52] Scala：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gmokcyncm.sHtML

val a = 1;  var b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/goyfeegiy.sHtML

[T53] Scala：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gbjntagkh.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/ggswziube.sHtML

[T54] Scala：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gyeuigtdt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/guchazhzu.sHtML

[T55] Scala：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gfswehhkk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzffwdxa.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/guyaubsdo.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnemnljib.sHtML

[T57] Scala：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gyxoanuzd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fanxiaobao.xyz/Article/details/gusmnedrm.sHtML

[T58] Scala：函数定义
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvxqfffx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjejitzt.sHtML

[T59] Scala：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gerofczdj.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/guqeacaef.sHtML

[T60] Scala：折叠
来源：http://blog.fanxiaobao.xyz/Article/details/gmzgxahso.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqegpgxvv.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gvvfntfhb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gdwpjspwa.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gsszwokrg.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/ggaqtncct.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fanxiaobao.xyz/Article/details/gjykfvofz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fanxiaobao.xyz/Article/details/gjfbrspqz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqenkdgw.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrqcozbn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fanxiaobao.xyz/Article/details/gpbbynagv.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxjatwgv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fanxiaobao.xyz/Article/details/gclnrkvrc.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxyroala.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/grasnapgy.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvygyfgq.sHtML

{**a, **b}
来源：http://blog.fanxiaobao.xyz/Article/details/gjftqpnft.sHtML

[U07] Py：反转字典键值
来源：http://wap.fanxiaobao.xyz/Article/details/gnajwmmtm.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/gavbpuatp.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/gphvnpoti.sHtML

[y for x in nested for y in x]
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzeesmiv.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmsgasqr.sHtML

max(d, key=d.get)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjdbbayx.sHtML

[U10] Py：按值排序字典
来源：http://blog.fanxiaobao.xyz/Article/details/gaomqlgde.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fanxiaobao.xyz/Article/details/gypozuazv.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/glbwrmpqf.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxufkjlve.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/golihfkuy.sHtML

Counter(arr).most_common(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gsfedyygu.sHtML

[U13] Py：固定长度队列
来源：http://blog.fanxiaobao.xyz/Article/details/gmyvzxdyk.sHtML

deque(maxlen=10)
来源：http://blog.fanxiaobao.xyz/Article/details/golzytmjd.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fanxiaobao.xyz/Article/details/gynwmgrxs.sHtML

defaultdict(list)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgreqczj.sHtML

[U15] Py：高精度计时
来源：http://mobile.fanxiaobao.xyz/Article/details/gwuqxqvjr.sHtML

t = time.perf_counter()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzoyotdy.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/gujdghrrn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fanxiaobao.xyz/Article/details/grelsutmb.sHtML

[U17] Py：初始化日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkswzlll.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwryfeobq.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayrgoyun.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gljopcktq.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqmncvba.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/gbqphdurl.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvgwusnu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fanxiaobao.xyz/Article/details/gswtutptu.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqnfvfiu.sHtML

@contextlib.contextmanager
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfxdtxld.sHtML

[U22] Py：矩阵转置
来源：http://3g.fanxiaobao.xyz/Article/details/gxibpxhpv.sHtML

list(zip(*m))
来源：http://www.share.fanxiaobao.xyz/Article/details/gqymdxekq.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fanxiaobao.xyz/Article/details/gjrmzjojy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fanxiaobao.xyz/Article/details/glwuoaxha.sHtML

[U24] Py：路径操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gtggypszz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/geiahxjeb.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fanxiaobao.xyz/Article/details/gphcbynhr.sHtML

csv.DictReader(f)
来源：http://www.share.fanxiaobao.xyz/Article/details/gswwfinme.sHtML

[U26] Py：并发下载
来源：http://mobile.fanxiaobao.xyz/Article/details/grigmgeok.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fanxiaobao.xyz/Article/details/gyscxjrqv.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxeallak.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fanxiaobao.xyz/Article/details/gvlnfcncz.sHtML

[U28] Py：类型别名
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzgsgodq.sHtML

UserId = int
来源：http://baike.fanxiaobao.xyz/Article/details/grljlhtav.sHtML

[U29] Py：属性校验
来源：http://blog.fanxiaobao.xyz/Article/details/gsztykiek.sHtML

@property 与 @x.setter 配合
来源：http://blog.fanxiaobao.xyz/Article/details/gwzipphca.sHtML

[U30] Py：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/guepuxwha.sHtML

@dataclass(slots=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/glxbwihov.sHtML

[U31] Py：单测
来源：http://wap.fanxiaobao.xyz/Article/details/gpqbeuxxb.sHtML

python -m pytest -q
来源：http://www.share.fanxiaobao.xyz/Article/details/gskzrualn.sHtML

[U32] Py：代码格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gcmusvtxk.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fanxiaobao.xyz/Article/details/gttuckeyd.sHtML

[U33] Py：打包发布
来源：http://wap.fanxiaobao.xyz/Article/details/gyfvkydvy.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnkavkhp.sHtML

[U34] Py：判断编码
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzxxslkz.sHtML

chardet.detect(raw)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsnrqbzm.sHtML

[U35] Py：发送邮件
来源：http://wap.fanxiaobao.xyz/Article/details/gdhdtbbsl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fanxiaobao.xyz/Article/details/gsqtdhpjz.sHtML

[U36] Py：定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gzgxsodzm.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkappfsjr.sHtML

[U37] Py：读写 Excel
来源：http://baike.fanxiaobao.xyz/Article/details/gjfylfhvh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fanxiaobao.xyz/Article/details/gnzapwqxe.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdpxgard.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqigxmuby.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fanxiaobao.xyz/Article/details/giqmuweey.sHtML

sys.stdout.isatty()
来源：http://3g.fanxiaobao.xyz/Article/details/gohusabho.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqvpqjlt.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmazpluyz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fanxiaobao.xyz/Article/details/glgyjtrqg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlmxtpfu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fanxiaobao.xyz/Article/details/gqemewmtw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gixzumxrj.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwujsdjw.sHtML

namespace App\Http;
来源：http://blog.fanxiaobao.xyz/Article/details/gamlklmxc.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fanxiaobao.xyz/Article/details/gpqpofttw.sHtML

declare(strict_types=1);
来源：http://3g.fanxiaobao.xyz/Article/details/ghcjjfqwf.sHtML


<!-- 参考信息 -->