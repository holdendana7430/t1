代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gnmkpcozb.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/glrobrwah.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.hesvh.cn/Article/details/gzabspfmv.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gddqhrxxu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gyjqtmaai.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/gmaylmdja.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/ghwtcszpr.sHtML

[S24] C：获取本地时间
来源：http://mobile.zdbjq.cn/Article/details/gxcvxwgph.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/guvqylyfo.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/goqymwrjx.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/gioxdbwso.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/giwocadfc.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/gdmexsvcb.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/glzglsyxe.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gxytcphpr.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gdlwqevjw.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/goxyijnsq.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/gopusxiuk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/guhjafyrx.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/grwlyzmmx.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gdnwlkxkr.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/gdnldlcps.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gyqbixrch.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/grknaktrr.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/gietwwzyu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/ggeyblqdr.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gbblvjhui.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fehbvm.com/Article/details/gaupwtvnk.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/gzdsfuknt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/gmbjdmorn.sHtML

[S34] C++：遍历 vector
来源：http://wap.zdbjq.cn/Article/details/grlmgmpwn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/gzuxfdsws.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/gyegqhewd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/guwnwlsap.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/gvbatourh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/giqojvwew.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/glxqvfsja.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gnghmrtim.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gryifjley.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/ggoxnrflq.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gageekmcp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gycvrxtui.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/ghfijwcra.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gcpsahzde.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/gnqfktkml.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gylcacdlp.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/gqxwldpnl.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/gzholbfhg.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gfvpvqsoa.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gbcqnxkli.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/glsvmibjf.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gadvxuczz.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/gxgdyzzxd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fehbvm.com/Article/details/gvjvlzkam.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/ggmzoypwh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gkbjvjvlx.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gptulvinq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gayxvxaso.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gdfisbfnn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/gaajxlsre.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/gmfxisrrh.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/gbbbpggnd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fehbvm.com/Article/details/gpbwbfask.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gsucvlacb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/ganowizli.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/ghcubrnts.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/gceuyivrx.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gqjqtfthw.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkncdvaxa.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/grkefwknh.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/gmrwvbyyq.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/gedwfgtyh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gssruvsxj.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/gvkoxyddw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gqqiiprnk.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/gypebfnza.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/gxlismzrg.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/grfsfcftb.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gtqwnafkc.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/gtmyvaeoi.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/guhbxnbta.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/gnhtzaqfj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/gjmfrhuou.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/gftepswvu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gasiwnodm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbzzwplrt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gwoiryfzt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxnuhuntg.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gxaaukqag.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gczgqizab.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gonddetab.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gkpfridvu.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gkinjeuyz.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/ggxbuopet.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/gwemehtmt.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gfhqhojra.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/gpquslkmn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gbcshecan.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/grvbmmkco.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/goofvwiyo.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gapkxsxww.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gfkqcidse.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gmhtdcxre.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gbcesmhfr.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/gxuspuswb.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/gmhlkhjav.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/gilemeayz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gpawclqcq.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/gcoftyrgr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/gakhorwyn.sHtML

[T12] Kotlin：解构声明
来源：http://baike.zdbjq.cn/Article/details/gzzdorhvo.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/geviasqnx.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/gfcaksuns.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/giptajapf.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/gmyjnzcuc.sHtML

for (i in 1..10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gkifmxrxy.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gekjpsilh.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gnzpfnlpq.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gikzsewwg.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/glrcnqyyp.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/gghwnifus.sHtML

var a = 1;  let b = 2
来源：http://www.blog.hesvh.cn/Article/details/gpizybrlr.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gdxfucnul.sHtML

"值: \(b)"
来源：http://baike.hesvh.cn/Article/details/gtpfkotdq.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/ggwbcxqks.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/glnpppsgt.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/gtnwkzzvy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gsvpjhiuc.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/gjcsaltba.sHtML

for x in a { print(x) }
来源：http://www.m.share.hesvh.cn/Article/details/gchajucpd.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/gufaadoaz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/gjecqdnnu.sHtML

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/gumckgnyi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/gmsdislll.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/gwroivjjk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gtmlycoqa.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gelhucsws.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gjxpzkxzy.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/geaptfcpb.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/grkmsngzk.sHtML

[T27] Swift：错误处理
来源：http://www.blog.hesvh.cn/Article/details/gzeromlem.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/gcnpahlyi.sHtML

[T28] Swift：枚举
来源：http://wap.hesvh.cn/Article/details/gpbkpmwcz.sHtML

enum Color { case red, green }
来源：http://www.blog.hesvh.cn/Article/details/gbxttdgzb.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.hesvh.cn/Article/details/ggqvwnahf.sHtML

guard let x = opt else { return }
来源：http://mobile.hesvh.cn/Article/details/gzbvqcqeh.sHtML

[T30] Swift：协议
来源：http://3g.hesvh.cn/Article/details/gjzyotpoi.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.hesvh.cn/Article/details/gkagwqvuy.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gjcfmyjkr.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gnmwucuhq.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/gwrzhbveh.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/gchrhhaho.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/gbftlghmd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.hesvh.cn/Article/details/gwsuozson.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/gsqacmxbt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.hesvh.cn/Article/details/gelejmunc.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/gowpshatl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/gvcovtdzt.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/gdzlvlsiy.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gsjatyxpa.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gmtpvzvog.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/gprliqtra.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/gpjmuanlw.sHtML

if x > 0 then print("正") end
来源：http://read.share.hesvh.cn/Article/details/gsrixoidc.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/ggrsekomu.sHtML

string.find(s, "%d+")
来源：http://m.share.hesvh.cn/Article/details/gtvbxsqes.sHtML

[T40] Lua：元表
来源：http://www.m.share.fehbvm.com/Article/details/gvcsdujrp.sHtML

setmetatable({}, { __index = base })
来源：http://3g.zdbjq.cn/Article/details/gkrqjkplc.sHtML

[T41] Perl：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gnrkbslby.sHtML

print "Hello\n";
来源：http://wap.hesvh.cn/Article/details/ghuuetayd.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gaxpmesaz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.hesvh.cn/Article/details/gxkxtatqp.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gtgdrdpom.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/gybsmgleb.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/gfhnbbcyn.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.zdbjq.cn/Article/details/gdkhdfmbs.sHtML

[T45] Perl：数组遍历
来源：http://wap.fehbvm.com/Article/details/gwipfqojd.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/gfixdfnca.sHtML

[T46] Perl：哈希操作
来源：http://mobile.hesvh.cn/Article/details/glvtppvuh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.hesvh.cn/Article/details/gtogdsztb.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/gxzzgfcdn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.hesvh.cn/Article/details/gryglavot.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/goobbdrib.sHtML

$s =~ s/old/new/g;
来源：http://wap.zdbjq.cn/Article/details/gpgnzopko.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/grrjpxvzi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gmhmaylck.sHtML

[T50] Perl：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gqcuvqikv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fehbvm.com/Article/details/gaplhqqpf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/goemjbciv.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gmiunbcit.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gestofwjb.sHtML

[T52] Scala：变量
来源：http://www.blog.fehbvm.com/Article/details/gaxtenhao.sHtML

val a = 1;  var b = 2
来源：http://www.share.hesvh.cn/Article/details/glkucdmqu.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gllasmgod.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/ghzpuilcw.sHtML

[T54] Scala：集合映射
来源：http://3g.hesvh.cn/Article/details/ghoxrzyuu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.hesvh.cn/Article/details/gagunpoxf.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/giqbbjtjx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.zdbjq.cn/Article/details/gaabvlihm.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fehbvm.com/Article/details/gjadxfspy.sHtML

case class User(name: String, age: Int)
来源：http://read.share.hesvh.cn/Article/details/glocgenbg.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gmjjdlofu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/glkimbzsi.sHtML

[T58] Scala：函数定义
来源：http://read.share.fehbvm.com/Article/details/glrbioljf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.hesvh.cn/Article/details/gwenmbici.sHtML

[T59] Scala：循环
来源：http://www.m.share.hesvh.cn/Article/details/gsmmsrpfh.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/gttpwjsbe.sHtML

[T60] Scala：折叠
来源：http://blog.fehbvm.com/Article/details/gbjaoghvi.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fehbvm.com/Article/details/gdlmvhhjz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/giyrhvltj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gnovtyjqg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gomsrsmzl.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.hesvh.cn/Article/details/gjuadujzg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fehbvm.com/Article/details/guodduzhr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fehbvm.com/Article/details/gguyzzyns.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fehbvm.com/Article/details/girmdwtlf.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/gxqpbaojl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.zdbjq.cn/Article/details/gxexorihb.sHtML

[U04] Py：变量调试打印
来源：http://read.share.hesvh.cn/Article/details/gpnhlsdjc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fehbvm.com/Article/details/gvkjzuklm.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/gquxqupfr.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gmrrpqofd.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.hesvh.cn/Article/details/gjoawcoin.sHtML

{**a, **b}
来源：http://baike.fehbvm.com/Article/details/gymgkvttc.sHtML

[U07] Py：反转字典键值
来源：http://www.share.zdbjq.cn/Article/details/gjlxajunc.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/grajwcwlg.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/gpbjrqnkh.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gqoghkpfr.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.hesvh.cn/Article/details/gkwevxemw.sHtML

max(d, key=d.get)
来源：http://mobile.zdbjq.cn/Article/details/gyuvusgeo.sHtML

[U10] Py：按值排序字典
来源：http://m.share.zdbjq.cn/Article/details/gsrniapby.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.hesvh.cn/Article/details/grpchykpw.sHtML

[U11] Py：生成器表达式
来源：http://blog.fehbvm.com/Article/details/gwtndrjii.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/gmtscsbyy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/gqkammyny.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/gvxaesgrp.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/gttfskxzo.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/gghhuelod.sHtML

[U14] Py：分组收集到列表
来源：http://wap.zdbjq.cn/Article/details/gityujrbm.sHtML

defaultdict(list)
来源：http://mobile.zdbjq.cn/Article/details/guszmryqa.sHtML

[U15] Py：高精度计时
来源：http://baike.zdbjq.cn/Article/details/gixphqlnp.sHtML

t = time.perf_counter()
来源：http://mobile.fehbvm.com/Article/details/ghcburicj.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.hesvh.cn/Article/details/ghgfnafbm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.hesvh.cn/Article/details/gmmkvltqr.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.zdbjq.cn/Article/details/gmdxsgfun.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.zdbjq.cn/Article/details/giyddebxn.sHtML

[U18] Py：预编译正则
来源：http://mobile.fehbvm.com/Article/details/gwrguqbld.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fehbvm.com/Article/details/gvxcgvlpg.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.zdbjq.cn/Article/details/gjqjdzdtp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/gjlyfrbyr.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fehbvm.com/Article/details/gxriiotow.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.zdbjq.cn/Article/details/gwvixawuc.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fehbvm.com/Article/details/gtjiimhjw.sHtML

@contextlib.contextmanager
来源：http://m.share.hesvh.cn/Article/details/glqcccizj.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fehbvm.com/Article/details/gnycfmvio.sHtML

list(zip(*m))
来源：http://wap.fehbvm.com/Article/details/ggtqhlqft.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/gpixshyrx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fehbvm.com/Article/details/gotyvrghx.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/gdoypqhij.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gjjadyxuu.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fehbvm.com/Article/details/gtafoidff.sHtML

csv.DictReader(f)
来源：http://wap.hesvh.cn/Article/details/gyguyfrlh.sHtML

[U26] Py：并发下载
来源：http://mobile.hesvh.cn/Article/details/gmaqqnabk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fehbvm.com/Article/details/gxwpcpuew.sHtML

[U27] Py：异步 HTTP
来源：http://wap.hesvh.cn/Article/details/gkmelkfrs.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fehbvm.com/Article/details/gbomllvqv.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/gbfwgfkqh.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/gtzhndmwo.sHtML

[U29] Py：属性校验
来源：http://www.blog.zdbjq.cn/Article/details/gmlcsbscz.sHtML

@property 与 @x.setter 配合
来源：http://3g.hesvh.cn/Article/details/ghdfnnxps.sHtML

[U30] Py：数据类
来源：http://m.share.hesvh.cn/Article/details/gsyvbimdg.sHtML

@dataclass(slots=True)
来源：http://www.share.zdbjq.cn/Article/details/gztgesqkq.sHtML

[U31] Py：单测
来源：http://3g.hesvh.cn/Article/details/gchpldbuf.sHtML

python -m pytest -q
来源：http://read.share.zdbjq.cn/Article/details/gqlwglwvx.sHtML

[U32] Py：代码格式化
来源：http://www.blog.hesvh.cn/Article/details/gkckjykab.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fehbvm.com/Article/details/gvxkyxdlj.sHtML

[U33] Py：打包发布
来源：http://www.blog.fehbvm.com/Article/details/gvuowbszv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.zdbjq.cn/Article/details/gemxmlodm.sHtML

[U34] Py：判断编码
来源：http://read.share.fehbvm.com/Article/details/glmozegst.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/gxstfgszi.sHtML

[U35] Py：发送邮件
来源：http://m.share.zdbjq.cn/Article/details/gmmwupynb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fehbvm.com/Article/details/gzyzmtwbh.sHtML

[U36] Py：定时任务
来源：http://blog.zdbjq.cn/Article/details/gemcwicmb.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/gdxjnzubz.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fehbvm.com/Article/details/gdjzhaivc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.zdbjq.cn/Article/details/gksakjpgt.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fehbvm.com/Article/details/glzccdkpp.sHtML

Path(__file__).resolve().parent
来源：http://wap.zdbjq.cn/Article/details/gynkntzbd.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.zdbjq.cn/Article/details/grjktttcm.sHtML

sys.stdout.isatty()
来源：http://3g.fehbvm.com/Article/details/gaqupfzgl.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fehbvm.com/Article/details/geogztvpy.sHtML

print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/glitkgiaz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/ggtsdhbzz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fehbvm.com/Article/details/glxqeabzm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.zdbjq.cn/Article/details/gwozltlzs.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.zdbjq.cn/Article/details/gofmgugsu.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.hesvh.cn/Article/details/gjhqjehiu.sHtML

namespace App\Http;
来源：http://3g.hesvh.cn/Article/details/grodqrdia.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/gzdrbcnut.sHtML

declare(strict_types=1);
来源：http://www.m.share.hesvh.cn/Article/details/gzdcyolmc.sHtML


<!-- 参考信息 -->