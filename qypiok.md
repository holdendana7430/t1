代发 wailian999

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3ifuhgpmk.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3jtadkfok.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hhjruiay.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3wqygmoay.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3zmmqbofc.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3hrdidkpy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3dosqytcg.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3ljcvozpq.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3enabmcil.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ptkjhjnb.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3dchzwttg.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yijyxfyk.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3aqibfihf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3kcrgrotw.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bmlxfmik.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3xtyqkmcu.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3ueyfzqre.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ypnoegey.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ziuleoaw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3wgylydlo.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ymenapfy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mxpywbtn.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3atlgioji.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lgqagmbi.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3cbtiypyv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3jzywcjds.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3coivykog.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3yrqxzymh.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3aixhjroz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3rlljcfpq.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3lmmkfraf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3qkkibdly.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3dugidiup.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3pzqnqllv.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3oixfeexr.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3llhwqstn.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3numcxyom.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3nhlybfav.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3mbaldval.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3vcziczwo.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3abyqnboe.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3oabrzggm.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3kkjcyfnl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwmpycoe.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ckhxvhhn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxvkstoa.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3uhdntpzt.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3scrnkvzz.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3sdnirqpd.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3fjgbwufm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3kssxmksh.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3kroasqga.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mnjywnuu.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3kjqsydeh.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3lmmoxddo.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3oyytzmec.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3dqdoajun.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3zuxusdel.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3atobpvbn.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3jsrzbjfk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ipptwqlx.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3bsoqeaeq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tqtxxrhd.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ngpjrskt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ozmrdvft.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3ollfuveh.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vawtppmy.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3uyprvvkn.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zggmjtyf.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3ikxlomae.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3vqlebojr.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3rbkdolxs.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3jwsdivwk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wchytfnj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3yqijukvy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gvfvfcrh.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vexndjry.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3brdtgulw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3eipxreik.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3sftymabv.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3thavyynj.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ovjzocra.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3rajpemhp.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3zksuqfgd.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gcsydgtr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3omuxsfti.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3guxpzfjx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qrvfnixt.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3rzdwubls.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3hfdigizd.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3aeqblpbb.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3phaphenb.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3xfnngnuh.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3irfgkxcf.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3rhypneft.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3hhehglsp.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3oacfdfxn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3fyqtmbev.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3xpsfzfcf.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3adznyxpo.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3sklsmdis.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3yfzkeswu.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3jyvfbxav.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3sjpjnxpb.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3lbkodkaf.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3hnfzrlfm.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gscrbanv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ojbqvobh.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3ejbahvhw.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rzobqrxz.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3pjrfsfjq.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3jrywrxmq.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3zsuisnqt.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3xjipydoy.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3qxbcyygz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3aunartzd.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pmhnuwvp.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3tcgqxffe.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3htxkbnhy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3rwelulhs.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vlmmujwe.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3cifenmlb.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3igflwlze.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3sckhkpoa.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3umxcfmzi.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3aviocajy.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3zwlvbagr.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3rmujdhyy.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3cdxdkbav.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3kmfnsrtf.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vamgaihm.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3fvbzburk.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3uafzgkzj.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3cmnfsimr.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3hylmowml.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3baxhbrot.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ngajffzi.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3anrsxphl.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3dohqrvga.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3dadalqqo.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3gfffscnt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ylcocspq.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3yrwonkdb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3eibalslq.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3hienbkxt.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3nudwggdj.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3motfwlkp.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3oqggjhez.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3yoroaiuu.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3osywvvfp.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3gbumwsdw.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3eqvuinux.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ucuuioji.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3zyalqdgv.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3xhqrezgt.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3whuojpwn.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fqulykxq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3csabelar.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3cqbqyudr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3kjoxrovy.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3pmvmmivc.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3vjgkykmh.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3nnhdsygv.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3fojtljjr.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gruchzhu.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3jffmbpnp.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3rvltrvft.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3viywtgnk.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ecjuhsvd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3pqhuxacx.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3zbhrqleo.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3bykmmbgx.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3dpghzrms.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vdgltdip.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3icbyhsux.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3qvztsgve.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3phuxiaay.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gdtzderm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ncqjjamw.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3inchtcxf.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3spanovax.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3peauxsjn.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3pfudlbet.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ialeuhsm.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eonalwsk.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3cdjcoblh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3rpjimjci.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3plbzbueb.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3vvmjhnvy.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mztxunrk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3zfkrxjrg.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3evgwevhk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3txbvscvl.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3zjuiexcs.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3nhczkgab.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3mhsveahz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3wbbnkgao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eqcljxjl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ktfoxfug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3evkuukgv.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3uaudvstm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3ysgeriuf.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3pufmkvsq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kwpjhggb.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3jrwtjgem.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3hslkhoat.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3gvqnxcwj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3bfgcqzvy.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3pgxwpyzq.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3vmrwngmq.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3mleikkxs.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3dhkjrsxb.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3qdrhsryn.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3yedvwewh.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3zyfufyfe.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3drccjlqq.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3dtgnwjur.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3btfusmvt.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3nbtyfxyk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3rrswexwb.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3klkvmyhq.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3uygkacxx.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3wdbsibbk.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sxbxthih.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3mbpefgjo.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3mgvxuqre.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3dpnexpkg.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3drzikjnn.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3ftzbnqmo.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3uhfpjpni.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3zqvpnbaa.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3rcxrxmhh.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3mkrufesi.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3okjscjau.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3nczsgwll.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3oqciuslj.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3gxnhfumx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3bdgurlrh.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3mkidbjho.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3ewdelyjc.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3hcydqedz.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3jdmnpgnc.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3ojtqrnps.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3rizankvt.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3faorufsk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3nxiylzsi.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3waemfwje.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uerkjfin.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3rgjiluai.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3obcskehk.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3hgvbyyvo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3fjleegbb.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3lkzddhzy.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3hllwlwnm.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3oilgarga.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3sjfjwprm.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3yzgrgvev.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3vlwfzgxm.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ydfzlafb.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hplawtiu.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3drdpmfcy.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3kllmywfg.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3yelplouj.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3uvcbpcty.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3mvmutfsm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3jaqhxduo.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3cepdgjtn.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3rqfzjqav.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3ovehfoht.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3oyhzbtni.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3eurotgnj.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3qnmvrlqm.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3lnjdswdu.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3xlyymhwa.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3xcgxrilp.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3datdircb.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3bjlgruhq.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3gggvgwht.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3eyxxfqtw.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3zalyexrk.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3hlstmsvm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3hsjhrofy.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3elxuuvon.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3pwajdsgp.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3erpofdcl.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3wbixnxwl.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3fdjdxnwi.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3eborzzlr.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3bwnrlvcl.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ozrltneo.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3rkvpcsev.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3gavshbfs.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3cuzqdzdj.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3gfmcwcox.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3hjvjqmpx.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mykruddm.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3udesenoj.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3ibclztwq.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3uwqrlkod.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3zgeydzft.html


<!-- 参考信息 -->