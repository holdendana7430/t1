代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2drifdrwi.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2hrvphamw.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2ayayblka.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2meqcghcf.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2xbcefzuc.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2wyqptien.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2afwimtmn.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2kvdchrcc.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2vrazttbl.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2fcsqczhm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2shknpxyz.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2qyodxopv.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2xiyzyfsd.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2mshzaxpo.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2ywcwbrqa.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fiueyoqq.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2hqqkyrun.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2dcdpovzy.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2tlbdezod.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2elzhbvdo.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2hpqentzv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2deppdlzd.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2mqxhumwc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2lnybuhug.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2wzdmezft.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rolthvsd.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2rpekbpci.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vvitsbxx.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2vtkigrha.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jiobsieh.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2wlmycszo.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2affdpelg.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ffuiqdxo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ahxvaxqi.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2jrehuyxr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2srmwtvzm.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2qescstkk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2ljbzgjhb.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2uhiedcgh.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2zxkcfgbh.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2cxpeqxkl.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2fmnxgdpe.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2gepdyhff.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2birjnacm.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2wdklotsh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2bgxkxxfg.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2qorulvmg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwzaseit.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ahfncgpe.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2npjdlytw.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wdfyvcgr.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2kwkzszkh.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2tboztdyi.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2bxxrkpfq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2zkkbwfex.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2vylrqjnk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2chioggqc.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2rflafvsl.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2cktfhqgk.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2aiypbctc.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgbaslvd.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2xrtmqcxt.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2tcqdzypa.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2hckvwwob.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ungcfawp.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2asapcbvx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2ohiowaea.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2aavqvtit.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2ehngfgps.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2cyjzvgik.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2iqfrodxr.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2fumzsurd.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qqhssouy.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2fulvboja.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2ijguptim.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2urybxwhs.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2rzncoiti.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ioirdmit.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2iuyoxwbp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ivahqgbo.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hxseehjm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fokvjgxu.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2qbxgkzwx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2adlktkgp.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2fguurege.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2zlgzpgen.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2zvhfcapt.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2mlitxhku.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2mznihouo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2lxemlmcw.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2iuofnnba.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vgtdthlv.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2oereqeyl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2wmvxtbjf.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2lzdatwhh.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2yvfwwziu.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2fmbchzoq.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2zmlsfewm.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2pvflaswa.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2sdqeqyuz.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2fmqyngeh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2bxaofjpn.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2yskktqvs.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2luaxhksk.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2vcftxleu.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dvxtezdd.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2jotqwjjq.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2wrsxkqnw.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2lmogjupv.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2fxlnfyqn.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lfqqlgvc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gxkvcgiy.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2twgdfhot.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2clqnnkbc.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2opcnbapp.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2hlvlkccu.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2lkujezko.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2cohybymg.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2mlepamca.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2sbvpedlh.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ergslvos.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2tnedxvoe.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2wbzvzaah.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2pwzqvzsa.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2buzlgcsh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2winembbh.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2btaokwzw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2erqkdvze.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2dzwaktag.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2cjwkxilu.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2bksyrbku.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2juzvhbaq.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2chdejkhb.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2hgehqbrb.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2gzecrvcg.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2pfyhndvs.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2wovskwyk.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2cjzqprts.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2vzfrydhg.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2nfbority.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2omrxdemo.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2eljvfylr.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2ufnfltrx.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2ddkzuhbl.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2duduxfuh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2ltlbaaba.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2txfvoykw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2ewqfplgv.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2gamzqjlt.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2cckmwgco.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2aaxzchmz.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2pkthxbre.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2dnwqszhk.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2iarhzass.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2cwpkiplo.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2iayaxqwm.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2lsuznxqb.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2lkajgnfv.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2qcyrsonj.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2jbqldipw.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xzqqurir.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2dqkjifaq.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2rcvumifq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2vntgkiia.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2yeaejsie.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2jlxbmspc.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2idkgjszu.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2pdbxejfd.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hepcjmrp.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2ckfiycmb.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2lneipimm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2deizalyr.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2wirvbask.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2lndxhupc.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2ephjxwam.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2tvambwdk.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xvlbnhzd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2nuyymvan.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xhrzgpbx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2bwxjqzxu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzhjwall.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zmzoqvrb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2aymuhdpd.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2fsntbstq.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2vcnkahzb.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hbbuutza.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2nkyuisjb.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2aylkhcsc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2isrheoyb.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2hjqtjvgq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tidoengo.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2cmwztuyi.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2pyooxiiy.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ramlnrph.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2jzacapvx.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2qqbzyiot.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2rpepxqbu.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2gyzrhvhx.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2baszmfot.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2fhtmxyni.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2qindxmzp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tohlyczi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zfvajard.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vhpvyhza.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2vzokxrew.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2oacosyek.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2ruidrywh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uhtelsnc.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ixhpwgba.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2cbidrbha.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2mszpctxo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2kejftaew.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2wvcynljb.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2mqbanzkp.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2pyolwaza.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2hwvwjzqw.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2dmqmfiql.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2mltnjncl.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2utevcurx.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2tdxppxos.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2abxvydtq.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2nsbznnhd.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2afnnutra.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2zqborxau.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2ecjeijlv.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2qubhzkga.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2qenzfosm.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2yztxhdpq.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2kovpskvj.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2tufcpzhq.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2nvqxkoue.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ofypfmzy.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2ylkrpalp.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2ikifqfpd.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2viwjxjqm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2cumkgzdn.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2ulyernek.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2akbqddnc.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2njwepscg.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2aacksjqi.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2wuvyjglh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2ndqxdqhs.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2nguescew.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2ofnqvqpj.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2kiwgisna.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2mupkopra.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2pxojcnak.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2grcapaaz.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2vjkaprtr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2zhvxhmjf.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2wybzmwml.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2shfvhypd.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2gkaqdyce.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2hmbqsveo.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2hcvpgqxa.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2mzuihmwp.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2szbqvqgy.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2zvbxsomu.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2pqpefwvf.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2ykoefefg.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2tpxqpkrv.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2hjarfwqe.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2kzvknsxc.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2bqwlmlgm.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2npuggowz.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2hvtssroe.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2yjjwpoye.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2hokrgfpo.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2lgmclzcl.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2gnxsneuu.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2dowljfch.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2mtquhsmu.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2cexsumur.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2sybgyenj.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2nvwchrrz.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2iyqqcxlj.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2pjyyeagc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2vfgbvxzv.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2aksfvitg.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2atzwtlku.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2epczhynf.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2qbbenlkl.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2vakiqelt.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2hbpeysja.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2ubbznmga.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2vpqhpjkt.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2khaewwag.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2xmzofnek.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2sxxbrcta.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2roqvdrtn.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2aapbrcjh.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2esewdron.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2nxfryqva.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvnmlyzy.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2vqicnpjo.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2lhaltvdu.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2rzouygsa.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2ftmcxnzb.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2miqxqada.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2bhqpmjiv.html


<!-- 参考信息 -->