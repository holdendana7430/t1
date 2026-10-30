代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gaxxgjzia.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gjjndpwuc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/geztfqaom.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/gvoryxper.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/gnbvewpjf.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/gkuzceqhi.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gsvldjfzw.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/ggpjxtcfh.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/gxnqbxmgz.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gakweywfr.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/ggfmtgbxv.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/gzerhztqo.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/gpstgxsix.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/gaeveubek.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/gvurhkjee.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/gjwesbial.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/greryokiz.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/grfphmkaj.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gutmafkij.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gzgqzlicd.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gmzyavqnm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/gljjaaeyt.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gisniidav.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/guwasbhbc.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/gdtcxtwjl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gnyzgkhrp.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/gqwscgxww.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.hesvh.cn/Article/details/gauuvqhbq.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gaimblcnq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gllqwndgm.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gvmlobfhy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gslfbrgdm.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gakxplwph.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/gjxrdckjb.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/gxndtoyiy.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/gsbytpjet.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/gbwpfbwut.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gaaxcndsi.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gfsiyhfpt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gjyxwgjsq.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/goeqkymaj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gadiwjzeo.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/gkfulfmmq.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/gbacqywia.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gsbkejpim.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.zdbjq.cn/Article/details/grubasyer.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/goecasgdm.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/gdsbketrd.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gctpcudab.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/gtwzrcryn.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/gmkwjdlmq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/ghnuovpnv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gddznaksx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/glewldlrf.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gobanjeka.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/gelrdqotp.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/gddcwhmvh.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/gecgfteoc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/guldzrdam.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gktjpeqgd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.hesvh.cn/Article/details/gllylgxjm.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gyasfkbzl.sHtML

static_cast<double>(a) / b
来源：http://m.share.zdbjq.cn/Article/details/gcxuderhe.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/gprnqosbm.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/gytxtxgqv.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/gqytphylo.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/gjwohxvse.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gfcxfocch.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gfykzijaw.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gqukfszym.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gktjkfcbo.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/gyrdganxv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.zdbjq.cn/Article/details/gvidepbct.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/gmdkxrlfr.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gtlmvtzxy.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gsgumhoez.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/guhiscecq.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gsmvjtpmm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/gmfllfsdo.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gmrtipzea.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gqtpvjrhr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpwofvzok.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/goduechje.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmqrrnvro.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gvqdyvkuw.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gvotpwebn.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/ggicfizwu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/greuepohk.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gmdppjisy.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/ghelvaaga.sHtML

[T04] Kotlin：空安全
来源：http://m.share.hesvh.cn/Article/details/gmkicccok.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/gpxerlzrf.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/ghhyrabnf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fehbvm.com/Article/details/glwoghxfl.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fehbvm.com/Article/details/gekuproje.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gicawqpkp.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/glwexlpcd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/goefebpqb.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/gujmztlmg.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/giifwfglb.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/gylhscxcg.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.zdbjq.cn/Article/details/gzbnsqsle.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/gnwnxfnyv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/godpvqvoi.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gvyghrjww.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/gdwtjndjo.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/gabubdeae.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gmkushlvd.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gxjfibhkq.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/gytxdlqwv.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/grasrxdpr.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gatbbrwqk.sHtML

[T15] Kotlin：接口
来源：http://www.share.fehbvm.com/Article/details/gkmzuacga.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gtcpnnzpp.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gzqrhdhlk.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/goafgescz.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/goqtlmjyx.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/genmwnvoy.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gwlxyyyod.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/gylpmuwpv.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/glpboqfac.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/gdppaiqxu.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/groerrrhk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/grlmkfiwu.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/genxdfrxi.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/golholscd.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/gddwahfmk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/gxanqefbl.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gobrxfxji.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.zdbjq.cn/Article/details/gcydzvqog.sHtML

[T24] Swift：闭包
来源：http://www.share.hesvh.cn/Article/details/gessfnzww.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gmbxrzmal.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/gnenfjfsc.sHtML

struct P { var x: Int }
来源：http://m.share.fehbvm.com/Article/details/gvqoqcdya.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gkiaarnui.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/gnovyuuco.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gfsmiwprc.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/gkyztefol.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gwbzefbpa.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/gvkuvjpqz.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/gybnyzsew.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/glyahbmsb.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/giwfeysdp.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gasiihflc.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/gorjjdldu.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gicudgqdn.sHtML

[T32] Lua：局部变量
来源：http://www.share.fehbvm.com/Article/details/ghbtudanw.sHtML

local a = 1
来源：http://blog.zdbjq.cn/Article/details/gxokutaso.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fehbvm.com/Article/details/gleddrtmj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.hesvh.cn/Article/details/gbegymhne.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/gowzcutdz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/gqxqarozy.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/goaeiyvea.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gkqbotdst.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/ghjxvjlma.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/gxgtezetf.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gccomfqtv.sHtML

"a" .. "b"
来源：http://3g.fehbvm.com/Article/details/gmnweowyn.sHtML

[T38] Lua：条件
来源：http://wap.zdbjq.cn/Article/details/gruolnlym.sHtML

if x > 0 then print("正") end
来源：http://mobile.zdbjq.cn/Article/details/glxaqjfiv.sHtML

[T39] Lua：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gqkzyovrd.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/giprreugg.sHtML

[T40] Lua：元表
来源：http://3g.zdbjq.cn/Article/details/gvrrtzxyc.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/gmxqsraaz.sHtML

[T41] Perl：Hello World
来源：http://3g.fehbvm.com/Article/details/gyocwoybv.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/gzwpcinpl.sHtML

[T42] Perl：变量类型
来源：http://wap.hesvh.cn/Article/details/gohmfghrw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.hesvh.cn/Article/details/ggeyosnxq.sHtML

[T43] Perl：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gpjhlkpmy.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/gflcwrayz.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/gdlqwrbkw.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/gnnmirmrg.sHtML

[T45] Perl：数组遍历
来源：http://baike.hesvh.cn/Article/details/gcekzaocp.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/gkahztvyo.sHtML

[T46] Perl：哈希操作
来源：http://wap.fehbvm.com/Article/details/gggyzmjsr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/gjohekqei.sHtML

[T47] Perl：正则捕获
来源：http://baike.hesvh.cn/Article/details/goviuxddw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.zdbjq.cn/Article/details/gowyrzorp.sHtML

[T48] Perl：正则替换
来源：http://www.blog.zdbjq.cn/Article/details/geqwvscrv.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/gzqwrmfxh.sHtML

[T49] Perl：函数
来源：http://www.m.share.fehbvm.com/Article/details/gkbydiwzz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/galjpcnif.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gjtvainga.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/gkiazzqwm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fehbvm.com/Article/details/gsrxuukxf.sHtML

[T51] Scala：Hello World
来源：http://mobile.fehbvm.com/Article/details/gubkpkwei.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gwhgrckht.sHtML

[T52] Scala：变量
来源：http://m.share.zdbjq.cn/Article/details/gonbtrygn.sHtML

val a = 1;  var b = 2
来源：http://baike.hesvh.cn/Article/details/gdpdtinft.sHtML

[T53] Scala：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gaalwhlip.sHtML

s"值: $b"
来源：http://mobile.hesvh.cn/Article/details/ggvvljlte.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/gpbfmothw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/gsvyxukde.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gfwliocjn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gmtxkkidm.sHtML

[T56] Scala：样例类
来源：http://3g.zdbjq.cn/Article/details/gyzcpehui.sHtML

case class User(name: String, age: Int)
来源：http://blog.zdbjq.cn/Article/details/gfdsslfhg.sHtML

[T57] Scala：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gzbqvqpqx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fehbvm.com/Article/details/gawzysuqf.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/gkwbbsalw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fehbvm.com/Article/details/gyiskqogg.sHtML

[T59] Scala：循环
来源：http://baike.hesvh.cn/Article/details/gazofhidf.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gqgobspvd.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/gkuycxsvp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fehbvm.com/Article/details/gnajzdbdm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwekprvsf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gywkxjyva.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glfxcrxro.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/gnhxobxwm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/ghsepclem.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.zdbjq.cn/Article/details/gnoddaymc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.zdbjq.cn/Article/details/gthjhmdwr.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/gyqpvoilq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/glsdyfltw.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.zdbjq.cn/Article/details/gpljgyuzn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fehbvm.com/Article/details/gpgelwmkl.sHtML

[U05] Py：列表去重且保序
来源：http://wap.hesvh.cn/Article/details/giiqjlynd.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gfnpedqja.sHtML

[U06] Py：合并两个字典
来源：http://www.share.hesvh.cn/Article/details/grffpddjx.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/gtbzkeqsf.sHtML

[U07] Py：反转字典键值
来源：http://3g.fehbvm.com/Article/details/gvhbrsuhj.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gmaiusbjg.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fehbvm.com/Article/details/gtuqovkoi.sHtML

[y for x in nested for y in x]
来源：http://www.blog.hesvh.cn/Article/details/gofdxgnvm.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.zdbjq.cn/Article/details/grwutoxqi.sHtML

max(d, key=d.get)
来源：http://m.share.zdbjq.cn/Article/details/gcjhedqpl.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fehbvm.com/Article/details/gxyrryfgc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.zdbjq.cn/Article/details/gjoxlzwek.sHtML

[U11] Py：生成器表达式
来源：http://wap.fehbvm.com/Article/details/grtokujts.sHtML

(x * 2 for x in arr)
来源：http://wap.zdbjq.cn/Article/details/gscxbvxxa.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/gqrajrwxd.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fehbvm.com/Article/details/gqkzrdham.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/gmvlxxihk.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/guulioiop.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fehbvm.com/Article/details/gejquxmwh.sHtML

defaultdict(list)
来源：http://blog.zdbjq.cn/Article/details/gjyeyiqhu.sHtML

[U15] Py：高精度计时
来源：http://wap.zdbjq.cn/Article/details/gzdtsbila.sHtML

t = time.perf_counter()
来源：http://wap.hesvh.cn/Article/details/ghgbtclzg.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fehbvm.com/Article/details/glwqrqvhy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fehbvm.com/Article/details/gtpxednfr.sHtML

[U17] Py：初始化日志
来源：http://mobile.fehbvm.com/Article/details/gnwuucals.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.zdbjq.cn/Article/details/ggzctrxuu.sHtML

[U18] Py：预编译正则
来源：http://read.share.zdbjq.cn/Article/details/gaxnnhfjj.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.hesvh.cn/Article/details/grzspxmwq.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/gyanhzblz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fehbvm.com/Article/details/gorqhqkse.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.hesvh.cn/Article/details/gueccpyzv.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.hesvh.cn/Article/details/grvraigrs.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.zdbjq.cn/Article/details/gsoauvjsl.sHtML

@contextlib.contextmanager
来源：http://mobile.fehbvm.com/Article/details/gfijzwkto.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fehbvm.com/Article/details/grbtgfxok.sHtML

list(zip(*m))
来源：http://read.share.hesvh.cn/Article/details/gcdcxxiwr.sHtML

[U23] Py：分块读取大文件
来源：http://blog.zdbjq.cn/Article/details/gkbdtlzob.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fehbvm.com/Article/details/gonweajcr.sHtML

[U24] Py：路径操作
来源：http://read.share.fehbvm.com/Article/details/giixawpqc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gxdbkbfew.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.hesvh.cn/Article/details/gnxnsotug.sHtML

csv.DictReader(f)
来源：http://baike.hesvh.cn/Article/details/gwtgxlylo.sHtML

[U26] Py：并发下载
来源：http://www.share.hesvh.cn/Article/details/gexklgtjt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.zdbjq.cn/Article/details/gfhekjbfa.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.zdbjq.cn/Article/details/gupddmnrz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.hesvh.cn/Article/details/gatripybl.sHtML

[U28] Py：类型别名
来源：http://baike.zdbjq.cn/Article/details/gjpyzvdsl.sHtML

UserId = int
来源：http://baike.fehbvm.com/Article/details/gptkjyvre.sHtML

[U29] Py：属性校验
来源：http://read.share.zdbjq.cn/Article/details/gpiqkroxe.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fehbvm.com/Article/details/gxawmxjht.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gnamruhsw.sHtML

@dataclass(slots=True)
来源：http://www.share.hesvh.cn/Article/details/ghygtyocu.sHtML

[U31] Py：单测
来源：http://www.blog.hesvh.cn/Article/details/gxuxnzvyf.sHtML

python -m pytest -q
来源：http://www.m.share.zdbjq.cn/Article/details/ghnssfqwd.sHtML

[U32] Py：代码格式化
来源：http://baike.zdbjq.cn/Article/details/gmaxkjgqo.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fehbvm.com/Article/details/gdhcanlho.sHtML

[U33] Py：打包发布
来源：http://blog.fehbvm.com/Article/details/gfdfcpwpq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.zdbjq.cn/Article/details/gbfecfbqs.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fehbvm.com/Article/details/grufvmjsm.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/guyzomahw.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fehbvm.com/Article/details/gdlhqcpqr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.zdbjq.cn/Article/details/gunrzodcs.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/gaavqbmwd.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.zdbjq.cn/Article/details/gpqohfrhj.sHtML

[U37] Py：读写 Excel
来源：http://www.share.zdbjq.cn/Article/details/gvowxgxex.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.hesvh.cn/Article/details/gdkxmxmqk.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fehbvm.com/Article/details/gsmsvgunf.sHtML

Path(__file__).resolve().parent
来源：http://www.share.hesvh.cn/Article/details/gxidvrhlf.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.hesvh.cn/Article/details/gzxevzbkd.sHtML

sys.stdout.isatty()
来源：http://read.share.zdbjq.cn/Article/details/gstuvurea.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fehbvm.com/Article/details/gzkyafhzp.sHtML

print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gdsxltapy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.hesvh.cn/Article/details/gopsxlkob.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fehbvm.com/Article/details/gpxumglnh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/ggdgvlxgu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fehbvm.com/Article/details/goyrcvhus.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fehbvm.com/Article/details/gxlrnrzab.sHtML

namespace App\Http;
来源：http://m.share.hesvh.cn/Article/details/ghmmupuvi.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.zdbjq.cn/Article/details/ghdfvtqsd.sHtML

declare(strict_types=1);
来源：http://mobile.zdbjq.cn/Article/details/gmhziywtk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.zdbjq.cn/Article/details/grcdkubih.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gqtssarxq.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.zdbjq.cn/Article/details/gryqcvlxj.sHtML

?string $name = null
来源：http://baike.hesvh.cn/Article/details/gxhxgsabq.sHtML


<!-- 参考信息 -->