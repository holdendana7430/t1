代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3jssudpiw.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ivxmsgyu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3kgqfbcdc.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3krwxbiwj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3cbagexbb.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3wzajvknw.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3dtilnlsg.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3wbljlivu.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3lklirhvg.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3tbwcuory.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xybwcgfe.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3khpdmnwa.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3abthdlqz.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3svixroxh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3qxfqwfvu.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3rfsoberx.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3vcgykhry.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3fiswzfhy.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3iptidgma.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rdtdayrj.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3kxlwfkay.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cyyynngr.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3itduccys.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3tzngmqwx.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3yruefvra.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3eksjkdmr.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3uighbtga.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3snjzlvcg.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3gltwwfmu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ryqfoiak.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3hjyqskbt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qqmbasbb.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3kswrhlzv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3upuigpbu.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3lpaoykkg.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3xahxeejs.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3poaqhbkp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3pponyohm.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3awfftekb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3opsugelk.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3eiborehj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3arigddfc.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3wwqrhhtl.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3wcclwsrj.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3coscescj.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3nwprhoyu.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3ngsebetv.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3iifpehnq.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3mgbyiokd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3gyexyxqs.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3ppxsoopn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3aumugqno.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fwahywcn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3ozeteboy.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bajtxndg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3swyaympj.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3pdrjdrlq.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3fblzkhqh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3dlrlalok.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3fdtzbvht.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xbuylxhk.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3soyxknrp.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3fkpppawm.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3xygxinfh.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3wpvbuskx.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3lfdcejcp.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3fwvxtyzo.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3vjmjkpur.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3urertxuv.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3qdxdliip.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3gkycoufa.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3gayikdfd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwrqmeaw.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3zbdvfgog.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zhspkmrw.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3klyscezm.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3jnwfoikg.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3yithphfk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3qclchxre.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3bcwemkyg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3rlbiepia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hlgjneta.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3sdtpcyxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qlugkyrz.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wgjzvskm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3dudshafn.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3lrasluhd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3qeyitxfj.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3gsxfivac.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3aucomagx.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3konvumyp.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3zbbformj.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3jjodqqdz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3iqyvuzem.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3sdcfsllm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3orsmxmes.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3irlqxkgt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3iajshtxs.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3fumosxuh.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3cfrhproy.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3cwvebuuf.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3cihnuefc.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3coadbqvo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3qqxfseza.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3yhelqmfd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3lkdnkkta.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3dkbnktzt.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uftdszoj.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3gebabfjx.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ehgophpz.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3dzwgpmou.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3juvnhtlp.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3ddtpbuln.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3peyztskt.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3miafcvld.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3lnxzcdtf.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3zzcslgzs.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3seuxfghn.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3evawrrmv.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3dhetiqxz.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3lfobwlna.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3nmbrzcos.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3pfjsbxof.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3grrhsdhy.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3vhofgfbi.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3mwvbifjt.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3qhsjnhoc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3pydlgfgb.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3mbvckayq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3mpskgudx.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3xzvlfkbp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3oppornnc.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3hrxzzeav.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3wrkutbzs.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3bzoxxuvp.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3gwtdxvya.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3rzjadqlq.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ptqmtgqt.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3txvrfytb.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ibtfalzo.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3yaqjppcd.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3fjcjxymz.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3edlgbcit.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3clcdwqxl.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gptsziqu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hqjvintn.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3zkvrjbjr.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3faavmxpy.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3hngyhnpn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3rkfizboq.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3utcjjfov.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3rkytcmts.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3uxowunuu.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kjwcjdgj.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3dwgspkvk.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3gbozastl.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3nwjggqsp.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3umtsgoqe.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3plemzttw.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3awinnwlq.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3pvyetsbd.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3iegzmdal.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3tlihilmj.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3jjuboswh.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bmceqely.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3gazzftur.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3ruchhmvq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3wsuaftze.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tcxxyejb.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3rnlynxkj.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3axhmnktg.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdpuxvml.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sajdlpkn.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibffszxk.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3fwgaszii.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eylivepe.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3euvtgunn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3qffgbuze.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3owmozfdp.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3gtnidgbh.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3ratghigd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbzfdpgk.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dnrxmkxa.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3zpohhhlx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3xfwhqjdg.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xiiiwheg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bxdnutqn.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3afyeccsk.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3tetjdmdp.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gbjolbjd.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3nuahersq.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3flztywgg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3xsduvfuq.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3tfdlusep.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3qkmbeeub.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3jyqrszfr.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3vkgfqmdh.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3tzuyfpus.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3gguufemq.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3iowqhhuy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3suoecfus.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3xxshncgo.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ipdbpvni.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3skjnnlua.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3dycgzpfx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wcqoyrld.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cwqrgssm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pwlxjuhs.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3jzwtbayg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3gcduxazy.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3wdsigbex.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vytqnkrl.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3kwsddhwy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3vzhjgvyd.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3mbytxadb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3bmvobwgg.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3gtmekdbx.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3xovwgbtj.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3dvnukmli.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3snpusxza.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3mbjoalbx.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3evesjesc.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3qmnsscre.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3pxasvtov.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3sflqjxmo.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3vjusynuy.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3qufoqjwx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3xduqkagr.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jwhjtznl.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3tuspglfh.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3awnffiyy.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kdsyniwb.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3iscgtmdy.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3xtsewlwl.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3miesedpg.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3lvnsrunh.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3qzfhntvs.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3ddusbcyz.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ydnxdfau.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3timxiegu.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3vewfsckk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3zydjpghf.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3osccocew.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3xpvovwhv.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3yqbjwzsm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3lpitbmrr.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3mgstnkam.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3cckwqjwb.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3lbiyhtos.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ajvahkfd.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3bimgvzon.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3cmudtmfe.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3amzmszhl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3osukihnq.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3dseeyrck.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3tuljfeua.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3vsnzgxay.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3lbcjoiul.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3moccjnxl.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3wfmxnbkc.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3weonhkhm.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3nrogpbdz.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3fllrxxay.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3jhizlyzp.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3olxwmcer.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3ccazylsj.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3tzjvpmdz.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3xthdocrc.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3xdgilwku.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3bpiemttn.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wdxmlfkv.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3irxmbxkh.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3esiaxlla.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3isbuieps.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3eeewpglj.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3irkjykvi.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3qnnzfuqa.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3fpgljqkn.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3todkvpcc.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3rfdgnkwu.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3nwptqlko.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3usntyiwm.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3nmvkvdkj.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3sfouqjub.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3knaqkfss.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3jmlbynxd.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3nosgajue.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3xlgwmjqd.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3cedgaqkr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3nlhevvik.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3ijcicvlr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3atuoqxex.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3qjmqcnzs.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3seqkdlvm.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3qjditvew.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3bjsrfkmu.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3dhsyqqee.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkxntdzz.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3jugryibw.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3pqggjfsd.html


<!-- 参考信息 -->