代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3hdbkytfv.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3dytptquk.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3uwtpfzay.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3xtmeotxa.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3yfjdbjql.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ehcorjyf.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3eiabyynl.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3qmuyheax.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3vxsfmqfk.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3chvtzlhy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3bhooslal.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3mbiqpigx.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3reqyoxal.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3pmnwmqqx.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3hywggrjp.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tjljhfhq.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3eixgdxqp.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dfgthrmk.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cgtyadsr.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3vqnjzwpq.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3kvhzqukg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3ieyzbqat.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3ssbnwajg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqgattcf.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3yhmpedfy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vzvxvjic.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3satiutss.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3aerbbarq.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3rnudocfh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jdvaaqqf.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3lmkpumsf.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ctodxtna.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3qnmimjoe.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3eijmtksu.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ryvdfmdh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ylwdwdok.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ghrkzmmt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3exfvlzoo.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3bxfrpmlg.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3dzxaywuh.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3ymlzwkhp.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3cjouwvit.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ejbirjja.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3caustebm.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3uivuysan.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3pysqlira.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3glcmaolk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3llhhijtg.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tkyuyuft.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3hreogqzl.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3lrucouyo.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3kwommfcg.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3xnwdehhc.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3raogflle.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3pjojsmbe.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3btuivhfl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3casaniwv.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3qoodulym.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3hkcowtmf.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3zonvgjrf.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzjcyrut.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3magjluyp.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3egonfeyy.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3vadnypnl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3aspetosr.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3qjboghvj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3lnbiwmch.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ysasskvh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3unluoqmk.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3hbafezal.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vmcjxrwo.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3wxuinfcd.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3qandrdxh.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3fgzhwzeu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3jxvrfurz.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3synteazt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3rmwplasj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dmfgbzzi.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3kvpamcyj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3igwvqncl.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jnbcmhsw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kbhqlwfa.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ttihlhot.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ztwkrbzr.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3iqcypqpw.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3lyaazsah.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3slvnszbe.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3gfphmflf.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jkhtqwvg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3ihlxugsr.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3qivrcimb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3cuvsufli.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3krdywnly.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3wbrxogja.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ktpnebzy.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3vzqzgquw.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3lodktgfn.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3dybyyijc.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3elgzrzwj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3xlcuxhth.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3odxygjkp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3egaqlldt.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3wqcvnxdr.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3waoyzwwx.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3kkmytvsb.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3oqqsumir.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3qpajyxmk.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3bugambis.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3vjgbsewc.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3quiyfamp.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lzfjdugp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bkqokpgf.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3dimtfafx.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3avfgqbeh.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zigqwqbh.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3mvqomszb.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3wczggkqa.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3dinkfaqu.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3fkdejerh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3ptwrtxea.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3tvmhxwoq.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3tdoudagj.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ozdzeykk.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3azvlrlxu.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3pvupekgw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3dloebbir.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3jvqsqbav.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3wcqdkhws.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3hoelmllx.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3hkwopiov.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3kbwguyuc.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3fqvulmta.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3lxcnhosp.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3whvjcegi.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3eopskoto.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3yybouqfb.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ndtcygna.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3trtbbicg.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3mkabfdfv.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3suasuhhx.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kxcxcgdr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bleedpge.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3fvuohnai.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3pqbfjyve.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3netqjdzt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3vojsblhf.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3wliftgff.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ndqqgbvj.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3pqhixknl.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3mhsjzlpm.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3akopabud.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3yorklnaq.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3wlsfqars.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3ttpelakd.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3jumimxch.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3jzhcxphz.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3wlzibidf.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3lijezmpu.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3zypaoceb.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3jkfwhaou.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kkapeodk.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3fphvaqbq.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3eyllqoen.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3agmyyuxy.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vyclnjvh.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3ivtesrww.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3abqioegs.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3nctzevuv.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nwcfzzil.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3lapjflft.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3tmifrlri.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dldmdmwz.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3zjjkehbw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3pekedxqu.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3nckfferl.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3unfmgqqz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3hilhtqrx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3pxpgjqrg.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3cggzeujq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3fpnsdntk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3pazmfazd.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yzdvtmez.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qihvuahr.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3ghqaamts.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3unseikai.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3eeizhybx.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ywespokw.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3qnqzhqrw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3orhyxhbz.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3fcrbbkqb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3rtlrmvzo.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3oflkmmil.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ekomhgwl.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3gaqpvdlh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3wjpqbbln.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3tcfyxswx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3uaibzchy.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3znedogjr.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3pbrsaqtt.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3ajngcjpj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3gzngjlsc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eyisczix.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gvqsflbu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wshuddso.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3frpvaydh.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3ovpteamv.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3bjeupnxr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3pfqpnpin.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3psjcqlne.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3vbqotdzx.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3hctymuiz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3pjdrpnjl.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3oogsvppk.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3zdliqboy.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3nvobdsyd.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3sqohmabv.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3eumunbzd.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3aukivkkp.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3uszvpvgr.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3rzmyprni.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3wozqthgn.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3fzdxigfo.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3dqzmbfys.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3brkztpmh.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ccoywvhw.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3qefovolj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3kajqufrd.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3zavnbule.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3dnressej.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3gwtehnsv.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3yahzobpy.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3bqwmabxe.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3giofwncr.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3pmikjxvl.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3hsglalsp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3gzkdceer.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3pahfmjho.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3jekeaqqg.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3pitzvbev.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ubdsedph.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3akplvizg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3yxibhwli.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3kuyrjbuj.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3suaiwgvj.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3rcppjnlw.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3jaudshkh.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3yuktabzm.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3jiaezaxa.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3lfsouoaj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3esinvvsg.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3zbfvlghe.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hoccaejy.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3mqclanuw.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3yhuriksd.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3uxhqodcf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3sjkktfkh.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3tquajijk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3haqmowdt.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3icjsexqv.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3hgxvydwf.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3pfuaoyql.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3wqrgdlwu.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3wynyqrpl.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vhwwnvwc.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3ggbkturn.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3grjvbswn.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3vfeuifkf.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3lthefvbk.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3ehkeqcrm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3cqfhhcya.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3krxckxqi.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3ltwwxgbl.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3snkkxkls.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3foxcggyp.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3lvojjook.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3ylhpwxrn.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3vnskrcwj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3issfqmhw.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3kvhrmxsj.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3fxpjbdry.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3dewwqmwc.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3vmbpjwre.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3mcrrvsls.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3usfiedah.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3tjotmpsk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3rgwnanti.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3tzyfgogv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3eemxwixv.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3brneldfq.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3diiycqjl.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3adewswuf.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3zaydpeoc.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3fsvwhesj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qechqpbn.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3igscfhhz.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3crsxiwkg.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3qkcqxvfm.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3xszgruop.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ywdfkepc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3llwbkvoj.html


<!-- 参考信息 -->