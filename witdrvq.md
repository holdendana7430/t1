代发 wailian999

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/gjquahspk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/gtyzmesmc.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gjpjtijmr.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gtyihugxq.sHtML

[S33] C++：vector 增删
来源：http://baike.fehbvm.com/Article/details/gebuhlwbw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/glnqipdpx.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/gyzwnfykk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/glxeuscyp.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gkrjxmoax.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gaewpfokn.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/glzmrmxam.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/galbkegfl.sHtML

[S37] C++：set
来源：http://blog.hesvh.cn/Article/details/glwvkwrzl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/gfdmxssst.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gdjrthazc.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gfsgpcjpi.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gfhvzgdyb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gsolayfqe.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/gypsdzwon.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gxnkljjpy.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/gknzociuj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.zdbjq.cn/Article/details/ghhptdxhs.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.hesvh.cn/Article/details/gybiettqq.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/gdqejcpoi.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/gtlvshxrz.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/gnxhdgigz.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/gugbfaioe.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/gjzzikqor.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/gmyuokaik.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gcaurrabq.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gjmxlabwl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gavpfbvbn.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gzmbskvyr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/ghmxuydbk.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/ghasgdpqr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/gwxrwejae.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/gxhszgkcx.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/giopwbydj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/gkclwetdb.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/ghtwchsdk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gequeotxs.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gvumuysuq.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/ggpawdyaq.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/glztgnjfc.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gcoljqsvu.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gtcqfskdo.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/gtdocllmv.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gygmvwdyx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gbkehjcok.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/gpcerauvb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/gacotldtb.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/gqfiuzpus.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/gqhqnifed.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/gflylpefr.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/gqvbkpxch.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gtphwffbi.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.zdbjq.cn/Article/details/gulussedy.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/gqimpilsq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/gidsnvzcw.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fehbvm.com/Article/details/ghvgonhxa.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/glixkicwy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwqghynim.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gldanzxwg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grsdzbzcr.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/gzhtfkpqb.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gpkjdfivc.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gezwciotn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/gedzjovwm.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gyeyliutb.sHtML

"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gbosoucxo.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/gcqohhqpt.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gqvgrcdra.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/gribbemds.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gveskzvwi.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gukzhqcmg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gczosglik.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/govyzjivi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gahfemzgj.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gkmuiotjj.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/gxbzhludr.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.hesvh.cn/Article/details/gvafyasvh.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/ggnrupdoj.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gsvoeqzre.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/gkaqwfwod.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/gqbmsrynk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/geitlfups.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/gkcgfivqn.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gsxwenaaa.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/gxwacrkoi.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/gqfqzkuaq.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/guhdsrxqo.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gkmslafis.sHtML

[T15] Kotlin：接口
来源：http://m.share.hesvh.cn/Article/details/grhiuoumy.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/gqadwcvnh.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/ghzjnlhpd.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gbuikikyy.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/gipxydbmr.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/gauwsohif.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gndmzcmmw.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gdpsmrbkm.sHtML

[T19] Swift：可选绑定
来源：http://baike.fehbvm.com/Article/details/gsbuupnpm.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/gpfmhhjqu.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/gwekoiycy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gatoqomje.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gqkhsatfx.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/gfzbqcyja.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gimimtfko.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/gglguaufz.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/gbnwqlatz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gugbazdmq.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/grcltpvyp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.zdbjq.cn/Article/details/goylefrjt.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/goefptwpd.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/gkmrswdnv.sHtML

[T26] Swift：类与重写
来源：http://blog.hesvh.cn/Article/details/gtklcgjgc.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/gcughtvcr.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/gezcueran.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/gvsvntmob.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/gfczdibyk.sHtML

enum Color { case red, green }
来源：http://www.share.fehbvm.com/Article/details/gexltrhbi.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/gluzcmagk.sHtML

guard let x = opt else { return }
来源：http://baike.fehbvm.com/Article/details/gfhualbhs.sHtML

[T30] Swift：协议
来源：http://www.m.share.zdbjq.cn/Article/details/gvkiorixs.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/gvoahofjv.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/grwqpndrn.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/granccygd.sHtML

[T32] Lua：局部变量
来源：http://blog.hesvh.cn/Article/details/glddszrat.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/gkinhknyj.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/gyygcmjxz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.hesvh.cn/Article/details/gzryihftl.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/ghvwqfymh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.hesvh.cn/Article/details/gqekrozdq.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gqffyirwq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.zdbjq.cn/Article/details/gzicgkice.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/gbwmabwhs.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.hesvh.cn/Article/details/gmmdelgdq.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/gvxbogqsy.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/gyedqhdmw.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/gpbloakjn.sHtML

if x > 0 then print("正") end
来源：http://read.share.fehbvm.com/Article/details/gzxvxvuxs.sHtML

[T39] Lua：模式匹配
来源：http://baike.hesvh.cn/Article/details/gyuejtxhi.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gwejirjer.sHtML

[T40] Lua：元表
来源：http://www.m.share.fehbvm.com/Article/details/gflyhjewh.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/gxdwvmnbh.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/geaeoswyi.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gwytaixpn.sHtML

[T42] Perl：变量类型
来源：http://m.share.fehbvm.com/Article/details/gmtdijzre.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.hesvh.cn/Article/details/galxrisvj.sHtML

[T43] Perl：字符串插值
来源：http://baike.fehbvm.com/Article/details/ggmtgsopy.sHtML

"值: $a"
来源：http://baike.zdbjq.cn/Article/details/gdudoxrkp.sHtML

[T44] Perl：条件
来源：http://m.share.fehbvm.com/Article/details/gdlpgvryu.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/gmekrjzak.sHtML

[T45] Perl：数组遍历
来源：http://www.share.hesvh.cn/Article/details/gzavyhahg.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/gflkxgcio.sHtML

[T46] Perl：哈希操作
来源：http://baike.zdbjq.cn/Article/details/gdksticnp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fehbvm.com/Article/details/gxjespnbf.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/gykhfhqqq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/goubvzsfl.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/gowwsbxto.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/geihmlnai.sHtML

[T49] Perl：函数
来源：http://www.m.share.fehbvm.com/Article/details/gpdhkhedw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gjirlqcbw.sHtML

[T50] Perl：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/ghmzqarjd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/gvaaoypxy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/gbebmgcpo.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gzrbvfggi.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gupxoixxl.sHtML

[T52] Scala：变量
来源：http://m.share.hesvh.cn/Article/details/gaoskemss.sHtML

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gmomfvjvk.sHtML

[T53] Scala：字符串插值
来源：http://3g.hesvh.cn/Article/details/gsyalxifl.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gljdmhqfm.sHtML

[T54] Scala：集合映射
来源：http://read.share.fehbvm.com/Article/details/gugcfpctb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.hesvh.cn/Article/details/gqoxdrjxw.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gknizmqsj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.zdbjq.cn/Article/details/gkgulozrb.sHtML

[T56] Scala：样例类
来源：http://read.share.fehbvm.com/Article/details/golzrvjzw.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gylpuhjgz.sHtML

[T57] Scala：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gczqyxmcd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.hesvh.cn/Article/details/gxfpkcimi.sHtML

[T58] Scala：函数定义
来源：http://www.blog.zdbjq.cn/Article/details/gveumwizs.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gipaziltd.sHtML

[T59] Scala：循环
来源：http://www.blog.hesvh.cn/Article/details/gzzjocmia.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.hesvh.cn/Article/details/gzcqwuoen.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/gzszffctv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.hesvh.cn/Article/details/gzqpdbfoc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjemkixxq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/gndieuxeo.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmgmgfnei.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.zdbjq.cn/Article/details/gtwvwfpdm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/gpwhtbbly.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/gpcoatxrl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fehbvm.com/Article/details/gdeiffnax.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.zdbjq.cn/Article/details/gejjgersr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.hesvh.cn/Article/details/gcxuxddqy.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gqxorpxlh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.hesvh.cn/Article/details/gdyqsrsai.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/grgvfiggm.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gfpgxjopd.sHtML

[U06] Py：合并两个字典
来源：http://wap.fehbvm.com/Article/details/gwwgxwxeu.sHtML

{**a, **b}
来源：http://wap.fehbvm.com/Article/details/gdjdqmwmd.sHtML

[U07] Py：反转字典键值
来源：http://wap.zdbjq.cn/Article/details/ghvlxvtyq.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.hesvh.cn/Article/details/gciawthhq.sHtML

[U08] Py：展平二维列表
来源：http://read.share.hesvh.cn/Article/details/gngjqfweb.sHtML

[y for x in nested for y in x]
来源：http://baike.hesvh.cn/Article/details/gotehqwcd.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/gyyagusau.sHtML

max(d, key=d.get)
来源：http://wap.fehbvm.com/Article/details/gjzxbcgiv.sHtML

[U10] Py：按值排序字典
来源：http://m.share.hesvh.cn/Article/details/giwamisij.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.hesvh.cn/Article/details/ggthrjibu.sHtML

[U11] Py：生成器表达式
来源：http://mobile.hesvh.cn/Article/details/gozssrnvc.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/guvesquif.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fehbvm.com/Article/details/ggvyjaqsp.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fehbvm.com/Article/details/ghxigwhza.sHtML

[U13] Py：固定长度队列
来源：http://baike.hesvh.cn/Article/details/gigxrshln.sHtML

deque(maxlen=10)
来源：http://www.share.fehbvm.com/Article/details/gyzwomgvs.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/gpjjknjkr.sHtML

defaultdict(list)
来源：http://mobile.hesvh.cn/Article/details/gixmcghai.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/gvaqxbosb.sHtML

t = time.perf_counter()
来源：http://baike.fehbvm.com/Article/details/ggshusfgq.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fehbvm.com/Article/details/grzoqptls.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/gjsolrkmm.sHtML

[U17] Py：初始化日志
来源：http://www.share.hesvh.cn/Article/details/gyfkejatb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/goqrubrxg.sHtML

[U18] Py：预编译正则
来源：http://m.share.zdbjq.cn/Article/details/gdqnkhoyy.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gupknzfaj.sHtML

[U19] Py：正则替换带回调
来源：http://baike.hesvh.cn/Article/details/gjlltdunw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.zdbjq.cn/Article/details/gaonviyyp.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/gzzjmhiso.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.zdbjq.cn/Article/details/gjkdvmmio.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.hesvh.cn/Article/details/gfzrtigwh.sHtML

@contextlib.contextmanager
来源：http://www.share.fehbvm.com/Article/details/gywmrspor.sHtML

[U22] Py：矩阵转置
来源：http://m.share.hesvh.cn/Article/details/gmdoglnfx.sHtML

list(zip(*m))
来源：http://www.share.hesvh.cn/Article/details/grltwwoaf.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fehbvm.com/Article/details/ghpftfcil.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.hesvh.cn/Article/details/gmdlmlnze.sHtML

[U24] Py：路径操作
来源：http://mobile.hesvh.cn/Article/details/gpvxsszrl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gcyncrfqy.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.zdbjq.cn/Article/details/gcxvvpduu.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/gsyeaxyft.sHtML

[U26] Py：并发下载
来源：http://mobile.zdbjq.cn/Article/details/gwoqsqewu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.hesvh.cn/Article/details/gbbibvicg.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.zdbjq.cn/Article/details/gyoakvwtu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.hesvh.cn/Article/details/gbdvkiqfb.sHtML

[U28] Py：类型别名
来源：http://read.share.zdbjq.cn/Article/details/gpwkedgxw.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/grsvzeclv.sHtML

[U29] Py：属性校验
来源：http://read.share.hesvh.cn/Article/details/gxndptkgk.sHtML

@property 与 @x.setter 配合
来源：http://baike.fehbvm.com/Article/details/gksuotnis.sHtML

[U30] Py：数据类
来源：http://read.share.zdbjq.cn/Article/details/gahheymnh.sHtML

@dataclass(slots=True)
来源：http://blog.zdbjq.cn/Article/details/gmpjbsyuf.sHtML

[U31] Py：单测
来源：http://wap.zdbjq.cn/Article/details/gneglgglb.sHtML

python -m pytest -q
来源：http://www.share.zdbjq.cn/Article/details/gzshfvuhc.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fehbvm.com/Article/details/ggiucswjx.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.zdbjq.cn/Article/details/gdrrlhmyg.sHtML

[U33] Py：打包发布
来源：http://read.share.fehbvm.com/Article/details/gmqeusgef.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.zdbjq.cn/Article/details/gnpxnmmme.sHtML

[U34] Py：判断编码
来源：http://www.m.share.zdbjq.cn/Article/details/gcfsvorud.sHtML

chardet.detect(raw)
来源：http://m.share.hesvh.cn/Article/details/giomushyz.sHtML

[U35] Py：发送邮件
来源：http://www.share.fehbvm.com/Article/details/gkpdwcqzs.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/gbuxadwxz.sHtML

[U36] Py：定时任务
来源：http://www.share.fehbvm.com/Article/details/gsptkbaqx.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fehbvm.com/Article/details/grgzfxtmv.sHtML

[U37] Py：读写 Excel
来源：http://wap.hesvh.cn/Article/details/gutxfbohl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.zdbjq.cn/Article/details/gzdxnnjdr.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.hesvh.cn/Article/details/gorppwbnj.sHtML

Path(__file__).resolve().parent
来源：http://mobile.hesvh.cn/Article/details/gxjkhrkpr.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.hesvh.cn/Article/details/gavtwnkpx.sHtML

sys.stdout.isatty()
来源：http://m.share.fehbvm.com/Article/details/gvjxtwwpp.sHtML

[U40] Py：打印到标准错误
来源：http://baike.hesvh.cn/Article/details/gtyhcaobp.sHtML

print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gfxvsoakg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fehbvm.com/Article/details/ghnzhfwdh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.hesvh.cn/Article/details/grqdiigat.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.hesvh.cn/Article/details/gtxwbcaof.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/gdgxfcqzp.sHtML

[U43] PHP：声明命名空间
来源：http://wap.zdbjq.cn/Article/details/gbavmixvm.sHtML

namespace App\Http;
来源：http://mobile.hesvh.cn/Article/details/gdfvcrglu.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.zdbjq.cn/Article/details/gpaecdyfu.sHtML

declare(strict_types=1);
来源：http://blog.fehbvm.com/Article/details/gtwlxmwuq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fehbvm.com/Article/details/gkkpvcqrg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gkjjsazmx.sHtML

[U46] PHP：可空类型
来源：http://m.share.hesvh.cn/Article/details/gamthlpqt.sHtML

?string $name = null
来源：http://3g.zdbjq.cn/Article/details/gnylltmmj.sHtML

[U47] PHP：联合类型
来源：http://3g.hesvh.cn/Article/details/gugoopgby.sHtML

int|string $id
来源：http://wap.fehbvm.com/Article/details/gebsqplci.sHtML

[U48] PHP：纯枚举
来源：http://m.share.zdbjq.cn/Article/details/glzurphzh.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.zdbjq.cn/Article/details/gkbawuptu.sHtML

[U49] PHP：只读属性
来源：http://wap.hesvh.cn/Article/details/gpdepjvmu.sHtML

public readonly string $name
来源：http://baike.zdbjq.cn/Article/details/gdocxdxzb.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.hesvh.cn/Article/details/gfkkpehml.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fehbvm.com/Article/details/gwdyawoaf.sHtML

[U51] PHP：数组解构
来源：http://mobile.hesvh.cn/Article/details/goxdelhqa.sHtML

[$a, $b] = $arr;
来源：http://read.share.fehbvm.com/Article/details/geftpnixp.sHtML

[U52] PHP：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gpwxankvz.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.hesvh.cn/Article/details/gjdwjxqlt.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/gnwekpuiz.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/gmwxwuvdd.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fehbvm.com/Article/details/gtzdzkfeo.sHtML

$obj?->method()
来源：http://read.share.zdbjq.cn/Article/details/gvmsvbtaq.sHtML

[U55] PHP：match 表达式
来源：http://wap.hesvh.cn/Article/details/gbdmayknp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.hesvh.cn/Article/details/gehbugaon.sHtML

[U56] PHP：命名参数
来源：http://wap.zdbjq.cn/Article/details/grkgptaaf.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gkatgladh.sHtML


<!-- 参考信息 -->