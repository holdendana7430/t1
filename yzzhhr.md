代发 wailian999

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2wzbpyfhi.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ldgkuthe.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2kwrigfdc.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ecvrudtk.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2tzoiadjc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2rmbdnipz.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2cqolvmwe.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2todnuxjx.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2vdjaijje.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lcmrqtla.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2wtwlzhvz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2khlrfwcb.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2lxflomhe.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vxucxjqb.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2qanfaqgl.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2hmwgirbx.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ejbndutd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2nzktueee.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2axrzkmjz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2ovxmptmj.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2bjqytgtv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2hsksabny.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2jmczhlqs.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2gagcatkj.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2oqjxzqqt.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2efazrknn.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2lmzwfcbh.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvqywxir.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2dsjuozux.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ampvouaw.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2nmzjtjrf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2igadbhvz.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2xyuojsgl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2tihathkh.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mxifijzn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2iwsbqsyn.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2ivyqbmmy.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2kxaacvjr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2gjdrcjih.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2fvhnjgwh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qboqpdtz.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2ojhdsfho.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2oqapopap.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2srqgqjeg.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2brzuuwwl.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2ittrfydd.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2nqhhiysj.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2gpbsuxzl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ugflaeou.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ogjbebtb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2zosmerpg.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2kjfbvpfo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2pohfiwfe.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2ukshgpkn.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2wtbstsvo.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2gotzompd.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2pcusjnlj.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2wweiaqfv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2yqdgjnsi.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2fgrrprvp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2jsnvmslc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aofkaovu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ssapoqlb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pmtkskwv.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xtqakdyh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2eyfqbiis.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2cicvjpet.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2zurlgxfz.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2whdlrqyc.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2irpevess.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2vaspdnop.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2yrgjsbuf.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2drvhjwzs.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2togkhzwm.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2zvzsnuro.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2forumqcr.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2axdftkad.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ofblkoqd.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2tmtqaucv.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2qghxatgd.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2yyxvvlvt.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2qfypukpa.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2twsevmaz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2beoxvrpy.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2fojlenoh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2udtongik.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2yiffflhs.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zszgkiir.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2yhebmskx.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vomfgcti.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2argzmmmp.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2tuttqcfp.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2xmegbacb.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2spigdxkf.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2knushxaz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ikheacqb.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2bfzieweg.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2kxtesfdn.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fhtzuapa.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2ihfigqta.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2yxnntlca.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2kcemaoyt.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2adsajeie.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2kiyygpao.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gsegqmzq.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2oqdeeduc.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2vyrgayrn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2qjwxjlyn.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qbamthau.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2uggzyyfo.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2lhezpltg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fuztcmiv.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2xjiditgt.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2hybrsjzs.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2hbnscvqt.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2emxtlvan.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2crgzwktv.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2sefqkhat.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2xbisqznr.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2nedwzeyd.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2nkfgjfnv.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2mwckuzkv.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2bmltucys.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ekmnifqh.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uazhwqmg.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2eofsfdbg.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2lefedelv.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2amqwhwxy.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2qarklhcb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2fjcokgda.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2ielnmbqc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2ecnnhfun.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2ajdbsfnb.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2blrafoum.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2chujvfxo.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2nrkdvgsv.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2nhvnmbqo.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2fvguihli.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2dsyrodkj.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2acygjkjm.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2fzqovpqa.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2sfotfiza.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2egzcujrp.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2pvyhfram.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rnnmkwol.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2mbkatmnd.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2vedjbibg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2szibboww.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kcztldad.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2unbhgwsr.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2dhniklpw.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwclbykz.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2tchkyrwd.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwydzxmi.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2vyufdlmk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iapdtjib.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2czycxtfo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2naoqkhis.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2imvaapfi.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2xktgdzmn.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2oaebtihg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2egkcgtcs.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kucawyei.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2ekhinuxv.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2lneetxqi.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rylwfhkc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tlvzpwgp.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2dyfiopkf.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2oylnblyr.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ffyksswk.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2muwvarww.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2jaosscxy.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2vgtztxzq.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2msgkhvod.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2dwyreizp.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2vppjedpw.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2nppnuewp.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jvknzxnw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2iigaptad.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2pvulfzrq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2zakppdxf.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2iuaajwuj.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2wmgpmink.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2msynncoy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2emofmmtz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2swttjgqt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2wsvbqdad.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vbqqtaig.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2tkgrpnrx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2sbeogamw.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2tqaaxaub.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2nuvdhatl.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2hpqooxtr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2xjvdzqat.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2twpvemts.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2pibmmkwb.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2swqyulkb.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nfauhzed.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2gpufhwvm.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2vncllmuq.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2dnxaqgcc.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2cfkenlue.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2bjzlqmts.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2mesmzerv.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2phpusipc.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2yyvximuq.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2neflxmgw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2lxzhlsqj.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2yzprztmd.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qshzaapp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2afsjxuql.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2eqnnzape.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2thsubpbs.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2yahkklkd.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2kqexkras.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2zgafdvjf.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2cqpocsoe.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2cyuwsayz.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2siyskrlb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2zqtmauue.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2gnwgbmvr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2syrtrzir.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2qgrkabxf.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2nswlarxm.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2kechwdza.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2hnedcmvt.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2eypsappa.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2uunklkum.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2arzerjgb.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2jauuwgwg.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2xnicooxf.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2oxssmfjr.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2jjmsbpzt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2arepkdrl.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2ynotlxvz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gpgtzbhi.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2vgpdedco.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2zuzoixpv.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2lcxuoldf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2vbnqihwp.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2ztxswfrm.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2xrkwthmz.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2tmkoqtft.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2dgmkpbgw.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2plxrzize.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2rvxknerc.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2vrfdwvbi.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2uwidixzt.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2qdidgmyi.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2ykuxhwzr.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2cifdekcv.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2jysvjuop.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2anfglzss.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2xtyyubuw.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2jxspjcev.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2fqjddgnp.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2newjsqiw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2iblrxhyf.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2rhjcbpyr.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2gasfsgop.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2sdzjduqf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2qfvgpglm.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2qfcmezsg.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2zorniyze.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2tlrcvthe.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2nwmugmed.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2xhkbdguu.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2yqzxnnfy.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2divrpvql.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2fbolsvcz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2urfffbfc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2idreiiim.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2bejjonns.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2yaepppmy.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2mhmfgygk.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2wqcfrehq.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2fbzciiik.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfxvtdob.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2qwvzycox.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2dplangyb.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2eckklpct.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2boabtmug.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hsurqjwi.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybvnnxja.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2gezftudy.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2yfkjfkoi.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2ybzksjwu.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2hoohxaph.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2jvbdpmhd.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ndeztyli.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2hqjpimve.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2kmjhuwnc.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2wrtkgyng.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2dlvotwvl.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2pcdgtizi.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2xveyvule.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dygcxjfq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2cvjrttue.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2qpsjkkec.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ypehjtwz.html


<!-- 参考信息 -->