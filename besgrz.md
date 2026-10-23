代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3erwzeaej.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3cnpyqcba.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3zvvbsiha.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3hwkxddmq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3auhlletz.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3bsxekcnx.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3texuvijc.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3pdwpjlgg.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3dbmxnqxc.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3fflfyuse.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3diksqquo.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3uaxkmlpt.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3eorxqnki.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3vfwbqvnm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3krrqwshp.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3rcgsnpqm.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3crzznqvg.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3wcolmfjg.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3wekplgvi.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3iqbvytjr.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3tlsjiwsn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3evpcuplf.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3nxjosnmw.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ipotmvvw.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3aywokuua.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3qsvznbjp.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3xsaoyqyq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3sftfsedw.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3kncurhhv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nvglcmzk.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3ssnbqjrl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3culikjty.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3iunbdqqi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3cmdxoapj.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3qvpfrach.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3huwsmjmz.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3xzzuygmc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3llqtmath.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3geexdaen.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3bujgqktw.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3xzsxitjs.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3udxjxsbl.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3xyalilgv.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3rilwxvmo.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3wxgxlcxx.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ofxtzdlm.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3mvlqiahx.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxembfya.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3hmcftzfs.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3tzhifayv.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3lliymkwb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qplwyteu.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3clqiaxjz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3lmehlpem.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ymajzntq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3mipibtde.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3einzpbmg.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3vhrjuvma.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3cebitsjx.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3vavrxpvj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vqprhwup.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3veqrwzmt.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3dzdamcqt.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3espydmzh.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwgcpeso.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3sbjbwtrw.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3sactqoyw.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3usewpbsx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lnnovszp.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3aclihgog.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3drlfnqib.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3gtzslwvz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ruhitvqi.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3qxwhskxl.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xjqbsmjw.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3rcehlzbo.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bdyaapuq.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3furauluq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3mgvlkndf.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3thdqhnae.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3usdthgaa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ldswxrbl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3cfilireg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cifybizi.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gizlqwpg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3smyrunwe.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3kobmiipp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3lqtlbjms.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3stcjepui.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3qxtzwcai.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3zcvacaxu.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3aobvekyo.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jgcoqzhv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3zornlzgz.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ybhqfrmw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qewngxyw.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3kgvivuhx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3wmingajr.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3pngbldcp.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3fzcxupqx.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3gngmxxix.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3uxatbzil.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3zbsrwicv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3pzeuktym.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3lmimsvxv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3hvuvlqtt.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3gaakhelp.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jprrbtvk.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3ffyfgnxy.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pstmvkxg.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3lxldymfi.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3zgjutnaf.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3euxcmvhe.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3bxoupuft.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qlkppyma.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zuthjdfe.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3bxlcgnkb.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hwnpgtoy.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xjlotxmf.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3hlnxtahw.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3zagnrazc.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3fjpqqszt.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3euabqfwr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3qqgencex.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qgiwqpoi.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3uimejwhf.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ersogvjv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3lmccpxsy.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3ckdykzeo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3cshzjmzc.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3vmeoozlj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qarpyabf.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3spsjigtp.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3mujmbrhr.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3ppfowtum.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3xakewnqo.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3xnwcdvmr.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3lxwerubc.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3sqokwedz.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3hseaufrl.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3apzoqfbn.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3xhtsupcl.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ytztbtgp.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3njjzzbye.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qxlomagm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vbxonkdv.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3zyymxkiz.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3lcenqwhg.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3iwhfwrkt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ccsxqdap.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3uzgosgre.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3plheoyce.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3xwwhvstd.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3woizwbjb.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3eygixmqy.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3cdggrrlw.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3vtvmtykb.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3kpzidtkc.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3dmfwizft.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ihiiyezp.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3uoosjrze.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3mijnknyb.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3pajqfymk.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3koshsgnv.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uhhsjcrp.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3rytesjrd.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3bxbkirzx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3pdnwpves.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3npjlqqyo.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3zilrvvfp.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3bmuljabt.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uflswlkk.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3dlqfxfsh.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3acscsfbr.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3hcmktgiu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3rpdlpsvt.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3dzovsaaz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwqmklqg.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3mnylbgcz.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3syfgasty.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3edmybegj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bqbjbjyc.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jgmrxelm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3qbrvmmcr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3afcqhdhk.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lcdxfxvs.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3iyfccfpw.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3nmzwkqhs.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3goqhrjum.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wvmdggpz.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ifuueatz.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3xzueavzx.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xnhjpgsj.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3udkjitbm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3hatzrqvp.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3nrpaxnni.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3fbjkixhf.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fdyrucwq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3cnbngqnb.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3akyolbin.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3uxkxviwh.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3vepgqbcn.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3kgfenqvk.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3nckbarrl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3dfeqnxex.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yxbnsclo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ceazmgmu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xmozolpa.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3ewwqxeby.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3qhrtgrep.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3ljhxscyu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3oaifrffl.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3geudauko.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3uhaqxfbf.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3uymbyugn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3kdunojwu.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3pyuxsxns.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3fbbzutan.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3kopvowgd.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3uhehijsd.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3kekyrshw.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3dfiaguhr.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3qlejntnt.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3neypiaeu.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3tjaokzzi.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3fueintjk.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3zncpomms.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3urvdsifz.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3zfsufigh.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wbuqqcjd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3tvzvkyke.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3uphasjdk.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3hzbydnba.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3dfkfxsml.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3qqyxvgvt.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3akyzuabm.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3wjaywanf.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3glexhnin.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ehtokpwd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3hefljnni.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3khltftvq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3zldijjje.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3znfdwrmm.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3kduurdbe.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3ncaeqzgg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3nhowtstw.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3pjzozhmm.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3splrmnyd.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3mhngnveb.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ludhzpiu.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3qbofryey.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3rxedslip.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3nnjevekv.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3afoqrvil.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3gkezgewn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3oiqqvmgj.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3yipnbwnr.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3jatzflwz.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3lhavtwxf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3dftufwry.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3jzoxjipt.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3ygqqlsqr.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3zkhqlvot.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3jcewngqt.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3idaclxpg.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3asgszmpf.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3hqvpqaou.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3tcwsjjuh.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3kpmargko.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3kyznyrmy.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3qgftixqw.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3fawcwsed.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3esxfqwtq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3nohbgrjb.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3dnarzsfr.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3noyyumva.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3zmponzks.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3ocmqdigr.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3xjgrodmb.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3ndrpexfd.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3oyficpwx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3dbhiodrt.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3unbnjkci.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3ovjhkbqp.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3xtjzqzid.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3bsylgkur.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3mimujddp.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3dqkqqqkm.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3gjuuncul.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3gajhhzxe.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3budjjgks.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3mbfskkuw.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3astyuyuj.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3uezucmsc.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3cyhclbwp.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3oeveedca.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3fizbwvuj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtexuofc.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3iedcikbf.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3ixumxzgn.html


<!-- 参考信息 -->