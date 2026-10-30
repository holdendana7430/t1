代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/ginoovsbf.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/ghayuyzuf.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/gavgiolzf.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gotoicwle.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/gleohwtcs.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gdinzubjq.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/geoezwtqq.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/gbkpqdpil.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/guzfyjdfm.sHtML

[S29] C：变参函数
来源：http://mobile.hesvh.cn/Article/details/gancpaaqz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gomnrzeic.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/gwgkeivzu.sHtML

#ifndef X_H
来源：http://3g.hesvh.cn/Article/details/gymhxmums.sHtML

#define X_H
来源：http://mobile.zdbjq.cn/Article/details/gnrepjrou.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gvaiqcwer.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gutgxhchg.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/granqeair.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gegczfamt.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/grmonhaeo.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/ggkmoeojn.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/grjugbvnm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/gytqcmfuh.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/gtiwtkgmt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/gbqtaduun.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gmdlbpkfb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/ggglmceas.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gzcoswykd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gsscbiwnj.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gczgzgsxv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/ghrixynif.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gtkvxuhba.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/gdjpfmsae.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gsxhhoojz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/gfzrgepwr.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gyagenqqy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/giuizphfw.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/grzckvzeh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/goeposknk.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/gbrahssev.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/gfogdxljc.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/gnlpqdode.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.hesvh.cn/Article/details/gjjwtbykv.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/ggwldpise.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gqocgbtfi.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gpmotudpz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/gwtlqyend.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gcnixxduu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/gcbrqrxtw.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gvmlephax.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gtmxlkswm.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gongtapwv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/geajrrzyz.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gpucyggtn.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/gquumbklo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gwsglqfez.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/gajnmvnmc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gcdnohevs.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/goxeiojyj.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/gdvpniqna.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gxnpbexgg.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gcvflcbwo.sHtML

[S53] C++：移动语义
来源：http://www.share.hesvh.cn/Article/details/gpxfhojaw.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/ghnljjadt.sHtML

[S54] C++：异常处理
来源：http://wap.hesvh.cn/Article/details/gfwnquljd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/gsgwwuhtl.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/gvexyrkgg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gwwotuker.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gzrhhtxvv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/gfthwyosq.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/gduqqfugi.sHtML

constexpr int N = 10;
来源：http://baike.fehbvm.com/Article/details/gmxshsrjb.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/grvypsoex.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gklhiqtjd.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/gryelcoxa.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gtixifths.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/gaeidqcdz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gvrbvpgoy.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtgkeggld.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gazdlkeqw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gysupicqs.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gmsxzvkut.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gsezrvpqp.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/ggbemmmxv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/gdzbazyil.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gwcqwyfxj.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gwcphghsc.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gexcgrwqx.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.hesvh.cn/Article/details/gdwmjqprk.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gaiszbqdu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/ghpdgmtfo.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gldjiqack.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gdvmiyked.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gqjzbmgjy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gatannnoi.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/ghrbznzjj.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gefbjxapy.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/guobisywn.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/ghbatnuvs.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/girowvlkg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/glzswrzsr.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/gmmxigzcw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/gsbuqogbd.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gphggakek.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gqxhktgjw.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gpfrwndjm.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/gsgoryzty.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gbrmvijhq.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gnyoujjlj.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/gghpivwbb.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/glolvrvjh.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gteteegnp.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gzeeeeaci.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/gtmdvlxqf.sHtML

var a = 1;  let b = 2
来源：http://www.share.hesvh.cn/Article/details/gqrhgrikr.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gaidbbkhj.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/gjakyeqmu.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/gmrndkeui.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/gjletdfir.sHtML

[T20] Swift：数组操作
来源：http://www.share.fehbvm.com/Article/details/gdukfptwi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/gpcwelggw.sHtML

[T21] Swift：遍历
来源：http://baike.hesvh.cn/Article/details/gplbhbfjw.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/gkztnojwh.sHtML

[T22] Swift：字典
来源：http://www.blog.hesvh.cn/Article/details/gpztmhwll.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.zdbjq.cn/Article/details/gzayjfzcq.sHtML

[T23] Swift：函数
来源：http://www.blog.hesvh.cn/Article/details/gmdqssfqn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.hesvh.cn/Article/details/guwligrwa.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/gkjkqtqyb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.hesvh.cn/Article/details/gwucxamch.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/grnsqdhuh.sHtML

struct P { var x: Int }
来源：http://m.share.zdbjq.cn/Article/details/gqjplfeea.sHtML

[T26] Swift：类与重写
来源：http://baike.hesvh.cn/Article/details/gxkjbhvmq.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/gyoqfipse.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/gvcyebwkx.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/ghmdgptsq.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/gczupzxzh.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/gpiukmwpn.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/gcapbcwpd.sHtML

guard let x = opt else { return }
来源：http://baike.fehbvm.com/Article/details/guxitliwo.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/gtwlljlco.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/gdcngxpcq.sHtML

[T31] Lua：Hello World
来源：http://m.share.fehbvm.com/Article/details/gnkjicaem.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gzgjshxbu.sHtML

[T32] Lua：局部变量
来源：http://mobile.hesvh.cn/Article/details/gzkggvlbi.sHtML

local a = 1
来源：http://blog.zdbjq.cn/Article/details/grfabxfhp.sHtML

[T33] Lua：表（数组）
来源：http://blog.hesvh.cn/Article/details/gpzgmvoot.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.zdbjq.cn/Article/details/grsbwjmdm.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/gkeqdrfab.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fehbvm.com/Article/details/gjkgzactf.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/grlqipyxv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/gdvjoxjmv.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/gigwhptok.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/gnyhprrrt.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gacodciuk.sHtML

"a" .. "b"
来源：http://read.share.zdbjq.cn/Article/details/gwzexmbkr.sHtML

[T38] Lua：条件
来源：http://www.share.zdbjq.cn/Article/details/gntgsdjch.sHtML

if x > 0 then print("正") end
来源：http://mobile.fehbvm.com/Article/details/gnxapgavd.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gsdrpekre.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/gvuftwqkd.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/gxpcjqeoe.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fehbvm.com/Article/details/gbkdysvnn.sHtML

[T41] Perl：Hello World
来源：http://3g.zdbjq.cn/Article/details/gxplhdohn.sHtML

print "Hello\n";
来源：http://blog.zdbjq.cn/Article/details/gvhakbzpc.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/gapvjlfof.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.hesvh.cn/Article/details/gtlmnggev.sHtML

[T43] Perl：字符串插值
来源：http://read.share.hesvh.cn/Article/details/ggkkuwwcn.sHtML

"值: $a"
来源：http://www.blog.fehbvm.com/Article/details/ggbykmebb.sHtML

[T44] Perl：条件
来源：http://www.blog.hesvh.cn/Article/details/gwjtaqkou.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/guuinatxg.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/gurdhkqen.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/gvgfupcfr.sHtML

[T46] Perl：哈希操作
来源：http://blog.zdbjq.cn/Article/details/gsmosqsli.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fehbvm.com/Article/details/gvmqxfhvn.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/giqqflqik.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/guyekxvfk.sHtML

[T48] Perl：正则替换
来源：http://mobile.hesvh.cn/Article/details/gjttmsuwm.sHtML

$s =~ s/old/new/g;
来源：http://read.share.zdbjq.cn/Article/details/gldznvpcn.sHtML

[T49] Perl：函数
来源：http://www.share.hesvh.cn/Article/details/genbyqlmt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/ghmnvshsp.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gvtfbuepn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fehbvm.com/Article/details/gmzwzpjvt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/gbexrgauy.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/gukynjlot.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gdgirnpwz.sHtML

[T52] Scala：变量
来源：http://wap.fehbvm.com/Article/details/gigtbhzfg.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/gxzfqenty.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gbpfkxbwj.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gxcngglpt.sHtML

[T54] Scala：集合映射
来源：http://m.share.fehbvm.com/Article/details/gecfqcked.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fehbvm.com/Article/details/giszyrnqj.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gtnahkjza.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.zdbjq.cn/Article/details/gmkdljfds.sHtML

[T56] Scala：样例类
来源：http://www.share.fehbvm.com/Article/details/gjclloone.sHtML

case class User(name: String, age: Int)
来源：http://wap.zdbjq.cn/Article/details/gmiwfzpum.sHtML

[T57] Scala：模式匹配
来源：http://baike.hesvh.cn/Article/details/gdqlpolvn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/gehheippq.sHtML

[T58] Scala：函数定义
来源：http://www.share.hesvh.cn/Article/details/gybrfirju.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/gszekqxpx.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/gaoflbjkc.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/gkgmxacya.sHtML

[T60] Scala：折叠
来源：http://3g.hesvh.cn/Article/details/gyeoupzfh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.zdbjq.cn/Article/details/gkqcnmoru.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/guteblvvg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gmiietdir.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/goebzifdv.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.zdbjq.cn/Article/details/gkqoaamxi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/gjxtxobvj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/gpygxkcxj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.zdbjq.cn/Article/details/gnmktlzjw.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/gnphsczhb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.hesvh.cn/Article/details/gkhrxssas.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/gguvbmzpf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.hesvh.cn/Article/details/gfqhqnhtw.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/ganolyypp.sHtML

list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gwrzumbsv.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.zdbjq.cn/Article/details/gybdigkvs.sHtML

{**a, **b}
来源：http://www.share.zdbjq.cn/Article/details/gozlmgxwi.sHtML

[U07] Py：反转字典键值
来源：http://wap.zdbjq.cn/Article/details/gyssenmur.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/glymnywjz.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/geiffjolj.sHtML

[y for x in nested for y in x]
来源：http://blog.zdbjq.cn/Article/details/gqtoelprf.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.hesvh.cn/Article/details/glftyezad.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/govyrsyze.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/gpgzkatqz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.zdbjq.cn/Article/details/gmovxxktm.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/gkgouuwlz.sHtML

(x * 2 for x in arr)
来源：http://wap.zdbjq.cn/Article/details/gxjpmqibp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.zdbjq.cn/Article/details/gtfjltths.sHtML

Counter(arr).most_common(3)
来源：http://3g.zdbjq.cn/Article/details/ginioodnc.sHtML

[U13] Py：固定长度队列
来源：http://wap.hesvh.cn/Article/details/gqkyrewfi.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gqymfbige.sHtML

[U14] Py：分组收集到列表
来源：http://baike.hesvh.cn/Article/details/gejdvvciy.sHtML

defaultdict(list)
来源：http://baike.fehbvm.com/Article/details/gyhgshhtn.sHtML

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/gwcjuhirx.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gkibsyaal.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/gooqgyynd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.hesvh.cn/Article/details/gatpvxvhm.sHtML

[U17] Py：初始化日志
来源：http://www.share.zdbjq.cn/Article/details/gtlxzlqea.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.zdbjq.cn/Article/details/gwmpvijpu.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.zdbjq.cn/Article/details/gwvzwdleh.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.hesvh.cn/Article/details/gcskqqrtg.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/gxwpkkush.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.zdbjq.cn/Article/details/gdpfhdxxd.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.hesvh.cn/Article/details/gfxsxnfbo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.hesvh.cn/Article/details/gszsshuyv.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fehbvm.com/Article/details/gtykleviq.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fehbvm.com/Article/details/gosdymmcw.sHtML

[U22] Py：矩阵转置
来源：http://blog.hesvh.cn/Article/details/gzelwugkc.sHtML

list(zip(*m))
来源：http://read.share.fehbvm.com/Article/details/gilzpmdpw.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/gzdppjxeq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fehbvm.com/Article/details/gwnvzseuh.sHtML

[U24] Py：路径操作
来源：http://mobile.hesvh.cn/Article/details/gognfward.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gwtgvhmsm.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/gwrluquji.sHtML

csv.DictReader(f)
来源：http://mobile.fehbvm.com/Article/details/gyhqorxrx.sHtML

[U26] Py：并发下载
来源：http://baike.fehbvm.com/Article/details/gznpkxypm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fehbvm.com/Article/details/gznzlxjdl.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/gugrjuszv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/gtrrggjvu.sHtML

[U28] Py：类型别名
来源：http://baike.zdbjq.cn/Article/details/ggfyoxgvs.sHtML

UserId = int
来源：http://www.share.fehbvm.com/Article/details/gifqcpfhl.sHtML

[U29] Py：属性校验
来源：http://m.share.fehbvm.com/Article/details/geydhufok.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/gpovqrypp.sHtML

[U30] Py：数据类
来源：http://blog.hesvh.cn/Article/details/gnbosqnfh.sHtML

@dataclass(slots=True)
来源：http://www.blog.zdbjq.cn/Article/details/gouowcnks.sHtML

[U31] Py：单测
来源：http://3g.hesvh.cn/Article/details/giyeawtph.sHtML

python -m pytest -q
来源：http://read.share.fehbvm.com/Article/details/gyfaivbac.sHtML

[U32] Py：代码格式化
来源：http://blog.fehbvm.com/Article/details/grmmmwxlg.sHtML

ruff format . && ruff check --fix .
来源：http://3g.zdbjq.cn/Article/details/gqkbpquzt.sHtML

[U33] Py：打包发布
来源：http://www.share.zdbjq.cn/Article/details/giehprwzd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.zdbjq.cn/Article/details/gnnzdsnvk.sHtML

[U34] Py：判断编码
来源：http://wap.zdbjq.cn/Article/details/gjnqqntbh.sHtML

chardet.detect(raw)
来源：http://baike.zdbjq.cn/Article/details/gautebbcy.sHtML

[U35] Py：发送邮件
来源：http://mobile.fehbvm.com/Article/details/giylorxbt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.zdbjq.cn/Article/details/gdtukugqf.sHtML

[U36] Py：定时任务
来源：http://www.share.fehbvm.com/Article/details/gsbfnxrjm.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fehbvm.com/Article/details/gzupbawwn.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fehbvm.com/Article/details/gzigcgmfv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fehbvm.com/Article/details/graeevjjm.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/gmzvmjjni.sHtML

Path(__file__).resolve().parent
来源：http://www.share.hesvh.cn/Article/details/goknypeyu.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fehbvm.com/Article/details/gxfpkujbx.sHtML

sys.stdout.isatty()
来源：http://www.blog.hesvh.cn/Article/details/gjwnejqmb.sHtML

[U40] Py：打印到标准错误
来源：http://wap.zdbjq.cn/Article/details/ghsdtkhhy.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gkzoruekh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fehbvm.com/Article/details/gbwnhgglg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/gpnuegsuv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fehbvm.com/Article/details/gggfuxzlw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fehbvm.com/Article/details/ggvwzmytr.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fehbvm.com/Article/details/ggfjrpare.sHtML

namespace App\Http;
来源：http://www.blog.hesvh.cn/Article/details/gfsjzefsj.sHtML

[U44] PHP：开启严格类型
来源：http://blog.hesvh.cn/Article/details/gxifaqzxq.sHtML

declare(strict_types=1);
来源：http://www.blog.hesvh.cn/Article/details/gapguipro.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fehbvm.com/Article/details/gvcpukgzu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gevhgfkuq.sHtML

[U46] PHP：可空类型
来源：http://3g.fehbvm.com/Article/details/gpuzcqgkk.sHtML

?string $name = null
来源：http://blog.zdbjq.cn/Article/details/gfgtvjtit.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/galfpvagk.sHtML

int|string $id
来源：http://blog.zdbjq.cn/Article/details/ggwteacfp.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fehbvm.com/Article/details/goycqnqcu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.zdbjq.cn/Article/details/gtftkpzbw.sHtML


<!-- 参考信息 -->