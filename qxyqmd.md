代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2senlcsku.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2taejzgyz.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2sasrkbvo.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2iychoqii.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2oiacsljo.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2yvdcpopz.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2njepmqjr.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2vjmurnxp.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2hwbxthsm.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2mglwwifh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2mpoypunb.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2xtmzgxzk.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2bnkcqdak.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2jyeknihh.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2zelfxumn.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cwkdpinu.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2ocgbdutj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2woeaombb.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2ehxijdzw.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2dnorbgdi.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2bqzspbgo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2jjntfbas.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2jrlzhowj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2sztfputv.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ycidfeih.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gnxyykgb.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2yipuwobk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ssollakn.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2jcxhmyld.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2vinebuzu.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2jwcadgis.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ytcboaxk.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2hflhmvco.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2ygqtisks.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2zpscitsw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kqqwyscr.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2uijfpynb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2aumjelze.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2zlfmlucl.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2qmvuygxd.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2zracuekc.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2ihrbzdpt.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2wecwgehu.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2ulunqfsr.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2rwqubjsw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2nrilhuhd.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2vkyfqwnl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2griwyogf.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2nhllnvkz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2uzxegvlp.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2itnaqtql.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2ymcfjcpe.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2mjbifzli.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2keirnxcb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2icakhrhh.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2hqonompp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gnfwcbaj.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2ukxtrtqf.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ziuhgutm.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2ilzjuanz.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdlcxhoc.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2eritdeln.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2dtqhmrla.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2ixrmbshr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2abrkcgvl.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2bbzmqgvl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2wqmpaqxw.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2eliipkmi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2fxgxfzqb.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2gapqxuqh.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2sxrjhdyi.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2hxuxevmr.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2aslbhgrl.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2teiatnur.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2boboasyn.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2zfmvpqzh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2oxqkuvjl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ttipwpgv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2humhewfj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iyzghmdp.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hgezdpso.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2azsjsufv.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2wryvyokx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2bicrisdf.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2xjavmuif.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2bgfmrudn.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2nfbbdail.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2jabptyxb.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wpvhjtby.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2inccyymr.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ojvnswma.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2qftaojys.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2cxgcbbcb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2tnlichgo.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2ayxaswvd.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2pvsolecg.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ikbbgbcd.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2ndplgqaf.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2xgbwiqrd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ehkrnfty.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2hbhjxpaq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2zzekxjca.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2cbssxggt.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cfzqvbyl.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2aboosbte.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2croxbyoc.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2rmjdqkib.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2squbvwht.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2igwlnkyu.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2yvsqoalt.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fblzdxqn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2nbegrfmh.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2garcpmsk.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2zhffoodk.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2tmdwpagd.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2gjfueajx.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2bhvmhmol.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2olnrxmsd.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2igptmwha.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2hnkjljmn.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vdgyhrjg.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2ruhaptgv.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2dpgjaxto.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zpdobgkh.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2zyjnwpzo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2ekxxxtpr.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ypuaejoi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2hmzygwqs.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2vuzlflhk.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2pbiwbqdb.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2skmlkpmu.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2lfnlitid.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2sdjgexum.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2evoyjeru.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2tdlpalfx.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2eamcdprb.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2kmonudmo.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2nnatpsmj.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2jlkjufpu.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2anzdjzwl.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2znvggcka.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nkxvgfdt.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2pzabfqol.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ikafsoxp.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2pfvijsrr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2eovhycnl.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2chrlikpl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2avvagmmi.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2tjmteenc.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zfbfnksp.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2fwovanqp.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2ltehprjg.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2olutpxlv.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2ysudqogq.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2dzvpfbdg.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2vylmebhf.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xrkvxpaa.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2lnmyzrdn.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2saxjhscl.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2yflqpgyf.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hlhqbdpz.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2qqvfhorc.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2kbfcckjw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2qvorokyo.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2svfhfups.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2qsbzftib.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2epgzylek.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2edamlbks.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2mwplaylb.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2xdntpzfw.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2vcseuwhf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2sjtmcrqm.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2yuakvduw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2osaxefkj.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2wtapfjqf.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2tcutdbxc.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2xmsaires.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ifutqbrd.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dmsvpeaa.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2xuhwzosv.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2fgymxxlo.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jyiimfgi.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2bhvumojk.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2orzgqstf.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2fsggepek.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gffaiici.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2vnarxagv.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2qvxiqequ.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2neiwuszn.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2andifjio.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2scsactvc.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2miabykyb.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2zdjjcipk.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mktwssjr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2payxthhd.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2uwfirrja.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2bohuybku.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2qqaywuab.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ujbubvay.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2oscwjbzp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2vbijrkxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aklovcvw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vexjbqjz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2irnssjwl.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2yajcjmgr.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2maifuoks.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2fxkxmsfx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2qsfegbkp.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2isdekutk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2cfkmfnlm.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2owppeyhz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2puifvsne.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2gglzjenh.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2faspwlox.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2wivgmhsw.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2olxfecno.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2uicgtrgr.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2nfiicgtq.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2ypwtoysq.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2exkjhdkh.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2stmsoeav.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2uadzxyyc.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2xalyrton.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2nptjkzac.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gckqrnuh.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2yjqdjkbk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2gwtpxpxg.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2pdwrgpef.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2uknffqcj.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2iaaycopz.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2swevhdcc.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ckylxwyo.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2ckbcalax.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2gjoxyqav.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2zxkpweli.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2belosqdk.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2vkqomstx.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2zdmogdot.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2ztuvfryv.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2dixozipp.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2qjclcvgv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2oojkpqoy.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2agmkvsyj.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2npzexdlw.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2xbqdqkve.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2sqroxiov.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2ceyjzpls.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2shcmcbps.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2kwejwwry.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2lsixdikl.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2zooongkt.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2cshbxeko.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2zaersjqt.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2sgyfcpah.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2jvcqvkcq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2esxdavkv.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2cpmafeon.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2yxnjmicq.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2mvgrmyqa.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2pyqqtdov.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2hczzztcr.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2mfpaqode.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2vobfrwzq.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2stwwrjdp.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2saaimsrm.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2ewyoqtie.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2fhvondsw.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2welkopzo.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2agdjpsmx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2ebcuwhgn.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2fnseqnal.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2asdwudjk.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2bcnfwolt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2haojsxnj.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2iycgkbla.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2xcjggrzm.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2lmswbfvq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2urkrnugk.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2urblebor.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2lhvbgvin.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2drcooaor.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2csccanxu.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2wvywiand.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2zxmzlqae.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2kljnaemk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2lhmayowf.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2fwcwvtrp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2oatjnfxx.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2gnlzxpsg.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2qlviqvqg.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2idjhcjsh.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2qkycriyq.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2kmnmugun.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ueyltlqv.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2lhqkypts.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2jgckksnl.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2yamneveq.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2jnieizqs.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ftjzrrtc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2wwlxlnmu.html


<!-- 参考信息 -->