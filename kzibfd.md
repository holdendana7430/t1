代发 wailian999

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2gsmsyxel.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2yusotyku.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2oiymahxp.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2nzwbazdw.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2qibgeawk.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2wuvcviqr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2nkdschsm.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2xndfzqgq.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2qitxawxf.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2gqxhrlco.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2dfsoolpr.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pjtkgses.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2mtairasx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2eqyxwmib.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kcddtygb.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2tlwtatik.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2hclydwfp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ppdomywa.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2safkipcn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdjzogxb.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2xvennael.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2phjegzpl.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2qpyizpvn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ptqbtesq.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2nzajulnm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2sfldafpe.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2rygrfvmi.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2taamfkbp.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2xmnggwej.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2dtjxuzzv.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2bteobfef.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2gpmblpxd.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2qioahbms.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2xuibkoey.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ykbnjqsz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2kfrhnicq.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2qtxgbasg.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2icdzossd.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2fwcwxbqz.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2gswmqiml.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2sewewziz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2tpnmwtxv.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2hioordiu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ypuljjvj.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ybnlmihs.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2vtspaizw.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2oqvvvmsq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2qtlywbfa.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dsjjqvzb.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2zwpkemgc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2herfjzwg.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2dkpehgyw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2uzpfwyxg.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2gqszsicx.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2edqvlflr.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2okuomwfo.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2rtqerhqx.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2ykyfibsb.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2yyxniddv.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2tlxxrdtv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2tpmkqvck.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2igabqmvn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jrggfhgp.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2myexslwz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2fjdngsyf.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2zndejhox.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2aezzysxe.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2sevnxufo.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tdqnsjac.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2uwfaqekt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2okvvlefy.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2vryqtyyo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vkcpqeqn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sxxoaznm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2wmmtmyvh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sbejdupq.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xxjfeztl.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qoqcwrra.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2kvtjayfb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2xyrarpbt.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ntfhzasf.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2mvkdandz.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2bwrcpjiy.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2bcyltgqu.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2lceqfrdf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ttxpjztv.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2stbswkrs.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ueujzyev.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2uybakgbv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2tvswvbpb.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2upfbimwx.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2khzjufkt.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2bwiwvoag.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2qdhwnxpl.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2mdcmizwe.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2xkzkatlc.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2ralsvqzp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2fzqnpmqg.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2svntbrot.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mlcikcrq.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2pqebytii.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2mafvatjp.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2italztzq.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2uftophdb.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2xghkqfsg.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2gyltfkyh.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2aymvfcgh.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ctjnivvu.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2eowiriqz.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2pgeeogqu.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2oxyccicg.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2jfxnkepc.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2msoxvkew.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2usknmsgc.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2fhmvaeyv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2cnojcakx.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2fxxgmekr.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2mqttdpai.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2lafymtem.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2mywecfiu.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2rggiyrlt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2fwitqrqy.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2nytqolfy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2hqiwbfxl.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2huhcmtod.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2tvsivfks.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2hmdrvkkm.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2olhuripo.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2nrvmzgam.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2lbwnugqn.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2czulzqqx.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2dojsrefz.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2bttfpmgr.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2xzbmgrjs.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2hbucgyvv.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2lbitunrp.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2shftxevv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lzssurqb.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2irinpddm.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2iwikdews.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2hkyolanr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2ccgeycdw.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2cuxtctzu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2kgmrzdum.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2lehoysmp.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xyjovvre.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2tdyjiemn.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2mpehfyeb.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2tnvzzpzk.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2zemdbreh.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2hjivnhmk.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2ayiudtpo.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2potyohwy.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2dtllnbdt.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2tmqhzmch.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2onibodor.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tqkxhbyy.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2yeghzrmu.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2npvrdfex.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2wbmsnncu.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gprbcxvo.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2zwihyvqf.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2kwigubwd.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nubghbyw.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2utdowzfd.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2pwxdfwey.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ykvlywrs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2msauqodo.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2mpwcdhrh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2qyztucgu.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2wqtnngmb.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2ipdmcjoz.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2kepubkgl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkrutlbp.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qhyjtvxh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2qnmdpojo.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2jycdsaya.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kvqjlubn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jicobbzx.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2sazwibtt.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2fvcubzcp.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ymytutpo.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2lrgpyobi.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2xmavcxnj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2nxbzwzyf.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2zpvpaxcr.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bdlhelzf.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2iboblxkp.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2mdoptgoy.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gaqujtiq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ousgvpga.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2dpnpyuhi.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2qmoezzku.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2bekfbxhq.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ntjvhbyz.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2lgadcixo.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2jpjckaud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aaympffa.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2klmxbyez.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ktubrqsw.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2msnmehrm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2driuarre.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ifuedpvu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2bsvigofb.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2hjkbprhu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2dgkjkowo.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2liexcpzg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2xfzbuwsd.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2xsctjigj.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nwhpwqtt.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2szxiqfzn.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2tmwrnhpw.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2lemybbxq.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2lutjrvgw.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2zmsbfwjr.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2inmoihyc.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2qeimryet.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2cuhkgfnh.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2ucbvqjsb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2lmahkpcr.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2fvecofdh.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2cfgagfpb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2orblabzk.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2wyruyikm.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2cpkpkbzc.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2vqsbzobk.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2lzcqhnsi.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2aauhzwun.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2keskmewb.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2fiodvclq.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2qvmfxnns.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2biuelrxj.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2xgkqmibb.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2kxzwiqob.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2uiyyrnlv.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2arujrvxb.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2zkmskaxf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2filnnokl.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2iiihwvix.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2iobyxfnk.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2crvnnndu.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2wgqphqeb.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ijiuekwg.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2qguhydss.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2lzscmhsl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2gzjnjohj.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2yxieyhfz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ogcxmvaf.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2dltlfatl.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2gzdgxoai.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2fmjwqwom.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2hvhcbdiu.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2wdqfknis.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2oxqqvgjq.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2rdcmdwab.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2jrqciaxl.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2afmsmued.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2forjcnsx.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2pannybej.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zddvejaz.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2ulbsqhfq.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2vlwqwaya.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2aslfqifm.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2lqvocasq.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2dozhtxmf.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2fjvvmynw.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2hjnhxtgb.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2irhozdwt.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2efqnmtoe.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2evqzrnug.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2cicwukpo.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2qpzbyewd.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2bdrfkokg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2xvnxkqco.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2nehlkqzb.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2qtcnuwnw.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2jxlkwglr.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2fwejivjl.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2rphdgbrt.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2mwpguoso.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2gvvbrxdb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2reatfgpk.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2ozyuhckr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2xpkdxlrm.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2jusjvkjh.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2klxqspix.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2mndcyujk.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2weqrdgxe.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2dewqkgsy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fayaoujg.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2dwenofvs.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2qwfrjrbp.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2dyzbyqfo.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2cbayntum.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2nubalbwh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2lshyvqwz.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2wohqwmnx.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2hszjatqp.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2bufeufjs.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2rqwtcjjg.html


<!-- 参考信息 -->