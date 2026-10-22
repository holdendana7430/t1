代发 wailian999

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2rrnblncy.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2vbshmoyy.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2znehwgdv.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cbgkmafh.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2pqxnhcpy.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uffrrjsv.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2fgtuxzxb.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2kpeyqjwx.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2suyzjmtq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2gcnmrjjy.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2gpajtfxi.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2oomfxkvt.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ljkprltu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2chtomxet.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2tsceubwj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dtdvaodq.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2hvypqwni.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2cennqfln.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2ohzrqpmy.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2wqmxdahu.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2kbsmzggv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2eugxltgw.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2pkliyuqb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sqcysaop.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2peguwiwn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2qechyfwf.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2bmiravia.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2injlqmce.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2dkflcpue.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2tlfyyinf.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2icfqshoa.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2avuqwjua.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2xsqapbgy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2buoeawps.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ytckprtx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkzvibjy.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2euepvirg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2izwjwhyj.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gbezcldh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2mlllitsn.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jraenmot.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2baddtmqu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ledcxsab.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2gwazfavm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nghhqhdt.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2ehovsdpl.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2wfyqqdzt.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2wadmrsco.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2baipdovz.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2afurlymf.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2omeablwa.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2tfanwtvx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2izyruvke.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2mqqqgegf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fhtpbwct.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2qqyuixwb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2deglaose.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2vhsghtxn.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2kkkntwqf.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2noghvpev.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2gwvnszse.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2dbxyggnd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2qevvfskk.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2rgkrromt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2xdnyegmo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2plihxytz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2pyyyqunv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hckeszir.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xxbcuxfh.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zfmohsyy.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2wtgyykfj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2jknqbiey.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2gpezfbal.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2zvvdfsbr.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2mowokchb.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2pnjdosuy.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2ksejifxu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2isonnixn.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2fuxcoofn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2afgkgloo.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ewdnonnk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2blruvfjl.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2rrvtzzmd.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2dqjmbucz.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2pnmdgozd.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2mzxhpmfo.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2qpnocvqj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2kfqsexba.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2qxxwuwgj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2ltapnoiw.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ddbohlbs.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2igrrmaqh.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ondfvjie.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2szidhvha.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2jtdhdhys.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2yzcjvjke.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2hdudtsvg.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2riwkkmcr.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gdjzobkl.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jyetoyij.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2jastigut.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2djuftxew.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2pjvtmwkh.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2xhahmouu.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2vggubtrc.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2fjdaidif.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2nrijvrdc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2koaawbxj.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bkosawkz.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2mjxryxuh.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2bpujqiwd.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2muvnpapo.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2culabyjs.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2yajqrzxr.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2fheanltw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mcgzphqw.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2fsawtxps.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2jnsyaewe.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2tgqfilnt.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2utpvvlkf.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2tvaksstm.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2ianxuync.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kxpynksr.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2hmgiefdc.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2kujjoubc.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2yyotghvl.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2azewddyn.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2nujnaunt.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gcqusndv.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qzvywtfc.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2ixoyggmd.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2nvahjwsi.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2cqkkhbgm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2lrphefpc.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2xfltpycx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2tffaqyyd.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2ebmliihz.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2coounzuh.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wgqmcgxf.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2npxuuzfb.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2layubahf.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2nrmzckvi.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2vhhjzkrl.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2gslabvpc.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xyuibupy.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2ljurszui.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2jddgnrou.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2wdenxxze.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jusoojrx.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2jgpbosmc.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2upcoaqhk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2pxdcbata.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rtapgqna.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2qiskhtzb.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2gaqczidt.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2invxuqzq.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2irbwzfyg.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybfjbbyn.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2onikirad.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2mpgbxoeq.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2hmmyetas.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2azgltegl.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2vnxyrasn.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2ravnjtxn.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2kdwadogh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nellzpkt.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xtlzsdds.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2wmovfuav.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2sfgmhzxa.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uvedonyb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2cunvpaxf.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2sgjkqcjm.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2nekccrfh.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hzujlcqt.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ycdyspmi.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ufoujfhh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bfjeerml.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wrjzhwkk.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cntilyid.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2jyciyaog.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2dhyxccil.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dujtuejc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2znzcldwt.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2xdknhjrs.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2siklpmhd.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2saharwnu.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2bbzdoywn.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2crbqfnuv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2tqvavled.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iuqqkeot.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2gfereekr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wqkckeil.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2uuorygmp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2hrfntcde.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2lhwmacsw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2lggbwuso.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2zucwgptn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2sivtdwdg.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2vhsqloln.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2fchlseob.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2btqxdabm.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2sbumjger.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2flnkihfz.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2uhyriwmc.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ugpgowgj.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2cmlbwmhv.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2szstdqzi.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2sjyacwnc.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2ykbrucha.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2cbzisjyj.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2gkuuidow.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2jusoyxuc.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2oyugnyey.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xsbqrwsm.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2inotuvkj.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2lrxxhmwl.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2bbrxjopj.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2fvqekujv.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2hhtprxbm.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2mdqpssjs.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2bxkvqnjf.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2znrjguoc.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2rmrulrxu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2qnyrrddz.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2naltpoxy.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2hctactuc.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2kipgrpkr.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2jxucadkq.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2fnzyatkl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2hxotxrcg.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2snyhuanh.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2yyyxeadl.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2gfizacmw.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2egpahtmy.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2tylhxqzp.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2tnktkabc.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2grnqygir.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2ukcbcfsu.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2nkcrguor.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jayixzxz.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2zdfqkdai.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2ozviuxij.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2fpzutsjh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2qhcjvjey.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2ydffpsbg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2aojtwfuh.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2awpyfhau.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2hiddrtlf.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2zvlfaksn.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2dxfaaytz.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2jxpfwprm.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xuwtypuy.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2kwddoouq.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2baaawvbt.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ogkfjqvu.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2hduhyrgx.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2lwxqchef.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2rjjpfjnu.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2wgkjitze.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2moruardq.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2qkvhrilj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2uepugtzv.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2pxcohhne.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2dgnbipeh.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2xjsclrex.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2hzfjthvf.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2wigggysc.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2xpiqkkwc.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2ytjjgftv.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2szvtdcmu.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2lzxhbcru.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ipxlbgxe.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2siesvdda.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2hcyvcqan.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2imxvjehi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2tgwsroof.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2ybnxggqx.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2epupzkic.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2aguhqaci.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2yxvxdxnx.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2hzdmiewt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vklhzijp.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2otwxwkgc.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2dtkpiapl.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2cayfimzo.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2ghzuhctt.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hioigcpc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2mmhondpe.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2isbfqadc.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2gyraqura.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2kzuypsbk.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2yllqwimy.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2neirvsmi.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2uhkoehso.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2gagabame.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2fvwzkhlz.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2mdtxsyjh.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2wiaxsshy.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2xrbasjec.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2jkktqgxm.html


<!-- 参考信息 -->