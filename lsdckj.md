代发 wailian999

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2bbwbteld.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2grnlmpma.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ftpujile.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2xiiahlho.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2lerlfwrh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2zteenlvw.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ghogcwxc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2jyxxxscm.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2wttowgxn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ortthcpl.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2roccxdvp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vpemlroy.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2raaxmscr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2dcselitu.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2pgkxeimb.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2kfffzquy.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2whdnowht.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2vwnyavym.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2azjcotgu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2afnidehi.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ccdnkktv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2eeetdmvv.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2gdrsldpm.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2zpvbzjxm.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ymsgkybv.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2dyjwpoyp.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2warzodtz.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wcfzcpdq.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2mvborprk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2jmdhqvmw.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2ygoxbnfu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2cecxhmvj.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gbzriyax.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2pgnplajy.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zvivbxbb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2llkwluii.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2qrsgjxdf.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2azuutckh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2jorbyuoi.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2qddhcfcq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lvhbxysu.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2gisbubiq.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ucqlnchl.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2utyutyme.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2abilalxs.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2lzsmehxr.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2qxfigron.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2aggbfxdq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ifslcdnf.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qyftchzn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ocioruer.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2zakibnxg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2gykntjsf.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ntyghzfd.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ebmxzvfr.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2sldkajna.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xmqzxvoh.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2fbifaigx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2osmcozzk.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ojjgyqap.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2rzyxtjwo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ghtnrosq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2xajrfdqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tvaoybbs.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2czhhnusd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2izvpitab.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2dovgkxgy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2banjenku.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2lpfzdmtt.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2nijljqwd.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2vyagswgv.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2uetlgdyr.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zytdkgip.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2tvakhkxm.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2mkzpuaxc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2prskqodj.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2tprfhwel.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2dqccykdr.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2wnlonlcg.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2lpndxoel.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ypdrcgxd.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2ojnuclls.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2abhazanr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2petvxtdm.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2sakxnlqk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2aigkdphx.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2xjmglblz.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wzrobsan.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2wtmknuya.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2xgmqadnw.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2vsnyyxro.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2trwencvr.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2htylbixn.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2xyyjqxau.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pujktbvr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2iffmpiai.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2tihoxgwq.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2weqegfwj.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wctlshtb.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2yoijpzrl.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qwkpmigh.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2rngghmam.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2tmkriwbe.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2wntaabzh.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2qvrfgajz.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2najpxeiw.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2iagoxpsh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ctorzedh.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2rkwpprqz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2phwgboub.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2wxwxsaqm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2oirvsqwr.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2zmafqaif.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2ilhocpay.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ribkrtqf.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2mjhxuhze.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2bnhwmdpi.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ktzoiass.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2tmtaknzi.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2fkhyowhp.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2veyaymsv.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2tleljhba.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2gyxmsmil.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2peimkjhi.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ovuqinix.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2usfmznii.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ipjcdfdi.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2izbpkssj.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2nryvqgvx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2flzlohbx.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2oawlitkw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2dqumwgyi.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2hnwgpefg.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ahpsldvs.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ywmgsjov.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2pbebjnoj.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2cnrvrihm.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2pbzezbik.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2festnfil.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2cgrqvpen.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kiybaepm.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2mpzmgzlh.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2xpqnwsot.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2uuxnlgxw.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wgwnldzp.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2elpoqpag.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2adamginn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vhlatvgo.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wlbidcyy.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2wvkjlozn.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ezqlxrpj.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2starzhnt.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2umrosqep.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2tywhiazz.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2wqmghwed.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2fyijvpup.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2vbpjhfik.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwmnulai.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2wioioqlw.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2hkijcrtx.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2kbenilhm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzdfimde.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ehdeyfix.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2kmefcbqg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2lnexbdpg.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wdkqspaa.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ffchjwfh.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2gymwynvm.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2psdyxztw.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2tyuxzuxj.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2yqeppmkw.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2vrdtbywr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iwidbfen.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lepupuva.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qxdttyhk.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2cbrlvrqn.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2pmjzyxmc.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jkkycawr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2kvmmediy.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2zyquuqud.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2rszyshqv.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2zfzyqefn.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2mofpezrg.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2lhseavxa.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2gzyzoitu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2izofxdsu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2lsleyhbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vgyuujhq.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2buhbodwe.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2jtuwwsck.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2euiurcnj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vnhppvzo.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2khrmmruy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2fwguvokj.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2pmpnhded.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ouotpwno.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2qpwgpoge.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2oizbavka.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2mtvtfmud.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2tvcguwbi.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2vbtjyogv.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2zryqhjpd.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2yhxzuvnr.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2qvahgvwr.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2yictsywt.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2nvyokhpa.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2thkgdcss.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2ohdesrcf.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wlduanft.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yoqhamsl.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2dgmopwyk.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2emmedlld.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2kbvsiqnq.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2vpamaccc.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2toznablp.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2fvctqesr.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2tawxksza.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2fngeeqjz.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2wowsilcc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2brlpeaqh.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2ewrfjsyo.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2fsutwxui.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2avvtxmch.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2bzqxkgrg.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2jxahhlps.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2vqfmszqn.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2djxcerkm.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2bvihsntf.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2qqcagros.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2lpltfzms.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2boepcsid.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2vkfyxhrk.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2meuggrdm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2swaqwqir.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2fivlwyes.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ugwafwjj.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2ocnrvkdr.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2vcztcfyj.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2avcpeypp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2dppnjmvt.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2blmlcgtj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2mduamikq.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2kkvplzzs.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2upxdtvmj.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2gchciqgf.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2agbutzyi.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2lqwdviaz.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rjslrckq.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2yvzwhcbg.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2nynhctif.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ntqmxaez.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2tgbhtypg.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2bmwtqqsm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2hiiqekjh.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2dhkelamg.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ayqzqcmp.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2rajgmpzi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2heqwvqex.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2awelvuic.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2rnelpgff.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2lysfuggq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2djfpfyam.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2scjdpjpa.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2dboluxpf.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2ffoiykdx.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2crxapvem.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2pyarglhi.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2cqxvvcin.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2rgsnfzrf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2ywewbiuh.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2knadsaek.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2fxblpbih.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2uycwfxzw.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2wcsolwyz.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2vafzhsxz.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2njakcjwt.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2yuvmigqu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mexvedhq.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2xfipwxpw.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2hfgzkncg.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2egnqnljy.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2cwmcycip.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2wdwlgrkz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2jjjdnahj.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2bzphfgle.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2rwmwyrim.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2cfoiodmb.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2ymoyeqxm.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2rifgvjyw.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2mhcnlfwp.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2wjzlkaeu.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2osupqenh.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2cpdxoanu.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2toplymxe.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2xfzzaqoi.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2ftyvxzsm.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vappoooh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2rjjsoaup.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2aancrgpq.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qylaudlc.html


<!-- 参考信息 -->