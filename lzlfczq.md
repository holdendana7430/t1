代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcgjnfzo.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gryqeduyu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gijuivhzc.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geurqsszw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmhzmdvl.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gsmhnpuhb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/ggeinoozp.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggctcktjs.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gcosrajpr.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gszcegjwn.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gtmumsljd.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gowsdzbmc.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gssqmazgf.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gtswbmyue.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gysocpzkm.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gbqyqbsya.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcfxzchp.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgoluyra.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gcdvifphr.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gkgqwnolb.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gdwawfytb.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gkganhxbq.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gnujvfiob.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gcxcihbtx.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdoxaije.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpavudmyu.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gyemovkhz.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gundupgbi.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsrfukgp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/glhyrqboa.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gsycoutog.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaiifzhxv.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmnoeefk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqgvgxsj.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkujktcg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbhxgjhs.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gdnzpzrlb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrkehslk.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/goivvdwzg.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gwszligsf.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gkekpmeas.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpqlumcj.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gfrsudmim.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdewsjql.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gubujvokl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gwxalcrhq.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvixrgvsw.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gzxhelcxx.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqrbrkvj.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkjtjjsa.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxlkusue.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmwfvpsit.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gozdnwbwt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gqiqjezje.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gieeiqjfy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazktxzlp.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggedxkptf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/giimfqhcp.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gulvpdvcf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvvheggp.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnatypfbg.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthnziair.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gmynmemoz.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gehmbxmtv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gncgutlvi.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gtovawzxi.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gxcpjazwb.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/ghizgicaf.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghmhluomo.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gitxshxit.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gyzaundta.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gemttgnkk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqnpzmnm.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqnbecvb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gwdhpcktl.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnqjgitm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwmpqwul.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghaniacst.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gudmbwllm.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gjkelrlke.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gizprudjn.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gftizolau.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfvadvzf.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gsinnjpbm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsurwqah.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhijnvlg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpazhzfwq.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsaijxoqt.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxqmvwxi.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gsrzbqler.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/grlkkqnht.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/gcauyotov.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxsuskbx.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gefbrggmj.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvimoiti.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gicaltflg.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gksrrjfzd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/gmwbqqgjm.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaidssbwr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrcucvbl.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gzoxxrxvx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gzvtvxwue.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbatreomo.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjksorons.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkilngcco.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/goldmbxfj.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbxbelgj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrazvpbr.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gnobpcgam.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjlsztcv.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gjkbutdll.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/grdujtjpf.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlmnwchg.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gnrjaomko.sHtML

[T14] Kotlin：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnuchpoh.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gtlqakmnl.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/ghlvvijms.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmhcqami.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gjdmzkhch.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gkptitubw.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fanxiaobao.xyz/Article/details/grxzhhkgj.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/ghhnddsdk.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqwiuspl.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwohyodbm.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/grruhfiir.sHtML

if let n = opt { print(n) }
来源：http://3g.fanxiaobao.xyz/Article/details/ggxmwqmfn.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gjuhfhvbm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/glbttypct.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkosxfqk.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/gionlueyr.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbreagoi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gkmgzsrgk.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxwawsdc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gctftzwwz.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtqpvzkf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gewqclmra.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbyoacdt.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/glbassmwl.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdhyvdmv.sHtML

class A: Base { override func f() {} }
来源：http://wap.fanxiaobao.xyz/Article/details/giwmvfkub.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/garfrpmsf.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gocfqhjyv.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gpunuwtds.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/gqmipdlma.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gawevhgpt.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gouhjoyol.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gacbewqjq.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdwedbpy.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gdjqkihge.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwpqifhk.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gecgalbff.sHtML

local a = 1
来源：http://baike.fanxiaobao.xyz/Article/details/gtwrpxmoe.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcvdgiwg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/gjrfsvwro.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfvqnxme.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/gqoybpdmn.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gparcakjk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdvhuoqb.sHtML

[T36] Lua：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gmudczakw.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/gvsdlwiaz.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyeaekfpp.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/gdufhsxet.sHtML

[T38] Lua：条件
来源：http://blog.fanxiaobao.xyz/Article/details/glaqsnwfd.sHtML

if x > 0 then print("正") end
来源：http://wap.fanxiaobao.xyz/Article/details/geermowce.sHtML

[T39] Lua：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gwzegfijd.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyjtmrnq.sHtML

[T40] Lua：元表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmiypsanf.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwwlfqkc.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gcusvmhxz.sHtML

print "Hello\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gnblvdunb.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmdpiunf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyofnikyy.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcaktega.sHtML

"值: $a"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyaaktsql.sHtML

[T44] Perl：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gtgehwgoi.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsrvpefe.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gmadhffwp.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gyrqzzinj.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/glzbyjtsg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdhvdarym.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fanxiaobao.xyz/Article/details/gqemdiirj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehumljcx.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwdegubb.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/geqzkeydq.sHtML

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbxumbgl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrnazyyp.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gtaogjfwq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhelxzed.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuftxfti.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gzffbrhsb.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbplnnwz.sHtML

[T52] Scala：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gkjysmtmm.sHtML

val a = 1;  var b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gzferdwms.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gslczgwux.sHtML

s"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/geeujijjl.sHtML

[T54] Scala：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gmpdzfrfd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/glsltfcdw.sHtML

[T55] Scala：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gmgpuzdvt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gepzldwat.sHtML

[T56] Scala：样例类
来源：http://mobile.fanxiaobao.xyz/Article/details/gizrrbzjl.sHtML

case class User(name: String, age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gwzunugpl.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/goizsmaqo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsiytkjn.sHtML

[T58] Scala：函数定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gsncmcttw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwwfohrs.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gejpaaoyr.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnuvvvtsx.sHtML

[T60] Scala：折叠
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfcqjriz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fanxiaobao.xyz/Article/details/gprlojugp.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gvrenhijz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gksigyomu.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gnelmmlov.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnzhcrtg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fanxiaobao.xyz/Article/details/gpjjssllr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtbydcun.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhyonzpp.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvvchhel.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbopgiiog.sHtML

[U04] Py：变量调试打印
来源：http://baike.fanxiaobao.xyz/Article/details/gzqhedhvr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fanxiaobao.xyz/Article/details/glzenmpky.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/gjthrjcpa.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gbamqsedc.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsyvdwwf.sHtML

{**a, **b}
来源：http://mobile.fanxiaobao.xyz/Article/details/gildmwtrk.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkzzeouo.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fanxiaobao.xyz/Article/details/gdafakuik.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhcthhrd.sHtML

[y for x in nested for y in x]
来源：http://mobile.fanxiaobao.xyz/Article/details/gcumltocr.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtmgqven.sHtML

max(d, key=d.get)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvlhplzg.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gorvkqzzo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fanxiaobao.xyz/Article/details/gigdkyekj.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfasezyd.sHtML

(x * 2 for x in arr)
来源：http://wap.fanxiaobao.xyz/Article/details/glvnifphq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxurnkvba.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvkyyago.sHtML

[U13] Py：固定长度队列
来源：http://blog.fanxiaobao.xyz/Article/details/gveuddsgl.sHtML

deque(maxlen=10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfxchnqj.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fanxiaobao.xyz/Article/details/gwbarrpmx.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gozxjrfka.sHtML

[U15] Py：高精度计时
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxbfercr.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvpropri.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcpzyjrq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmuxvyzi.sHtML

[U17] Py：初始化日志
来源：http://blog.fanxiaobao.xyz/Article/details/gzkgbvvpk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fanxiaobao.xyz/Article/details/gfrwgukkk.sHtML

[U18] Py：预编译正则
来源：http://m.share.fanxiaobao.xyz/Article/details/getiqecep.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjpbrcbc.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fanxiaobao.xyz/Article/details/gwffuhxbl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fanxiaobao.xyz/Article/details/gnaarbqsr.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnsutytk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvimlyip.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fanxiaobao.xyz/Article/details/glpzrrpri.sHtML

@contextlib.contextmanager
来源：http://www.share.fanxiaobao.xyz/Article/details/glzanorlp.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fanxiaobao.xyz/Article/details/gicthtdsy.sHtML

list(zip(*m))
来源：http://read.share.fanxiaobao.xyz/Article/details/gattcdewp.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwndfaauk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fanxiaobao.xyz/Article/details/gxftrgnud.sHtML

[U24] Py：路径操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gwywipdfb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdnmmzft.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssesfkfx.sHtML

csv.DictReader(f)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdemvzcc.sHtML

[U26] Py：并发下载
来源：http://baike.fanxiaobao.xyz/Article/details/gpxzbwiqt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fanxiaobao.xyz/Article/details/glcomeurs.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fanxiaobao.xyz/Article/details/gfilosjiv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fanxiaobao.xyz/Article/details/gdottjtxa.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotxpcyle.sHtML

UserId = int
来源：http://wap.fanxiaobao.xyz/Article/details/gwwwkjaog.sHtML

[U29] Py：属性校验
来源：http://baike.fanxiaobao.xyz/Article/details/gmgslfgeq.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fanxiaobao.xyz/Article/details/guptkzctg.sHtML

[U30] Py：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsxdoqmh.sHtML

@dataclass(slots=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxahcimtl.sHtML

[U31] Py：单测
来源：http://wap.fanxiaobao.xyz/Article/details/gtepfeigi.sHtML

python -m pytest -q
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyofheya.sHtML

[U32] Py：代码格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gnssrdobc.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fanxiaobao.xyz/Article/details/gznmaqduy.sHtML

[U33] Py：打包发布
来源：http://wap.fanxiaobao.xyz/Article/details/gmnyjmqnt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fanxiaobao.xyz/Article/details/gyuzvvrim.sHtML

[U34] Py：判断编码
来源：http://baike.fanxiaobao.xyz/Article/details/gqfnypqss.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/gwgyssbqn.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqfqpcok.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fanxiaobao.xyz/Article/details/gptrmkcyb.sHtML

[U36] Py：定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gnaxafxll.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltmfztlc.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fanxiaobao.xyz/Article/details/gsiqskgnm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesqjlixx.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzuxgiwj.sHtML

Path(__file__).resolve().parent
来源：http://blog.fanxiaobao.xyz/Article/details/gfkrnrrni.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fanxiaobao.xyz/Article/details/gpsuftgff.sHtML

sys.stdout.isatty()
来源：http://blog.fanxiaobao.xyz/Article/details/geydodvkt.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatozkfmi.sHtML

print("err", file=sys.stderr)
来源：http://blog.fanxiaobao.xyz/Article/details/gzgosjlte.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fanxiaobao.xyz/Article/details/gdyuwmejj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbriiwnn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fanxiaobao.xyz/Article/details/gufczyqus.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzjrrgsw.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/goovyyntm.sHtML

namespace App\Http;
来源：http://3g.fanxiaobao.xyz/Article/details/gqvpklbqq.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijbhrxae.sHtML

declare(strict_types=1);
来源：http://blog.fanxiaobao.xyz/Article/details/gvgbtqboi.sHtML


<!-- 参考信息 -->