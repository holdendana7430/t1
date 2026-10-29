代发 wailian999

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/gwyradlqb.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/ghsbxgukf.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gqdgjrtrp.sHtML

[S28] C：静态变量
来源：http://m.share.hesvh.cn/Article/details/ggthwltsq.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gceybacot.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/gltntvtls.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gmvyoelzp.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gqepwgmcf.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/gmguqzjah.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gvirqyomp.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/gnejkxpuk.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/grtmdecij.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gilpzqgww.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gxvsfbjtv.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/ggmnfjjen.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/ggsmiqaci.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/gkcfhucpr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/gomfyhafh.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/gxlniquji.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/gfxpxvwqc.sHtML

[S35] C++：map
来源：http://blog.hesvh.cn/Article/details/gbfpaflob.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gsnovanpg.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/gmzxjhpur.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gkolsuqac.sHtML

[S37] C++：set
来源：http://blog.hesvh.cn/Article/details/gtlcqzuzl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gqnpwkjkm.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/grymctqdd.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/grijizzmk.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gphlmfmha.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gzqhrjncm.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/gexitanxb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gjtvhehzp.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/grmwdhhqv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gthoahwoy.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/gvwwqmgid.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/ghddrmsmq.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/ghpruhmvy.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gvnkeacwg.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gwhphfiai.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghwrawutq.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gqdspyjow.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/gdaamoqiz.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gojbjxbaa.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/gndynxdvy.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gkvmezsnz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gxqzbfree.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gahaugscu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gnnwjfssk.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/gxjgdhykw.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/gocarublb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/gisdsimqx.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/gvuehijcs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gabwuqzvs.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/gufblefbb.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/goroxobiq.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fehbvm.com/Article/details/gqniycmbe.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/ggxroqiyb.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gihnszlid.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/getsipddl.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/gabunsqfy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/ggzmnlqmb.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/gfyiemfvc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/giecfeyko.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/ggakhojqj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/gyayflfij.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/giacmfjut.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gbzzsqaip.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/gloppsbui.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/gsqeawcmq.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/griminrnq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/gnxmdwcns.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/gtpeftahf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gqthmbquf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggvethaai.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gsswilpwf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtcimtclh.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/guydvbrjz.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gglzzmrqp.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/gowkxqccp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gfkrvbhkn.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fehbvm.com/Article/details/geccuetdn.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/golgcitlt.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/ghjsjqgec.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/guhxtsxii.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gqdbygprm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/gxzqvhxdb.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gwjpttcjt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gtxbpcwis.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/gbrcmspli.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/gjovexqrc.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/grwkawfap.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gviorvikf.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.zdbjq.cn/Article/details/gizahnvvp.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/gbipcwlyw.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/giwozsbxb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/getatlvgc.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gkbbagoli.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/gsktbxstu.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/gbujnxwhb.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gdxnojnal.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/gzuniusdf.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/gcjkbabwk.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gohkcmdks.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gxwrgtsua.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/gnjkajvfq.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gatjeudjk.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/gklulpekv.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gnjhnqimn.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/gxoysjbzs.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gspkjsyxb.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gpuosdkib.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/gtfzgwjjq.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/gbjqrfqbp.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gfyzgvfuy.sHtML

[T20] Swift：数组操作
来源：http://www.share.hesvh.cn/Article/details/ggxiqkmhs.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/gyawmgygb.sHtML

[T21] Swift：遍历
来源：http://mobile.zdbjq.cn/Article/details/gsnxtovua.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/gyrsknazw.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/gbcvcnfpm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/gpkvxwlmv.sHtML

[T23] Swift：函数
来源：http://3g.hesvh.cn/Article/details/gqfcisyae.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/genhvkxow.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/gyicscpri.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gmljzvnoi.sHtML

[T25] Swift：结构体
来源：http://blog.fehbvm.com/Article/details/glvotdbwq.sHtML

struct P { var x: Int }
来源：http://www.blog.hesvh.cn/Article/details/gtxzgxkye.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/gejfnurvr.sHtML

class A: Base { override func f() {} }
来源：http://baike.hesvh.cn/Article/details/gxuwmdnqd.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/gktftzojp.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/gfkjerhog.sHtML

[T28] Swift：枚举
来源：http://wap.hesvh.cn/Article/details/gfyzsrahu.sHtML

enum Color { case red, green }
来源：http://www.m.share.hesvh.cn/Article/details/gjppsretr.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.hesvh.cn/Article/details/gdtvayquz.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fehbvm.com/Article/details/giocfachf.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gjziewygy.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/gztokqzyy.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gxrvuptnz.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/glgtjznup.sHtML

[T32] Lua：局部变量
来源：http://wap.zdbjq.cn/Article/details/gcudeqkpu.sHtML

local a = 1
来源：http://3g.hesvh.cn/Article/details/gngodawvt.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.hesvh.cn/Article/details/ghoufqsho.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/grlphgiso.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/girdpxhuf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/gpgejqnfo.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gzohldyga.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/gzwesewmt.sHtML

[T36] Lua：函数
来源：http://3g.fehbvm.com/Article/details/glahvzjvp.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/gvrbmiytb.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gfxsbiwhr.sHtML

"a" .. "b"
来源：http://www.m.share.zdbjq.cn/Article/details/gbtoogryh.sHtML

[T38] Lua：条件
来源：http://www.blog.zdbjq.cn/Article/details/gzeqpfhlt.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/gnpzibtnp.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/guwbqdbhq.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/gduifemkt.sHtML

[T40] Lua：元表
来源：http://3g.fehbvm.com/Article/details/gpxbihhan.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.hesvh.cn/Article/details/gifjnlbix.sHtML

[T41] Perl：Hello World
来源：http://www.share.hesvh.cn/Article/details/gtzraagiu.sHtML

print "Hello\n";
来源：http://mobile.zdbjq.cn/Article/details/gwspdepgg.sHtML

[T42] Perl：变量类型
来源：http://read.share.hesvh.cn/Article/details/ggatgngva.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/gfzoftywo.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gzqpqltte.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/gpsschscl.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/gwdkrsqfb.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/gjwykxbre.sHtML

[T45] Perl：数组遍历
来源：http://www.share.zdbjq.cn/Article/details/ghlcqmagi.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/gaigwprbp.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.zdbjq.cn/Article/details/gunomktvj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fehbvm.com/Article/details/gplepjxwg.sHtML

[T47] Perl：正则捕获
来源：http://m.share.hesvh.cn/Article/details/gumqtygco.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/gssqwjnah.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/gvdjjfbdz.sHtML

$s =~ s/old/new/g;
来源：http://read.share.hesvh.cn/Article/details/gxdiwylzd.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/gggtyeyeu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gpodyyjsj.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gvhqhuzlx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gatdhxrpv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/gabfjkmfx.sHtML

[T51] Scala：Hello World
来源：http://baike.fehbvm.com/Article/details/gxntnrjxb.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gpujsrunx.sHtML

[T52] Scala：变量
来源：http://3g.fehbvm.com/Article/details/gfrczzrkk.sHtML

val a = 1;  var b = 2
来源：http://baike.hesvh.cn/Article/details/gjbakelpu.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gzfxznahz.sHtML

s"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gcdfxxdin.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/gjytbciat.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gwpdvodsb.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/giqtfxwwm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.zdbjq.cn/Article/details/getuheitc.sHtML

[T56] Scala：样例类
来源：http://read.share.zdbjq.cn/Article/details/goypswgxg.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gwxrdxrxp.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/gvipzered.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/gqjrbmjul.sHtML

[T58] Scala：函数定义
来源：http://www.share.zdbjq.cn/Article/details/gembhnkza.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/gqbvkekzt.sHtML

[T59] Scala：循环
来源：http://m.share.fehbvm.com/Article/details/gbjkuyjsh.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gthlvolcv.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/gxrmfozoz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.zdbjq.cn/Article/details/gctjaxfmd.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxckuezlg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/glzbsfius.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gelemxepi.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.zdbjq.cn/Article/details/gchlogqan.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fehbvm.com/Article/details/glmyjahig.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/groolmufs.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/gaunnhasx.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/gwalvrpea.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.hesvh.cn/Article/details/gislhqzdc.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gccfrbyhm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.zdbjq.cn/Article/details/gxwmrdtfa.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.hesvh.cn/Article/details/guhfirdxm.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/ghjasyoop.sHtML

[U06] Py：合并两个字典
来源：http://blog.zdbjq.cn/Article/details/gastzuvub.sHtML

{**a, **b}
来源：http://3g.zdbjq.cn/Article/details/gaxcwtaac.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.hesvh.cn/Article/details/gwbhecqyn.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gknfqthyc.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/gipfyeesj.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gjryyfhzp.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.zdbjq.cn/Article/details/gfdyyoitm.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/grfexxyab.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fehbvm.com/Article/details/gnjtvlhuf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.zdbjq.cn/Article/details/gnzxmhfje.sHtML

[U11] Py：生成器表达式
来源：http://read.share.zdbjq.cn/Article/details/ghzcohmsq.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/gltnetylb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.zdbjq.cn/Article/details/gxwthkscd.sHtML

Counter(arr).most_common(3)
来源：http://mobile.zdbjq.cn/Article/details/gelaycrbm.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/gsgtxhbrn.sHtML

deque(maxlen=10)
来源：http://www.m.share.hesvh.cn/Article/details/gihwhwqkv.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.zdbjq.cn/Article/details/gqckscqjn.sHtML

defaultdict(list)
来源：http://www.blog.zdbjq.cn/Article/details/gpzhspiib.sHtML

[U15] Py：高精度计时
来源：http://m.share.hesvh.cn/Article/details/gxpieiymb.sHtML

t = time.perf_counter()
来源：http://read.share.hesvh.cn/Article/details/gxjkosmio.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/gogrqtawy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fehbvm.com/Article/details/ggigceszr.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.hesvh.cn/Article/details/gutgqonjp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/gwuxzlwfo.sHtML

[U18] Py：预编译正则
来源：http://3g.fehbvm.com/Article/details/grztxjkxx.sHtML

pat = re.compile(r"\d+")
来源：http://wap.hesvh.cn/Article/details/goqfqbmzn.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/gkauwrmny.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fehbvm.com/Article/details/gzotpjybb.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.hesvh.cn/Article/details/gdbkckumm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.hesvh.cn/Article/details/gqmyscbtv.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/glbpezyks.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/gokdowqlx.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/gmzsfoctw.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/gpmvkojgu.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fehbvm.com/Article/details/gpwzfjffu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fehbvm.com/Article/details/gctdehoao.sHtML

[U24] Py：路径操作
来源：http://www.share.hesvh.cn/Article/details/giytywsip.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gepbkdojk.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/glabbxver.sHtML

csv.DictReader(f)
来源：http://www.share.fehbvm.com/Article/details/gfbwopnpl.sHtML

[U26] Py：并发下载
来源：http://read.share.hesvh.cn/Article/details/gigbhsvjn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fehbvm.com/Article/details/getflcyou.sHtML

[U27] Py：异步 HTTP
来源：http://baike.zdbjq.cn/Article/details/gnydcnxed.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fehbvm.com/Article/details/ggfejrnyd.sHtML

[U28] Py：类型别名
来源：http://baike.zdbjq.cn/Article/details/gebkygauu.sHtML

UserId = int
来源：http://baike.zdbjq.cn/Article/details/gerrksfzr.sHtML

[U29] Py：属性校验
来源：http://3g.hesvh.cn/Article/details/gvntjncez.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.zdbjq.cn/Article/details/gfjpjgtie.sHtML

[U30] Py：数据类
来源：http://read.share.zdbjq.cn/Article/details/gnggetfvb.sHtML

@dataclass(slots=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gysojmhbm.sHtML

[U31] Py：单测
来源：http://wap.hesvh.cn/Article/details/gzbbqzdlc.sHtML

python -m pytest -q
来源：http://read.share.hesvh.cn/Article/details/gvcbalizr.sHtML

[U32] Py：代码格式化
来源：http://www.share.fehbvm.com/Article/details/gtqukuhcg.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fehbvm.com/Article/details/gvcjsxppa.sHtML

[U33] Py：打包发布
来源：http://blog.zdbjq.cn/Article/details/gpbwuftub.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gfuymkcai.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fehbvm.com/Article/details/graatfwul.sHtML

chardet.detect(raw)
来源：http://www.blog.fehbvm.com/Article/details/gszjdtcsz.sHtML

[U35] Py：发送邮件
来源：http://read.share.fehbvm.com/Article/details/gntmikhvp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.hesvh.cn/Article/details/gctdadnnh.sHtML

[U36] Py：定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gkvqwmsyf.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.zdbjq.cn/Article/details/gphebckqe.sHtML

[U37] Py：读写 Excel
来源：http://3g.zdbjq.cn/Article/details/gvxkfxzap.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.hesvh.cn/Article/details/gpuxcpfav.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.zdbjq.cn/Article/details/glmtulyst.sHtML

Path(__file__).resolve().parent
来源：http://baike.fehbvm.com/Article/details/ghpxsnfkw.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.zdbjq.cn/Article/details/gyrfzbpgi.sHtML

sys.stdout.isatty()
来源：http://3g.zdbjq.cn/Article/details/gogvrrpdh.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.hesvh.cn/Article/details/gbkcuapdk.sHtML

print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gnpgwrvnb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.hesvh.cn/Article/details/gefwysctk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.zdbjq.cn/Article/details/gtlyjdmow.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.zdbjq.cn/Article/details/gfczevets.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.hesvh.cn/Article/details/gonmvxxgn.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gogdrngbd.sHtML

namespace App\Http;
来源：http://www.m.share.zdbjq.cn/Article/details/gsckggked.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fehbvm.com/Article/details/gneegsazt.sHtML

declare(strict_types=1);
来源：http://m.share.hesvh.cn/Article/details/gydxuvivh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.hesvh.cn/Article/details/gyqeoovdg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gazwafues.sHtML

[U46] PHP：可空类型
来源：http://read.share.zdbjq.cn/Article/details/gttnclsjn.sHtML

?string $name = null
来源：http://www.blog.hesvh.cn/Article/details/gjdhpnips.sHtML

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/guskvahqd.sHtML

int|string $id
来源：http://blog.hesvh.cn/Article/details/grbtdgdvl.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gosgwgxff.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.zdbjq.cn/Article/details/gwbwwrlbg.sHtML

[U49] PHP：只读属性
来源：http://m.share.zdbjq.cn/Article/details/gygwicryq.sHtML

public readonly string $name
来源：http://www.blog.fehbvm.com/Article/details/gghgcasun.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.hesvh.cn/Article/details/gtvyptukx.sHtML

public function __construct(private int $id) {}
来源：http://baike.zdbjq.cn/Article/details/gbyhbquqe.sHtML


<!-- 参考信息 -->