代发 wailian999

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3txsjtwnp.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3tthujvnl.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3znqkmsjm.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3trtnuxip.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3kcuiprhv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhaembml.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wlgymfur.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3bbsyjwry.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3cvyijfuz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3pazxclfx.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3wqeahdml.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3xibyxkzm.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3iavslids.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rrxnphqn.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3uezqnmla.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3erllfirc.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3lxomujrj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hiyqtlvj.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3hfwkfpuc.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3zepwwqjz.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3meuhbkfw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3qvauvdwn.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3kifqkmgg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3fdgvbnle.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3cqglceyn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3wcxefleu.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3jdazlwll.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3stfcxvur.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3zxrexcaq.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3alsgmlef.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3pidnqfyt.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3wxdlsajn.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3dakcnslr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3wlzgdeav.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3foywvswi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uielakfe.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3bpagrfrm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3knsyuhpy.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vlgedkpc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3yzliwbkx.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3oyxycpag.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3baozwqod.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3tbclptxo.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3ultkoqcm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zxxlhyyr.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3zooucvft.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3vlzmrxjx.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3ryeilrjx.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3wykjhdwp.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3egvesdhf.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3iheumqea.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3huugqbva.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3lwhaxryj.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3dbgagmle.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3fctchctw.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3wezkbmoo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3zeqsgxgp.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3uaqzfipn.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3trngdfmx.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3tsxkjtkq.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3koypezqv.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3uzgbkqow.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3mnfeotsn.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3tnnsusuq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ccyhkfde.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yyfyqdxf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3pigrdnwd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dkhcbllk.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uwvpjwnj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3lylnauyc.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3cvqlvabb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3dqljulgg.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3jnpratis.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3wcpmrlor.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ggwgzkal.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3numezsal.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3ivyptjzk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3uuaqwgct.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3fanysavp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qbbgpiex.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mzdnhhug.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3serczhfu.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3dtzejprh.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ewupakkv.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3pmhosxbw.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3bbwcsuih.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3yorintot.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3oaawoluu.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3hvjdoomx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3pnzlaleq.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3yersmwqs.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kynrecgn.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3cqrqztdp.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nxizbxrx.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3uxwysxes.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3twpkmmtq.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3udguhvbs.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3fmghfweo.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nnhboiqj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3aqmptpsl.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3jfkuhgpe.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3nguowysy.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3cpkhtlxi.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3izvmoilv.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ivjtftzc.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3eyzfdfhz.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3eeacupmv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3yarnpmcg.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3sqegppuh.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3pcfvwnmp.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3oebhizmh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3synkauts.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3divjldev.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3xpvmnwrn.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3tornkzdq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ndyparvy.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3vudxgkqd.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3owvyprwi.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3ncjyhbjz.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3pwkagsan.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3hrlnijlk.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3mkckbfjk.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dhjmdqcd.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ldipvmij.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3djuhskoq.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3rftcjwxa.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3rixbhfmh.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ejrysavi.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wjvpeyxw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gpwgbpmy.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3mvuvnmfb.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3irwchrjw.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3gqrlfsyf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3dmdlfpxd.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3mqtztghf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3bnufadhs.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3hmrgwdop.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3grrlhkvj.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3vnmyukex.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3bfrgtmkk.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3pkxkzofs.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3stbpoiwz.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3qxwwozhf.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3dwuapkzo.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3mggfunun.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3gdmkgiqu.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3azxihhrc.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3kikdmura.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kyalbvat.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3lesnacik.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3hkohmfjt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ydpqxjoq.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vmyifpbl.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3bdtyiodl.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3tyqdvjxz.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3iyzrqfbp.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ohxlpere.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ytnaadxp.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3svldzido.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwrhhuzv.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3bqyjoyol.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3womhjpdl.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3tpeedxsb.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3qzviolii.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3lhygrkqk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qxrnnqek.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hbmkagou.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3hunputhq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3bsajlotv.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qdwoznlb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3iclgrahg.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3bqenlwhv.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3bprjmudu.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3duwhyeev.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3kkmxfrko.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3syauxutv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3cmqhcfvv.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ijuaidac.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3srzrlfwt.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3xxpfhsvm.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3recrodeu.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nbgmhbbp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3vjbeiiab.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3omahpjtb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ktgnuujd.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3byskxfxw.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3rkzbbwqn.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ftjsjyme.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3xbghuoee.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3irmtfsoh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3kmnjrvbw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oqbhuhkz.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3djogsboo.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3vusnwphv.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3ouqbjgai.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3fcdkibiu.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3qetfcfkm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3bpfljglv.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3nxsxeakh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3lcjmzrgo.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3grlbxyko.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tzuuskbr.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3olaypmzj.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3clabjudb.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3vdgmwtgl.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3pavadkdd.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3azzclmwo.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3pyqonliw.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3yebodmym.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3onvtcmqh.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3yecfekzi.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3qyvnwkjz.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3jxxhredf.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dssqfbct.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3tvnicwta.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3pgxuajyz.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3qxcffmat.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3edsylxeg.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3afobpvjt.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3jihxkiaz.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3murtlmpy.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3ykmvycum.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3smtpjyts.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3tlbktwzz.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3jprwjeeo.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3rdtiazju.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3dwoahhyk.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3dzizntzq.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3iklblsrw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3fegnpmyi.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3rhahxqxh.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3dzlybase.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3lupmhdsu.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3wgqksbxy.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3qjnyysgk.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3riuldokh.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3uifttzvu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3aqvopbyr.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3smpqjgxg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3khfnqwmq.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3rkvkbfxk.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3fqresfyy.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3kifolnew.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3bpulqipt.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3ecarjpxl.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3mypirmdk.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3urvxagvo.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3ocagzhmi.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3dxvycnpq.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3yeulruwe.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3ngqlxurt.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lfxltkkg.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3pssqrzyk.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3dxuxtwgq.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3sgmxchsi.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3cytfdpfr.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3pjqaovss.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3qfoiozyt.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3jryeztcg.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3bnelgjgy.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ddrotzrd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3mgprapfi.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3xbtwwbee.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3vqtxfhfa.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3eccjfzfd.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3bakqvzjv.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3lbuyilhd.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3gpohtemk.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3tupsxyik.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3cuiqlbto.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3moubvilu.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3iewkehyw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3avkilusi.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3rmbnngzy.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3oshzcxdq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3dohcgbxg.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3zollilbt.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3bkdwaakg.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3qaixoamf.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3yhrqqnha.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3scsywsat.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hgtsvlye.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3ethmretz.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3cmzzsdot.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3finlfcdu.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3ajyaopcx.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3olxgelfj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3xnurqwlt.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3zesaigfe.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3qymtabth.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3mfgfujuh.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3cotympkb.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3ypqjvlnc.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3hpwythpf.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3mcugdwax.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3fsjlamyl.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3pvgoamfi.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3kktrnydr.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3weanoyhs.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3mlyfjsno.html


<!-- 参考信息 -->