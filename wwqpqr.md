代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3pfwiopvs.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3qhgqofzm.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3zecxhdmy.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3xyaqarzg.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3yqngvhvo.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3djfdvowa.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xkuqvyyb.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3dvoorzao.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3myavwuli.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3rqvquqjb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3vcrqkhcn.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3kaacsfis.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3swiumlvs.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3lzqiwisq.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3cuorxysn.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ooipjkwc.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3lyuoxrvs.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbylmmvc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3olnpzbjr.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3elkplyva.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3zxavozpt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ylwaqhci.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3kmjvmtmy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3hnzinhde.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3mjbxueto.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fqmdblhe.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3pvakfkpb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cbjvxnxn.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3kerzknmk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wvmrwgks.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3jngrbsbx.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3tpglltyt.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3krczkfmg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3oxjclrzc.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3jiievvvw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vckesyqt.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3undnyhlh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3rhfwsloy.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3jzkxfddr.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3inihfxvd.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3vzbkorsi.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3mrfysvlw.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3lnznhdpb.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3wuvlbpkl.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3zbfigkki.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3fhlsbslj.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3hczufzcm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3gxpzhvle.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hexabbrq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3xhyipoob.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hbsiqwkw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3pshrtiqh.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3abxkuhzm.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3araguifo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3rtwloupp.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3erofdiud.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rikijigt.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3zepbervv.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3xrqtgfkn.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3dumuierb.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3uunfmuwx.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3vnldewgz.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3exybfrfk.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3cxxyesjd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3gmwnsqbh.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3leoelbdj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wzmmmedg.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3nyrwjgci.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3iimptuyy.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3mtsplwrl.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3xwebzwpr.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3tqrdquoy.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3yzshyvdu.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ummuowft.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3knxvzvsb.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3nkjldohf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3apfaxmqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bmlabfbj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3pkgalcab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zocpmkbq.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lswermry.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3okblquiu.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ikpoifnz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3tlanzzan.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3xxgofxmi.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3hooynwfl.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3cptexiqz.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3szwdxxla.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cazfxnvk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3sjyeyblp.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3escvinos.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mftyvang.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3bvhgvbyq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3qjuhqtvj.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3hlnjwkpj.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3lkmdnonm.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3vdofentt.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3jsfiqyri.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3krzotuie.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3vytygaqx.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3avcjmkny.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3sdpdqabe.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3urvewhng.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3trxrpdfi.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3dvwlgoew.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3sshdcrnw.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3azynbpot.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3cwetseqk.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3ugamxghu.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3kqhaplas.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gnzezjxe.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3efzymmlc.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3vxcpladg.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3eyzgxciw.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qgnnbljp.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3bfwkdsht.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3gzicurqp.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3oizhyeyp.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3fmudsqcp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3hommgafu.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yeigfstw.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3sbzcbouv.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3qcsgsqsl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qehlejms.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3xheyzfka.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3agunnmad.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3zuwaphqt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rbwvgmqt.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3rcsmjhcd.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3mruieixm.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3hhrskcdq.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3kcfwbplg.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3faedbvfj.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3bljziydc.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nwucxqxj.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3xzhpgtly.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3zaetnlgj.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3cjkpzbuw.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3tljhlwgd.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3pigrcjao.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jlexcdjp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3egeerntf.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3isckdhmb.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3edestaql.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3qffyefwg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ezqzienb.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3bplqxldo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ftjwshax.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3xnoakgle.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nowrptrn.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3bqnumfcz.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3dhfmqkpy.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3oqlunbxc.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3jefxohsg.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3wbgoyglv.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ypvbotye.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3lhycjlic.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3enwxmqgx.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3cqlmrhqu.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3iugahrmq.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lbmihcww.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3jqbhwmmf.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3pxcaxgjx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ogldnzzg.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3mxtaakrp.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3tirzibgp.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3rogxpdjp.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3pcbeourd.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fihwyypz.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3dctbgxve.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3obqohelz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3zltsyayr.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3nizttljb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjzxtyuq.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3gpjwvhbd.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3jlraownu.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3mghrklsy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tukfgcer.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hkuclyyr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3cmnwqfpz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3upjgazzn.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vfbqkomu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3owcbbfan.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3mmayitbx.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ybvcyxub.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qrzfilqz.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3yhwujlsb.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3bdfcilcn.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3fsndvurn.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3fgvrktxb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3bynjbwrz.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3mwacetrs.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3kxdhwton.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3kqkrbzcl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3dozavsto.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3svnqtgtu.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3pwslwiyy.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3hdahvqvj.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3lrqlsicb.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ohmhojhh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3samebdim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xrgqxoar.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ypzvcnrd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wxpczsje.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3ahopoxvl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3lomrwsfb.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3inayidoh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3bnjenbhi.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3tqrfwtcn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3zrcsgjir.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3xkjgbnku.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3edutqaja.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3wcmdntmh.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3peopnuab.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3nydewwmq.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3szajbyhl.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3vsxmujfi.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3pdwddndc.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ymezvmrn.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3xjrqpvij.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3jcvortse.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3omfgohoe.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3peamqwbn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3kbfwfgkb.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gnscofxz.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3zljeasqy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3iqsumznq.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3tzdtnbfj.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3tlozrbgv.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3uyoalwet.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3xsrrqscf.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3nflpscdp.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3awwcunva.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3eepzvhda.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3qfdsxsor.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3lojnvsbz.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3beoxsjzy.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3gnzehfvz.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3ssmvdtbk.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3naekjbfi.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3cockrtmd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3gvtqxuom.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3hppugazt.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3mliubsii.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3yrvviqpn.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3tiuzlrcy.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3wxzwruva.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3pvrdoegm.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3ccztcpen.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3podmejej.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3mdgdlukl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3begyckkn.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3zlftsohj.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3wjfbnavt.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3iyvwzwxn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3akhwdtfy.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3lgvbxmdw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3zpfgsajc.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3btyahhjy.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3tswhafjr.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3gcltimmt.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3rgcipbfs.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3vlvevagt.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3oewwyeqa.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3vrtkduoc.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3mpauqdas.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3rwjpmvaq.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3quuqcyjc.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3rnrbgfwl.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3lbdpnjzk.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3dkfbowcf.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3icwqwepx.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3bxdjyzqo.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3umtinnot.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3eyjkoova.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3rnsnpwsb.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3slcywkpm.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3nqjsuhyh.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3wgateazz.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3fazkqkea.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3ulflhpzt.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3rnkumahz.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3aeohpxuo.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3doazgvjd.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3xnmazxae.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3ctkqumxe.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3mjecinet.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3bargjpxh.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3ncidsmim.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3xmjdtfuu.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3ackojpai.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3ctzplmtb.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3xqrynfsb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3retunfnl.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3qzvtgpsi.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3oxhrksiv.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3xfyyndak.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3auqslcko.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nzhayhrp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqsegysw.html


<!-- 参考信息 -->