代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3olvahtfw.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3lmuyxtzv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3vqqtettj.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3pvlwlsph.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3oncztsef.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3zlmesbwz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3uhgcgone.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3ubwdbvcm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3iqrhlklo.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3wbxqudwe.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3xecysigi.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3gduloyvf.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3jtfuxrjd.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3bmqewdcy.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3suxmuorz.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3kdqonwfv.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3jwqmzyhy.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3wybsupxe.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3atocqvyb.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3zofburqz.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3zwhtyoys.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3txuvnuoq.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3llbtkvfv.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bplfwmrz.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3axmgrxoy.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3xlnxippo.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eljiftwo.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3idtuuxkl.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3pilyrksi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3owoxdhhx.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3yfvsxnoc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3mmucivev.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3jpgrrxng.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dfappyvt.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3jscasxxw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ciqkwimf.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3sktghqly.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3wqfcplcv.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3uhrtsguw.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3rlgnaatg.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3dyoehvju.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ruaxbgam.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3efyduxxo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3xaqexnru.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3crcfihhn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3qduqtkir.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3tbvduvxd.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3yxjtmwrd.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3pyqkxvfc.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3curxfocc.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3lylcyeqe.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3gbzetqwf.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3mdtsaomd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ojkbveeb.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ffxlcapm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjnvljgs.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dohbjlgk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3sikowbub.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hltrpdmf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3uxmbmgcd.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3hfqkqibp.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ckalujqi.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3ojuwxjbc.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3cchfuojo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3spucwypa.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3yaroigvz.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3wdeuoanx.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3jvmiwafx.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3hjyoolte.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3kciazwaf.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3tftfewbj.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3kdbjucib.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ssajdnvu.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ugyluqex.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xrjsblgr.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3vcwejaqx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3unbeqqyb.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3vxsfogsc.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3twzndqny.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3doxnsqdm.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xhdyzrgi.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3nqhsudcx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3mtfnnjny.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3ueabmvlh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3feicokel.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qevyhnbh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3vhogunsi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lwzbgaud.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3acyvhdzw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pcygkoii.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3icfygktx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3gqdupaqv.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3tmlbfibj.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3odkuiitm.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3vxejjpef.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3ghuuentv.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3dfgrbqzj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3yhsptrwt.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3kbdobpei.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zvalgbiu.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ezesxxxz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3dneeetrf.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3wfnvybrt.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3cuohhyge.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3ytqqckzn.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3hhjhuaph.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3ojcicerw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3yrhhjixv.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3vkclxsli.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3psvvantk.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3pwcglljs.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ebzopszh.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3bhzwyues.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3apbiyolj.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3rnygnkrk.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3xllokgoo.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3vdhmadjr.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3kqlolyrv.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yqsedjwu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3imsljwvt.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3hjgdldlv.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3zyrutyiw.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3cggqfrsm.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3xfnhzclm.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3kquotjoj.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3kuhwtkfd.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3lrmdztgw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3panmtikn.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3vrxeixlm.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3sgnrwytw.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3hqkyyudi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qasechgm.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3ajjjildw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3ycaxegfu.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ghrbefit.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lelnmpbu.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3ysxlzmex.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3wrfjwnad.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3hkcbgoac.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3pooydwkt.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3rznudrop.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3espuqukn.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3amiamrog.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3nsxjomio.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3mruuikzh.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3angtawow.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3epaiyxek.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3cduxkljs.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wipbrjqu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3snaurect.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3inzxhabh.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ckovtpzb.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ooxkzkmc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3xxwvojbh.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3zxyhohoa.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3wunqnlra.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3ccjuvulb.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3qnbkzrhl.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3vshnysgp.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3yvifbzub.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ldylaaxm.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3eqceddvi.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3dmdynngf.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3trfwwlom.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3cucoouyn.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3freihopv.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3muydrnqt.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3rnamgdqp.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gziheyed.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ncjqhwir.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3iecydewf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3saxxbgdm.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rgewwtzl.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3zarcicqx.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3rlmqjyyp.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3kwpfkvuq.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3apfgveaa.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ztpakrng.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3zmpyyvkl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3lkctazsb.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3tiqcdzgr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3qxhjkuhg.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3qmdpkyca.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3veljlabn.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3awqidvsu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmevdbtz.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gcrrisjc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3dyzfrsri.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbvyfdyk.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3milouons.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3odniwmxr.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3kjuqwnvu.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3hpvvzlvm.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zgymwyca.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3sbtqfekn.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3mgtzimlw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3rhnkjbmz.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3secqqhxd.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3wgdijcak.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3zejasawx.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3mnidizgv.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3fwnffdug.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3spebkycd.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3ayrnwbvz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jwhvnast.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3xffrsnma.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3lpxryokq.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3xiklhhdy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3myoydnzj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3quvrrifx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3eavftfyp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hsbxwzew.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3zfzssurv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3arhjpwwr.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3dslbjuoz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wjhxdoox.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3lsitzuah.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3gmswxyup.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3rquaejqk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3iayvxhkp.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3hcvyuruj.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3daprfjmp.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3ybbnkicu.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3xbdahnvl.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3aaylspht.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3vrmbroed.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3xmrhkpum.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ojslvrqt.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3zgciwdhf.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3tvinnfjg.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3hihfnyyh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3ndstzlkb.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wkyvdhav.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tdowqrpu.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3trovofqb.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cjsvspko.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3xkaxjyfq.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3uttrzaca.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3ckmifzyi.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3hupmloao.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3rvhlrxmd.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3xxnvcjvu.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3apwsepbi.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3nauevmtx.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3erakytjf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3gtscmdvx.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3ivkwtidf.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3dhblhsxp.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3owssefzz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3njymvxlk.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3vigsetkx.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3tftcenpg.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3xsedyfcz.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3rulsyvej.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3fhqhdzxb.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3foldaqkm.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3oeyrlpyt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3begqalfe.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3lwetgsyr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jixcrncu.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3xvdtgaax.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3haghtxja.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3csklvaxg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3fgvxvopl.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3gbcbobji.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3houbjdtu.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3oqrjvvsw.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3ehyywwtg.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3mrnsocbj.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3rmoplvos.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3dpnyeuyz.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3cjzdbpdw.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3pocwpgbx.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3xmrkfnif.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3tnsgnqzh.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3zdndmrvi.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3pkcvaelw.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3dlhwjoxn.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3jxyrhyys.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3fgknuupt.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3bnqzwkar.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3upnlogqs.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3yjpbodeg.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3aeupbpyf.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3ynbzvczu.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3bdcgzxia.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3rsgpwpof.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3blgosdjq.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3lfozbipv.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3stajgmtt.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3shifpunq.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3panjmmwa.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3qrbmlcxp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3bejpnuob.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3bmgaokel.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3nktseinv.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3ekpsvbkc.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3efpsxini.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3lwwxzxcq.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3owyjixpb.html


<!-- 参考信息 -->