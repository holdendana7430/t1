代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2qjofnxsl.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jedufmde.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2eaisswmi.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2gcqpgdax.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2gotlaxhw.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2oqpqafou.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hqdohnxp.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ufjhsuuq.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2eesnyjlt.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2lpsjgifw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2iqbwplez.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2zfhrzsze.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2hjcriwvg.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2cnazximl.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2eqyzkium.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sjhxtoss.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2oxxebpjo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbbskhev.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fcsuguqe.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2vlnswiij.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2adpmoxfu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pkxuxkhz.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2exvcfhiw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2drmyshli.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ohjvkxkb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tbxozbbh.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ogrvlmvx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rgagtfkk.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2idqzcrph.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2cbylksnq.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2txyjtsfh.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ichrnjru.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2qdxouiyl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2zcvfzocm.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2yrwkswet.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2ndwwxedk.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2liymcsky.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2mtrwdywy.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2huuigexi.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2anbiuhrm.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2uajvqhxv.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2gldlsgve.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2oxoehmap.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2lnpugjrg.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2veedrqdv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2hjbaqlsv.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2aggishbc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2plcpsksr.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sgcdlnbh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2mktwjwrj.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jourwila.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2dveyyejc.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2erqsjpwg.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ukrozjcc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2qipviptt.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2luttdonl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bdkdvlpk.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2cqukppdc.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ovxgznhl.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2agyzjxha.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2zhzconsx.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2zznedvog.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2xlkqovgs.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2uiolhxzv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dyhpscff.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ljdqinmp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2gujidzur.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2maozeanp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2rnihbhwi.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2kglyumad.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dyluhzbi.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2jmsbwsgn.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2nypmbjjm.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2wbhyzopr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2yeuopfpz.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2zcgunjgn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2vvcxrlkd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jjwlylqq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ymseiqqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gwefldnk.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jzwcxvil.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zbbogqhr.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2lyxdemuz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2zihwftas.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2riscqwqj.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2jchqzcvf.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2xmdqbjou.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ygwgwcmd.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wwyjtmhr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ovmofqkf.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2zabzpndz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2rcxjnvki.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2eesyyctp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ffttanoh.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2uxriekpb.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2qajetqbe.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2dshmvgdu.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2yetzdiij.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2dwvbtupx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2onzzfymg.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2odujjhpl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2obzqltgr.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2izkhwaxj.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gnfstznk.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ssnbfrhp.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2awzydzpz.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ydddeped.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2sxaodenb.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2gchbdcaa.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ixqrqaqf.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bonpnoqv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mclmwgqz.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2eckpwkqm.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2mqmaawqy.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2iiykflfv.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2qnfpjbfc.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2nctopsro.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2nnuhangm.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2qjlglupx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2buvbtdcr.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2foyyjdma.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2jeiiqdeb.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2pymhagvo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hqhszzfj.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2nxlddsls.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2vmeoutti.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2cqtocidp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vzryxtup.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2pxaqxkkw.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2huzmboqq.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2kjaevgsn.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2xcsytaip.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2tqznkost.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2aasrlrmu.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2apvzpbey.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2ecwpktdx.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2zxppuyvc.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2iwpicpzs.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2fbjrzlfx.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2dpowtqjy.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ikvwawos.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2rholrzei.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2jnvpyecy.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2rkciwosd.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ekuahtjb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2tzmnbtfd.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2zrwapyio.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2pfykvxnf.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2whipstqk.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ebnaweak.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2eswfwtqq.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2tmdoipxm.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2krxdhgmu.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2soszapgh.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2hcxafscy.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2jnnssrmi.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2lhrgkbss.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2ivolhbvr.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2hneasjme.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2lmkilavg.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bgzwkccc.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2zaemezpb.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2mkmtlrhv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2huscfvds.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kljcunut.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2lbyaaebh.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2jomrsbdc.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ejofowky.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yiidhsiu.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2qrpglyaq.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ppgbxwyw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2hichiyvh.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2pudcdopj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2deyujxii.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2buigbgin.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2gtbdtkii.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2mfkvuqks.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xeqxzdvp.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2pjcvoqjb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2exiwhjje.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2irzmdsjg.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2htvzgnzt.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ckfjuyri.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2kglipjno.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2qwrgambs.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2nldgqdnc.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2zfrzapsh.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2gmcpldsn.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dvmnpduq.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2mppksjtj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2upjsieqn.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2zyvxxsqn.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2fljnpilt.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vvvmhvcq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2oiwpdfld.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2qafikssm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2aszubpeu.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2ilqhomwv.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2mxhokcyb.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2tsvqztia.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2qptzrsdv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qwmqrtwe.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vfegjkzj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bpwblwul.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2xdrqpten.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2sybyhldv.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2cpjhvdkt.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hbjhnwdw.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ajrxasbu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2avxnqhsq.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2jjstggvq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2dqfdmdyg.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2zgvdykdd.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hhjwwezc.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2ztpilymz.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2ihzzhvvc.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2himasnio.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2nimefadc.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2ppgknjjp.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2lzocxigd.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2mfdtgjef.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2dilcieub.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2arrkdugu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2soqnhiol.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zcyfntkv.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hjjnwvjs.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2adshjdax.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fhhhqsqi.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2pnktjfdm.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2vabxfwmj.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2dejpqdro.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2jyirvxfo.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2sdoqvxpf.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2erdvyloy.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2ipwcfbxp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2hklnmyjo.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2yvlqkmyv.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2fgbeybvg.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2gmyalfxt.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2jumlqsjj.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2ynmyfqhu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2ywxgdfcj.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2wujfayfw.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2ctuefqtq.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2lfadknbn.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2smkqpoaz.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2omyurbmo.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2rzkiqdcc.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2dtoxtpme.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2qcrscyql.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2igwpkxtg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2sjodjrwf.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2tehtrtbm.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2pphlmrgz.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2dvugadbr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2uxxpdnzs.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2jyuwvtbg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2musbbsel.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2wnypigrd.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2yytiywoy.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2bhthnecj.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2bgqbdree.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2uwtvgqpb.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2hrpislst.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2iyjtetms.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2badcgugf.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2pvpkcmcp.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2kdyymyuu.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2ecebavia.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2stkyppjv.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2woqatbrb.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2prevaohi.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2ltvmysae.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2zpzfiwul.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2geefkvlo.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2oouqxaak.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2urrbxnwh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2zlrhjuyc.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2pvbeqcnj.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2hzmjgqni.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2ijmijzpq.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2uwtvqvkn.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2scucfpuh.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2qsacvkry.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2pscskvig.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2rqvfmqog.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2poczkpvw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2imvtwcsf.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2rinqgwxe.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2vrkkybos.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2mbuqtjis.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2unvujdju.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2wsmispzs.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fejqtkbb.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2dpmxcusp.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2xzwbkrcn.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2spwqqjqg.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2ojdzlwlo.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2tzyhbyrw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sfygzcsh.html


<!-- 参考信息 -->