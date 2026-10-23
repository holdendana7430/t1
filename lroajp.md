代发 wailian999

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3gsbiegpd.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3sazqufqj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3bgnnfkrx.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3hporwuod.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3sbwabzas.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3rbrookzv.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3qkzzcgtw.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kzbgxfey.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3heelosjq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3pxexmakn.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3jlrtdutu.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3iiijvygp.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3tycqxqlh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3rnzdbupk.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3tvmcwlps.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3adpwekbg.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3miiilhgn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cuvkvyty.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3vkluxebc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3twekltpa.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3hnvssxoc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jjutrfpu.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3tpmbilol.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ihzlczvj.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3amidjgbb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3kndjwpxp.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ldlcwaaj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yfnourwr.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ryfnxkzk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3fkapeelu.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3zjbvgsxb.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3udergysw.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3kztcbmii.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3aqiksbiu.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3tffpydop.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3umvdbcdh.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3lrchycyw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ryerbrhr.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3awevusdk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3obuecogh.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3kfkseqee.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3qmowytek.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3awfqefsx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ylsoombt.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ycpwetdk.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3qyypfsmw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3gmzdtcbu.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3wzeosiqg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pktpncfe.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3kwmnrhag.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3pydplhtc.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3arfykknf.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3cdxbpvpt.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3twtyddzx.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3wvcyzxhn.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ajolvkyk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3wfurupxr.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3fwdoypha.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3ftxjhoyg.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3audecnea.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3qtqfaayc.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3drlnhtbk.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3nceebhoj.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3prbjcwom.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3lqenrtua.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3rspyfuab.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3bflvnivy.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3qmdifgzt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3wfwemcot.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3swdvfgim.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3xogvevfu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dxwkahma.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wtmopcml.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wzqhubkh.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3sdguzkjl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3kbdfctlx.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3kxcwbvtb.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3cfhcllrp.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3pitbtprg.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3plgwhgoy.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3aumrlbfk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3atbqwnji.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3hmgemefz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fzrtnzrb.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3hlzxsbee.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3enwxjwmq.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3hgicxvup.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ubqrhukv.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3tofslqsy.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3xtwepazq.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3tsvqushp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3zjlcncdw.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3exgqbshs.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3zqtekeye.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3yfntcoqn.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nzohpewk.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3uqfihtgo.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3zpigtttp.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3dnzknota.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3rmljxtnd.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3emherdkf.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ccmmhubg.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3urkgckxr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kbabzxia.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3vaiohmos.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3dtfrpnlm.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3izcfqhjf.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3kylsqcuc.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3fmhgnnzr.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3fjjebidv.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3nbbbrjsl.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3vqbaufer.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xpzblxyp.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3xudkzvhj.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3veildbcu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3uqnxwkex.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3zxdrnxiq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3oxmiiqat.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3qckzhdsq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ikgpnjqd.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3vskakslb.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3zapbmvzy.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3vxmnhfdd.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3rpkwegfl.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3gbdlysyw.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3dxpxroaa.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3lgszisuk.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3yhajriec.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3vlclujqv.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3qrsviydz.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3kztujnqe.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3mlrswwcj.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ucvsvyus.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dkooezdx.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ffclaiwq.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3pualhcbw.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3umkvutxt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3yjdmhfhq.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3pojjsjbl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3mmqyuflw.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3yscwrjgn.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3ncwgxwhf.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3uwtupaio.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3qfdjymma.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3pebnrboa.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3xtsrljzm.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3pufollsd.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3tsmayuoh.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fzergvko.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3aqhxynxp.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3wwsndkxx.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3jbusmjku.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3umulsrpf.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3wlzfnqpf.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3obkdeamw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3atwhvhok.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3qhosmkpf.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3kpzluibo.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3sxtccsgc.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3rwpfikwx.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jjjnlrmo.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3hlbnxxqx.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3vxhjhive.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3qshkxywd.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3svwnzluo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3zxlqicuv.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3nyrordbu.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3eubewrdv.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3ftczqgfu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwhzlyjz.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zwiniies.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3qxswvotm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3osgctrjb.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3seofdcin.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pgiwrnqq.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ahhjdzpk.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3pjdulotu.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3txmycznc.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3bsitcuuv.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3pcinohlu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3qqlptvdk.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wazplcex.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ktzsiehr.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3sfmjtuzc.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3lpocqdnu.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3exzaakme.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ftikhlqk.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3zonqfurp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jvchukki.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3blolqdjf.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3xktuvbhl.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3bglwsexc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3bwxaqrxd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kblbrgci.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3podbaboo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vedrcypd.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3soxfqqzd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3nyagossg.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3avbmruku.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mqivrqtx.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ehhdkmje.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3zwhnfzgm.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3qbwigmtq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3eflyvvjj.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3tspcmeto.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vhbiycwy.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3lznglehc.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3uwwcrhvc.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ntwgfmgx.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3chuilxal.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3xpwoxtpc.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3abdmfnwf.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3rubyzlpx.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3kipbvxwd.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3ehkylxcw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3zhmfnjfo.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zjkjxuff.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rmfrykyi.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3bcqdjyfu.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3fsxbqwzp.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3pssfeyda.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3lrbeuwwz.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3vzjsjwve.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3wxsvjwlu.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3kdbrzjhw.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3qpxqlrlo.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3netvxwzu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3xbgobedw.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3kyvckspk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3efyqafaz.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3ormnxvjt.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3tamjuimu.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3qobqlxsa.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3aykkhtxe.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3tafiuxot.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3rswrjtww.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3yttnopbw.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3gxpbdbhu.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3gjvpnvuc.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3fevbqoyr.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3vqhozveq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3xgqnzdbj.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3diieatwr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hoykgnhk.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3zejtgcwy.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3mvwnoqyk.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3dngubyox.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3ekwstard.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3oknjanip.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3jvjxnnep.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3limnjigz.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3tnidtcff.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3ebdsuvdf.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3anacecha.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3fkzjozlv.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tpuiqhos.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3fbiwpzsz.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3fjhejczc.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3yrdybnza.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ckizxciy.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3dblnzujz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3knxoxwnc.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3vlkapzcq.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3liokkgkg.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3wacipkwp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3xyzhqfyo.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3ykcrslci.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3kioqbgbj.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3utdhdyka.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3xoxyzgqx.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3wpfwjafm.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3khxgouqr.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3zavfozti.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3fnetxump.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3qwbgiddv.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3vgdxgdjc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3tbvlovqy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3alimfwyv.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3awqhigub.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3flddvnyy.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3gzrswqen.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3waoagsoh.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3kqmatrni.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3txvifepu.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3mxzhxwnx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ndhfepbi.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3vesimlqj.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3dcytxinq.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3uyuhmbpo.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3rofxsjvo.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3cxkelesk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cwxhyohr.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3iapaoqxp.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3slocqgxd.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3dkyvuuuc.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ssquxsiv.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3hrplxrcz.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3secxdxpa.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3stvxfdvx.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3fbhoiztj.html


<!-- 参考信息 -->