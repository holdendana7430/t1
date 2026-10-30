代发 wailian999

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/ghumnahqy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gtmgjkkek.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gjtnulwef.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gbqokjxxo.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/gcmlulyah.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/gmmtzpstc.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/gsrwaphif.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/gaopjtkwr.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gkpdlmlfg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/ggqewkgjb.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/grqcewtva.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/ganfkouyx.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/gxtrghdgr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/gqhebnozk.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/gnzvilhvj.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gtfisvakq.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gqbyyuloo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gtcqqcuak.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/gjifgjicy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/garwqflcl.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/gihteoztw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/giwreydqg.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gdjsddznq.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gonlbafhb.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/gvoulnpae.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fehbvm.com/Article/details/ggwcrxysa.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/glxtqkxip.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/guxwuvunj.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/gvcxzqcvj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gwhrmecdq.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gwmabrmnw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/gosbhnxdo.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/gwaozsmop.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/gzrktiftn.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gwmoxbgsa.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gsxugonkn.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/gxjsojiey.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/golmbkdlp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/gzbhyfpzk.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/guxvyfxhi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/gpuwiotut.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/gaqyalght.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gmjjqbwjl.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gultfbolt.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/gxxqcluho.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gqmihqxme.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gxqqvvixr.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gtmhvgnjw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/giwjziopc.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/ggvjuxyen.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/gfrxkjyli.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/guiigklab.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/goainwkmq.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gmzpevxcg.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/gmceuvegc.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/ghfruczld.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/gckbgjowb.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gsfwmazob.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/glhltgnsb.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/glwnjczoz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/galjzgvku.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfzymgcva.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/ggsyvgauk.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnujnbrrx.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gxvhbtksa.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gsuhdxksk.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/gpglttqoc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.zdbjq.cn/Article/details/gqbsqebui.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/gcogwrvms.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/gitqjxhcn.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/gwzxcpppe.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/gnouzkvhf.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gshvntuxt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gqapccbyz.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gilljmljd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/gysuivwdl.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gdpmomtzg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/gtgvnuael.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gpwfpwfdb.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gtjjwjuvc.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/gxpigtkbi.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gtbtybpjg.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gxvnvqifw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/giiljbrdm.sHtML

[T11] Kotlin：协程
来源：http://wap.hesvh.cn/Article/details/gpitraeqw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/gfptumveg.sHtML

[T12] Kotlin：解构声明
来源：http://3g.zdbjq.cn/Article/details/gfgmjudmg.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gyttmwfgx.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/gahkzsqsm.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/gyxzzodon.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/glhqyhhbw.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gelkhgkeu.sHtML

[T15] Kotlin：接口
来源：http://wap.fehbvm.com/Article/details/gjvwifpbf.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/gwirjrynu.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gxmlwiaaj.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/ggcpstfjd.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/golarldll.sHtML

var a = 1;  let b = 2
来源：http://read.share.hesvh.cn/Article/details/gcndnkbnf.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gtmtaknll.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gfxvcxptx.sHtML

[T19] Swift：可选绑定
来源：http://3g.fehbvm.com/Article/details/gzaheqrqt.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/ggaaxmwpl.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/guqtklezh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gpvqizmow.sHtML

[T21] Swift：遍历
来源：http://mobile.zdbjq.cn/Article/details/ghbelojit.sHtML

for x in a { print(x) }
来源：http://blog.zdbjq.cn/Article/details/gsxlompzu.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/gewoixfjo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.zdbjq.cn/Article/details/gvpsdtirq.sHtML

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/gijfbkfxi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.zdbjq.cn/Article/details/gjsnfhdob.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/gxlgamwii.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/giwycixuq.sHtML

[T25] Swift：结构体
来源：http://baike.hesvh.cn/Article/details/gbiyhrwwy.sHtML

struct P { var x: Int }
来源：http://mobile.fehbvm.com/Article/details/gauqwosit.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/grsjyblzk.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/gmomkptdp.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/gpngckhzz.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/gxxlzzcxo.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/gpenjtxwd.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/gjeplsvcv.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/guptlebra.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/gumpggtzy.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/gwmqxjyrn.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gpsowtlox.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/ganbfcpus.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gzyjukzgr.sHtML

[T32] Lua：局部变量
来源：http://mobile.hesvh.cn/Article/details/gtryhfqvu.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/gxjtqvtvn.sHtML

[T33] Lua：表（数组）
来源：http://baike.zdbjq.cn/Article/details/gslkqlowc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/glcbqcqbk.sHtML

[T34] Lua：遍历表
来源：http://mobile.zdbjq.cn/Article/details/gwmxmxszt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/gtbwmfkek.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/glxhiqblm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/gjxdkmmdp.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gvdpkyrum.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fehbvm.com/Article/details/guongbzql.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/gcyngrmcm.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/gqjtrlioi.sHtML

[T38] Lua：条件
来源：http://www.m.share.fehbvm.com/Article/details/gylifsxqt.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/gckjovzob.sHtML

[T39] Lua：模式匹配
来源：http://blog.hesvh.cn/Article/details/gvkuhpdco.sHtML

string.find(s, "%d+")
来源：http://m.share.hesvh.cn/Article/details/gthxzuphc.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/gbytxjksq.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/gapfwzllw.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gprlhzvjq.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/giasbiaev.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fehbvm.com/Article/details/gchhbuvea.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/goemqthrf.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/ghcglggby.sHtML

"值: $a"
来源：http://baike.fehbvm.com/Article/details/gnprgszzx.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/gniceyzad.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/gasbpoeky.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/ggdhaurie.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.zdbjq.cn/Article/details/ghjnnxtbe.sHtML

[T46] Perl：哈希操作
来源：http://read.share.zdbjq.cn/Article/details/gxovufbai.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.hesvh.cn/Article/details/gqbuhyyxt.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/gfldlivhz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.hesvh.cn/Article/details/gazsgtxjw.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/gclukpcpt.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/gvppwjzvj.sHtML

[T49] Perl：函数
来源：http://mobile.fehbvm.com/Article/details/gxyujrccf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gjzjagvbp.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gyoeywuaw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/gtczdzeuq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/glomqtfoh.sHtML

[T51] Scala：Hello World
来源：http://blog.fehbvm.com/Article/details/gajlpuvud.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gndszglrv.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/gabyntail.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/gaefivkcz.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gowzosqlj.sHtML

s"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gdtmvjvwp.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gbnoazubj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/gxgjjpjfr.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gejpnoqba.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/geuxpzikg.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/gmesaqluw.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fehbvm.com/Article/details/gzqaeyonq.sHtML

[T57] Scala：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gtutuqbct.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gqqqvvjzd.sHtML

[T58] Scala：函数定义
来源：http://baike.fehbvm.com/Article/details/gwanzwggf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fehbvm.com/Article/details/gtqdovlrg.sHtML

[T59] Scala：循环
来源：http://3g.hesvh.cn/Article/details/gyxqjvmmy.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gdyftdzsx.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/gsikrwami.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gmyzmbmko.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcmtnaknl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gdkwssuzp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/geygzyipl.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/geqsbtmej.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.zdbjq.cn/Article/details/gvwlbssgs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/gmwrnuaum.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/gnecajzfo.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/gexvcofgm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.hesvh.cn/Article/details/ggviyaiqv.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/ghjpowmrj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/grtxveuuh.sHtML

[U05] Py：列表去重且保序
来源：http://blog.hesvh.cn/Article/details/ghfsfxevv.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gegtaricf.sHtML

[U06] Py：合并两个字典
来源：http://www.share.zdbjq.cn/Article/details/geyzzuplv.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gjcnnwlcj.sHtML

[U07] Py：反转字典键值
来源：http://blog.fehbvm.com/Article/details/gzicpyxvm.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/ghfqnsoid.sHtML

[U08] Py：展平二维列表
来源：http://read.share.hesvh.cn/Article/details/gccrwnjlf.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.zdbjq.cn/Article/details/glptqghcv.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fehbvm.com/Article/details/glcqzprpa.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/gwaouspsw.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/gurlmbibc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.zdbjq.cn/Article/details/glndodcgw.sHtML

[U11] Py：生成器表达式
来源：http://blog.fehbvm.com/Article/details/gdfvypmnu.sHtML

(x * 2 for x in arr)
来源：http://wap.fehbvm.com/Article/details/gdpfdrckj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fehbvm.com/Article/details/gnackelrw.sHtML

Counter(arr).most_common(3)
来源：http://read.share.hesvh.cn/Article/details/gmyoqmulu.sHtML

[U13] Py：固定长度队列
来源：http://blog.hesvh.cn/Article/details/gvwskogzo.sHtML

deque(maxlen=10)
来源：http://www.m.share.zdbjq.cn/Article/details/gwbhrzaks.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fehbvm.com/Article/details/gaaaedlsw.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/gspoedrrv.sHtML

[U15] Py：高精度计时
来源：http://read.share.zdbjq.cn/Article/details/gnydmqevu.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/gwzlvelhx.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fehbvm.com/Article/details/ggxvmneuf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.hesvh.cn/Article/details/gcyyypdix.sHtML

[U17] Py：初始化日志
来源：http://3g.zdbjq.cn/Article/details/gwbweqvma.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.hesvh.cn/Article/details/goqeymqst.sHtML

[U18] Py：预编译正则
来源：http://www.share.zdbjq.cn/Article/details/gqsoyrccp.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/godutiktq.sHtML

[U19] Py：正则替换带回调
来源：http://wap.zdbjq.cn/Article/details/gzwwlcxvt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/gddrbuugp.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.hesvh.cn/Article/details/gkunpzrtd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.zdbjq.cn/Article/details/gdrdqddcs.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fehbvm.com/Article/details/gexqacqsz.sHtML

@contextlib.contextmanager
来源：http://m.share.fehbvm.com/Article/details/gudcdbvcb.sHtML

[U22] Py：矩阵转置
来源：http://baike.zdbjq.cn/Article/details/glbfiaaro.sHtML

list(zip(*m))
来源：http://www.m.share.zdbjq.cn/Article/details/gdwqlfieo.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.zdbjq.cn/Article/details/gzimvfjbf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.hesvh.cn/Article/details/gqzcgzctg.sHtML

[U24] Py：路径操作
来源：http://www.share.hesvh.cn/Article/details/gwjdklbnu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gvloykkyh.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/gjwqntefi.sHtML

csv.DictReader(f)
来源：http://baike.hesvh.cn/Article/details/gmilltdgs.sHtML

[U26] Py：并发下载
来源：http://m.share.zdbjq.cn/Article/details/gpqcjbmyf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.zdbjq.cn/Article/details/gkykvaghw.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fehbvm.com/Article/details/gqinrbsmc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fehbvm.com/Article/details/gdkbdvnnn.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/gejjdomsx.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/gvwrbyvzu.sHtML

[U29] Py：属性校验
来源：http://mobile.fehbvm.com/Article/details/gozoevjwz.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.zdbjq.cn/Article/details/goxemiqhp.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/guzwuhgmn.sHtML

@dataclass(slots=True)
来源：http://www.blog.zdbjq.cn/Article/details/gralykbqd.sHtML

[U31] Py：单测
来源：http://wap.fehbvm.com/Article/details/gpnnmevzh.sHtML

python -m pytest -q
来源：http://www.m.share.zdbjq.cn/Article/details/gbnyxlqyl.sHtML

[U32] Py：代码格式化
来源：http://www.blog.hesvh.cn/Article/details/gnxzsslbn.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.hesvh.cn/Article/details/gxligwvcx.sHtML

[U33] Py：打包发布
来源：http://mobile.zdbjq.cn/Article/details/gcdjddevd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gdhemibke.sHtML

[U34] Py：判断编码
来源：http://3g.fehbvm.com/Article/details/gslenbxhj.sHtML

chardet.detect(raw)
来源：http://baike.hesvh.cn/Article/details/gwdkvkdvu.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fehbvm.com/Article/details/gmhkgoazv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.zdbjq.cn/Article/details/gelxpdmcs.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/gjtbrjgrw.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.zdbjq.cn/Article/details/giaitlqgl.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fehbvm.com/Article/details/glyfagogw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/ginjqtasa.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/gbnfeoqki.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.hesvh.cn/Article/details/gryxeunsb.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.hesvh.cn/Article/details/gjdkyxrzg.sHtML

sys.stdout.isatty()
来源：http://mobile.zdbjq.cn/Article/details/gfsforzwg.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/giwiydksu.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gxnhxjgdk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.zdbjq.cn/Article/details/gbzgqquwa.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.zdbjq.cn/Article/details/gtaxbjjam.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fehbvm.com/Article/details/gyrmvnyhc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fehbvm.com/Article/details/gglqwzrsx.sHtML

[U43] PHP：声明命名空间
来源：http://blog.zdbjq.cn/Article/details/gbatgymkm.sHtML

namespace App\Http;
来源：http://blog.hesvh.cn/Article/details/gdlvwbrsw.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.hesvh.cn/Article/details/glpmmtoen.sHtML

declare(strict_types=1);
来源：http://read.share.zdbjq.cn/Article/details/getfjvajg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.hesvh.cn/Article/details/gdzqqqmdd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gnoyibkxj.sHtML

[U46] PHP：可空类型
来源：http://www.share.zdbjq.cn/Article/details/grulbtoii.sHtML

?string $name = null
来源：http://m.share.fehbvm.com/Article/details/gkguryvlx.sHtML

[U47] PHP：联合类型
来源：http://read.share.fehbvm.com/Article/details/gafegdzpb.sHtML

int|string $id
来源：http://www.share.hesvh.cn/Article/details/glnufvidc.sHtML

[U48] PHP：纯枚举
来源：http://read.share.zdbjq.cn/Article/details/gttffumec.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gquwbopej.sHtML

[U49] PHP：只读属性
来源：http://m.share.zdbjq.cn/Article/details/gzgtlsvnl.sHtML

public readonly string $name
来源：http://www.blog.hesvh.cn/Article/details/gwvaplnnp.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fehbvm.com/Article/details/gpntawzmz.sHtML

public function __construct(private int $id) {}
来源：http://blog.zdbjq.cn/Article/details/gmvttxrrz.sHtML

[U51] PHP：数组解构
来源：http://read.share.zdbjq.cn/Article/details/gnhcbfdgy.sHtML

[$a, $b] = $arr;
来源：http://wap.fehbvm.com/Article/details/gzpvqmvmk.sHtML

[U52] PHP：箭头函数
来源：http://wap.hesvh.cn/Article/details/gztgubhqh.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/grmwgcoqi.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fehbvm.com/Article/details/gqwhpbwvq.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/gmcgoleld.sHtML

[U54] PHP：空安全调用
来源：http://3g.zdbjq.cn/Article/details/gmzwpnnjn.sHtML

$obj?->method()
来源：http://baike.fehbvm.com/Article/details/ggawgyctx.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fehbvm.com/Article/details/gkoviqhky.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.hesvh.cn/Article/details/gsfdynfbk.sHtML

[U56] PHP：命名参数
来源：http://read.share.fehbvm.com/Article/details/gtpbvrmvw.sHtML

f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/glyfhduft.sHtML


<!-- 参考信息 -->