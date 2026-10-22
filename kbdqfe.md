代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2urpumxqn.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2fgmhiidu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2pwqxnika.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2paiyqjel.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2fljfbnvs.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2jhwriziz.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2xpbjffzp.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2lfealrkf.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2kmvacxcd.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2rhdqntab.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vmxnwllx.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2eeqyvkxa.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2yeyezoik.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ulszmphi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2inzuttay.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2kbtkoyad.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2xgxtoiju.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2swozleel.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2wjckwrxz.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bdrkltdd.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2fqryzqxt.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrnpoqna.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2djaosdvv.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2xphcpjuv.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2pmjnndyt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hzwrlrie.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2nwwoyumc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2sovlydbr.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2acbeitxm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rwmzmmwq.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2elpvstnx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kkkkvvvs.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2rexpznky.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uulujghc.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2nhkntyod.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2chlgtbml.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2hersmcpm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2xkaevdbv.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2mggfslia.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dhnfqtdr.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xszwgdos.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2kdsekode.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2usatpunk.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2fkibvztk.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2yvokmwhf.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2gxsurmfl.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2dttmybcn.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjcclnwo.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2zhtdqbxs.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ppigagsm.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2ctlzwhbt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2rucjubin.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2hysfuyyu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2zutfnbvr.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2fwgukxob.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2djieomlg.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zsbdpgpl.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2mvfvzoel.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2lyxffbza.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2ykwolvps.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kqjlquvn.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2fryirirr.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2oeczvzpc.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2kbjtmykx.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2pghjnaiq.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2rxkmgaeb.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2kpxlqoxh.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2ismhubyu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2veifvwir.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2jaosqtyb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uupqyomg.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2hydujysy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ugwsjxaw.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2xssqfomi.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2tavnijbf.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ggqcexwo.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2ierwsswm.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2rfyupwhe.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2untyoimk.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ltyywmjy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2uomksmzi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2klqmtqdw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2tdcljvah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pwsevuuv.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jwdlrgar.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xrydbsza.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2rqcpxauk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2kpteshsz.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2tejzfstn.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2pselikvf.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2lrgdtdjv.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2bkjytszh.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2vvprnzsj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2bhkfzfzd.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2msyodbro.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2yrnwzwcp.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gotmlgjs.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2fxfeesvj.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2vfvzrsow.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ywuvmdwv.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ccjreyjj.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2dofzqqpf.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2emchiqyp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2sdpyineu.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2gdjuwpfd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2jzazqzhc.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2wcpnwkwm.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cnxtfydv.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2vwzfphwk.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gpygqkex.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2bjgyjmwk.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2fgewgyib.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2hyqvxiba.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2mymgpims.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tzcfdtjy.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lsfubmiw.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2tyauvlza.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2kkzfmrxz.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ruknvksh.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2icxlzikw.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2nzonkdvt.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2szppagfa.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2hlkqxqgc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2rqmmvcwt.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dfwmanjn.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2hlvcslyf.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2hctszquy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vxyszjfr.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2kwgochuf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2zafjmikt.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2egqmgchz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2kafvugkx.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2hbryqlgi.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2hdsafcrb.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2bscwymaf.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2dxgzwkbg.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2xfdkbaox.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2thiqwvgz.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2yrkniyxr.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2khrjdnvn.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2rpabisks.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2txpuohfa.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2dagzpudj.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2coavmpjt.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gbgqpndj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jbbfbkoc.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2nbwpayyh.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2mqofqukv.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ghppgcmb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2wuixxxbo.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2bzotkpbg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2tipjtqro.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2jyxuuswj.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ghmsjsmm.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2nlhgiijd.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2irolpqnk.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2wtjodesd.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2xiwpdpmu.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2szrprdxk.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2erdulmah.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2smzbxccv.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2iteajric.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2rhzdbnvx.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2isgcbhdc.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ticzdhol.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2ydurcxti.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2koqfbqhv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ojowwqed.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2btqzgexu.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2colcbcjb.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2wxxwmmfq.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2sylwritc.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2stmrsazj.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2ltwsuvty.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2pazpultk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpjfdshg.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2enkkqhuf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2dfjuzxff.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2oxtkistf.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2gbtobbyo.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2dqznfigu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dkajqraf.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2tqdtqvzu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2wcrxoiqp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2kvifmdai.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nkpihvwz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2myvryafi.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2onaoqyvt.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2kymypvrr.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mvqagvfn.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2dtmllzrd.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2vohqjzsq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2jozblygk.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2fjhbsipo.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2nroypnoa.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2wupjgcak.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2raiyqwpz.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2oaljqjti.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2uorpzphn.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2tswpmktq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2yowqnokm.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2caiaoudw.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2jktmdpwt.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2xbjsakcn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2owytoajd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ivtckltc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gzwxubey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lbmadmnl.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2byustsaf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2ksvgujzs.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2efrfwcmd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2rqeewvmi.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2xeockbqo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2brbyeicm.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2yceniwln.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2pbjcfsxe.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2yyenuvnw.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2upwkfajf.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2siguhzvr.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2mjkvszwa.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2hmphsgrs.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2ijampwpl.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2ezbttnlq.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2fshaueiu.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2lslnykll.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2mpmixviu.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2jxunuvgf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2uaantkcs.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2frrcrxaa.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bqdxkhjd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2qxchqcwb.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2xtfuzwha.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2chpaxzfx.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2zzwwdgay.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2usapeqfh.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2mnvvinww.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2piqgvhlc.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2mevddgxx.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2pewskyur.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2xhrffwtg.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2whsgvjky.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2ykmmpbii.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2nbdschkk.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2oaybppcd.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2bzqqmspf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2nfrqvcmm.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2nfivjnov.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2jpubxcva.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2gxxidjtq.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2yfbaptfn.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2rzeorkdr.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2geafsmib.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2wdytdvxt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2kxozagow.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2ffrcaomu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2avszaxbj.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2vbatxfip.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2uuewznni.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2qhkplkbl.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2kmuwdijt.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2fihimzao.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2mqlilaue.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2lggrcjru.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2zzxmkuyh.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2dowupwku.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2eilaoyck.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2rahaklrq.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2hlglwrin.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2oodobupp.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2nxxeoplb.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2omoxyvys.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2doclyzvb.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2mmowyfcd.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2hrepxojq.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2llkgwzcw.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2mqtmtbjz.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2xixqvfdf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2ipzskhsw.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ofbeuhwq.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2pyrxvwge.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2zkrbpsvr.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2tjmxcpdf.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2wccqbqtw.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2hhagvdly.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2qtpgzaau.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2qjrdpzep.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2xvzgshsn.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2nyhksyyf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2nqkplkfl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2hezlslkb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2szysmrey.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2rygcgkis.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2pvakbyxf.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2kspwetao.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2hjdbcymh.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2ttwvwqaw.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ukyptigw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pfndeaad.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2ellmbgsz.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2fvuykhbg.html


<!-- 参考信息 -->