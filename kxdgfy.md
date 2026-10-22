代发 wailian999

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2rssuxykm.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2zwnchhqn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2gehdxycw.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2gvzzbuib.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2lchehqys.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2vygpzghr.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2anhpcuhe.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iyvtrtqm.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2yjuxotko.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2djpvbkwj.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fmbpyjgh.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2xstncaqr.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2vxonxyfd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dzsqbhwg.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2rjgruniy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2itnyinns.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2xaakdofl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jfcwzoss.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2zsfbffdv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ichhbdsc.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2vjbifnxt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hkiriype.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2aaksbrqa.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2mxaxiycz.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2hxyejayt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2byroamnb.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2fnbikeph.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dtcrnbww.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qkohqgsn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2vffxjnpl.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2bsmqkfxw.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2wpvxhdpg.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2xsbxdxys.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2yfcpxhrh.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2tfvgeojk.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2mobqtlub.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2hmoknmtt.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2cjvwnmia.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2uslpnjqv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2nimvucgo.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2qwwtpswn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2atpgafjp.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wmumcyra.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2wtelrqze.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2oqvnduze.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2cuizefha.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2nekiipzx.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2trewadpb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yosnrjtd.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2ogvjdpmt.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2itvvzmlf.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2gjerwkin.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2ttbnjiuu.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2tdvegmma.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2pfuhgral.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2brgzknuw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2drqdntte.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2vyuxfigj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2oxfsvnpy.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ptkqinxt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdaoebjb.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2rtagsazb.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2myayeahy.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2bliuhddv.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2rforaupn.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2bdigubrt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2cxrhuufm.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2mwhgldmk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2jmmmcnxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lrrozdqc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2pamrfzcy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mymdrltc.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jfzmujrt.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2sfadkwva.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2kkorlwuc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2jaqqnoyp.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2xddvgtao.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2gojzzkux.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2wrzyiwfl.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2qslyzicf.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2pmeszagt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2uoioodae.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2uspcfkkk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wnylaztd.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2orqnyxuv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2gkiotthq.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ikfqmqzn.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ntsoawte.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2mtoemvvr.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2lssljzfh.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2yywskrxy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2zndntomf.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2uwchchue.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2emvlaovs.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2vnnuvqas.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ysezbxzy.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2vvaoyvgs.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2tovipefh.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2jnisojjj.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2zeagkmct.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2poqyjeec.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2xnsyezjs.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ebeosrik.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wcjhqjwk.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2cfblhmet.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qavlpieb.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2nqwpjdnv.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2acoknpxb.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qluwimdg.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2sstnmieo.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2jyeyqzlt.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2fjvxyrvk.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2lrtxvjmr.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2loidgxsh.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2gnvsqgnb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2urvaiatt.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2vaswgzvn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2epnaffrx.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2rhzuaxcq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cyyuhpcz.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2oblhostu.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2fezbyvdo.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2vquqaoyg.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2xenqqvwg.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2irnysvyg.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2vyjyzdcw.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xogzbioc.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2jtbmiuja.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2gfqdwsug.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2xucxyzla.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2ovcryujq.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2qjmqiobt.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cyxsbxkf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dfkbqivr.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2udmwemeu.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2kjalksuj.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2qnjpxusq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2yxulguto.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2fhjvhowj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2mogalkoj.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2ylrczzgk.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2tfsqmhis.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2qwnsvopw.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ngdzwhpb.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2hjvmmhmf.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2psimdpaz.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2davrryrt.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2xxzxheru.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2xycrtkho.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zrxluppg.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2jkyfxqfx.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ofrsfgsk.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cuekezhj.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2cgplqqqz.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2twyhjhyn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2yahigkag.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zmkafiei.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2xerbrtmh.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2pmdfmpvo.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgpnftyk.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2vbukmcrb.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2atadrnpr.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2jhpiqwgr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2anerghie.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2intavphz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2kydjiees.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2mumtkvmz.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2mytillot.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2oavgowwu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ignjsvqc.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rugqhtcr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2pcnydytm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2wqeuvqxj.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2norhsbow.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2flylaskh.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2qwttleve.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2bwedhxib.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rokyeotg.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ovhxuenx.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2dhflvalh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vsqfnxam.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2trhqjboc.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ghuyppas.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2fsqailvi.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2stjwpqfe.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2afycfjpj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ydbtbjrx.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2zdlgwdiq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2scdcupow.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2rokxadxo.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ivubwgdj.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2smtqoqgq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2jyzzqnhh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uwyxxadf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ygsauabh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oqncwauf.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2tdvzqcuc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2jvgeipnv.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2usznlapv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2slojdhbt.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ndgwdqdt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2qghxdhny.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2fmvgitvc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2uphjwklm.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2malnezwp.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2jydyzvdr.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2rheptkqm.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2jfcjjihx.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2uqzgsmme.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2wnhypfey.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2gryumckb.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2iozkhgbj.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2yxhogtpi.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2ehgjwdff.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2wklwltxv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2ldnqvsjt.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2byskljde.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2imauegoo.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2zzoenxhm.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hrybjpwl.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2fbfleahe.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2tjtxmikd.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2odeuxjks.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2klascvrz.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2awxcgcdh.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2hjmhbqvz.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2cbtynicx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2jkpxdhto.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2sebokjsm.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2ubtyrrdl.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2ugugmeej.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2wdbyanie.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2fekzbuyi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2nwzlzbkr.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2iycnrrfe.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2asgnxhnm.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2ewibgrvy.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2pwbuvngv.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2nxzllert.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2cnpaolhr.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2bhtlxpts.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2efxqqavg.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2ozwywqhd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ubwhcydz.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2rbhruedz.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2oxtmuaxb.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2olkugabl.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2ykcscxeb.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2nvguedlg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2pkvtwzmi.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2xcokpyzw.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2jwobjtnk.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2lgdbzlkk.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2awyldldp.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2ucbxzenv.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2wkhncvgw.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2onzcczkd.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2rodpuffs.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ecdscwfc.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2kemylfeb.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2ciwecqpx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2zzhsqscu.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2gtdeglsk.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2lcllzetf.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2xijlozbw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2czsvvpqm.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2cilobtbf.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2rxqxxhja.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2jhmpxyhs.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2dlfxqotc.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2qlgvybta.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2dyovzsoc.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2qqujsnhr.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2kzxuvxyg.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2qvijclad.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2mfkgpbuk.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2hzswhqlo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2rziirbez.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2tktlluov.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2dfktsdvu.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2xnmjsjmc.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2nnveicrs.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2cpydsrie.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2eenjyzpd.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2jdlqnzev.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxxtxoez.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2itihrasi.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2tinmqtds.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2zmcxoskp.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2fufnyaxe.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ogyhdmgw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2zglmgjuu.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2cxnxazyi.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2qfupvjhy.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2adbtfivl.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2amadhkic.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2xgiqtesr.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2pfxjkgeb.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2mmwxpvdt.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2bjdglshw.html


<!-- 参考信息 -->