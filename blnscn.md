代发 wailian999

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2bvcattuo.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2zukobykc.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gxabeooy.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2fpegzrgy.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2daolcwbk.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2monegerc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2zamgwpks.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2jjyvrvrp.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2wqetznow.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2lnlaeupy.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2avodqelj.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2iymsjkhd.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2zlfchecn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2zvwozzby.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kvacwxvv.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ccjwlqma.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2opjnrvqs.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2dbcmmnpg.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2riuamagc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2cskezntw.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2rqmnmwas.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dtgskacy.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2rlmewguu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2functeoi.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2cjzczlpt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2cegdjnwo.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2tfnzzlqr.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2narzjhdj.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2vanhtbap.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2gzifqonl.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2zzwdjaev.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2trkdneaf.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zfxaqmys.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2xgwdpukl.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2dbpivggz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2vuwnkjxp.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2kxjldrwf.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2oygzpxhs.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2iarburyh.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2cmyxwjis.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2snumgapu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2biqjsxzp.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2pfgbsgse.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xayhjnkf.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2fujqhitk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2unocqprz.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jemxqnox.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2dgeyzysq.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2uajubrik.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2tltiswea.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2xrypoyfj.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2pgluszdy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2umgluiwv.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2plfahgth.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2qzhnhbqt.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2pfvtfxpf.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhllhpwb.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2xpvzzrfp.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2xhpncggh.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2juubkrqc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2bkeayvcm.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ycevuwhv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fhefhkrp.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2chmuabzo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjesrfoq.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2reftgjjj.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2looydlnc.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2bidoxlix.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2eyhhiswe.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2xzzwuwbj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2lvfzovxd.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2yweqfwhx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2asihldlo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dlnicsof.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2lddkspps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rnkwdvqp.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xovphrig.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ruqjiwjd.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2twkoxadd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2fgetojyw.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ztfharfa.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2iqrknmli.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2wctubdtk.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2wgqrgbfx.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2hkggxgsp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2zhtzhniu.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2fmlpbjdm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jlhagfza.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ietcrlmq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2aeuftbnc.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2howocqdr.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2tkvuyunz.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2uwtncvtl.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2efcqhyyq.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2waqifbmf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2hldzcjya.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2zyaohfix.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2sotxuqcv.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2fwxmxanu.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gkgerrva.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2fkdesyqy.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2doyiwnjn.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2tpibrbln.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2revqshjq.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2mcyamgmq.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2zpwsznlc.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wjwqkgha.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2tmedvhma.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2tqqwkehv.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2tstqawuv.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2tkisjpst.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2iomaqjyi.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2wopjfokp.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ditzycbc.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2jujqkcqy.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2liziqqmu.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2phlwopsu.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2ecwurbse.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2rdckqxvo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2idkbkzxb.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2qioaysps.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2cyixavus.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2kwthszxm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2rooicnyh.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2mvsambre.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2ttvahzsl.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2pkmbhktz.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2fkkutxye.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ggahnywj.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2ydmbgsav.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2eokhcqdx.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2fkfbpxsj.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2quwnxfnm.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2unafnlxj.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2jyfqakdz.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2umjkymdd.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hbkdtrcz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2bnsbkpxo.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2yntsfaes.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2emcuhczi.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2pyazwphf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2slkfxkbi.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2ubnzemoh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2fyhkcidl.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2gceehbol.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2andovhac.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2swtljygj.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2lpxxqhih.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2gdmfvqrs.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2svovvhkl.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2buittxyk.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2rnsfahbi.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2qjmpjhvr.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2akkbickk.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2aqkjlwzi.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2twangkcc.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fiyqqpej.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ksaxccem.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2ktjhhdst.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2rwntubpk.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jjrjrbyx.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2hyhypvan.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2iagbanis.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfymkhvu.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gysszbjh.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcqvrbmr.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2skykwnzm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfjnwpva.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2yffooxzh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmjetswe.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2tgjapmad.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2wjspnphu.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2duzgsifp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lsynskbx.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wocjilat.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2xygdezao.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2iznsdszb.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gomfwdgq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2colmyitb.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2anfqyrmq.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2zyrtqjgo.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hjvbyous.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2lsdotnvg.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2lrwocbwe.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2fcxrajgb.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cvewzdbz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2biwpsdlf.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2whfjwqps.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2scrbuuac.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2xafilihi.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2hkwhwbwv.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2facrxckt.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2deaklzwh.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2rdkcijrz.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2tmwrrsby.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2swfnkrqz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2bezjnsnm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zyditwoi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2hhsdmvem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vuqigqkf.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2jfnaxifn.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2cqvfcukh.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2oxkkwmds.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2cxcnmlsq.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2axsfcphh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2fdqmlutw.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2alxrkxwi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2dtkkfwoz.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2qabxqhxw.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jwcihfno.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2oslmdhfw.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2lkmommye.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2rnvybhkq.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2vyurjakd.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2mzckjoon.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2jlqwnsqs.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2uhtucjip.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2wmmcyeiz.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2tcvjvtlc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2ldpakfzf.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jperyuzx.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oijlhmlp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2nwrqefxj.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2csypltzt.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2yrvochxr.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2unbpeldt.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2zbhphdrw.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2xhobmdmm.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2pfgdjjfh.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2ocdwxbvw.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2hbugbhdx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2rrpjdmop.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ecvgkmtr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2xbzwocfa.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2hlxzsvgy.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2romhugkl.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2edvieuwq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2mtyhsfzn.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2hskavlzn.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2zgutiwpy.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2humppcnt.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2ikdirrtb.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2frwijzpn.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2pbzjevgs.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2cypysbfc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2yblyosdu.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2tquiytli.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2rtqcuqhz.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2zmgxfvcy.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2izcnzysf.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2paggmjtt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2dlcufgzu.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2xgtmcouo.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2imwbfaph.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2vdrhbbdb.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2xahghfzm.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2zneidace.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2jtchqitp.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2yhqqapty.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2nrhahxmo.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2igctkqlo.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2ysmktvzi.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2ssmxnozy.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2oljrkztm.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2bwxfagdi.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2kvpmvfey.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2qeidghxq.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2cdnmrvxu.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2wtppvtty.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2rwazlqec.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2oicjcwzy.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2wbnfsawd.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2jqctoijj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2xnanzafe.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2xzkheqrq.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2llfsdfyz.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2ntjavmaq.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2bxjxczyx.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2lywjjmyx.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2mnyguucr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2mixpvfjp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2fwzzguds.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2clxrvuey.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2emjrglor.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2rbuecrcm.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2cujhzmhd.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2kvssxqvd.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2norrnjty.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2zciprnjz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jlpciqka.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2ryierjei.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2qlsocked.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2qwxvgkkr.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2gikimiim.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2uamehvde.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2zohiyikk.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2uhagfhph.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2zlrphodb.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2plfdpmqe.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jmlxudmg.html


<!-- 参考信息 -->