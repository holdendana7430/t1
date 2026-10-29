代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/guzbaxjpl.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gzkmhttlu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/glmjjsqwb.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/gsxxtvpxn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gdwlofoni.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gnjhrfoue.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/ggkmvzmjk.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gikbdsjbh.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/goisvfoqk.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gyrahxtmd.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/ghwsacvmz.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/gxjlwxfez.sHtML

static int counter = 0;
来源：http://mobile.hesvh.cn/Article/details/gyuzbiezb.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/guhmjjbae.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/gkxelbdsz.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/gjkjcazap.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/givivembb.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gyabkxcwu.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/gybqylreh.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gluvmlzhs.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gbwshqcpv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/gjvagfoms.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gxgjfwvex.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gfveqfccw.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/gaxicqhdd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/gkjiunutg.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fehbvm.com/Article/details/gcahueiia.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/glwiqqawy.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gfzoidcyv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gihqplsvg.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/gdzuupsow.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gowhjhcao.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/gjpxtdwot.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/gergqunik.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gnxifevxo.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/gfvckvmeq.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/gdpbrizyp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/gzvtkugkg.sHtML

[S40] C++：查找元素
来源：http://www.blog.fehbvm.com/Article/details/gwhwevpmz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/grdezqfke.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/grnlquwgo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gxywjpuyb.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/gpdvwldzc.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gkeulfkxz.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/gfzcuwkhx.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.hesvh.cn/Article/details/gmacbkeke.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/glwuriflq.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gviywklio.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/ggqxjgdeu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gppfzldex.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gmtpunuqd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/grshiuqzz.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/glpnavsfv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/gopmvkwed.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gytwbpuag.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gwqosfdnw.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/gxkldxubh.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/golxjngok.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gyfnxcgfa.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gnbeglohq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gvuevsmcl.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/gkcadyuim.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/ggcvrnctx.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gdkewodpd.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/gvynumtqk.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/gxtgtivyk.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gmflqlcqz.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/gwhvjtgea.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gaisgssvr.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/geiovdkjf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.zdbjq.cn/Article/details/gijxdbrga.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gvcdvcchk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gywdlroxr.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/geutnkbht.sHtML

constexpr int N = 10;
来源：http://m.share.fehbvm.com/Article/details/gjussitxz.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/gyqgotufp.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/gnreyxydn.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/goqwmcwhp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gehbdlfje.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/gsijrauzi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/gfnevxocy.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbyngywiu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gwjvqjxfs.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gillyvvfq.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/gaffmtnmi.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gnibhdxwj.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.hesvh.cn/Article/details/gvuxnhofh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gfrltabcj.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fehbvm.com/Article/details/gxhvliggm.sHtML

"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gfjyefyiy.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/grhjjvxzm.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/guruzipum.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/ggvzxwvgm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gvttoozat.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/geljahpga.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gloeoctmf.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gvsmsayiy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/ggjbltlap.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/gxxezbykk.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/gtpqoztlw.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gnepftwhb.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/gepgvgdlq.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gclqbbfsy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/gmvhrfcnd.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/glscdrzbi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/gjwogqdtb.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/gxovkkacz.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gvklawkhm.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gggzsgqzm.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/glwnynmhu.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/gqhatbmcc.sHtML

for (i in 1..10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gjykruehn.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/gdtiodgtd.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/goqcnkasb.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/gzlbsexhs.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/glugojfeo.sHtML

[T17] Swift：变量与常量
来源：http://m.share.hesvh.cn/Article/details/gsqgfuubv.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/grzmjxska.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gqzlefeqf.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/ggjtujskg.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gckrzryyx.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gtmfcefto.sHtML

[T20] Swift：数组操作
来源：http://baike.zdbjq.cn/Article/details/gczljswja.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/gkrzfefst.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/gccnxyubn.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gjxsjznxu.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/glsbkeaxv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.zdbjq.cn/Article/details/gpeeuacmf.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gmdpyqexj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fehbvm.com/Article/details/gqmtxzcur.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/gyoqrwedv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/gxndvzwbg.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/ghdtbnftq.sHtML

struct P { var x: Int }
来源：http://blog.zdbjq.cn/Article/details/ghgrolgbd.sHtML

[T26] Swift：类与重写
来源：http://www.blog.hesvh.cn/Article/details/gresybbrd.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gaqnzzvcr.sHtML

[T27] Swift：错误处理
来源：http://mobile.fehbvm.com/Article/details/gvfvmdxlq.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fehbvm.com/Article/details/giiqgjdhr.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/gwsaqkvkt.sHtML

enum Color { case red, green }
来源：http://wap.zdbjq.cn/Article/details/glhzsgrgf.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gdrmjwtek.sHtML

guard let x = opt else { return }
来源：http://baike.fehbvm.com/Article/details/grgcsmqyo.sHtML

[T30] Swift：协议
来源：http://blog.zdbjq.cn/Article/details/gvpluvfvu.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/gqjitbrwd.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/guvsuquuh.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gfevyttoe.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/gzyxrkskn.sHtML

local a = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gaoxifukz.sHtML

[T33] Lua：表（数组）
来源：http://m.share.hesvh.cn/Article/details/gpmgxrknz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/gnulosuzq.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/gkyspyixj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gatohjxza.sHtML

[T35] Lua：字典表
来源：http://blog.fehbvm.com/Article/details/gvzkcgudj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.zdbjq.cn/Article/details/givpznhfn.sHtML

[T36] Lua：函数
来源：http://www.share.hesvh.cn/Article/details/gfzchastx.sHtML

function add(a, b) return a + b end
来源：http://wap.zdbjq.cn/Article/details/glcxeomjr.sHtML

[T37] Lua：字符串拼接
来源：http://wap.hesvh.cn/Article/details/gnglrcwry.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/gmtdaspsr.sHtML

[T38] Lua：条件
来源：http://mobile.zdbjq.cn/Article/details/gsmzaghck.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/gawyoebrc.sHtML

[T39] Lua：模式匹配
来源：http://baike.fehbvm.com/Article/details/gprwsldeu.sHtML

string.find(s, "%d+")
来源：http://mobile.hesvh.cn/Article/details/gdfwjqebs.sHtML

[T40] Lua：元表
来源：http://www.blog.hesvh.cn/Article/details/gzwnnnlon.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.hesvh.cn/Article/details/gaifuffiq.sHtML

[T41] Perl：Hello World
来源：http://3g.hesvh.cn/Article/details/gxviymnzm.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/gvulmtpyo.sHtML

[T42] Perl：变量类型
来源：http://wap.hesvh.cn/Article/details/glmhtwnvl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/gkpjowkvm.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gcpqhsbyt.sHtML

"值: $a"
来源：http://www.m.share.zdbjq.cn/Article/details/gytybasbe.sHtML

[T44] Perl：条件
来源：http://3g.hesvh.cn/Article/details/gulavtjlk.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/guizzpyky.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.zdbjq.cn/Article/details/gzaicqcgq.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/gdquydxgg.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/golutnhtk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fehbvm.com/Article/details/gnhzqyjxa.sHtML

[T47] Perl：正则捕获
来源：http://baike.hesvh.cn/Article/details/ghkxofkqm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/guywtidew.sHtML

[T48] Perl：正则替换
来源：http://www.blog.zdbjq.cn/Article/details/ggmujfhxl.sHtML

$s =~ s/old/new/g;
来源：http://blog.hesvh.cn/Article/details/gbuunvjbv.sHtML

[T49] Perl：函数
来源：http://wap.fehbvm.com/Article/details/gsgidrdxx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gbzafuzun.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gsleoysak.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.hesvh.cn/Article/details/gzykycvep.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.zdbjq.cn/Article/details/ggmsnsqnl.sHtML

[T51] Scala：Hello World
来源：http://mobile.hesvh.cn/Article/details/gaognkiqo.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gvoyvfgaa.sHtML

[T52] Scala：变量
来源：http://www.share.hesvh.cn/Article/details/gugahqfdw.sHtML

val a = 1;  var b = 2
来源：http://www.share.zdbjq.cn/Article/details/gmjedcvqd.sHtML

[T53] Scala：字符串插值
来源：http://3g.hesvh.cn/Article/details/gtbjykmdf.sHtML

s"值: $b"
来源：http://wap.fehbvm.com/Article/details/gfrwgprvb.sHtML

[T54] Scala：集合映射
来源：http://3g.fehbvm.com/Article/details/glhvupdat.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/gaxdyunit.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/glzckahlo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.zdbjq.cn/Article/details/gqfvsflhk.sHtML

[T56] Scala：样例类
来源：http://mobile.fehbvm.com/Article/details/gypbzbbtj.sHtML

case class User(name: String, age: Int)
来源：http://wap.zdbjq.cn/Article/details/gdlxcwvdm.sHtML

[T57] Scala：模式匹配
来源：http://wap.hesvh.cn/Article/details/gzixudjtl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/gtwtazoug.sHtML

[T58] Scala：函数定义
来源：http://m.share.zdbjq.cn/Article/details/guwssygsv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gxudxkbzn.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/gbfvuffrn.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gsyrmgvyt.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/gokidenli.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fehbvm.com/Article/details/gpyrfmjew.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gselkbfee.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gdcvgmmnz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtplqlrgp.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.zdbjq.cn/Article/details/gtplxbrhv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fehbvm.com/Article/details/gmnnwyyjn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/ggsgwuqlf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.zdbjq.cn/Article/details/gdffcjpxt.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fehbvm.com/Article/details/ghvmsmcdh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.zdbjq.cn/Article/details/gyfxbrveo.sHtML

[U04] Py：变量调试打印
来源：http://wap.hesvh.cn/Article/details/ghwwnqvua.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.hesvh.cn/Article/details/gwjvsamis.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/gvcbdijyw.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gpzcqdqig.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/gueiueqwu.sHtML

{**a, **b}
来源：http://blog.hesvh.cn/Article/details/gdmnhisvo.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/gqghkoqpm.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/gdotqzsvs.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fehbvm.com/Article/details/gzbllhzyu.sHtML

[y for x in nested for y in x]
来源：http://blog.hesvh.cn/Article/details/gdgcbovlx.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fehbvm.com/Article/details/gxmmdmmex.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/gkpabedwe.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fehbvm.com/Article/details/gkqvzozln.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/gsicudtdn.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/grdqtenmk.sHtML

(x * 2 for x in arr)
来源：http://3g.fehbvm.com/Article/details/gdmilajpc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fehbvm.com/Article/details/gbfhcpakg.sHtML

Counter(arr).most_common(3)
来源：http://blog.zdbjq.cn/Article/details/gbopdgpsu.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/gubaxotrr.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/gakaegafs.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.zdbjq.cn/Article/details/gysgwsnah.sHtML

defaultdict(list)
来源：http://baike.fehbvm.com/Article/details/gxvlzmyhy.sHtML

[U15] Py：高精度计时
来源：http://read.share.zdbjq.cn/Article/details/gioyrnifh.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/gcetggajl.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fehbvm.com/Article/details/ggmvtxjcz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fehbvm.com/Article/details/gehhvqwhz.sHtML

[U17] Py：初始化日志
来源：http://www.blog.zdbjq.cn/Article/details/gunytcdsr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.zdbjq.cn/Article/details/gcuxysajt.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/gdcuwpisu.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gmwjgytsa.sHtML

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/guswguxhk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.hesvh.cn/Article/details/gortiwmgr.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fehbvm.com/Article/details/ghcvzbteh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fehbvm.com/Article/details/gpnfmdmeg.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.hesvh.cn/Article/details/gawerpzkh.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/gdqtqzifx.sHtML

[U22] Py：矩阵转置
来源：http://baike.fehbvm.com/Article/details/gfhezorda.sHtML

list(zip(*m))
来源：http://baike.hesvh.cn/Article/details/guwqeiuye.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.hesvh.cn/Article/details/gsbmmhyjn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/gihsjroiq.sHtML

[U24] Py：路径操作
来源：http://www.share.zdbjq.cn/Article/details/gpakwacue.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gbmtyinbu.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.hesvh.cn/Article/details/gnfmwnpoe.sHtML

csv.DictReader(f)
来源：http://wap.zdbjq.cn/Article/details/gltqflnni.sHtML

[U26] Py：并发下载
来源：http://wap.zdbjq.cn/Article/details/gttvasqou.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fehbvm.com/Article/details/gshuyrifu.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.zdbjq.cn/Article/details/guikpzjfm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fehbvm.com/Article/details/getmnrqjz.sHtML

[U28] Py：类型别名
来源：http://www.m.share.hesvh.cn/Article/details/gildwuskf.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/giwxhshgk.sHtML

[U29] Py：属性校验
来源：http://read.share.fehbvm.com/Article/details/gvcwnlqxm.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/grfuilppb.sHtML

[U30] Py：数据类
来源：http://www.blog.hesvh.cn/Article/details/gfwkxnyup.sHtML

@dataclass(slots=True)
来源：http://www.share.zdbjq.cn/Article/details/glxvjzbig.sHtML

[U31] Py：单测
来源：http://blog.hesvh.cn/Article/details/gmidxgonj.sHtML

python -m pytest -q
来源：http://read.share.fehbvm.com/Article/details/gokvjtnbc.sHtML

[U32] Py：代码格式化
来源：http://www.share.fehbvm.com/Article/details/gvokvwxzr.sHtML

ruff format . && ruff check --fix .
来源：http://blog.zdbjq.cn/Article/details/gkxcnemxx.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/gcszucaew.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.hesvh.cn/Article/details/gblmlnqsr.sHtML

[U34] Py：判断编码
来源：http://blog.fehbvm.com/Article/details/gyhxrqtid.sHtML

chardet.detect(raw)
来源：http://www.blog.fehbvm.com/Article/details/gmtnkyjvh.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/gfdgckeez.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/gvwzyginc.sHtML

[U36] Py：定时任务
来源：http://www.m.share.hesvh.cn/Article/details/grgbrswsr.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.hesvh.cn/Article/details/gykpwwgxw.sHtML

[U37] Py：读写 Excel
来源：http://3g.fehbvm.com/Article/details/gslkgyupc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.zdbjq.cn/Article/details/gwncfntyh.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fehbvm.com/Article/details/ghrbssgtq.sHtML

Path(__file__).resolve().parent
来源：http://3g.zdbjq.cn/Article/details/gwxecvpbu.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.hesvh.cn/Article/details/gdxkyvqdc.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/gswrgdwqr.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/ginwbzwwx.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gqigcucpr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.hesvh.cn/Article/details/ggznmtmcz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/ggrobvjcr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.zdbjq.cn/Article/details/gzwabyxjb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.hesvh.cn/Article/details/gdinxorty.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.hesvh.cn/Article/details/gyffsnfls.sHtML

namespace App\Http;
来源：http://wap.fehbvm.com/Article/details/gmjjctcoy.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.zdbjq.cn/Article/details/grcpajkmi.sHtML

declare(strict_types=1);
来源：http://www.m.share.fehbvm.com/Article/details/gvktlmvry.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.hesvh.cn/Article/details/ghuvdgxwn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtnpdzoqd.sHtML

[U46] PHP：可空类型
来源：http://www.share.zdbjq.cn/Article/details/gunzakjxe.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/gsppyyihm.sHtML


<!-- 参考信息 -->