代发 wailian999

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2osbshqri.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2klgetlon.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2mwucklvt.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bjdjmbny.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2ojrsyybb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ajcldiyp.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2yvbwwrcz.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2fouktgua.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2gdczlcvk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ylmodnex.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2cbtgsbhj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntkbphew.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2iynsefcc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cyqeszmm.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2lcgdxzaw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2iwbaqflc.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2lrvhsajf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2msjmlltc.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2pxfyomnc.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ppehzslj.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2cwziqcko.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2wlwbuqin.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2uexfmilp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2cqhblzep.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2slqcaqyl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2hvicdebk.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2ocpudqnz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2oosumbfp.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2xxejrenf.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2gadeglrf.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2yxktjrxq.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzpjodhy.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2rwvsqtuc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2ajvupumu.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2zhgcobyu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2bjtsmeeo.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2hvyuwzll.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2zjowlvjt.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2unjfcwtu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2rdwqqsds.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2jniidghn.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2mvnwrvmf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2wzevhjak.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2nolvfphv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ajafdxdm.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2uikvqins.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ymblccnl.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2dzhhtupy.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2xfrarumy.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2trthakvn.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2yhntuymo.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2pwxbtsib.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2yhhhweky.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2nfaywxad.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2wnfhqflm.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2cymbfqtw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2fumrquge.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2ktfzttnn.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xekxvwyk.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ntifthpa.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2ncekolgz.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2endkedpe.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2vuuhqbpa.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2detfrtlj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2pxzxdjpk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bkssigec.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2tcpxieao.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cwlgxiyt.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fpxotksp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fsleukyw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2grkozrfh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2uaptvhkc.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2vrhdwgpx.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2hgkhodps.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2sbgezgjv.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ypvvgysz.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2imgouopp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ralkhvjs.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2flaerzlx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jdxjfgks.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2udclxjra.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2hqwzkzow.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2fbohlynq.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2dnedegoy.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2xnwwkxhr.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2cmvelfmw.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2eezoktzs.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2fcnyjpij.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2xxdjiogk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2jbrgahuy.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2bmbufxzy.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oygzcvuj.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2gjacrhdn.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2iruhfjle.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2aqscswjj.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2prsefexu.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2uyvneryn.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2kzriqucx.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yzwaxzzz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2htblcbdt.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2yfgdbqbv.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2ygomaisn.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2erykfyar.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2nampokah.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2fhsfiegc.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ypggkrgt.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2dwriqokx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2cnoekded.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qfuvmngz.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2selsnvsc.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2auiuvruw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2upylezfm.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2twgicyrm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2efghonel.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2tkmmidxq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2qaojbcxi.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2yqzeznfw.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2okxpivmj.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2epyrjhgc.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2ccmfsdbc.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2auyvnkig.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2xcyaslhq.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2aracxxsu.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2fuivdamr.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2nobrqesv.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2kcxnbubo.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2zwmjigby.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2dlanoyhc.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2znqnvpvl.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2tknkfjwd.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2wtojcvcc.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2zynyhcgf.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2jxjokypx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2ogqeugau.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2tyiyrcmm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2vgjkrxgz.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2uedcabsj.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2flzrgucf.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2txzoqmmy.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2vwwfcsla.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2netilscx.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2trnikbjx.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2aadzhaqn.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2fngkwbpo.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ktnqbkqx.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2fwqnydig.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2mvsexyst.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2cirebhne.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zazqameb.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2rqzdgbbe.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ggkjqara.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2keuagrma.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2cgbrlxau.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2eozszwaj.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2wliztdlx.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jsphvith.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2ssaipoza.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2migrwjoq.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2yihjycub.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mvigxhry.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2pvkwfmue.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2mojwnnkb.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ghzhogjz.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2lstuvpdd.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2xdqxhwgo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mzbchekn.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bucujjrb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2rjdkvvin.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2xbwagjdm.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rndnpzdu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gbnplkvr.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2wjhquniu.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2velnrhmm.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rggepxph.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2uwxdkbxf.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2lxxwvpvi.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xkmoryue.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2useyopmt.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sbwvtnml.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2odnxthhx.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2eendolht.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2mhmoylbv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2egtftizt.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2qtfwewyj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2kedsnpfu.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2qoeazjje.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2nikozaxs.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2lmjwzxxu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2mwemvdni.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gesjvuzr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2laylttai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kvznbnps.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2ggyfnxjl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2xjoihkcj.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2iiyrvlfm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2nfzjxmxe.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2okgmgsdr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2naepbmvr.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2nqapmsuu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2tleyfuvw.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2mraqhwyf.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2spailqbz.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2wmcepniz.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2exlclpml.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2xeemiccc.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2memdhahk.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2uvkefdhy.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2hjlkyxte.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2goiigoqx.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2huasjqss.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2larfpcwo.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2wmkwawkn.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2wynvxskk.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2vwqnvelk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2rdypulcr.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2twnhyxef.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2blbriuyg.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2ombgqwvg.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2onenhttc.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2bfvcwxne.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2piwnwfrx.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2ecijmpdl.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2qnjraxfc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2bnarpyqu.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2waqpkjql.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2rpkfgqkt.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2dhadkgzv.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ymtpmics.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2rgkzzjgh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2gjtucjkg.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2jgksiduq.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2fkpgzibv.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2qozdpcxk.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2aotrbmii.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2doxxzrrl.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2pihrzzez.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2nebxufoc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2ojzmodyv.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2ukjoeavr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ymabzeof.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2ryriyewo.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2kcrgipwk.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2araffmwx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2paljngie.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2ptgqwaxx.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2lpvkyeks.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2zpbeyzyg.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2gqodzpwj.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2ptkmpehf.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2rjlhyprc.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2uocvjhym.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2dtvkisph.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2oeacadho.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2kyohnltj.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2tbgnxpwj.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2ofcqylbf.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2wsvbpadg.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2wgwrmkxy.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2gzptznwp.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2mwcbjgnc.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2cuzltowp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2acfslgmr.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2dngnoxov.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2vezibfgs.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2eaaigfys.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2jswlixnn.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2rcnvlbls.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2jizciscr.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2zelgaupi.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2decffasv.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2vszvnakl.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2xgabhgfs.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2fyqwhige.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2nhzrhnui.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2jxwrltdf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2qwtldxya.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2pgbvodrx.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2emtnfwhq.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2exwfiapz.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2xhnvieig.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2kmkccfcj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jbhaqbnl.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2plqxrekf.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2htatlgyp.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2tebboytt.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2kergculw.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2pqvdbufc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2kyoryykl.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2bhgcejtn.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2wglhuwuv.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2kdrpmcxo.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eooknyme.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2aylwrtuz.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2krqgtujx.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2womxergy.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2gwkatvzb.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2impxitsj.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2fewolvpu.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2uqqgbmfy.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2bdadpyhg.html


<!-- 参考信息 -->