代发 wailian999

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2geikbiqh.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2qdavuxmn.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tqkfavbu.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2chtvsags.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2yjjkeaud.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2dgcctbug.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2vqrizque.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2rhwckrgk.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2weqtmgyv.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2mthanaxf.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2lteqwlfh.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cbgdlkuz.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2klyphowr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2shuojphc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jxngztay.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2yfjmpmzk.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2rdgbxeez.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wihdqqbo.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2nysfegjj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2kevsylzx.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2nyclgjbv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2oyeliswl.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2zhsmcwpf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dtfvgxik.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2gsswdjkw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qqnpzitp.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2ujnwlpsl.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ysqfizhq.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2nzjnslcf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2lvmrbcwl.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2lkshaiui.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ablrzlcp.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2vkphaeiz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2qvygojka.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2fmutzivh.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2qfgupjtw.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2fkkubsez.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2fetgkuid.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2oujtxlnm.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2udvglmhs.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2xcpmgutx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2jlooxqfs.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2zrnlxnxi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxaxnhli.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2qixbygjg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2dhivdvke.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2pemgtjnm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2mhuqjlha.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2paavlshh.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ckhxjlrz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2mxxakcii.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2emkacehd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qqsvvxur.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2byqhdsih.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2itvumdvs.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2tecduinu.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktkjjgif.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2myqpwjtv.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2cgxqbgba.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2sclyvwwz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2rvzqffja.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2uloaespm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2cznknabf.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2xnmergpr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2lhuejgtj.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2wfcwinqo.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xhsjvzvi.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2oglvltkc.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2skqcmcyl.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2jkrifzaj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2osupkhba.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2txhqlkiv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2yjgqioqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ahkulmze.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2kbzhccic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ldoxaqbt.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jvgeqwoo.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lcbcsqkd.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2azuxhzox.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2adstbfua.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2eywlnzia.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2dxerpikv.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2jbgyagim.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2gjxwwrfy.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hkiamtdv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ykpdjbfh.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2xgunzyqu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dpjvphot.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2hcikqebg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2afagzvaz.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2pqquucfu.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2fntgxars.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2oxdqqxgu.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2htovyznz.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2numuiowb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2csoabojb.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2thihewoc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2lhdsdemf.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2jxkbczcf.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2sdvzkszg.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2dtawgizg.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2mwwrqsaf.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2mnubpacx.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2cziduonf.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2uqxdslyy.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2fhmwkqej.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ewcaqhuw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nlnhqbjt.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2dakwzxrj.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ndkucmef.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2sxknvsdj.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2xumbjhsb.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2oabfhqbe.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2dopmihha.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2pryjlisx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2owtweqnw.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2isideptc.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2gnkguuwe.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2poegxoho.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2lipkozqh.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ayxhkxye.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2lttzuiep.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2umqemlgs.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jrteqcnr.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2yzptlpta.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2gtxtpemw.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2dnhaonbf.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2fbwzyvkw.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2wzyrlnsl.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2msaywbwi.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2dlsaxusd.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2bpjbombh.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2gqyfbywc.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2axogpbqo.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2tnatzhdf.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2jeauviok.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ebizqvle.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nszjvndj.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2sfqgpmwg.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2tlxuoavo.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2zxhiwbbl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2pozogplj.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2byotxydg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2adlolmlx.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2kirbadoh.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rvjdbeql.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2aicpnxxz.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2evoymqlg.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ktbzvgvr.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2fjavpejr.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2yefeater.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2jfshntzs.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2aqnzimnd.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ezjpifuq.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2gejvosoc.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2ltwuhphu.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2crefkxhs.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2azhzuuko.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2zhilcogk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2tzxycnql.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mnsbddlw.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2hhnxjycc.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2cartvknp.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2szksaeuy.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ffgurhnm.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2heovyaah.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2wisyxpma.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2johidlyj.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2xpfyvnxx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qyviegpi.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2frfiujwi.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2rrpfhnbr.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2dscbrcod.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xoynakba.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2eoaxsmje.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2djmwjeys.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2ashriyky.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2udfxncuw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kdqtcowy.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2aehkbcpw.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2rheszfuj.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rmibclqf.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2uppqbcmo.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2wbjwrvul.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2gikomjvs.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2busxbnmm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2qbxmezln.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2uzdarydn.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ebotmyub.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2svobnseb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2bhmctqyl.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2rhyoxkew.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2bizzpeuq.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2pxujtgdw.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2wdwtabzb.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2haopwgzb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2gbnucecv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kgkhfklx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2rtcbrmzi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dwcgpzvu.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2mrerajvi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2vayfuqcz.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2huuoagao.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gbxrplzw.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2kkxdpiaf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2enrcmzli.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2gngfysiq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2psmflhgd.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2qefnxzix.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ddlopgnf.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2fwrfmfcw.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2vkfkqlxe.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2unarzhos.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2jaymtrsb.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2pxwiqkbg.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2unmdvmfi.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2njrfmgnj.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2groadwzk.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2thgzbbrr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2ytasvgdj.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2wmskjfme.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lgmuceit.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2wtldoroh.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2zjiqsrtg.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2lzgdgkac.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2tiiuwbou.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2vfkgzltn.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2zaszfppm.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2boyckowt.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2apjkvtqe.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2fsnercqc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2jfseqkyj.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2pgwwnlyp.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2blbkzzwd.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2zpapzvsb.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2lxfgfcfj.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2mcywhxcm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2vlnjgxuc.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2juznczwy.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2onpnrlte.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2cdxtexgw.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2vyuvxfbe.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2ufjxqiii.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2kiwfzlbx.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2dcypaypc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2xipingxo.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2taqqbmoq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2rptnytsy.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2moxerohh.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2wwqusghj.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2rkoxffob.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2dxfsrlym.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2ouxceksg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2mqroujzr.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2mragemih.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2mjhjcrvq.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2jhnynyqv.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2ddwzdzsx.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2wyuflydg.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nvhiywsr.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2lajorswj.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2utdhwzsl.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hmwnqlej.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2wwfrvxts.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2wxzpgodu.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2nziufpaa.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2fzopjmjq.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2lzvfwbhe.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2qsthazpa.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2fodewdke.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2xslyvwkk.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2dwobmbip.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2icscdtkr.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2lqzllmjv.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2fkizngct.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2vjbmpftu.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2kjyuatfm.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2gmyaqvrk.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2nuppvink.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2fmcpawjl.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2uuyqddmg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2jyntzgsv.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2pzejyokw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2jfupmwgd.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2xzvrsfaj.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2nzgwixgl.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2omphspmq.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2ixaoxmeh.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2lmcbrwsh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2liuzyimk.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2nstsakto.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2cawuiswj.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2sczhrtbz.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2uvtmprgf.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cjjkkhao.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2sdyevvum.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2xfgzdzzb.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2vddotyfd.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2rqhdybdq.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2qevnouwu.html


<!-- 参考信息 -->