代发 wailian999

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2mzaujcdz.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2hhaahrcm.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vhbljtkm.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2rcfwtzrn.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2gbgavpmg.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2qablclcu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2bqsxlwwv.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2waotlujp.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2mpwcznph.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2choqxdcu.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2vnmvpqbi.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2aaqkpgpj.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2kotbhcra.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2bvhttbva.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ubfmshey.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2kugwzorz.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2paeyzefx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hxqiaolj.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2qdnrrvrw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2gktomtjl.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2gxcbmrhs.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gabsrhrc.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2jddbvnvm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wtbjqcxe.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2gstzvhql.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ajyzawbn.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2euowhbxq.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2hvmygiby.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2lxhcscjd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2fsydyjxy.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2jewcymuh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2bttgqywi.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2bvqltbjb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2vefifxoi.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2zraqlecy.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2xncpybck.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2gaxibjru.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2slmjhfwk.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2cntxkhgo.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2oeaxnsqe.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2upsvbqax.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2kqkpbhti.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2shubvral.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2dtkjwrdy.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gurxpfty.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2qzimflpa.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bzyabnxx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2mamleqzy.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2xvhjptgx.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2zwmfpuzf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2xcjeyrit.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2htyfkujr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2chabskzc.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2ioprpedd.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2fiftswlr.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2otuskmeb.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghgyqewt.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2iqptsyjg.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2dqwiqllk.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2hdzjzjfu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2gtpwxtxu.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ukkjknvy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pocuyzyz.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2fpdgsuqv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2burxagms.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2traglswc.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2anxaxwgh.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2rnksigom.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uozhemgy.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2kuqilffv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2qmvsxhit.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2mtdayvfb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ayrajgur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qquplzpl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2gxqrubwc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2idutnqoa.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2efkrouls.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cgsquxkw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2thrpovhp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2otetgxii.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2xezrwnai.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2wekffwmc.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2rmkujzxx.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2fdzratev.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2udqorupd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2jpolqgwo.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2xhghygnz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yscgpgjw.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ceoikqzi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2geibcfvw.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2mxurqgvw.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2mbjuzlup.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2bldhdqxz.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2cmgtscek.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2cpmafskn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2jlhkcnpg.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2bxmygddt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2lqrxscma.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2taoqtztt.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dimlzzeb.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2pzrcnddt.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pclsfxvm.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2cpyuhtlk.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2bwsbmabh.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2axgosvjm.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2qnskpedt.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fcwoxrlg.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2bbyxqxbd.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2asdrnxwc.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2cjcvvzxp.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wfzyzfsk.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2ydyaufaa.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2sfgyxfno.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2otckjttt.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2cymianqn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2pfhfhmfy.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tkydgjaj.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2cbtgthzo.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2tbbuiito.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2shumiydc.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2yqmlueda.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2tfhqursu.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ogsqwgib.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kobservv.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2plbebili.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2vvkwtgzy.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2drlltzwr.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2etgpfafw.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2zowprjsi.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2mxjgugne.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2iwbvnmuy.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2gehngdap.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2chdjxrdl.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2njrcfmvt.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2brdnkvwe.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2rjrckhdt.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mcnpwkmt.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xmeopkyc.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2kvvvpdko.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2amsegmds.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2sejqzays.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2gghgdkee.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2wjkdghbb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2dldigwek.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2ejgxsnia.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vpwlqnie.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2eicyygsu.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2zdmwjpix.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2mhvaaxou.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2opendecn.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2puxrmipp.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2mffpxuud.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ajhjwfgx.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2yalcliif.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2rircjcpi.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2nzdlihka.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pfahzflt.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2ncyfhglx.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2qxslxele.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2mvtbifbn.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2sveqwllr.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2euerftyz.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2hmxijddf.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fikbilfd.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2yswaphsw.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2nhvdrdhu.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2eqmhowxs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzhwuyeb.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2hzyqyyuo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2steetiqj.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2cgkzmodu.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2rzipftpi.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2zqtoggmc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2krhglatc.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2emhowich.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2ddkkpjbz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2lldjaoeh.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2arlfjbfw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ftawlusa.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2iaybfaiy.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2mxiaqqfv.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2pbgvxquq.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2fjionrcb.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2vokgjunz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2efloomep.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ypxrdiby.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2fxslpeqj.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2nwjhhvpp.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2lcsxsmmv.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wjsmnwea.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2txzdsdbs.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2kupuuiyj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2uhexwtkw.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2wctgogti.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2aogkvmcl.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2qbvvegyy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2vppyquhx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qnguzdwj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2xcfosnfn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2istcddqa.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2uzqbwncl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2byppioue.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2nwjtsekf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2oogwgjtl.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2fcmzajyz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2xbjprqvh.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2uxiizurh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ngfuykfv.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2ljtxhqyb.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2hffeuqfu.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2hgdycebz.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2ixngnolv.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ajukfzhe.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2vxnqxime.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2zipexijb.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2cexmojje.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2kwswxntg.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2megrrhpq.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2pldczeqf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2whrvkwsf.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2rlcjnomq.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2hbeqzwru.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2pfbdgltn.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2czldicim.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2uwlduoyx.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2tbmrrrlc.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2jgfvwzue.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2yydicjui.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2ncbqmkrk.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2tqcvxppw.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2otiyolwg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2bogyrvra.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2sipdgkde.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2ixmtrcjs.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2jhqvqhou.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2smadehww.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2jysfpsoy.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2kjarmrfa.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2juasbohi.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2miltmqpu.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2vbbrwlsg.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2dteiaecm.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2ducmkdkp.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2eyznwtfl.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2hpbvgoeg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2bbhfofqe.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2tofsgzvq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2gbprpxqt.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2oxwgsoff.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2wrpcfkto.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2ceesahpt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2geehtlxw.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2hhbberxt.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2puhevyqd.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2prakzlpz.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2wazwhmec.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2mvxrhwqd.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2rikakdoi.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2iuhnrdua.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2naoeygry.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2uhqgcshd.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2xxbmjdtk.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ecboqswx.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2azdyxvvt.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2igpnyagf.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2utqhlqci.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2hmftljtu.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2xdmhyatj.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2kvyuzflp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2xfcvnbpo.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2wfovorav.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2arsobfpb.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2fnlqvcol.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2iinmuxwj.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2fhxjpxrw.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2hnnzhkpi.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2enecqcwc.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2dpycbjia.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2pmfrroux.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2mvklpxsq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2jrezbeht.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2fcnutnxu.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2pelrrznm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2gwurhaev.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2jhmsychm.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2klsaseui.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2uitblfds.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2wwsetkub.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2uavrkoyw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hcvkaqvi.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2wkhtvldk.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2zpshrthx.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2zbijfvlw.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2iyaakdkc.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rwiuotzg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2tbqpfobr.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2icmimmum.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2lbnfowct.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2qcpwchvr.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2dljimora.html


<!-- 参考信息 -->