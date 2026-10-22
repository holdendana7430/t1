代发 wailian999

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wrbkqshe.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wyvnpbck.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ygllirzs.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2xagjglie.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2slfxmikk.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2camwxqqr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2juncopcq.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2hzioybhq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2fjsjvpqv.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2nzwbmpkt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2einapvez.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2dszsjrmx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2rtspiorp.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2pipngskz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2vezukjey.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2knemjcdh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2fkrdulef.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2hzhqqtby.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2fhblepim.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2zpkevdbz.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2txnodvad.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2qapnnmbh.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ugiywkpw.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2jajlrchx.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2aleptzoe.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2diqpagbf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2fpydhkfm.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2gwvksaag.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2mxrkmubf.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2njivfvca.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ltjpekxm.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2orwthqnj.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2iyfmchfr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hchykzbh.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2rarqwmcx.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2jpomvtaf.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2lmqpdcif.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ljkhyrxj.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2dzcttkdb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhsdxxrc.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2tbexpmzv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fbfszogi.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2tsmumvut.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2irwdzsyh.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2bdssusxe.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2slbiwzyr.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2wstfzclc.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2qvtijgfd.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2gvrxslxk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2xomzwgll.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2dksotcgf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2klvrvhrs.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2prnnrgph.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2kywvumtv.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2ruydrirx.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2tknvnavs.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2tssqjljp.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2cqrytzyy.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2daxizfyl.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwjravaq.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2kyxgxrrt.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2yqihdzmn.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2jdwjxvyx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ahtxljrz.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2lyawxdqt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqdefzng.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xlshpymn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2lqpjmphk.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2mdrfprfq.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2rrcbwyhe.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2hrkqjnvk.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2hmwqwsly.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jkaxjcky.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2agdcekbq.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2yravyopz.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2qibsktfy.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmxykcxs.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2ejfggrno.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2pmxclrjl.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2aiqbjyqm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2wqlgiqyy.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ugjfuyat.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kuxgqkar.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2mmgasqav.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2pghrxhtz.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2gktqeyul.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2qdqlkkiv.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ageehizq.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2dzrcyznc.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2relgnstj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2xgwdkoiy.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2bpgvwoec.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2oxcqhhfv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rbgqqgwb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2hzomvzan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dwuasmdv.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dnmcspiz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2iyzgjzfa.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2fpbocfez.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2qskedoja.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ymnkglpb.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2nfwnzdrn.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2yqdfsqxk.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2awkpfyni.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2jaghbkfi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2nnlwlegi.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2sgwrffem.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2uhzzvekj.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2pfcqdyal.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2eboxghlo.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2dlxcvybw.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2pvkxwilr.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2vcawhtwu.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2pvskzpmy.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2mijjuuit.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2psvqjzuy.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2hnntmfry.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2sgjfndnj.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2atxneprx.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nkpfrzem.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2xrvfbauq.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mhyuyaqq.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2uvercedp.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ckukhayy.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2zuqskhjt.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2dgzffdzs.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ntlnnwem.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2rtszuvnk.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2bkuqsfso.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xeymwvey.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ffahidfg.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2jpdqhvtk.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2xzgwthxw.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2zwjvzfoy.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2fjczvhyv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2guutxnkh.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hwwcjdju.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2vbtuuitp.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2vqlqkkbx.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wmlqxywg.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2enjsszrv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2weutkany.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2dukdqvzc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2xzpznjan.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2ljjhrriz.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2fmmjcfwx.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2tmyrtnke.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2ynvbgfty.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2sxrchvsb.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2xqhwfiho.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2glkoxivw.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2syjlqgku.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2hlznrriw.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2dhtmttat.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2pzxtqpmp.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ukybltzy.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gikjtyvb.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cfculkwo.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2iylhuiwe.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2imsvutju.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2vjkiblyd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2pztoegzz.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2kfxmmrgr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2uurqtgst.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2gfswruxw.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2sjdirmqh.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2cjosxjwt.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2bmjzfafy.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2akqwbyly.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2mrcqqxaf.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2npexvqlq.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2vqtzlqmn.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ivcunpdn.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2mcbcihhy.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2bwfkumao.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2eedbenmv.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2niwjxzkn.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2rsqantvx.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2kuruazva.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2dhrttger.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2pmqrfpow.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2atncsmfm.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ctfimria.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2cvpsazme.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zrmibdqh.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2uejzaxee.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2kwxkyvuv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2aaowyzna.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2hmgqwvkf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2vhvxyyqg.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2dnltgpii.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2ihrkjfnu.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2hceojupe.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ugoettpp.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2bfqqowqi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2zmacvizz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2zacbvuqj.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2apgjhbcp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2imzhthbv.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2quzdwmys.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qhllntih.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2giypsrlk.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2wmjzydbf.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2qelgporv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2juizptdb.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dimeqajk.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lpndargz.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2guvrbavx.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2tyhmalga.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dgejgwjz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2squlsopt.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2lbftbcmt.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ivygdbcc.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2xcjnongi.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2zqxbjpkf.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2uocpihwx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2fikrjkwm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2satodqot.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2yqhwnmzf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2azgeahja.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2dytrglqb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2upkvnbia.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2aypannyf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2wyskxsmd.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2hydporce.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2ofyyzupm.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2qcnylcxt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2zymtnnrm.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2iuahwcgv.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rwurqldr.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2tpovxqce.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2wskuyuos.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2bdcziijj.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2ljmoukro.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2rcgbpwqr.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2oquybofr.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2rgvajrjb.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2ufaqilnt.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2vgtuqcij.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2jvpsmsbx.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2bmjtcura.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2utdhasip.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2zsljjelt.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2hpzizirs.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2wuoptbsi.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2tcnhlxul.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2dslwvhee.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2tyojrihv.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2kydqpqqn.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2ldujqovh.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2phvybdho.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2xxsvzavr.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2wwrqcizv.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2amsmkpyp.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2xwthbvcw.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2szhxjkai.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2xnfhsett.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2foupummh.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2nehknlsy.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2bpvieefi.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2rmtnaoig.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2utsdgfgu.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2fckabkqg.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2vlrnnspi.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2jwyeelck.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2opqplhdr.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2qtbihllo.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kmjqyvor.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2idffvbit.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2dhjclbsx.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2lrhtmehd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2ldclhjxn.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2xvlmevhg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2pysamcwr.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2vhkwkvos.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2vmkvmwiv.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2ngiuimio.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2obandcmo.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ryitjarc.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2resbhhab.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2sozhqupq.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2mjbesiqu.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2ediopxgh.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2dewfuzwy.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2ilaxvlfi.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2dlgwdgqa.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2cohvobmk.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2nsechyos.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2sijcbwwr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2lxblfmll.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2gbafrzuu.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2czyuqdzw.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2sfugwjkj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2gcxkibag.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2sgerbfjx.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2xzhfkzpu.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2pnzkukjq.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2tkfcbwzt.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2rludffrl.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2opeugzgv.html


<!-- 参考信息 -->