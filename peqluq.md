代发 wailian999

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2jlrhnllc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cftvfvsb.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yksvcqgy.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2gbuxgcmr.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2kznjegtp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wvvbraut.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2nyizqgjb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ayqgglvj.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2kpcbltvb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2whrdaswg.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2knlubwma.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2pcntbmiq.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2sntqvzbe.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gwfszigd.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2lyfopveb.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ybrnknzu.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2zobxzajf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2rowwfawc.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2gkwlbzns.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2ksttfckx.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2gjhqzakj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2tasqgkdv.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2suxgthxf.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2saxhiuwk.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2utpzuvmg.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2rgohcmcm.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2fkqjfynw.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2lsnfexbw.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2mgmrzioc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2madgndbw.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2qiqczeak.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfnoizap.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2iycmoeoa.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywdbpixf.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2andalnav.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2mkjkkpiw.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2pphwxxru.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2oajuzsah.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2wdqbwaqt.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2puwqztlm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bjmnrjlp.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2udakazor.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2bazfukmw.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2sutifrwm.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxzezeya.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2anibzjha.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2fvlqywfo.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2hxeqypda.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vcwzvyyd.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2fwsahjct.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2azvrtwlg.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2hjhmgvfm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2wxoojqmh.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2mbhskccn.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2xqvlovph.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2bvoybfeg.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ffnrquxx.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2dnmwjetn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2ocxwsbrz.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2yvzfjhjw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2fcxwjzij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zbzxgqce.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ssgzndkw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ocxpsllo.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mxzsmgfk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lnpqrncf.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2rttslddy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2apjxgeau.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2qfgvgzmu.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ccertulw.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2ekhkuzsv.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2vkfeiflo.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2arxamgsf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2kyshzisg.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2uagrgnbp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gpuvdgcv.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2laluirxq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2mcsvzksm.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2vfmgvtyg.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2lsjxjymu.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2bdtkipgo.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2bsxxqpby.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2aedphzvs.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2zvjasjah.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2kucjufgw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2iqygyrlk.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ggtmqqyn.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2uytwjszn.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2jbeemccp.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qczagqxc.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2wjigeejo.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2qnsudufk.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2gygbmxjk.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2ybmxokqn.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fgaekwzp.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jsedvdwr.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2gopipaza.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2kgxemihc.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vgplqbut.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2tgsibeun.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2xlbgdoer.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2ilforqaq.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2gvmfkghc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2uqvygasd.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ybjgkyga.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2ygycyuiy.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2brlgofgn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2stgtgghu.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2kfdcukwo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2xsgjxqmt.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ubxlztnt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nnbequzq.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2caxcaqjd.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2nzqhaiuv.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2zhzjcjlr.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2knlpbdth.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2tdgcpocm.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2koubnipt.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2csanzxww.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2pmmhrzto.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2itxspiuy.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ioahbpac.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2jyfzaggl.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2qabeyzat.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2puvgauin.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ubnfezei.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2scqiqnbe.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2joardfrm.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2cobqbarq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2zptinexp.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2bkmatumi.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2wdbuizuu.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2vwaidfve.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zaiwaodq.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2vcglilad.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2cyppfeuq.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2gfycewmi.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2oysthovn.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2lbketfbs.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2tefiklri.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2izmttfkx.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2ewcfhrlq.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2hsokakcx.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2dhtyzdwv.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2namdcatv.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2rrayrtpi.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2rbbvjitz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2zeahbidb.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wxyvbevb.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2zpnglkgg.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ssrlatoh.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2waxnocvo.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vgibwmth.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2zysgsxnc.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2bkzgdwwi.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xytsglbz.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2bmcokfvq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2qmuhwbrh.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2dreimjcs.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2cpswrrss.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ykyslkok.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xeutpkfg.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2twkzzvib.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2duequnue.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2mhmsbdyc.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fqqwgrcq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lqkjmhgf.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2wjyywtuo.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2esmpfysk.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2utzdrthh.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2njblzmxo.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2smboqhvb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2jpepdmct.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2iqmffpea.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2twtdzmge.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2zbbmadta.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2umafqhtu.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2tcpyypqp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2enpxkhfz.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2aiztcajj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2xvodrqjg.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ltikliiy.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2cdduuiod.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2pavfqcdv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2qtkkcwve.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jdfrfmcj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jejyahgp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hkuwjsle.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2ktvedbpr.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2ejwllamh.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2juwmdwij.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2alyzinsg.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2zvnibsap.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2eqvdcwhp.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2ucqyvxie.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2stgapivt.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2nbahkneg.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zsxpsodq.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2nildbzzn.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2mcwkesxk.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2cfwlrwpl.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2brimbovp.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2ndlkgfbd.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2lnliburc.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ruijaiav.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2dcxzbtja.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2nkszjbtd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2zcmlpgwk.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ocfqpoos.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2kbjqzslq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2ahzslaqy.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ironzzkl.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2ejvjdkgi.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2ptqzbgvr.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2utykxwrt.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2imgpnsdu.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2wujsbisk.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2nfbcihxc.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2clwepcih.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2hpbisxfi.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2affuldpx.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2mmimoqrt.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2btmsisze.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2hsswknuu.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2apzzcmnw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2qncpepid.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2skcqepiz.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2qxmkalwd.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2ywivkrpi.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2gjoboqce.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2larwfkve.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2oaafbili.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2tbqnwejj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2gzrkrdds.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2mhckvrwf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2xwsdixrw.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2lntnnbrq.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2yxxqrthy.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2fjjanxxs.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2qakgderf.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2ikvbixql.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2wkrqgvkv.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2agjxjxii.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2ymdwtvro.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2nwhnbcaq.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2oftmazgr.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2xthtwjxa.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2fyrlziaq.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2uomuqowr.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2lbtpqcwe.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wkwhbbgv.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2iecxjfln.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2rhbmhnsn.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2wpljhzpd.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2bqedwdmk.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2ykxwvvjy.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2ztxqteow.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2vakxefyy.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2zlxihjik.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2tlqqigki.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2ihfirmpo.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2dcsyweia.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2krhpxxgk.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2joamzszo.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2kvixztef.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2jmuayjxw.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2zfylpkrk.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2dhefwmju.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2tqpnpfcx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2wyzbztmr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2nxkonoyd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2cadbgboj.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2oakinbrw.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2dwwynvnw.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2hioulzom.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2cdwtbomd.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2ehdwkual.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvltjgfg.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2cnuinuyt.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2oxtkkhrd.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2djzpczjz.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2iulzxrgl.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2cxepwntg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pfefnbtk.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2pvajknnn.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2fszodjeh.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2sylgjjrj.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gramycnd.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2sezbenxs.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2kfhjgtrz.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2wilsqoyi.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2rriotmhn.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2aubafavi.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2epjficcq.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2gdwbpkop.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2kwfrqect.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hveemrnh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2pxmlduzy.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ltksejqj.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2dxskcwoy.html


<!-- 参考信息 -->