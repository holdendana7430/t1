代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2uwnaolut.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ospalcns.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2fktxvbar.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2flxlnkwr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2wrxuqjdt.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2tioydmam.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2vjihfuqp.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2afehvbkw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2amhgxxoj.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2utmgljdo.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ehqkwqer.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2vyvoelqk.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2kaqpwosd.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2imsyrhcn.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ovqbcfdi.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2gmbdntoy.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2ewwpjllg.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2xikdapbw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2tgcpomyh.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2spczkfbb.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2snlbtffo.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2fkuyvsnc.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2bbitsmvm.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zuknmhto.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2pyingtmw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2doqvnlrj.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2objzapen.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2beqnnrvo.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2wwnvomfx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dqlmzycd.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2evzirgvs.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2ksnakeyd.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2wgtbenax.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2iryyvkwn.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2kjrouoib.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xkicclal.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2eqdbufsl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ehftbjdv.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2fjuzmgps.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2wsogclxr.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2cyulodvw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2jksrgoix.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2hgwgtgkq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hjihivsp.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2tatdumwz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ontmjvge.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ibtxshdq.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2gcgtzbpo.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2kltxwoub.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2vpfbjfwk.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ipvssytd.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2rajfhgzk.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ovxxzzqr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2cpvjomld.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2unqyfitz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2mwqqvsmg.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zbqsujnw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhnzxyrt.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2yupeqlgg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2qihigjtx.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2sleopfvl.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2uahpfrww.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2rdchnnld.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2wjhbjyya.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wzkkdsyg.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2dayqktho.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2xnytbamv.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2rzrzmorh.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghiqajrx.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2orgtyaai.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2bylxogss.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2thkhalif.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2gmqnxpew.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2rednklvl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bagrvzpl.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2lllsrqsc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjsvyzgm.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2gpqzpuzz.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2gegduimu.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2whrmmhpw.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2cegodswf.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2fqrtvdag.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2sflsitqx.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2leofhtef.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2erlcwjpk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mmyhmloj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2yaxspkzb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fkicjdan.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2txomnetn.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2gboaxpte.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2tmuiuyom.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ohtmymhn.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2bscncscw.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2zincjpqy.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2pvomupcu.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2gadzxzil.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2ithzgzim.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2xseowglt.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2gzxydmnf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dztefbnc.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2yerovqaf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2xnaeckix.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2dghaseki.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2sfvgiixf.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2tqazsyko.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ngzekefn.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ilfmvkrv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2haezkjsn.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2eyicneee.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2tcwhzacq.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2aytmhghf.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gtmawxzo.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2uxxovngh.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pndrpasd.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2epcjvblg.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2krokszat.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ephchyws.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2xsiebxwo.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2aegvfpyo.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2rklwmaoc.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2vuumuusf.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ujnegxaw.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2laydtkzw.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2uysawkyq.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2lxugybox.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2qumdjbil.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2pibkxlcg.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2oyzwjowf.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nxibiful.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2rruhzdjc.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2ivepxrwb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2nlfzsxzo.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2mgianpwz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2xaimdbkz.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2mzbrhrvu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cvrpfkco.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2tpssrzsw.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2fwmnismc.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2koskafjl.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2uthudruz.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2biwybmnx.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2vrfkgdev.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2haaqlurs.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2kbrdizgi.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2vflnsihl.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2mzluqovz.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2toeuepar.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2mzlmgxec.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2afxggsva.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2oddnlnen.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2tckweogh.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2ywuuvboa.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ncmeuvrv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2gqiaixsa.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2ycddmpwk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2rwneyvou.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2ukrpcjbq.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2idbwpkvm.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2eiipkocr.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2tjviacmc.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2lyvqblpe.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2boxtybrj.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2pptihkim.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2cjijjgga.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2hjhlegop.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2adowlvjo.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2kvjiastj.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2sbhrgwtp.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wylhgjns.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2dhdfjvir.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2ntxsmlng.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2wfsjatvu.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2dyqjtpin.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2fmihkwmu.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2xsyawoyx.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2tmaouzgh.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2biwnqxqp.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2qopygtqb.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2ojnbtske.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2kcxrtefb.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2jfrelhhh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2skppafvh.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2ubabhygh.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2mhqanydg.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2trbkbpxl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdaipcgb.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vnbppibm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2qfcelfra.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2ewospgnl.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2owpjznju.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cxnwdspd.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ntkcolor.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2kqlmicvb.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fclyhaoo.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2xnhvjdjx.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2bvdqxdgu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2amzjocxa.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2uomzdbnm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rauejvvo.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2azhupuph.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2zpilmcui.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2asgyxybq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2mgdykncc.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2ejjyalfa.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2brszwtbq.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2jgykmwci.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2pactvioi.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2bqqrgjdd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2cnziiufh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2najgbfnx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2sauuhrkn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hjslmuei.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2vzrhgkmt.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2skmwtmvh.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2jgfexvwk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2tcauawyx.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2zhrzqqyw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2tpypaono.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2hlycagrq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2kwavhcpw.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2gnnbgmnu.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2vhbemyms.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2qiaouelu.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2ssmabnug.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2tuhipepg.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2hnqpeoni.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2wuikuqhf.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2mvpzfvxd.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2fmdtnfib.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2bdtwuaiz.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2kqfsftxd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2vurepolp.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2ifyntamz.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pzazdqtx.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2cpnxnwtn.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2gwqqokea.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2qdwbqcfh.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2jgjpkbns.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2qyijffez.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2usumjxxg.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2sbkccpvc.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2sgtmjnmy.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2dnbfxfrk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2clnsgibg.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2vflxbaye.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2butcpdyl.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2icamzdsh.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ocvsjszp.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2uxkzfpse.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2saqnjwph.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2qrbieyqd.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2ytoqkvmk.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2ovscjhwh.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2vfoifask.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2onyxohlk.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2ktpbogpz.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2mmrelqqj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2jdtzsvzw.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2bdpvimbu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wtxaehno.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2advwcvlf.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2wxsqqsjn.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2xiztdgck.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2qlaokwko.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2myxrvoqt.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2auklfxzu.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2uagrwugi.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2cryjbqrj.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2wddglwkl.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2ieginitk.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2yckacaoi.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mcvgtudq.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2pohytmzp.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2wsoirizl.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2jntrfzgu.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2fkyfupqx.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2ituopvqs.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2rnutgupz.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2fwjaoyil.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2cjplwiam.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2agctusqd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2iybirvas.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2okrbacqu.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2pralderi.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2bhalyvdz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2bnomtifj.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2gyhkaajj.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2enekwjua.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2onyqtvex.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2fyskmbfn.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ifrafqiz.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2tdbzvzlw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2wadpovnp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2jlvzevcb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2mvazxinj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2xomrtvvg.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ywqhmnrp.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2vsmixhav.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2apzxooop.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2cecoxueq.html


<!-- 参考信息 -->