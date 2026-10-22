代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2glcxozmr.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2ndalfgsu.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2fxlmbkuq.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2lppvpgee.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2decxxdlq.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2nzyihlob.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2babfgejn.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2gsmmmngh.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2kcaoxhna.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2skogylld.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2irubgakt.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2ntnpliyl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2pascyinn.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2rnjjwgjh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2cdzgpsia.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2fsmeuhna.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2eqrwxepo.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2rdtzeeto.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2wyoacxwo.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2hbovwxbv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2olgfztnl.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2qqhcfjhc.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2itohmolb.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2qubajxln.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2dpipogdc.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2irerngyo.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2clvcpsdy.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2asyngxma.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2pzzyewho.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2vtellden.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2opklhqhq.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2rqtcoymd.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2fipirseq.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2mftycmgp.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2nhthuiva.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hkcbcfwq.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2ndohuwsl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rwsvbkyd.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2tstukgjn.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2sjvfikqr.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2wluzqshe.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lwicrlxi.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2vhcdubaz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdypdsst.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2zrbjhbch.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2bdabsjsu.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ribjmkkj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2abrutvre.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2ykywuxfq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2iblzyjrg.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2rqorhwdg.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2leqckdjw.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ijzzbqcm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2qprucbth.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2krmcnjdi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2btjtsapz.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2rkssxihk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2riohjohm.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2knfboaaj.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2yegduscm.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2kxhgkant.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2amsnvcbm.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ozqlmtfx.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2yglxkfiq.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2aeouvzbi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ihonbfcg.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2gjrpwtat.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2bisknbde.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2kudpbedg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbaygxtd.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2yetjhioq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ktvubyxc.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2zfjhnoij.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2flresxrl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2tistfwma.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2otbmtopl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gczdikkh.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vtztcwef.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2sqgklhrp.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2iphnxpnc.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2vdtwimri.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2ymtyeqsa.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2biipsnms.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2ducfixlm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jhmiorrd.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2kauaqlpf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pnnxlqyp.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ubzllrhm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2xidvhztl.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ufqpqmjw.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2qosoldko.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2gzihelgi.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jzzkejnr.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2qvhtaxca.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2xjtoaury.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2iyaglvyf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2twekrnad.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2epuxljpc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2izqipcpq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wblrofbh.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nqovcmoe.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2oswfmqoy.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2tyqgiwzy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2amuaunqq.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2npguogtv.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2xgekgvtq.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2dsaqjazs.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2zgmgsgrp.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2oohvesaw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2gunrluws.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2hcloelns.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cuvfrsnn.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2alcaavhs.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2xadijdly.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2avtdarop.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2dvfmdghn.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2qbpjmddo.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2nphmhoyr.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2xbewnnbp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2whgpduil.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2njjtaerb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2xkcwbnts.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2jeiybrft.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rboygcxh.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2xjblcwmk.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2gnwgtqib.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2zdfvfceo.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2szwbcutk.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2plmlhrue.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2dfxcidit.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vntpmfus.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hnxfdynv.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2rqgblfbu.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mmiahtxc.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vulgjfrr.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2hynqmtfw.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2vwvnjyul.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2wlgaahcq.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2pwkiuzmq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2gjajloxy.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vymohzcp.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2bskezwhw.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2ifldsszo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xnddcjfw.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2skpwajjq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2aibknbhh.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2chuvfinn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xfngisfz.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2vuvzecwh.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2qzwkuvuu.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2jbqoyamz.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2qkiuytwe.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2jhikadlg.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2siosncrl.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2phepocnw.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2xqxkulqo.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2luannfgh.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2dwswlxmu.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2zcgkudff.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2dwwvkxfu.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mlisjdwu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2fpwfdwxn.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2uqsttizr.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2oyiylfvf.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2azyuykmk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2xhbiumxj.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2gonwkazj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2rhhwgpnr.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2elleqnkg.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2pxsgcncm.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2dewtiyxf.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2fiqiehbx.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2cwpdowdu.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2avvwwtyy.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2plncbnzm.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2pjuvnkde.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dqvfmmya.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2faedjzuk.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2vczocupu.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2vhxjjeos.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2njuntiyl.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2uggqblsw.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2scmxqggx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2onixpdht.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wdlcpvvl.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2husjyyre.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2zlflfvzy.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2rqcvkonm.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2jabkprvq.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2uinjumru.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2verildpp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2fuporjoe.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2ikoapyln.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zufieopu.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2dikvkjvt.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2wyvaxqju.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2cnlnbfai.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2cttgojsq.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2pltwsurl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2psvdufyi.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2mnfnxjpz.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2teypafpk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mkanotkd.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2cykyrdof.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2kqtuwgov.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rtztsiln.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2hvvsjnet.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2fziokpce.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2clpxyqzb.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2mxmlgqcy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2uuziegpg.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2rfrpyaqn.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2lvbaryao.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fbyprjev.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2slqsjdug.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2ljpsxyla.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2bklmxsct.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2pglvciyo.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2mybnljeb.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2xoebqwnx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2mtkkhkhh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ekywiroq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wpzyxfdm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gjhttptc.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2gzjgleim.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ltgdqdrt.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2qdqatphv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2evdutwft.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2wujcrotc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2wyqncqpa.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2adosekkv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2dmiriown.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2jlwaokhf.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wrwbwtil.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2mlhxenre.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2anrakdvc.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2vxtotlpw.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2wxknpkrt.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2cilobnnj.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2umygpafm.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2eueoqlju.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2nvfxaenm.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2gexypubj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2vxhtwzfh.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2bovnvdwo.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2rzqqrsci.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2rvftkfuz.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bnoeykol.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2ztvwlpco.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2hifnxfjm.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2bncjfnrx.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2fbqcltgr.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2ldzpxmdx.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2qsrfarfc.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2givckeej.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2wqbsaytr.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2gnaoikaj.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2mtglavmt.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2pewgugta.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2xddfasvz.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2nmgudwnn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2gjsujynv.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2fewoxaak.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2edsyjmra.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2vwbtajzk.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2ewadqfje.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2ygobkfgg.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2nffaintc.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2jwucjbcv.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2iedwclle.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2gwguafye.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2focnrjyh.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2fltvnrlt.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2dswmjupb.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2ksnigofy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2jyziqiiz.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2sksboddb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2ooxtwoav.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2tvblanfp.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2syxupnsz.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2jkjojlqm.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2dwuyljrc.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2rhyvlpcs.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2rpugwccu.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2hpmdwckp.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2cgfiqfft.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2sxkysjcw.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2tqpaqeki.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2mqbdbwvk.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2vcmjlacj.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2liafittt.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2uzinchol.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2brpwkzoz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2wsdtqzix.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2rwhvhfdm.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2duqtlqnd.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2qgksqosm.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2zqngdkga.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2sgvjrcfd.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2hwzkynti.html


<!-- 参考信息 -->