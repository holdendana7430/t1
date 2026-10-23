代发 wailian999

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3grxdttzo.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3eshnkpzr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ivealyqj.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3srgpywca.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3alrzidcm.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3sprdolmh.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3hydskrly.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ukcnygab.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3psvbaewi.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3kalrxjhx.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fkgclmzy.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3zndwcvgp.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3tijtjulv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3jsxpromx.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3loqqdcvm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3mefvnuty.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3mrsbheda.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bzvzauqy.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3crgedyzx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vkszsfqe.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3mbrzurto.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hwagzrdr.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3eniuwgmx.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ixcsgcws.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3fmwnbkcv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3fofwirph.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3wxcpbzqc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ohcubpkj.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3eazletef.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ugdmovai.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3kpobtdpc.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3rwhbdepv.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3jqhupxtl.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3mcymiyzh.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3odapzzqr.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmuozxln.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ixlrepnj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3drbcmctz.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3hbgjdipw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ouibfxkx.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nbdqwwiy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3oahblotv.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ofywbxfw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3jxjuytwl.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3abxmnxwx.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3unkicfwi.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3pgrtdyzw.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3pwfneljv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3aduwoqzc.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3nrqaeuzy.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3shivoylj.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3sahehuct.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3asgwiuof.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3eluklopf.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3esrjmvvk.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3lzdbthic.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3evgsgohc.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3vzqwiidb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tuukyfom.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3edswsqlv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3flvggvjs.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3etlcowtb.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ruvsyyih.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3oojjkkuj.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3cijzbodr.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3qypvedch.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3hkkobakz.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3tpabmhme.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3lcfkvlxu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vfmcpunt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ikjfeacn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3brydiprk.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tsxhauux.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ngrzcxcc.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3ajvckxvs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ukscgelg.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3oqemjsch.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3osecclwu.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3awwwqyag.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3dtntyazx.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dvwnoifx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3zhkkelpq.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3oivztbzy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bjzwjoni.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pfkmvrdl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3rcqlunnk.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3qdljnvel.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3cevrnadr.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ufscxxsv.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3umtlabuo.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3itqfejxn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3prordtcz.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3selmdewh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3bjyjbpan.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3wriokwad.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3afwwflin.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3idbhciat.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3nrmchtqy.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3golgmewf.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3qqurfwzb.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3qomlapal.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3qtievyka.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lwyalngq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jlkrxbvl.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3frrixmbf.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3suggczkb.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3clkbuaap.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3cthtqkyr.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3fpfheiaz.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3xrphoyno.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3tlcorgyy.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3mvwtaovh.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3jknsygls.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3scnpzjab.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3qxgkshci.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3lbptxclh.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3lmjvztei.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3oxibxupe.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3tegqdfuv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mozuluqc.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3pkbreyrg.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3pbhjktqs.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3vkwxyfjv.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3hubcotcn.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3meciurdk.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3ufqreqkh.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qzmfxqke.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3dqbejpxs.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3cqraohjp.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ftjinicv.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3xbvndsgj.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3mudmvods.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qmatxetq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3didzlowm.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3uxjuqfdv.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3nyzspmvn.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3hqemxtsa.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3idosfigj.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3ncwckepx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3pahwxkup.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3zyugoupv.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qfnkdabz.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3wmtazcvl.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3yxaipfdi.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3fexngfes.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3coonhqik.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3mdiortst.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3jspmwxss.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dqnolopp.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3jbasykhz.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3amfudpfq.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3uakmnflk.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tgytnpoo.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3otocsvoc.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ifqqmawd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hogpwakz.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zoqjwnkm.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3txbjrtlv.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3xmxyujzj.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ioucqytf.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3karxompo.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzwudort.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3qpxjgkme.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvtdetlf.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3hwwftack.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3npvrpmfw.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3wfjgzoqh.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3foqcxcat.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3jxylmxgm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3spcccmud.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jtlpqgqf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3qklxsybh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3akyrlqwq.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3sjaeqgzd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cddisqqj.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3axjecvah.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mjodpzwq.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3heswdlum.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ptfbeozm.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3rdjajmlu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3sbmkuomi.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3skdpydrh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3gaxejevr.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3hhaqfxxi.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3udjofluj.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3uqljeiyr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3glhonnqq.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3tkmgsgcz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3gfemartq.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3zkzvjwym.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3gbbbfugf.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3jhzxaomg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3yicqmfmm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qfvygqlg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3udctgiom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3szghrrhz.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3lixhmrxf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3juhlenmm.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3pydwssya.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3gwsyyikv.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3pwnncnqk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3foyqblix.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3xgfcydkr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3vkjtvxfo.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3ezzkiztq.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3vlvaayfe.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3grmtujou.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3yllhornm.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3dedfgswb.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3mwfwbpow.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3zwocpujm.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3ixvptmgr.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3dyzyejui.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3jqiufnqo.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3ybwmzrmr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3wtmzquso.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3duifuhwd.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3komlayqm.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3rspflzme.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zgtdakdd.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3ndbeeeip.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3jpptyemf.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3fitmavsc.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3kfsaghgr.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3ylcdjmro.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3nvlptjwk.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3bkbfsszd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3veoazgas.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3lttopyit.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3ghiwspbi.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3uwyvoesi.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ahlxfuew.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3rismaihb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3sfeqowvi.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3doophpng.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3qvokflgt.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3zzusdrvk.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3ezivblwg.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3lmgepsar.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3divxregx.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3vcbgnpnc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3pubaepby.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3muhpxmxl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3uxclylyb.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3eoazwicm.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3qoyojvdx.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3hayadogo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3tkdawypa.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3iylressq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3nvacazhg.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3pistgnua.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3jkanrtkp.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3zkziuujg.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3zzvyhaau.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3vvpgzouj.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3xvtosplx.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3rqjxodyu.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3dqicbrlw.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3mtyxmbwr.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3losvqmoo.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3ctamveup.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3yjdeavnb.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3ufdebwrh.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3gtguvptu.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3hfkwydfv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3topeysqk.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3pjfbppwp.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3kwyfcgec.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3fuhpmpbl.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3xrcefdnw.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3lkemeyya.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3mdxqmioc.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3iaybjpbo.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3pzsxsehx.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3jorlitux.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3scxigonv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3ckmnghqx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3myscabcg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3miuamcfc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3bsbovhvo.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3ljjhvvoy.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3drkyairh.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3mtgrvlln.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3xfxwxfby.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3lgcotfia.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkmuonmw.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3adfywdos.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3htvqplzx.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3dgeuuhub.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3rqxdmelo.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ygwzwjaa.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3irlnruox.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3mjduzzhz.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3midecgqi.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3qmpvqeje.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fkgathcp.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3onulmeip.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3jlrzvmvx.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ddhchfjm.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3asryxhrs.html


<!-- 参考信息 -->