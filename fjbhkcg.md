代发 wailian999

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/gnroahelh.sHtML

[S19] C：快速排序
来源：http://mobile.hesvh.cn/Article/details/gmiqnyusa.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gblxckshl.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gvtxrolll.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gwvykvqyi.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/ggnkyhzdw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gdukmbsbe.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/grkeevfdv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gnubyfzbn.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gazjsalrb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gliukcawz.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/gsnbhhaww.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/goyblyqdp.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gbqhtxcit.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/gairdlphl.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/gnpcksasr.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gftqozpwe.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/gclwvmwfn.sHtML

const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gyaltphwl.sHtML

[S28] C：静态变量
来源：http://m.share.hesvh.cn/Article/details/gfvniwwlo.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gingcleuc.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/gvueeglos.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fehbvm.com/Article/details/gbmuhcbdc.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gaztkfupd.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gsacrxsmm.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gsxovxnqg.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/guwfebgkn.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/gpzccjbmt.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gniwewapt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggmhwhiip.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gsdlaxpit.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.hesvh.cn/Article/details/gpxwherpd.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gjplodlzp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/gefmlufnv.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gvkpgmsnc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gnniumwuy.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/gxqpdabhu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gdwrgimls.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/geepbkyss.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gxugxopnc.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gweygyggu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/gunyihlvt.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/guxjjccar.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/gwqajncqg.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gbihmxlek.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gyydqdehm.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/gmogzcxub.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/gfpuhbdtx.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/gsuspgnab.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/gjmmemrrj.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/ggglqvuzz.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fehbvm.com/Article/details/gdvbncyak.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/gfiujzzyz.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/gbztgjquf.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/gijmpuqiu.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gizmudipk.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gcoowlmwx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/gumjnlqgv.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/ggjdgsrmc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gawwgahlp.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/ggjfmfrjm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gezgtvfmf.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gxlnrhfus.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gnsybjpvn.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/ggmvevdgs.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/ggauqimhh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/gbruflzww.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gikigkfhk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/ggumeenmr.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/gowjnonio.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/gzimditbs.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/ghnvxecem.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/gkpdomkyt.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/gwoeedfen.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gborupmjs.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gddfgrdba.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gugzgugvb.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/goarsfmum.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/gzopnkmbb.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gghkslkxi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gxhdziolt.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/gztrqamxm.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gwtjodhsl.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/gjucjgale.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gpgfbhgor.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gotyhbyny.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gpevdpciu.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/gmstriwbg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gcnjmmpcz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggditqwra.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/ggsfawkjb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggsyscagq.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.hesvh.cn/Article/details/gjdsqwuze.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gljrbzxtz.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/ggrijpsvm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gurdhqjwv.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gkbpzlweq.sHtML

"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gtoeooour.sHtML

[T04] Kotlin：空安全
来源：http://m.share.hesvh.cn/Article/details/gijavuyaq.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gxscytxws.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/godtribsf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gmkupxorl.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gesexxsjv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/gczltfyau.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gbkmsyhwp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gsekyyorx.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gpansdeat.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/gqskkbeha.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gftskvoyn.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/gheziktlc.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/gordgvhxg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fehbvm.com/Article/details/gcqfhjmxh.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/giibsrmae.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/gwxviafgv.sHtML

[T12] Kotlin：解构声明
来源：http://3g.hesvh.cn/Article/details/gpbgulgan.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/guzwdraqv.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/gqnvknvou.sHtML

val m = mapOf("a" to 1)
来源：http://baike.hesvh.cn/Article/details/gdiqzrnme.sHtML

[T14] Kotlin：循环
来源：http://3g.hesvh.cn/Article/details/gprscouob.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/guzafviwi.sHtML

[T15] Kotlin：接口
来源：http://wap.fehbvm.com/Article/details/gfvsfuwvf.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/govyuyddf.sHtML

[T16] Swift：Hello World
来源：http://wap.fehbvm.com/Article/details/gicppuiav.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gifratmof.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/gamjbzmwa.sHtML

var a = 1;  let b = 2
来源：http://read.share.hesvh.cn/Article/details/gqrjswqwj.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gxfpnxzzr.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gjltslcid.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/grwmqcizf.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/gazgkavgw.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/guwtwbplg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/gxrlkjyai.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/gxiomnpup.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/gmrcqjlmn.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/gooaynhjf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/gipkrlful.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gokqioncd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/gsncnbrqz.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/gemgsqlmd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fehbvm.com/Article/details/ghchfkyan.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gzkdsisaq.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/gbwwhcfuq.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/gaqdgxcbz.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/gpvvmduue.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/ggpxbobuj.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fehbvm.com/Article/details/gysucnnol.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/gsefdcaag.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/golvcgqth.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/gybkvtskt.sHtML

guard let x = opt else { return }
来源：http://read.share.zdbjq.cn/Article/details/grvwejrbc.sHtML

[T30] Swift：协议
来源：http://www.share.zdbjq.cn/Article/details/gfiuebskq.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/gkrkwckme.sHtML

[T31] Lua：Hello World
来源：http://www.share.hesvh.cn/Article/details/gttebbgbu.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/ghxyynuvo.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/glpkynvvd.sHtML

local a = 1
来源：http://blog.zdbjq.cn/Article/details/gvwhttueg.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/gwkqpjkdo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/ghjyskmxr.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/gnfwftdol.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/gcolmiwsw.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/gyrcnkgpy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/gdnkkmadd.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/gsbsgxbsl.sHtML

function add(a, b) return a + b end
来源：http://read.share.zdbjq.cn/Article/details/ghukekchd.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fehbvm.com/Article/details/gvmwctlgj.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/gkpqdomlk.sHtML

[T38] Lua：条件
来源：http://www.blog.zdbjq.cn/Article/details/ggteuhxif.sHtML

if x > 0 then print("正") end
来源：http://mobile.fehbvm.com/Article/details/gtystcbbx.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/gxriensup.sHtML

string.find(s, "%d+")
来源：http://mobile.fehbvm.com/Article/details/gogpkbdjs.sHtML

[T40] Lua：元表
来源：http://read.share.fehbvm.com/Article/details/gpnanwjmb.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/gnvvagmyc.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gsowttwch.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/gfpqfxwfp.sHtML

[T42] Perl：变量类型
来源：http://www.blog.hesvh.cn/Article/details/gkboadbei.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.hesvh.cn/Article/details/grswmynuk.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gvejqboyd.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/giwdgvuzt.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/gtfkhojpp.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.zdbjq.cn/Article/details/giwbucejo.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gnyvqdhmv.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.zdbjq.cn/Article/details/ggnpwjtde.sHtML

[T46] Perl：哈希操作
来源：http://www.share.hesvh.cn/Article/details/gsatygudh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gtmbdqqeg.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fehbvm.com/Article/details/guhfdauqd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.hesvh.cn/Article/details/gmosofsio.sHtML

[T48] Perl：正则替换
来源：http://m.share.hesvh.cn/Article/details/ghytadxrp.sHtML

$s =~ s/old/new/g;
来源：http://3g.zdbjq.cn/Article/details/gyieykbpa.sHtML

[T49] Perl：函数
来源：http://3g.zdbjq.cn/Article/details/gscioenhd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gfwovtamk.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gbwjszdnf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/gegngwzfj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.zdbjq.cn/Article/details/gcpicljjn.sHtML

[T51] Scala：Hello World
来源：http://read.share.fehbvm.com/Article/details/gvzxmixjb.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gquxzkwbo.sHtML

[T52] Scala：变量
来源：http://blog.zdbjq.cn/Article/details/gzgdvxjth.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/ggqbryazq.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/grfjnzyxg.sHtML

s"值: $b"
来源：http://wap.fehbvm.com/Article/details/gbmtlydqd.sHtML

[T54] Scala：集合映射
来源：http://3g.fehbvm.com/Article/details/gzecvjgzv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fehbvm.com/Article/details/gdhjvqmnf.sHtML

[T55] Scala：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gknkpktqn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.zdbjq.cn/Article/details/gvdapnbxw.sHtML

[T56] Scala：样例类
来源：http://blog.fehbvm.com/Article/details/gnemzpspq.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gfpkmkjta.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gvtscmohd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/gwcozajsr.sHtML

[T58] Scala：函数定义
来源：http://wap.fehbvm.com/Article/details/gwrpcqkhe.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fehbvm.com/Article/details/gkfdaqnvb.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gvguoycse.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gjuhmeata.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/gdlhmlltl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/gxcxafxam.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjcnfmimv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/grxuelwsu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/guavehdiu.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fehbvm.com/Article/details/grmsrsaxa.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.zdbjq.cn/Article/details/grbbyntyo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fehbvm.com/Article/details/gqjxlkzgc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.zdbjq.cn/Article/details/gfnfvazno.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fehbvm.com/Article/details/ggcnkphab.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/gyvuiydxa.sHtML

[U04] Py：变量调试打印
来源：http://wap.hesvh.cn/Article/details/gxepyothb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fehbvm.com/Article/details/gfbeoisna.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/gmxljrqgr.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gpehtlntj.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fehbvm.com/Article/details/gzwcexqkp.sHtML

{**a, **b}
来源：http://3g.fehbvm.com/Article/details/gtmqetboa.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fehbvm.com/Article/details/gucmxsmyk.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fehbvm.com/Article/details/glnqgrdyd.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.hesvh.cn/Article/details/gdywdypph.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gdqbzpjvm.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/gmohwxjzr.sHtML

max(d, key=d.get)
来源：http://mobile.zdbjq.cn/Article/details/gmkoeuusl.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fehbvm.com/Article/details/gagdonekv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/gqfqvowil.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/gumlhxikj.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/gvhacmdvo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.hesvh.cn/Article/details/glvtzfnhg.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fehbvm.com/Article/details/gnmtiwgil.sHtML

[U13] Py：固定长度队列
来源：http://baike.zdbjq.cn/Article/details/glqcwpirq.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/gvfuritnv.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/guvxjdttm.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/gpdfuykfg.sHtML

[U15] Py：高精度计时
来源：http://baike.hesvh.cn/Article/details/gdrwndjkg.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/gimqxfivr.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/gwhocqhcm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/ggcbznvza.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.zdbjq.cn/Article/details/gkiaijboc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.hesvh.cn/Article/details/gvujhkapz.sHtML

[U18] Py：预编译正则
来源：http://www.share.fehbvm.com/Article/details/gucpoounh.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.hesvh.cn/Article/details/gmqpbndxh.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.zdbjq.cn/Article/details/gefgspbyw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.hesvh.cn/Article/details/giptmaeoh.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/gkwwnlpbz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.hesvh.cn/Article/details/gczzllwzo.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/gqaeevonl.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/gsxbipnqn.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/gmlfilisl.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/grntgmagm.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.zdbjq.cn/Article/details/ggscbbfsi.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/gkwniwsyu.sHtML

[U24] Py：路径操作
来源：http://read.share.hesvh.cn/Article/details/gnohmgpyi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gbcjrisvi.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fehbvm.com/Article/details/gavybvnwg.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/gcucdxlqo.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/grddyljjc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.hesvh.cn/Article/details/gunaadeng.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/ghentqzmt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.zdbjq.cn/Article/details/gyajhumwl.sHtML

[U28] Py：类型别名
来源：http://read.share.fehbvm.com/Article/details/glmvwfsuh.sHtML

UserId = int
来源：http://mobile.hesvh.cn/Article/details/gbprkaucx.sHtML

[U29] Py：属性校验
来源：http://mobile.fehbvm.com/Article/details/gzihsgias.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fehbvm.com/Article/details/gdgfobzer.sHtML

[U30] Py：数据类
来源：http://www.share.fehbvm.com/Article/details/gpctfbsse.sHtML

@dataclass(slots=True)
来源：http://3g.fehbvm.com/Article/details/gefqbmrgp.sHtML

[U31] Py：单测
来源：http://read.share.hesvh.cn/Article/details/gtlztvdnt.sHtML

python -m pytest -q
来源：http://www.share.fehbvm.com/Article/details/gzvsinyvy.sHtML

[U32] Py：代码格式化
来源：http://m.share.fehbvm.com/Article/details/gysblzvwa.sHtML

ruff format . && ruff check --fix .
来源：http://baike.hesvh.cn/Article/details/glupoetvh.sHtML

[U33] Py：打包发布
来源：http://mobile.fehbvm.com/Article/details/gylbfhqqg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.zdbjq.cn/Article/details/gwspayaxa.sHtML

[U34] Py：判断编码
来源：http://m.share.fehbvm.com/Article/details/gaiukfmga.sHtML

chardet.detect(raw)
来源：http://www.share.fehbvm.com/Article/details/grjbprjti.sHtML

[U35] Py：发送邮件
来源：http://www.share.hesvh.cn/Article/details/ghlrqnnsq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/glvauhmyr.sHtML

[U36] Py：定时任务
来源：http://baike.fehbvm.com/Article/details/gtszkjwvg.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fehbvm.com/Article/details/gzlsyfneq.sHtML

[U37] Py：读写 Excel
来源：http://m.share.zdbjq.cn/Article/details/gdlbdoqqn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.zdbjq.cn/Article/details/gcvmzdmep.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.zdbjq.cn/Article/details/gcpafrvsm.sHtML

Path(__file__).resolve().parent
来源：http://m.share.hesvh.cn/Article/details/gkxhhdlqu.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fehbvm.com/Article/details/ghsypgxxj.sHtML

sys.stdout.isatty()
来源：http://read.share.zdbjq.cn/Article/details/gygsgjesh.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.zdbjq.cn/Article/details/gseqdehtt.sHtML

print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gwmnhkttc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.hesvh.cn/Article/details/gwdofdwjj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.hesvh.cn/Article/details/geugsdsqx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.hesvh.cn/Article/details/glovdphrq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.hesvh.cn/Article/details/gxnzfuwsi.sHtML


<!-- 参考信息 -->