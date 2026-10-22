代发 wailian999

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2uqcmuohr.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2mltvcbrc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2atghlosp.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2sqhczuft.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2blkwyfoh.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2pfvnapxy.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2hvsuhern.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vrkruciw.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2iggfhgxr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2yxkcwyjj.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yhavxjhe.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2vmlutsyq.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2qszpzqos.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2uoqppejz.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2nlsohlyw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2ulvjagmt.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2pfymoquk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pyzvrmjx.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2wrxdcowv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kirkohqr.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2zcshfwod.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2joymaisi.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2dwnisrix.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2fydpxbqu.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2txeeeluq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2etofvjfi.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2kxnpdbgc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rzggexow.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2lfvaxwfy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2sebewoei.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2nsbheuvs.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2anqmbzcs.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2slnvghgy.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2bnyxqcih.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2eewhawhk.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2dpbppkbo.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2dewydiaf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2zwjuitsf.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2qjqculnv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2nvdxefqu.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2guryegqz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2mtrcyvlj.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gskygxvx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2lzozoejf.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2abecfxey.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2ohihbfbh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2kqmrlzir.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2jtstziek.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fxsfkwlw.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ckuaeqmj.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2nprdyuqh.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2taudwygg.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2ygtuxcut.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2knkufqaj.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2uidwiqbu.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2jmekiqim.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2asilwulb.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2okdtfzvh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2jzunnojf.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2zglfxdiw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2xguxmseu.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2tlstzcqf.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2uqjllzhz.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2fujtriei.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tpeinpfm.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2ukdkwvng.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2jyqtensl.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2hpssbwix.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ieiaiywd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hkkqkqwr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2exsrlugh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uqvdhmqs.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wssceopg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2feqtygwo.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2xldwzzyx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2iqcilvzr.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2bnwvnsiq.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2jehjrjxq.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2inqzyyqt.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2yjgmknrr.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2thxmvrav.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2gzmsjswt.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2griyuisy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2cfktjgbx.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lrlejrkp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2vbfxcubz.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2elfoobva.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2twysgsfr.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ncraywji.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2tycqooji.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2tchlwyxw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2crwpfxhi.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ryuxffwr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2naqxwcxe.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2irkdlruh.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dnywhlim.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2befcnzee.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2lugmwsbe.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2mbqkbelg.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2waedislf.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ryxesegd.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2kiinmdyj.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2oshkuzgh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kletljfp.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2haivkskm.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qiwsoxdn.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rrmnnqaj.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2txshnhnj.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ddaxsbmf.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2qapojeea.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2zkcvzfrj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2hbmxqyxq.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2vpfwncwj.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2naotypmv.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2cljtmdoc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2izhejiej.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2hcvgqpir.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2jlxcjodu.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2rruryadc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bijacaxz.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2nqrqiqci.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2czjvukps.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2gtzslfxr.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2mizbzkhv.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2agroxnnw.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2gpijbfko.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2qlphnxgj.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2upawerap.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2dhoisgey.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2bgpfmxpa.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2mhoolisz.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2nbidytvj.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cioqbyik.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gvhqgcpf.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2zpaqpizv.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2lhnmdarn.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ivotqnbg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2ztvsdinb.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2xuimkvqw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2uwwqmliz.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2rsillvxj.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xobsfwtn.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2tszqjpei.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2lavljdjv.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2rrwhuyip.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2strndopb.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ujjlpnxk.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2gjarmqvn.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gvwjnvki.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2cyrswllz.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2hatbzrrd.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2schqygrx.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vpucladq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2axyvrzvw.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2qjndwcwy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2nxgyggmd.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mirpmkgf.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2kzgehave.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2aldonabb.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqdavfaz.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yexrtkma.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2fqrwhofc.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2jsjzntee.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2wswcfjms.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2yjmwrojn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2agrgleoh.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2qjudnwra.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2fxvplqzn.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2fpegjcxj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nekzgbil.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kvwwbyvp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2tclmaxdw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxniqygv.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bqmtmmhl.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vnddhoxo.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2gurxdyrd.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2tjgynsjt.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hcewfaxz.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2udpfhhgi.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2zpsxrfga.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lqpphnhk.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ebitywqd.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2srdplhev.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2zascwnhh.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2dhvkpuit.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vrqmksmt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2yxjdsqmx.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2nzpipzag.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2qbsyafry.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2wnndosvz.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2quyutbmp.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2brdnxkif.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2ngtminqq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wvlzkxmq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hitjnxdi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pucsdjou.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2mapjaqok.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2nrlnlggv.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2mvanrsro.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2ucdupyhh.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2xjoclbcl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2evsetqcg.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2lztpbwfi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2unsedutk.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2pmvutigd.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gjmrwkls.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2qraxycxl.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2ukxsulpl.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2vkfdhtfn.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2jduyzvpj.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2bkkgezoh.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2gwhrlgil.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2hqqahara.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2fwupvtzi.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2hvjclamd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2rjajmsty.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2fmygfmrq.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bzvgzcrp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2hctpzvbh.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2uowaxwxr.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2xdizxthr.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2zywqhdml.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2wbgozqdo.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2jeknkbwo.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2uspwrjke.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2hzddgtyf.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2ekbqynsl.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2janvbmpx.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2baoexthg.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2nydusmvq.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2fqoxvmro.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ubybxlzp.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2ezponatr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2kiolhcur.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2nzkjkqzm.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2dcmowqhn.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2cwkpdphe.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2kisqfshd.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2tznagcuo.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2ezgcvdgx.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2pjdmuvkj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2qpxdmavx.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2pydbjboz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2pgxlrvun.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2fibtbaof.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2lbcoqmej.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2sfqfkcfs.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2carkhvcp.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2shvnyyvm.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2cjbzzsiy.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2zgpzhpqs.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2liderzax.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2qtppvcuk.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2vtrpwnzd.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2nceeqbqo.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2peyjgcep.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2ykzuybrr.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2wmhqyzlc.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2nxtnhjza.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2ruwuxmph.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2tnxundyp.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2omzxfyig.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2atvhline.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ttgyasbx.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2gaxoqlpo.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2wydunhru.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2mbrsfrpm.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2qdbgtzrt.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2axhklhpr.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2oqosnjzy.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2jubbzxel.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2bajhlyfe.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2ygtpgpzb.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2xizxoscp.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2hsixqewr.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2xybtepyv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2kxdjirlt.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2myaxlsrs.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2fgdhduvt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2lbdugrob.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2qlpyzqur.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2wczmsfoq.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2qfazmvew.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2epsiyprv.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2oupylscm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdwmpnzh.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2janbarwh.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2amwuaflm.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2gqavlban.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2aioivqzb.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2mrrfizkt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2pyxykoqt.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2brwmwgvl.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2oqicjptz.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2hbnuzrbh.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pzsrarph.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2shemvyim.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2bnzhbuqf.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2cjfcwckj.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2mfwxpjat.html


<!-- 参考信息 -->