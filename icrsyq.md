代发 wailian999

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2zqupciaz.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2szlreruv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2wnsztupu.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2xarfwlpz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ykbzdebk.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2qjmgninw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2dyeopgqx.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2qtsvvbng.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2xsnjrxkc.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2evrbghcn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2oysezoni.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2mdakrags.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2cvvqosxy.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2hvahijmf.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2prcqojjj.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2fwycerdp.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2awckldmt.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2nxwvuito.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wxeumqnv.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2qmqfnwpn.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2cqjpmcbi.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ckgbkgqf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2slmvhutx.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2hadozimb.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2smbvcgkq.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2rfbyrbjd.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2srealxxj.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iwziywuy.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2efykdobm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2xpwzjsyx.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2tpraewnz.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2pzsikpgy.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2mkeldilc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2pcdflzuq.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2tiqjrzry.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vqnkndlo.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2tcvknyuh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xwyyiokq.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2ugkoguta.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ssukidcs.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2efvtbsli.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mtvbnwym.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2ovuqvgdp.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2fauinlbf.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2rytxvmtg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2ecwzpxvu.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2rrpcbldf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pulqscoh.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2rmptkyyu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2mhyyrfxw.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2czvgjint.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2tzgnazlm.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2uwwxqrjs.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2owxppvjb.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2zhrfavfs.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpgrmxqo.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2axharbhb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2qibjwmfi.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2xtpypcsa.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvtylhty.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2qbbyoand.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzodksaq.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wcickguv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ixpzenxr.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2osugzpsb.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2ewhxtlwg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2cxdexffn.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2zclckgzy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jiwxbfpu.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2otnhqgdl.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2yvaakdfe.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2eqtwvjoi.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2dnbzpyhi.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2zgjpjavg.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2pzhhvwev.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2kihasxdj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vsorczce.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2kvfruvzh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2jrlskrsv.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2gmygwqju.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2cfmvhnbq.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2sausqhqr.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2njioqgme.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2wwefrsti.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2hwicofji.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2vlstsemd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2huiagbrv.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2asvcdrpp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2wzdxukzm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lsjtlset.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2zgxnhczv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yyohgmrv.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2umxnyqdn.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wqpkajpn.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2kuisssqx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2cmhefchu.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ethayjwh.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2pwugbhke.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2tyxpaesm.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2jvbpkeun.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vnveebug.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2reqexryf.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ncrbblov.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qwhayhzn.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2rwpkippb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2aipqdwnc.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ylyeeash.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2hdnldvsk.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2hwmmxkmw.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2dqquwboz.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2qeyfgwzi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2igdpwfrk.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2aufnpnnu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2zupuaxes.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2uxzvzvqx.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gbnwgfhy.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2uzfveuol.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2cgkxqmiy.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2sfnrbsfl.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2qahfkxtg.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2maszbhms.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2dokwyhyj.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jxioiwhp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2yymvaxpp.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2eqdzhhzf.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zvknuobb.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vexwyjpx.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2mongzvjq.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2tjcoqpmm.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2kfsmumyn.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2yssfbqog.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2ybtlvtjs.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2pjglcfem.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2mzciilsp.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2gxwdklam.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2fcalpjlf.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2jyhhivvw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2rvbsruzp.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2ookdqjbn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vpqycxds.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2hhyluaba.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2ximdswbb.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2jvuixbiw.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2muyqaufi.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2vwlepmon.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2emqymhdf.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2oevxavdv.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2coqqqocu.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2fuuwbtfa.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2rmormybx.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2mpjugarg.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2gnkmzson.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lqmcohrb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ibwuellv.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2eejynnuj.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2mzvridxv.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ygiwlrca.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2sknilzzr.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2ihxuwygy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2kjnfolbz.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2lwbompgn.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2pmxzsdmm.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ddlvyvvw.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2ipdfruqj.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2klszyhwq.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2xnbcczlg.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2zkmeohxv.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2sbfzcqyq.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2pcucvhui.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2yjmdrdes.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2xlaiezpa.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2hrzxmecz.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kjkxxhdv.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2zocdmwoq.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2vyiaoimm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2oxyqopud.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bzpfredq.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2pcqvayih.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2tzczamcx.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2igvkkykf.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2ypeyadbz.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2chmbmmue.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2wlkkqxrx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjezifqm.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2jjciafjz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqswufwx.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2lqwzhttz.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2gmhzkmql.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2qdsparfz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2maqaxqbo.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2djfujemv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2wsxqyqem.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2cexfqclo.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gptrisyw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2bugeeqac.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2klbqsupa.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2gkwfxlzk.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mdmhffne.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2rthwjwea.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2jlapbgvv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2defyomnc.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2wwfuwyau.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yyyeaaqs.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2dfwegbqq.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2srjpcfhn.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bkvsbwyq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2nmvdstdv.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2rewkhmft.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ngkflufh.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2hoezetay.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vnwbegtl.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2kgdsdasd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2hubgukpe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zlxxrqqq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vdraksqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qnisjjsd.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2dvjmsnit.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ckfpinov.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2faduhjcu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jlvoembi.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2nqsmefiw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2lanqqtjc.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2xajwqaia.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2qgmovdrx.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2lwauchdw.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uvcpjscm.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2lzxtipto.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2rkgnvvbm.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2umqapfxc.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2rzwqglgv.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2xxooyibv.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2tzkgpiwf.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2zmykdeka.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2biqmnhai.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2qsmuyhhr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2gitknwiu.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ydbuzaqc.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jslaiqsw.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2jgsdyojq.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fqmvwgxk.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2wxyubtpu.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2wygbfkyk.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2gwdyadjo.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2pdagjmtb.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2pbhswjkn.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2nyzcjplg.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2mgkkjzvp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2uknqfnen.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2aqoivjah.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2dlmvsvzw.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2xlprrjcf.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2xortmtjr.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2fdxjvypq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2kzkzcrac.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2fpzqbqed.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2nfzcmerk.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2ptkcujhe.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2eqlwbkjn.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2popitupo.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2nxpajkgt.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2mooxrvwo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2mcywjbyf.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2azbwgbkm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jlrvclyi.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2fapmdmsy.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2wjrebfgi.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2uozkbuiy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2qdzodnca.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2dedypwou.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2kwaulqsu.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2wgfqvsyx.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2svybnkgd.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2dowhwcqo.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2kskmuwhv.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2abiqgyqx.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vveaocqh.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2svktfbxg.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2krutblyj.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2chptwfkp.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2twhvchyz.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2hbgczgff.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2qdvuyqhv.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2wllgpqpf.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2thrsiecv.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2zncyzccq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2jzunxdyq.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2cbczkmlr.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2uicheatk.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2nhlihuxd.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2zrgvbuqa.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2fsnpmjfs.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2izmzbioi.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2dqwvqsgo.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2aiskkrmk.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2lezrbkfp.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2wvikofft.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2lwemhcjd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2rmhmzerw.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2pzuqbklx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2quhusqrv.html


<!-- 参考信息 -->