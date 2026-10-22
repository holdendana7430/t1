代发 wailian999

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2knuxzkvf.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2ylopfbkf.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vxwexdyp.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2ofsjtrvb.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ynooeptt.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2uoggwyqy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2soczlueq.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2flntwhvc.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2acnupsab.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2bqqkfech.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2oyuxfojk.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2czpnwszi.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2titrnzzs.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2twrdvdtj.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cuxeizwn.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2tvyyatxy.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2bkwwmsey.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mgtogncs.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2ubsvqksa.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2bmizrczk.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2wrxxrirz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xxlnbeyb.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2bffdcwbq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vbdowvjp.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2igtsojbd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2gbxdhjtp.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2iamqsooe.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2zhkcsxzd.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2rpaixinf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2kslkwayf.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2cpyxamwn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2yutvsrbk.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ukkhkpla.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2plskehxl.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ejjdrjjj.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2gadrozpe.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2txtimcay.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2fkzwqakt.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2doyfmejp.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2ttzudfpt.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2kwqaxuoq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2cflholgv.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2gslhsqkd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkrqocxg.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2tqkuhkxa.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2dddftzek.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rkejvllv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2pfxamamj.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2fkybaaso.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2mdxtmcsu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ipwtuord.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2zgnvrjdm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xoswvgym.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2qjliouhq.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2dmlufjbx.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2qacssppb.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2khmihikd.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2qcikawqw.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2nsowoiuq.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2plvwsehr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ycxmkyqh.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2fkrkukdc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fzovbsxm.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2vritzpqu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2hagpsofi.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2sucfiepv.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2myvsiudw.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2noxwuhlo.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qayxckdb.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2jmzurngp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2nzghzqpz.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2cokxrmgg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2oxqdlvjo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hxhpaxxr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ulsctkca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dyoxczdv.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bzuqpmgd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2eojtkiwh.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2evoaobyv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2baiilrxo.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2fhupjmho.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ifuwxyyw.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2btecdalq.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ayicreav.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2bfrrfnhm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2ubgdwrjy.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2qnlyjeej.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2uodbkuuf.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2xseqkeck.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ufzrkibx.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2zzkxoezb.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2wzvdxbwx.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2kjjscjga.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2czrnfdtb.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2uvudglmr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2gfroonkf.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2ebiyeyiq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2qqektkos.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2lqxxahyk.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wxdvyisl.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2kqfpqiuk.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2aalyoguc.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2hvgyosuw.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2qchccfjl.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2hchwoavp.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2kalrocwt.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2djiqoemh.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ultpuilh.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2oqhbljnb.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2lppsiriu.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jqkfqmak.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2xlvviajq.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2vkfizqam.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2agkkwjhi.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2rpvzzwff.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2aivouxed.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2ijxgdzcp.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2irizfcuu.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2viuvfydo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2tsvintxr.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2eoeowjcm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2dsgumzmz.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2ypeslnqc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pqzlxowr.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2dxduslex.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2wmaxsntl.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2gzbvtphm.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2niwmbhhz.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2gdjqdmvb.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2sazkmtwh.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xscwvdyr.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2qoldhwbi.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2nqmdqehb.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2ihbccksh.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2ymqlfozh.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2avaqvhal.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iaricsti.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dewoiixv.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2njqumhyo.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2amjthjxv.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2iimbsvst.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2qqkwjnuc.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2wzrfzyri.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2tvzuqadv.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2hctgypun.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2kdhmluip.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2cvnwkwpy.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2sgltwzlh.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2gttsdagp.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2hdqspfxd.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2xrwmsvsb.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2mtxjesdu.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2zfyzqzha.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2acenjhde.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2fqtstkyr.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2hdukmowy.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ecuuqlpa.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2bnvlqwkh.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2rrcenizj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xextypeo.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wadlsufu.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2gpahfaie.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2glndndtv.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxpzlntx.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ofgpedqi.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2pghnpuvg.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ssqeikra.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sirvmvlk.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2yezabklq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ukbdfmwu.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2tsmfwmfq.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2ljdqvyyc.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2hgdtibxc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vguqhcti.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rgyegsyz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2zfxmgrwl.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2raaqkkql.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zepxjnyh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lbtceriv.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2mruwbjmw.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qoyezadc.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mymakzzf.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2powtdlof.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2mdahofog.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rgktnsvk.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xuqybiqo.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2yioikimq.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2jcxdiiqe.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2mcohbdoc.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2csdkrjcr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ylcuahts.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2xtwhwcio.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2ffbxzuqn.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2mbboumex.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2hbjbwtyq.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2zqjssqng.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2rhqqatea.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vsqfccxj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cgkgmjow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lrxwwwts.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2oryzuzah.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2cmsuvxqu.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2cwepnmqo.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wrdsmtmp.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ograjpzc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2dpmjbpwb.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2isgbijqc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2scsjsbap.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ihxhyzqt.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2dqxapzhe.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2ewhdkwic.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2hzevklsb.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2txbybsyk.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2lnoryfdm.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2fdugktoh.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2jepqqlws.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2xgmbbxkl.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2omrdvoaw.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2ndgwxoga.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2zirrdcfh.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pstwncpw.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2rckguxra.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2qwzveync.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2hxosumal.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2wnvobcvb.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2wzmcqfwm.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2argivytz.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2suclsdph.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2cqbisitw.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2twxnbfos.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2bmrsjjvf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ytvbphij.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2kyotxgsk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2bblgikkf.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2doebijuy.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2kzqowldy.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2rzackahp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2vpviuoza.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2alzxptum.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2lvnxjfvc.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2gvcoumtj.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2ogotixna.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ltdcwbhl.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2bgxsnzvt.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2jjsvheqm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2jlbrgdxp.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2meyoefin.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cqjguczm.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2gnzhwglk.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2fkseoefq.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2aclhqbou.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2apbbodok.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2ehtyfdvs.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2ujbrxkwh.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2iyunogkm.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2qyawazmi.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2bcdhecer.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2wnjeqwyj.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2rwntauac.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2owsinpkt.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2zxbytrbi.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2rvalgqlp.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2pnsdhthp.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2jyfxkjxr.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2oilfrorv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2mogluqbg.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2vhefpecm.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2ijrdqljg.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2kirfcxtn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2wjtemfta.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2vbsynvkf.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2wkqrvyes.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2ucwydfuq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2jrgfnfjq.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2abizlked.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2uhvhqnkp.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2vxmevzsg.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2pangzjdt.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2rtowtvzh.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2rjswmkyo.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2ruyshbyh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2hpsvdzkt.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2nppkstjc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2zulvrvvs.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2hafvhdkx.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2xqitsoip.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2nqzimurf.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2zncbitkq.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2nhcduroi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hurbtbzi.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2fskdnktx.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2domnehis.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2ihkaykrt.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2ymhwyjkt.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2ylldauzk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2thmekcwy.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2wxlpmxrc.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2tayiqnhc.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2doswclfk.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2rdyabdfl.html


<!-- 参考信息 -->