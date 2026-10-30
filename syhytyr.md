代发 wailian999

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gesxpidey.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gunzvwdlq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbesjnjv.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/grrjrdthi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvgttckc.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gsmxoeipk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gituhfjnw.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gerelpuog.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/ghisxhmzp.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/galdvlxfk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqxudsyx.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gdzsvpjdl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/guxkkakit.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/goyunnavi.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmeedzkk.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvamplfu.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmdleadv.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gdeugqder.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gszfiwakd.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gcweiiiik.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqalrrpd.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gxxwjrhcp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnazxtqgy.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwdwikpb.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkcezlcj.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmsvjcvd.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gyhlgwgca.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gxytavuoa.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gidisrbbc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/goippjojx.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhofgjlc.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gcejosfiv.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gcqnvnkjo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gdjssfeam.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gfunvqfyb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjubkmvsf.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/ggfefyekd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/goiiemqrr.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gtuzelckv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gljlzkeso.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmgouxpk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gdgdnllyx.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwznfwzb.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/ghsmekhry.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfqwtuvl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gczbosift.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqctirvkd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxuzxaua.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gesxurekx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdkvmiod.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzedsfjjh.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gqhczdixi.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjecbcdjo.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvozgeyj.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gigzrlpiz.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsqkdohv.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gpgctxxbq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/ggtohhjhd.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/ggnmlayxj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdolxrdyi.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gsvskxnef.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzehtsoe.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/grvlqqgyf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/glrxcymdn.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqubgjse.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmhnqasl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxbeqytn.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjyfzaoy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjypmjltr.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gltfnmizq.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/giszydayf.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhcdmphb.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdahowyxc.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/glmdepmgf.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gkjcxudoa.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmmfwbmg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gujqsrrli.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gfpmfemdr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxisxxpg.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjfihmtv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzwofwadr.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/gujjjzjhm.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gabiojnye.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gasnmkyze.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxljjmdmf.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/grhcogevd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfrzmeom.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gizsobtfq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gcoktkikc.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpelomcz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gtaqfpvyr.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqywreelq.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmczzabaj.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/geyzbrspt.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcjyyxfa.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gullxxvkv.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfldnnkzz.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnbletfm.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/gcaygirtn.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/gotpavcvl.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gehkbsumj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gqnpzgiyk.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gnopxjnod.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gugtbuyio.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grarbcaqx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/getxytmqh.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guurfdeue.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gzntsykph.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/giexmiqqr.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzkrgdsk.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpotkgdr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlmbohxx.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/ghzfdcwqu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/glyckrzmk.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gtghlkxym.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghoafgtac.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gvugwlmnl.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcohyvzdm.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gjmqrnoje.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givubsgif.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/grkdrgfbo.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbwmqwot.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/giqvydprn.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghetbimrv.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/ghqqkyaps.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gspvlyfdv.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkrhrzgi.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnzixoob.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gvjlgxsng.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzjzzlep.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gchkdtvhk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gedgambkp.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gkxshlhoi.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkembpxz.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwfuytza.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgntgvmo.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gcgcixmql.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvvvoeqo.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gktiwofds.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyidevoty.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfcporyc.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gilodbrdq.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/gxoseslvs.sHtML

class A: Base { override func f() {} }
来源：http://blog.fanxiaobao.xyz/Article/details/ghfuvzxcc.sHtML

[T27] Swift：错误处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gtimadciv.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxbwnagf.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gevrsrpvl.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtgefhzi.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsmvffns.sHtML

guard let x = opt else { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gykmerxsy.sHtML

[T30] Swift：协议
来源：http://baike.fanxiaobao.xyz/Article/details/goeiactsn.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fanxiaobao.xyz/Article/details/glndsegni.sHtML

[T31] Lua：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gncbuejig.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvfxscay.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/ginxssruu.sHtML

local a = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmvlcgqa.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/gdykepirp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fanxiaobao.xyz/Article/details/gieslmvyv.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzpgzkyu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhtldgoe.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzhpinbf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/ggphqwjyi.sHtML

[T36] Lua：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrnleafz.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfaqqcyb.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfsefyfy.sHtML

"a" .. "b"
来源：http://wap.fanxiaobao.xyz/Article/details/ggjhvhcsh.sHtML

[T38] Lua：条件
来源：http://blog.fanxiaobao.xyz/Article/details/groosbdas.sHtML

if x > 0 then print("正") end
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsuqdnmx.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuvqpkul.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdiyyvpdh.sHtML

[T40] Lua：元表
来源：http://baike.fanxiaobao.xyz/Article/details/gfqkbytdu.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fanxiaobao.xyz/Article/details/gazinehco.sHtML

[T41] Perl：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/glxvfxeqb.sHtML

print "Hello\n";
来源：http://3g.fanxiaobao.xyz/Article/details/goqsxaaqo.sHtML

[T42] Perl：变量类型
来源：http://wap.fanxiaobao.xyz/Article/details/gwrmqdogj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gucxcogld.sHtML

[T43] Perl：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/glbzjchft.sHtML

"值: $a"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnymurrkz.sHtML

[T44] Perl：条件
来源：http://baike.fanxiaobao.xyz/Article/details/goybhavbf.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/goltpbofy.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtmeszjh.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdzvoild.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gksziltsb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpzrnxaf.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnymprsm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwtjjejvn.sHtML

[T48] Perl：正则替换
来源：http://baike.fanxiaobao.xyz/Article/details/gwictsyof.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvxzmupj.sHtML

[T49] Perl：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghyicmpsp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbkeufny.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzekaqipv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkeeverx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsavgzwbk.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkjovvso.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjurrtuf.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/grasmgfpk.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gnfzfztfz.sHtML

[T53] Scala：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/goglpplmw.sHtML

s"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtvskwnv.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvimkszl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhncgoqj.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvuxbfig.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/grejbfbmu.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/gcneuqvpe.sHtML

case class User(name: String, age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gxibrpknx.sHtML

[T57] Scala：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gkclauuxo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/gbgwudxxg.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/guxlmwdwi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/giturzylg.sHtML

[T59] Scala：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxbrrzvv.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqghmkhti.sHtML

[T60] Scala：折叠
来源：http://baike.fanxiaobao.xyz/Article/details/gpprhevqg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fanxiaobao.xyz/Article/details/gfyfjmrns.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gfzyjvrdf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdytlyut.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/glhiwkiwl.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gexlsqdjp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fanxiaobao.xyz/Article/details/grfxhioub.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbbiscdx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gpinvbojr.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/guyvnacbh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fanxiaobao.xyz/Article/details/gbitveuqn.sHtML

[U04] Py：变量调试打印
来源：http://3g.fanxiaobao.xyz/Article/details/gqanmekss.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fanxiaobao.xyz/Article/details/gshvvdbtd.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fanxiaobao.xyz/Article/details/gvahhrvei.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gnykqqdwd.sHtML

[U06] Py：合并两个字典
来源：http://blog.fanxiaobao.xyz/Article/details/glvbyddpu.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/gytegiigx.sHtML

[U07] Py：反转字典键值
来源：http://blog.fanxiaobao.xyz/Article/details/gmkudbbhc.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/gazvjsxbd.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gwezvikpf.sHtML

[y for x in nested for y in x]
来源：http://www.share.fanxiaobao.xyz/Article/details/gurkvkvxc.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvulgioxp.sHtML

max(d, key=d.get)
来源：http://blog.fanxiaobao.xyz/Article/details/gltsldmnf.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpwbywaw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqcsxufo.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gglmgdyou.sHtML

(x * 2 for x in arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gqdpalmml.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fanxiaobao.xyz/Article/details/gouqrfgna.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/grdrmudax.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpnswzjt.sHtML

deque(maxlen=10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmcktjnv.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fanxiaobao.xyz/Article/details/gjpahqcon.sHtML

defaultdict(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcmzeikd.sHtML

[U15] Py：高精度计时
来源：http://3g.fanxiaobao.xyz/Article/details/gszvgcnjl.sHtML

t = time.perf_counter()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbpblhqk.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmuodrtvb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fanxiaobao.xyz/Article/details/gzckyxrts.sHtML

[U17] Py：初始化日志
来源：http://www.share.fanxiaobao.xyz/Article/details/giflfppbv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fanxiaobao.xyz/Article/details/grklilrjt.sHtML

[U18] Py：预编译正则
来源：http://baike.fanxiaobao.xyz/Article/details/gregyvtlf.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gfokwunsj.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fanxiaobao.xyz/Article/details/gyinamrja.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fanxiaobao.xyz/Article/details/goolpcsei.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fanxiaobao.xyz/Article/details/gckmruifq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjovldcjv.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fanxiaobao.xyz/Article/details/gnzsktvlx.sHtML

@contextlib.contextmanager
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrfipcln.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwxdgwvi.sHtML

list(zip(*m))
来源：http://baike.fanxiaobao.xyz/Article/details/gvdtrzwnl.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhtdplfi.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fanxiaobao.xyz/Article/details/gbawipfox.sHtML

[U24] Py：路径操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmigcdvb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fanxiaobao.xyz/Article/details/glqakskmp.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfoiubgp.sHtML

csv.DictReader(f)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpunvugmu.sHtML

[U26] Py：并发下载
来源：http://blog.fanxiaobao.xyz/Article/details/gfhmgwbpv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fanxiaobao.xyz/Article/details/giscarunr.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fanxiaobao.xyz/Article/details/gcythkcms.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxgaflcw.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/gavtmyxcg.sHtML

UserId = int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlgkguzo.sHtML

[U29] Py：属性校验
来源：http://baike.fanxiaobao.xyz/Article/details/ghwsomccb.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvploymgk.sHtML

[U30] Py：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gnoalakcy.sHtML

@dataclass(slots=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnstsrahf.sHtML

[U31] Py：单测
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhnondbb.sHtML

python -m pytest -q
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvsbmhke.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gakuiuxze.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjrmrylt.sHtML

[U33] Py：打包发布
来源：http://mobile.fanxiaobao.xyz/Article/details/giriwiadz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fanxiaobao.xyz/Article/details/gupglobmx.sHtML

[U34] Py：判断编码
来源：http://read.share.fanxiaobao.xyz/Article/details/gupvzxvas.sHtML

chardet.detect(raw)
来源：http://baike.fanxiaobao.xyz/Article/details/gmankmfji.sHtML

[U35] Py：发送邮件
来源：http://read.share.fanxiaobao.xyz/Article/details/gciseeyll.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fanxiaobao.xyz/Article/details/gbwcbxunc.sHtML

[U36] Py：定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gisdtbhxm.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxlxylkc.sHtML

[U37] Py：读写 Excel
来源：http://wap.fanxiaobao.xyz/Article/details/gkvfswgwv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fanxiaobao.xyz/Article/details/gnjietckn.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gtppjumnt.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fanxiaobao.xyz/Article/details/gialmcrib.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fanxiaobao.xyz/Article/details/ggqpapjba.sHtML

sys.stdout.isatty()
来源：http://3g.fanxiaobao.xyz/Article/details/gwvfwztux.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gujvuxoai.sHtML

print("err", file=sys.stderr)
来源：http://3g.fanxiaobao.xyz/Article/details/ghbvcwdey.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqnzvqwa.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwvchlev.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvmtqiuy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdqcidpi.sHtML


<!-- 参考信息 -->