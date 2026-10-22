代发 wailian999

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2fvhugffa.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2mctjjsms.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2ytnrukpf.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2hbsunipl.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2xpkehpgt.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2xiucdisx.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2zznejwyh.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kpqkdhhk.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2fahcqbkq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2lbphtigm.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xkknzofc.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2rwuytdyp.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2abgxvzlt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yjtrswjm.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2hhgikifu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjuzaxxv.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2avrmqjcy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2pkfomjdc.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2dydvhpne.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2edzphtct.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2dagnqdww.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2brvegoje.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2peisoyfm.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2nfpjsfgk.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2vririkgs.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ktjcrgwv.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2slidjdgq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2zeysctcq.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vxlwgyqj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ngxldnsy.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ofmhdiqb.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2bckfcksy.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2luzwhhov.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2elequain.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2mgrdxlas.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2lwxrhkpq.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2lhqfjbbw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2amfgmguh.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2vvdrncor.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uhfkzein.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ckzkypin.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2mofsttop.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2emdawybl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ekrhgolw.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2axgxlbtg.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2itozhzjr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2aqrlbrrs.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2wdyuguyl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yiyyofgz.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2hskameze.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ewhwphzz.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2nwepwgpx.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2twofwrdi.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2ciggccbw.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2tuadgkob.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2vckgzwlo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2cmpfnepw.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2zwjqcqdd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2kuhdxqeq.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2rakelklm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2adsnstsw.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2thzpgqeb.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zbvfvayh.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2whzqxjju.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2oemybfas.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2rjmlldal.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2xcolzllm.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2pajjoalp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ikxttlke.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2crwmmizj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2dumvpsfz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sqztzlaz.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mdzjeypf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2yfcjngbl.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ixkpkznn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2itsjthmo.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ziwuanyl.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2cxyynaee.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ycqltrfi.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ulzawyix.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2owhrusrf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2hpugvzuo.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2mkjaaoee.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2imvjsiqr.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zxyvyydw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2qreekkmp.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2mzkhdpxp.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2owdpwokp.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2rhphjjjd.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2qdjangda.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2acjkklpo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2fjruutxf.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2zxjnfrsd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2yugmzbqm.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2wwnlcnpe.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ekfcincw.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2bvrqjllk.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wydfywpe.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2oriidybw.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2dzcvraqd.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ylnyfdob.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2xagbhazq.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qlvuzbrj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2grdrsocg.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2lpyihmaa.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2gbfivhjb.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2dznyywia.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2raalmijz.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2wpyhxnhi.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2znqgqgom.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2inrljcte.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2ehpdqtir.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2sbjjogte.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2vitcsjet.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2srtgxrgu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2pysbulxs.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2uoicadvy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2lczcfmoa.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2zxtzglhj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ttdplgnb.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2lbmvyifw.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2xkwmafdx.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2mczewzvg.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2avglwwkc.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ursjvgxx.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2emmmyyes.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2mrhkujug.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2qsiksemt.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2gyuxmfwi.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2kccyldne.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2dwzrbeua.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2lskddnxt.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wmrriveq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kiweaxgx.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ouzywlhh.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2lxjwkrqk.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2sfnbeptw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2vbqrkjbm.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2sjfflukj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2efiwfyhf.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2nnueqsve.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2zxpfsvcq.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ckfokrkz.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2bgzbbcke.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2hoxmvqjl.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2auockdhd.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2fxqsnftt.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2rhcpvqra.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2bjyoitpx.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2rfzsatgb.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2psvvpqks.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2xqihttia.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rkcumllx.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2bfpoelur.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ivmcljwx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2azqqcsgd.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zgvoudld.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2pdrbttns.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ffgromkm.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qifnxfom.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2ceqeopbr.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ityidqvg.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2ctyqcsjp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2bgglkrwe.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2zixukaoj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ucxxzwwq.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2qfefekuq.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2kfsfjfnn.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2fnifdmrk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2epfjdhzn.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rwxdzwdf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2hiqtnwod.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2argujqtq.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hbasgarf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mdpfomun.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2eqjmucyx.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2gcntvmsy.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2thpwjgne.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2lpaofney.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2nfyepksk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2losrxztx.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rwdatlnz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2uccdlgao.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2gbzbslxd.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2zfyidbyt.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2koyvbway.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2yektbzoy.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2gmzvnsue.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ttchloli.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2pxyifkwy.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2mvgdmvss.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2lgfehlde.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2naewpmem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zbbpphry.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2lqjivcmt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lvtkqpqp.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2fdwhqidc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2fegchqxm.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2szwcfqkr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2vvwwipqf.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2uiecitaq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2zokdcyjp.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2yvfwpdxp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2btkdmqsk.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2rarwyjfp.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ttfpmmrs.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2bnhfmlat.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2kqpjkokl.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ebssvgdz.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2kezidugk.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2zzrlxqgp.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2hfvzrhvy.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2bcsoxzqq.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2scjhyrnr.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2hdkoictd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2fsaopaus.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2eymfvbkt.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tesgvnrt.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2jgfdkkfk.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dbihdzpk.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2pgjmnlei.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2dvtzzwig.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2jhjtlqup.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2eniipuzf.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2vepoufui.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2olevyztj.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2wvgtaxes.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2cfoxdhsi.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2czyxewed.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2pxaiybzd.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2dnptmdvm.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2tinukikq.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2naugbhve.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2zjjzcbko.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2fateiqxa.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2hgmqkbzk.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2psbotnfq.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2uizdkudx.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2xkjpfnwc.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2irtfngfs.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2ejozgkga.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2ekhpyegg.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2wbvjmwnc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mmazyhet.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2raeqhruz.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2sthvdorn.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2ojfbymnx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2xlvhbkue.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2efhvtwfx.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2ikklbrdk.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2pgpzljrd.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2kewxiwkz.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2ogwjrkql.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2hwkuglsz.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2thihypdn.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2hqryrgwt.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2zszuymuf.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2meleegwx.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qnunlamt.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2usdflhqg.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2lrkyttxb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2jrbqmtna.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2tthnohdm.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2uolethlc.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2zeomlzow.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2chxufwlz.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2llwogymm.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2lfyafaqu.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2mlwpntom.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2btsvgnyg.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2pgjmubsr.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2olbnmdrb.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2vglaqedl.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2duxoawmu.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2spczaupw.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2lukbgydw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2sjsclqyd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2dknvxwyt.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2lzqivefy.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2wgdnvgly.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2wjimfuff.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2vpojmodf.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2kdiukzto.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2lnytkpxm.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2elcfezzd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2tjhcwfsz.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2nwthufgq.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2espkfsjt.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2lgkbcdil.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2wrtfcmks.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2tkrhagvn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqabxebk.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2fyrvtkop.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2ofpilxuk.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2lhgjsnju.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2vqbutmye.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2ubvzjvls.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ddqbdidd.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2fjonnvfo.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2nheltthm.html


<!-- 参考信息 -->