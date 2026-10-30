代发 wailian999

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gkbuhyaqd.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/gqrnkzgrh.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gozesgnox.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gaaqoyoyg.sHtML

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/glsvxwbva.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gbuaqvbdn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/gxhexspaw.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/gwbvkrqyp.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gwxcmnxbk.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gdawexcde.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/groxnmsjg.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gjeapfxzk.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/grhdnxwun.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/gdgduzlcb.sHtML

[S32] C++：字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gjwgelfrk.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gkunbqnyb.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gsvojbmce.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gyrrecpmo.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gmdkphtle.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gkdebpruc.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/ghjbacyrp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gtmhwouhn.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/gcdlcajpe.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gggzvllxt.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/ggvrzibuf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/gcnwfkhhr.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/gbgoishmr.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gkjxkmthh.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gpsawyonw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/gmjtyrfrf.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gxhbqcmky.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gkiedidut.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/gsehlrcnp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/gkbcfbdpp.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/gdmzuwjrf.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/gpdscpxiq.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gkeflkton.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/gszaifwfi.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/gaexnqbpu.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/genvjtaxf.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/giflailcd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gohrmhjmr.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gdvgbrcqj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gzkcbmhzv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gzfwhkdrd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gyupmlmrs.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/grzrovnxy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/gpjomqhqf.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/gzbqkopfy.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gavykwnli.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/ggtcofcdt.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/gyqccdplx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gqdfpbign.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/gthpkhdhl.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/geokzqxhn.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/gfddxymak.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/gqsjjwuah.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/gwkxhewzh.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fehbvm.com/Article/details/gtusizkjn.sHtML

[S54] C++：异常处理
来源：http://www.blog.hesvh.cn/Article/details/gpdzuzliq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/gjewmjtje.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/guvzcdhsx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gddnastnt.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/gbfzcfquo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gzcuyafyv.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/gdddfssct.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gyjyxblgk.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/gqgruwmhq.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/gqpjwvjzr.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gvrhvupdg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/gqwzbyqht.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gxiscwozo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gjfdzaitm.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmlhmiirt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gqefstefd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gohxytzrt.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gkcmutdwy.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/geccreaup.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gmdlvpwfp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gxadoignb.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gsefapfqw.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gcpdstjpi.sHtML

[T04] Kotlin：空安全
来源：http://baike.zdbjq.cn/Article/details/ghjhsurgk.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/gqqumaozr.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/gqwbazcqb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gzyneyyth.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/ghlaxmpwc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fehbvm.com/Article/details/gtblntfru.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gdavmhcud.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gzlfeakpm.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/glfdjshje.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/gutybubja.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/gcwldihni.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/gmajleruc.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gtbibflws.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fehbvm.com/Article/details/ghyulfttn.sHtML

[T11] Kotlin：协程
来源：http://blog.fehbvm.com/Article/details/gvoyytrkk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/gnubyagpe.sHtML

[T12] Kotlin：解构声明
来源：http://blog.zdbjq.cn/Article/details/grgnquesz.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gphexeqya.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/gxriwbzlp.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.zdbjq.cn/Article/details/ggqbtegjp.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gxsifymhq.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gbypecobn.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/gatyiugom.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/guthaovom.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/getlaszuz.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gblaygneo.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gvgcuqjae.sHtML

var a = 1;  let b = 2
来源：http://3g.zdbjq.cn/Article/details/guwwkjtcl.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/gsdqupquw.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/gixugvzjg.sHtML

[T19] Swift：可选绑定
来源：http://m.share.zdbjq.cn/Article/details/gkuidebzk.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/gqqtsobds.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/gevznhlli.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/gpkdcrkxo.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/gjctvhjct.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/gqcsholkp.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/gfflnveft.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/gyqqffsmf.sHtML

[T23] Swift：函数
来源：http://www.blog.hesvh.cn/Article/details/gojfadfxx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.hesvh.cn/Article/details/gbwyivlek.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/grgrzqbod.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gxdeznlwe.sHtML

[T25] Swift：结构体
来源：http://wap.zdbjq.cn/Article/details/ghsaaqkdq.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gflhcowml.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/gbpalpgzw.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.zdbjq.cn/Article/details/gibmhmkxt.sHtML

[T27] Swift：错误处理
来源：http://mobile.fehbvm.com/Article/details/giihtvpgy.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/gsnzqbiqz.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/gymubzykf.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/gslothezz.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/gncwrdxkh.sHtML

guard let x = opt else { return }
来源：http://www.blog.fehbvm.com/Article/details/ggxouwjvf.sHtML

[T30] Swift：协议
来源：http://www.share.fehbvm.com/Article/details/gcdcnjfgi.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fehbvm.com/Article/details/gvfrjmlib.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gaboqazpt.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gzpqqnhhw.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gukcsuhmd.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/guzpelsqw.sHtML

[T33] Lua：表（数组）
来源：http://blog.fehbvm.com/Article/details/gcosxxlys.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.hesvh.cn/Article/details/gozphxrrt.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/gkivxzxvp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fehbvm.com/Article/details/gmbsicdrb.sHtML

[T35] Lua：字典表
来源：http://www.share.fehbvm.com/Article/details/gtioqcwna.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.hesvh.cn/Article/details/gvfrsemxd.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/givczqfns.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/gbffzsngp.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gagbbeuso.sHtML

"a" .. "b"
来源：http://www.blog.hesvh.cn/Article/details/gwwipstjn.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/ggyukuopu.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.zdbjq.cn/Article/details/gzqdeorap.sHtML

[T39] Lua：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gsgfdrqhy.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/gjbvgkwvc.sHtML

[T40] Lua：元表
来源：http://www.share.zdbjq.cn/Article/details/gvsrumjrm.sHtML

setmetatable({}, { __index = base })
来源：http://blog.hesvh.cn/Article/details/gxfoqjfqi.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/gdeggiboy.sHtML

print "Hello\n";
来源：http://baike.hesvh.cn/Article/details/ghfmjuyxk.sHtML

[T42] Perl：变量类型
来源：http://m.share.hesvh.cn/Article/details/gscqucfgz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/giywdhbfa.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/ggfaykikc.sHtML

"值: $a"
来源：http://wap.zdbjq.cn/Article/details/ghqoxmxgm.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/gohlrboza.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gvbfdnrzw.sHtML

[T45] Perl：数组遍历
来源：http://blog.hesvh.cn/Article/details/gmcpbfqdj.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.zdbjq.cn/Article/details/glscrvvcb.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.zdbjq.cn/Article/details/gdlwhuxoa.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.hesvh.cn/Article/details/glsexljwb.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/guiknxuxp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/gonqwkwgp.sHtML

[T48] Perl：正则替换
来源：http://m.share.hesvh.cn/Article/details/gxtxtenya.sHtML

$s =~ s/old/new/g;
来源：http://wap.zdbjq.cn/Article/details/gikyjxduw.sHtML

[T49] Perl：函数
来源：http://www.blog.fehbvm.com/Article/details/gkralaxux.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gbdrfuyzs.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gdouyrfqx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/gdiwobdrh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/gjfkwchwq.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/goqjlpxis.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gjkjegmhv.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/gcjpoacmx.sHtML

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gbhdmmovn.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gaxemrbeh.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/gigthwate.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/gbvqxkwfz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/ghzfkyhxz.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gdyjwhcwl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fehbvm.com/Article/details/gzwbmsacd.sHtML

[T56] Scala：样例类
来源：http://blog.zdbjq.cn/Article/details/gtjmrphdz.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gllixcubc.sHtML

[T57] Scala：模式匹配
来源：http://3g.zdbjq.cn/Article/details/giwxkdhbw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/gjqhwnmed.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/gcdzvptba.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.zdbjq.cn/Article/details/ginlxmxqo.sHtML

[T59] Scala：循环
来源：http://m.share.fehbvm.com/Article/details/gfpomxanm.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/gcqfevymq.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/gvkzmvrtm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.zdbjq.cn/Article/details/gmncofrxk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvgmztyke.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gbvejrxpo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gybrsgofp.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/gezpsbfkp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.hesvh.cn/Article/details/gnvhxnpuw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.zdbjq.cn/Article/details/gokuidsxc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/gpceancak.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/gxdxgwpyd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/gjtrxjuwc.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fehbvm.com/Article/details/gwalpqiwq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fehbvm.com/Article/details/gjccxusam.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/gqllamudr.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gjbahylzk.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gxvdtsnlw.sHtML

{**a, **b}
来源：http://www.share.fehbvm.com/Article/details/gtgntwlhy.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fehbvm.com/Article/details/gswdrbhtk.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fehbvm.com/Article/details/gfzoknkre.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/gyyygcmkj.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gmtcqkshw.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.zdbjq.cn/Article/details/gxxmkagma.sHtML

max(d, key=d.get)
来源：http://www.blog.zdbjq.cn/Article/details/gkrzyzwuq.sHtML

[U10] Py：按值排序字典
来源：http://mobile.hesvh.cn/Article/details/gmfnpqods.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/gppzwlftn.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/gtzsrmiyv.sHtML

(x * 2 for x in arr)
来源：http://read.share.zdbjq.cn/Article/details/gkpcgzsto.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.hesvh.cn/Article/details/gbtzahzhq.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/gjnvxbnvn.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fehbvm.com/Article/details/gharsglag.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/grjnhotas.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fehbvm.com/Article/details/gfxioleey.sHtML

defaultdict(list)
来源：http://wap.hesvh.cn/Article/details/gnpnefqpf.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gjhzbbwrt.sHtML

t = time.perf_counter()
来源：http://3g.zdbjq.cn/Article/details/glenrlzrl.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.hesvh.cn/Article/details/gvkiefqop.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fehbvm.com/Article/details/ggnpjfcfm.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/glvaztcvj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gitrwvccw.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/gxlypvbym.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fehbvm.com/Article/details/gohguallt.sHtML

[U19] Py：正则替换带回调
来源：http://blog.hesvh.cn/Article/details/gavuelxkr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.hesvh.cn/Article/details/gsrjrsznp.sHtML

[U20] Py：缓存函数结果
来源：http://wap.zdbjq.cn/Article/details/gzpdlpdcr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/gtyajncsr.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.zdbjq.cn/Article/details/gnlyzimqj.sHtML

@contextlib.contextmanager
来源：http://m.share.fehbvm.com/Article/details/gdtymisix.sHtML

[U22] Py：矩阵转置
来源：http://m.share.zdbjq.cn/Article/details/gjgdvkqox.sHtML

list(zip(*m))
来源：http://baike.fehbvm.com/Article/details/gnvfxadzc.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.hesvh.cn/Article/details/ggxslmqyw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.zdbjq.cn/Article/details/gsrnwodtk.sHtML

[U24] Py：路径操作
来源：http://www.share.hesvh.cn/Article/details/gvylavffr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gazptubht.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/govzgzvnc.sHtML

csv.DictReader(f)
来源：http://read.share.fehbvm.com/Article/details/gvxotxypu.sHtML

[U26] Py：并发下载
来源：http://mobile.fehbvm.com/Article/details/gvxqjyjzo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.zdbjq.cn/Article/details/geccfouha.sHtML

[U27] Py：异步 HTTP
来源：http://3g.zdbjq.cn/Article/details/gosyycrro.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.zdbjq.cn/Article/details/gfqrespxy.sHtML

[U28] Py：类型别名
来源：http://blog.hesvh.cn/Article/details/gkjwxspba.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/gncfoqmwx.sHtML

[U29] Py：属性校验
来源：http://wap.hesvh.cn/Article/details/glbfwonaw.sHtML

@property 与 @x.setter 配合
来源：http://m.share.zdbjq.cn/Article/details/gcmwijifw.sHtML

[U30] Py：数据类
来源：http://blog.hesvh.cn/Article/details/gfesvjogg.sHtML

@dataclass(slots=True)
来源：http://wap.fehbvm.com/Article/details/gmtzktucn.sHtML

[U31] Py：单测
来源：http://www.blog.zdbjq.cn/Article/details/gtdrehbpw.sHtML

python -m pytest -q
来源：http://blog.zdbjq.cn/Article/details/gcegvngkh.sHtML

[U32] Py：代码格式化
来源：http://wap.fehbvm.com/Article/details/geuobbmmh.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.zdbjq.cn/Article/details/gizqyyadx.sHtML

[U33] Py：打包发布
来源：http://mobile.hesvh.cn/Article/details/gdqbfafsv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/gqpzomcgy.sHtML

[U34] Py：判断编码
来源：http://baike.fehbvm.com/Article/details/guiovzkrc.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/gssxgimub.sHtML

[U35] Py：发送邮件
来源：http://wap.hesvh.cn/Article/details/gmbpekwwj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fehbvm.com/Article/details/gavirwkrt.sHtML

[U36] Py：定时任务
来源：http://mobile.fehbvm.com/Article/details/ghfljnuwf.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.zdbjq.cn/Article/details/gvygzajhu.sHtML

[U37] Py：读写 Excel
来源：http://blog.hesvh.cn/Article/details/gsaxwjleg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.hesvh.cn/Article/details/givyoaeat.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.zdbjq.cn/Article/details/gysdsdobz.sHtML

Path(__file__).resolve().parent
来源：http://wap.hesvh.cn/Article/details/gpskuccge.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.zdbjq.cn/Article/details/gcilbdpzq.sHtML

sys.stdout.isatty()
来源：http://3g.fehbvm.com/Article/details/gxptjasqe.sHtML

[U40] Py：打印到标准错误
来源：http://blog.zdbjq.cn/Article/details/gwlrsfqwo.sHtML

print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/geysjcrlx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.zdbjq.cn/Article/details/gyllchhey.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.hesvh.cn/Article/details/gfwwgcgfj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fehbvm.com/Article/details/gbzzqzdgy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.zdbjq.cn/Article/details/ggxmttjhq.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.zdbjq.cn/Article/details/glaxlbyhv.sHtML

namespace App\Http;
来源：http://mobile.fehbvm.com/Article/details/gyxtvzzqo.sHtML

[U44] PHP：开启严格类型
来源：http://baike.hesvh.cn/Article/details/ghkqcaizg.sHtML

declare(strict_types=1);
来源：http://mobile.fehbvm.com/Article/details/gnynfzemv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.hesvh.cn/Article/details/gzgcrhaee.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/ghridtwbr.sHtML

[U46] PHP：可空类型
来源：http://blog.zdbjq.cn/Article/details/grdopwxak.sHtML

?string $name = null
来源：http://www.blog.fehbvm.com/Article/details/ggzcilvmr.sHtML

[U47] PHP：联合类型
来源：http://mobile.fehbvm.com/Article/details/glohzhgyi.sHtML

int|string $id
来源：http://blog.zdbjq.cn/Article/details/gzhcrndwi.sHtML

[U48] PHP：纯枚举
来源：http://read.share.hesvh.cn/Article/details/ggpseluql.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.hesvh.cn/Article/details/gjgzjgrga.sHtML

[U49] PHP：只读属性
来源：http://www.share.zdbjq.cn/Article/details/gxhdwywyc.sHtML

public readonly string $name
来源：http://3g.hesvh.cn/Article/details/gixltbmqe.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.hesvh.cn/Article/details/godimnlck.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.hesvh.cn/Article/details/goxcdqjml.sHtML


<!-- 参考信息 -->