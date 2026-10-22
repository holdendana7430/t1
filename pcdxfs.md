代发 wailian999

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2xxapfkdk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2xxtricqo.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2tzhadzqg.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2mkluqtwe.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2lbmtiold.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2yctihsqt.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2kfsibxbw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2gbzbvmii.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2nrrndyso.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mvlzivsq.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2xgtegxbp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vwekbuuh.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2kdblmjsx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ofllxiae.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2gpiefinu.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2urprtcif.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2zgaotsoi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2kjlfzzyf.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2vayxpdsw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2znrjlhvk.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2jdsynsof.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2jqxoiivb.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2ncdxfrjf.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2oxdjaved.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2tvkcuxqh.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2zakwrsqk.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2rzpenbbu.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhrnxoxg.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2jzxfmwxz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2arouwvnp.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2jyggulou.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2znuysilk.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tvwsbnof.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2mcrqsadz.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2iksaiwko.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2jgczjrno.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2mnhgfdlt.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2cgjwhpqa.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2wmcqmydl.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2ihrtrcgw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pqcufvbw.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2puotnmeb.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2qxpdsxai.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2rbgqjqgb.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjhrsfqb.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2qwzmtugq.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2cqlkfsel.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2zpgfarxt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2stsyepky.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2aysogdqf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2yciveuyc.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2gfzwxuui.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2hzmsitdl.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2jkjjcgmx.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2gembqbrj.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2zpbmvvgt.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uyedcczk.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2azopuwdq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2nkyuabui.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2loedkqee.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2mwaqkrnn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2czvizfcb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2edpclbbo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vnzqrgjo.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uwywqxls.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fjhvrbzr.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2hsmvmnwi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2hklztpbh.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2mlywpgit.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2synzypzz.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2zrfrmxpn.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2celfmaeb.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zqthycoj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2tvjhpnkn.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ufnzirro.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2xelwdknv.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vwbisqfj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2kkokeinn.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2etsbbgks.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2jjphvchl.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2rgedzgzi.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2gaerznht.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2dcsrcwsx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2bfabutvy.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2lruxtsbk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2qcasoucm.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2xhczcove.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gtpylepz.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2hohobliz.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lcmrbmar.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2xymhwgtu.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ptygjyma.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2rjfcmkrh.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2rcaulris.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uyxevany.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hspxjwdi.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2zjkapdns.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2bqkiayha.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rgjbliwv.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2uaypnexz.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2bynepirz.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2fbhytsbb.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2pfiwxrhp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2mechnric.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2hmmysoux.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2kkqtmmgn.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2rfjnpgsq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2tjgexozz.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2pskujjzj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2tpqzzwzo.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2dtrwbsvw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2titcjnva.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2pykycymq.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2jjbtrcuq.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2gcxlvgci.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2fwqnehqj.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2slhimmjc.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2aencycug.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2qccewjwv.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2lwkrdqpf.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2rbsejmrx.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2azwtenkh.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2evkygxlz.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2cruzvlhr.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gtlaftcz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xqfexqke.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2zwvizxns.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2mpugzbcf.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2zfyfempm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2atnundne.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2erzzgefw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2meeaeiwd.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2ozmvwueb.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ekquxqbm.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2sdnnqvfe.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2cyfbkmio.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2wckavcfm.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2tkprjnmq.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2rnorskym.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2dwefctzv.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2qjurcgoy.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2ggwlpzoo.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2xjjdlber.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2hamiqgwj.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nrbmcmxu.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2rqplrvno.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2cwvuiwrr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2cdyofqlq.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2nllfvspr.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2yrjpcnkd.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2gtpyizfo.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcabuglh.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2kdodopwz.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2hoytkvlf.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2pqavecxp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2xbcsgzlp.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2szhezkda.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2jggttxfk.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2oxvnmuaw.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2sosrydbz.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2iwgqtfiz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2viltqdjr.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dfleebcc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2ekrqwdze.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2oykmoczy.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zuxurqih.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2oeeeyenc.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2cplkgqkx.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vlphybjb.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bbagapsl.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2jaxtextc.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2zgokyprp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2mefpfwzq.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gwcvwfoc.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pnmeawfp.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2ivcvcofl.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2wailksam.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2axwvxgvl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2dniejlvf.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2qmdjjgsq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2qstwjoql.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2vyowtgty.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2toahnarg.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2tbamjgjp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2fspinvba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ewdlfxux.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ccrwoivf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qqlegacj.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2jzdhohzf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2wiaxminx.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ifzjnjnw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2huqrffxh.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2bklkidfh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2tuuqowpy.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2gkarikyb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2aovcbrlv.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2giewsvjw.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2steqdmxu.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2kjfwnptt.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2wvekchqi.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2volkhpph.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2ivfdrgug.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2nknguwqv.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2wgldobmb.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2vgaldxoz.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2lotcjyvw.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2implarfl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2qdvyrnvs.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2uckzsxml.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2voyvjwkp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2lmgidfaz.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2vorrbqxc.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2zermtwxb.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2uyggueoy.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2dsgznomk.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2kidargtb.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2bzsehsde.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2guslybsg.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2burgrxfe.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2bieyhqof.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2rkihuyvm.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2lwrkoltf.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2ppjbqjrs.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2epfdlsjz.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2aazhnhbz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2ztbpueky.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2uqwflfyo.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2zjbsnpud.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2slkytexs.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2xbyoszeh.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2cagaykao.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2bmpmthlb.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2eeazikgm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2mjpxedkb.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2bboworkd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ejtzmfzb.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2zkinhkdp.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2yatmgswv.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2dsmasbnv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2isbeppym.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2hsrxueal.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2dkljatbx.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2ilifjigh.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2pnikistv.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2mprtnbxx.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2gilnexux.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2atqhumrr.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2jalwikxx.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2qmxsnroc.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2yyiydsyj.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2mkdunkbm.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2axlxsoua.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2vtrmakah.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2fanqurku.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2muchiuqc.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2vxrqunge.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2ingxmmnc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2zposdaic.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2apoybyed.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2qldknfgl.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2ajkydbky.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2qshfdflu.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2nkdtczsc.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2qsvzxzdh.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2yuopogqu.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2kxdfznuh.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2savlidpb.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2dcppmjer.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2ropudobs.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2tmzwjoor.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2vaqeqvor.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2hdnijfwy.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2gswpuzto.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2yaufsvxt.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2mbjieyrf.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2uaqsrybo.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2qabdroxh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmvvlidu.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2sxidxxur.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2nzvkiytq.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2mqkxwzla.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2bsymknmv.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mltvthpl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjlvtweg.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2pinnqvpq.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2ffpiaufb.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2djrqhxeo.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ffkpgesf.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2vhjzxxmy.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ehlumveb.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2vvpjzysv.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ufiitigv.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2mkaormdv.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2qqoorbzg.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2dwedtydu.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2bvbizott.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2bcpjnodl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ovtsnill.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2hlfniugl.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hcvjlqyd.html


<!-- 参考信息 -->