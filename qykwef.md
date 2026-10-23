代发 wailian999

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3qyrlbbuu.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3bjsgxyqp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3lvhtyuue.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3rtaozepw.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3qzissgem.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3cduhzsmb.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3zkkjyjzd.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3besrwhjp.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3jdzoynsx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3dywfzvnj.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3fmlkrrnq.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3bosgqifd.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3qpiiutwn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3xbjfbpoy.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3jxgcajbo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3rubxuuke.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3cknfjplg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3eaxhltff.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3quvrhtsw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xnklxjik.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3xuebpvxw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3sgvvloao.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3wpqngrdd.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3qzzaszwf.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3mgfkeaal.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3qpujhpxf.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3bzerloyc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jgywlegz.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3svfjpoly.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3amqwkwje.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3tmhujhfx.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3pwfrrnuo.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3odzwwclg.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3nrjpkhes.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3nwhilgkz.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3llogtlzb.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3hagvdvjy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3dxtwdzhk.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3edtvyedr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3dybumgwn.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3tzmfeoqa.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3tkwodxzs.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vcktbjnf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3thnrvtmo.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3dukvdlmt.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3yxhvfakg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3kcjtnosa.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3hodzjuzo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3einqqwtg.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3emxshtkh.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3btndepbj.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3nrpgfuym.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3dporccxs.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3rxpnmzln.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3rxvbmmri.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ftriohnj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ugpudsyc.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3halaubcw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fsuqkyzn.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3bwgeudpe.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3fotpyzgy.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3nvqkfptu.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ovvkgrim.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3qtorwicx.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qlnhpypu.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3qvdwkddb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3mphvfgje.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3degjaphv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ezzobhna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aehnmxmr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3bkqeluqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3otlimjnz.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hrdjygvz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kzmitlgy.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3rvsaohuj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3drrptoss.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3yvolqcsi.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3bjyzrvih.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3pzntlycn.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3ldjrjuve.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3zqnwspli.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3yhbodmmb.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3llnvseso.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3lxjwhnzq.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3triiymjf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3przzkxzs.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3qcfwascc.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3prspsgpu.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3bgzoxcnm.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3ztwejenl.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3dkkucnfi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3zkiberfu.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3yhzjdddu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3ygvmlmin.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3pakvensx.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nsteumcj.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3lsmalguf.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3kjqcmzmv.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3vikdiinx.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3jyzmqksd.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3wskfqrhz.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3qqrivnuw.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ljlkgnsy.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3aqbqcfck.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3apzoeewj.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3xbrdlmgs.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3epvplksb.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3nzijznlz.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3txdqivxg.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3rsbvhoel.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3pcjagsrz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3kvxiuctz.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xkjbxxsm.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3wlhszvfm.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3wpucpkzu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3rhyyoinv.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3jdfupzdl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3scmumtby.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ygpserxx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dasbfbai.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3ngndcmjz.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3nxbzuizm.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3gkmdnmvl.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3rmblnlfg.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3odpstamr.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3snxwsihb.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3qybdpvzb.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3tkysmxvk.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3pxmdxwlx.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ybvqplax.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3hxrfpxxf.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3pkkbfrhd.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hezdzadn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3imbfvcys.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3onmfpxbf.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3mbmsobty.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3utskgzxw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3daabista.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3ecgamebz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3hirqqdsa.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3mrftuerd.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3mzfooanf.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3uufcpfye.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3pjhlqtje.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ighdlllp.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3urmdissz.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3efotvigh.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3takwcxcp.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3kaiodwmc.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ogmjxuhf.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3dvvstgfw.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3qgyvcjpa.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fuxqgpzp.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3galkvsjc.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3hnywpcjy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3refuueqs.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3eznwsucl.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3ljxgeduw.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3mqcnxvtw.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ldxkgxpp.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3htidcufr.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3esgcgupg.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3nagamxbi.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3jyoiiqkq.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3lgpguwkz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtxdcekf.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3krdnxgup.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3guuucozq.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3guknrdkz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dcgjzduf.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hrzjeorl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3ejwhwvgy.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3pxmnhhlz.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dtbkojva.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3uhgqkgyq.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3divzceil.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rmspwaso.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rajvqegn.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3xutwoqic.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3wgqzpjmq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xyaikogw.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3wbffegyi.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mehfezpn.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3hqaedbyg.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3wsgwnyqk.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3jvmltcja.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3jvdpojez.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3mcudtpip.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3gudkiqic.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3smdrvtna.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ypcwdqvh.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3bywbnrju.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3odkqfrah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oevuglzi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eolyncpn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rbtehgid.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3wfekanza.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3lmgeysnv.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3fkfzyyml.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3hfsswneo.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3pkskukog.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3ntsuttgf.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3dmtovtzd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3njdmsoab.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3gksvdtzx.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gcjxrkuw.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3gazetcsb.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3ltcwirva.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3uljvtlgx.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3pvnzitkn.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3scnyrghn.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3mcjvlnyw.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3eaokjvly.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3jxaqkhak.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3jrbiolwl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3ebiiesob.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nzxqgjsg.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3zqqqutuu.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3kyjhulzc.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3pcjqnbga.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3jawmhsda.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3nhfigiwv.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3mfjwgmjt.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3jxzglwlq.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3qqlpxltu.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3utwobtjy.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3kvqqotbx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3wqkiclgk.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3qmgmrmsj.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3xuleszbp.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3fusgegse.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3clbhuudi.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3lozzghee.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3ahkwyulz.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3rxgftfcn.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3mkqokhpx.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3jnasjzll.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3xajpxnbm.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3cyhoucuf.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3lucbdxyg.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3hyyamatg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3kvjmznlc.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3atoljodg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ptdbzgjo.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3woieqfep.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3fbylbdaw.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3evajvjan.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ovzvrprl.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3ncttykeo.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3zdqjwfok.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3ohoxnlrd.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3axuryfmj.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3cxxaurxj.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3fhveusxz.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3mefutybs.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3exldnvjz.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3djqefvnx.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3csmvdehz.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3npimenwu.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3dwjumkxo.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3cqvfftfo.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3vmdgxyye.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3zchwjgwt.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3ukscccbi.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3gtbqudin.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3uosqniar.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3bcnxzdqa.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3rjgfihye.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3rcpatlvx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3oylavosp.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3dfobdvfm.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3vtifenvq.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3nyuklxhd.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3zjelubpx.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3agohqegl.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3jmndywus.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3firfehgi.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3tvblnzuz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3bpuutwfv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3wbbivnqn.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3kqbcjruv.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3jyfbpiwo.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3jaehxzir.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3wfwtvler.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3zaevfori.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3duiqxgyg.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3prdgurqh.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3kspjhyqe.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3bpblakhl.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3riiltwem.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3sckapust.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3xholmxrz.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3fqqconxu.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3gnilqwtz.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3wxxiltew.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3ykkhkdww.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3sfejwzyr.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3uovgvgpa.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3wmtdmiod.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3zswgwvvc.html


<!-- 参考信息 -->