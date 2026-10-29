代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/glegjijgs.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/gkdickixl.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/gwgpqaigr.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/ghojrvumd.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gsygzrzsc.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gpmypkiiy.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/guddcxnrc.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/gwxacrhfj.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gexiefcpq.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gsfhqmjty.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/gaulhhtdf.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/gprqfthwd.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/ghwnqqbsz.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/gfxhojcgc.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gqvdaedwo.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gcedziudm.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gcyocvcrn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/gjlnqpryq.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gbfpnmskg.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gyzadbyox.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/gxieqyfem.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gieyrilwz.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gfjykflpa.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gkfmatyds.sHtML

[S35] C++：map
来源：http://read.share.hesvh.cn/Article/details/glojgwjpe.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gcspdyvly.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/glscfwcgm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gpkzzjleb.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/gizuiqzon.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gsubkppzi.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gpjnbhhjp.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/grjdilwmu.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/glqfcpsgo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/grfpzbbsi.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gpthmjodl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gbtrybohs.sHtML

[S41] C++：类与构造函数
来源：http://www.share.zdbjq.cn/Article/details/ghkmfbffd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/gskfmhigu.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gaeennefm.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/gzoqrefkj.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gbfquarwk.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/geownmftq.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gjwpsgqnt.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gyacepzsh.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gxxypvrot.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gobtayhgx.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/gsvnrlswd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gtqshyofm.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gsnilnogg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.hesvh.cn/Article/details/gydqsnisj.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gzyatehif.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.zdbjq.cn/Article/details/gzkfofunf.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gawkigxij.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gtsqxhuhn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/gdmljivgi.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/gbcpicgid.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gbcqgmhyi.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/gujoczcwe.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/gbekbqfrr.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/gzbxvsmsv.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvfyvxooh.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/gyitlerjx.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gnxstoxcz.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/ghdalyiye.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gnsrxxqxs.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gvtftsefm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gblpxmqem.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/gmelzpmsa.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/gtbeamppe.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/giacdjrpm.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gusmbhjek.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gcpgxfrab.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/goexkglpi.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/gdpxvpqoe.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/giydrevwe.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gpmchklwq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gdoqepwun.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtuqdptta.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gnlhvgmmq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcgduaoco.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gxpljnuqb.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gctrnzpef.sHtML

[T02] Kotlin：变量
来源：http://blog.hesvh.cn/Article/details/gobvyugdy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/gtileplvn.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/gnervkydj.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gdewuptbf.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/gaqjzqicj.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/gysyhfooh.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/gltwwwfqb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/gqohcfvqv.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/gfhxdiqcm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gfpihfuft.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/grjborhfq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/gxvkeoxmq.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gsegzknig.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.zdbjq.cn/Article/details/gbxgpujnh.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.zdbjq.cn/Article/details/gdpqgfwoc.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/gqywynvfn.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gaqmoetop.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/gcevnnwgs.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/grgtpdenf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.zdbjq.cn/Article/details/glfhbknic.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/golypzwne.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gtjfqjltj.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gmowsqnfj.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/gxqdqtqog.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/gjddmrmwi.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/gsqsmvdfc.sHtML

[T15] Kotlin：接口
来源：http://3g.fehbvm.com/Article/details/goimdgqwe.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/gjykepvnt.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/gvmtmzgfn.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/ghmjmqnoe.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/giawajmab.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gfksggnfc.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/glmcejrng.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gipkqegsg.sHtML

[T19] Swift：可选绑定
来源：http://3g.hesvh.cn/Article/details/grabjavha.sHtML

if let n = opt { print(n) }
来源：http://m.share.fehbvm.com/Article/details/ggrssqvpi.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gjtuuuexa.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gqevwrbpl.sHtML

[T21] Swift：遍历
来源：http://mobile.zdbjq.cn/Article/details/glqkegugs.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/gjsojujvh.sHtML

[T22] Swift：字典
来源：http://read.share.fehbvm.com/Article/details/gjiaepgli.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/gkzdhrhbf.sHtML

[T23] Swift：函数
来源：http://www.m.share.fehbvm.com/Article/details/gjevwkoee.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.zdbjq.cn/Article/details/gggkdwqcd.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/gyewrxooc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gxejwfnmj.sHtML

[T25] Swift：结构体
来源：http://m.share.fehbvm.com/Article/details/gqdnajihr.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gljdrzkhi.sHtML

[T26] Swift：类与重写
来源：http://3g.hesvh.cn/Article/details/gptoexrcw.sHtML

class A: Base { override func f() {} }
来源：http://m.share.zdbjq.cn/Article/details/gbjcdzvmw.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/gcxnicctn.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gsvfixaqw.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/grjldgwua.sHtML

enum Color { case red, green }
来源：http://www.share.fehbvm.com/Article/details/gafvzaabh.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gnzkcqlre.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/gvygdujne.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/gwlnnwuqn.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.zdbjq.cn/Article/details/gkoyjkelp.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/ghwdfmdrz.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gofxfadaf.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gmgbfntan.sHtML

local a = 1
来源：http://m.share.fehbvm.com/Article/details/grqzggams.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gjqbadyhh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fehbvm.com/Article/details/gbxdfpjku.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/gvmlmqyco.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.hesvh.cn/Article/details/gsvtigxqn.sHtML

[T35] Lua：字典表
来源：http://read.share.zdbjq.cn/Article/details/gzmgybgnu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/gpnbxdlcr.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/gklgqwhob.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/gehzfldgu.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.hesvh.cn/Article/details/ghekcgoxk.sHtML

"a" .. "b"
来源：http://3g.fehbvm.com/Article/details/grlqzdggs.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/gmnlsjkkc.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/gtjluwglu.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fehbvm.com/Article/details/getnhnzsd.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/gzbhiulbn.sHtML

[T40] Lua：元表
来源：http://m.share.fehbvm.com/Article/details/gqrknaipg.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.hesvh.cn/Article/details/gyvuatrdt.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/ghosnprkw.sHtML

print "Hello\n";
来源：http://wap.zdbjq.cn/Article/details/gvjemryqn.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gybejoelb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.hesvh.cn/Article/details/gismmjmsh.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/gerwdjocs.sHtML

"值: $a"
来源：http://m.share.hesvh.cn/Article/details/gnvozsekb.sHtML

[T44] Perl：条件
来源：http://www.share.fehbvm.com/Article/details/gaqbrsqbd.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fehbvm.com/Article/details/gwgdpdkwz.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/gapanvfve.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.hesvh.cn/Article/details/grazajpdi.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/gbogtwmkn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/gvcfdklfx.sHtML

[T47] Perl：正则捕获
来源：http://wap.hesvh.cn/Article/details/goyilmcib.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.zdbjq.cn/Article/details/gugiurcfl.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/gzuuvjoul.sHtML

$s =~ s/old/new/g;
来源：http://baike.hesvh.cn/Article/details/gpgrtuxzg.sHtML

[T49] Perl：函数
来源：http://www.share.fehbvm.com/Article/details/gcwnfszwv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gnkwqgfog.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gyolxrlaq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.hesvh.cn/Article/details/gloafrpme.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.zdbjq.cn/Article/details/gevfwsthv.sHtML

[T51] Scala：Hello World
来源：http://baike.zdbjq.cn/Article/details/gaqfzctpp.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gdsygmkri.sHtML

[T52] Scala：变量
来源：http://read.share.zdbjq.cn/Article/details/griuisepv.sHtML

val a = 1;  var b = 2
来源：http://wap.fehbvm.com/Article/details/giqzyvcfj.sHtML

[T53] Scala：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gxmwwduxq.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/ggaiywent.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/ghebmtadj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/gowcksjrm.sHtML

[T55] Scala：集合过滤
来源：http://baike.fehbvm.com/Article/details/gmozewxqh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/gxafyjcfj.sHtML

[T56] Scala：样例类
来源：http://wap.fehbvm.com/Article/details/gwdloxteo.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gmyrubhak.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gtegberdr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gxgbtlwac.sHtML

[T58] Scala：函数定义
来源：http://3g.hesvh.cn/Article/details/ghdjxhfib.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/gymcwzyol.sHtML

[T59] Scala：循环
来源：http://wap.hesvh.cn/Article/details/ggipcbqyt.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gczubrkyd.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/glsujtdtu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fehbvm.com/Article/details/gmjdgtvfr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gguvamwda.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gmrdjxxre.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjpwugjyj.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.zdbjq.cn/Article/details/gqwbmgzyf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gsgneagzp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fehbvm.com/Article/details/gubhdykcv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.hesvh.cn/Article/details/giuuyteap.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fehbvm.com/Article/details/gcsozcryf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/gtujznofx.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.hesvh.cn/Article/details/gqidpszdq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.zdbjq.cn/Article/details/gbgavbhsb.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.hesvh.cn/Article/details/gxqxfmosm.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gltofnonw.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gwwiulxrj.sHtML

{**a, **b}
来源：http://baike.hesvh.cn/Article/details/grghcqdxj.sHtML

[U07] Py：反转字典键值
来源：http://baike.hesvh.cn/Article/details/gyeguolkh.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fehbvm.com/Article/details/gxglipjzb.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fehbvm.com/Article/details/gdiqbdlxc.sHtML

[y for x in nested for y in x]
来源：http://mobile.fehbvm.com/Article/details/gbosjbuje.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.hesvh.cn/Article/details/gtlaectdj.sHtML

max(d, key=d.get)
来源：http://www.blog.fehbvm.com/Article/details/gurwkqokl.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fehbvm.com/Article/details/gviutyzdw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/gycoftxip.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/gogofobnc.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fehbvm.com/Article/details/ghbomxtkb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.hesvh.cn/Article/details/gnhmradaz.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/gzqczzjgu.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/gnhxoyaix.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/gmhxmadda.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fehbvm.com/Article/details/gokjnmjwf.sHtML

defaultdict(list)
来源：http://mobile.zdbjq.cn/Article/details/gwdiqohvo.sHtML

[U15] Py：高精度计时
来源：http://mobile.hesvh.cn/Article/details/gwjpbhngz.sHtML

t = time.perf_counter()
来源：http://mobile.fehbvm.com/Article/details/gljwetuvp.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/goycdntxn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.hesvh.cn/Article/details/gvulwvylz.sHtML

[U17] Py：初始化日志
来源：http://baike.hesvh.cn/Article/details/gcsepybqd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.zdbjq.cn/Article/details/ggxuihaht.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/gvhxjolbi.sHtML

pat = re.compile(r"\d+")
来源：http://wap.hesvh.cn/Article/details/goozcezne.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fehbvm.com/Article/details/gmefqvigi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fehbvm.com/Article/details/gbvdraaqo.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/ghtopgako.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.hesvh.cn/Article/details/gskqdqyax.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fehbvm.com/Article/details/gmcrfmwsv.sHtML

@contextlib.contextmanager
来源：http://blog.zdbjq.cn/Article/details/ggeucgqvx.sHtML

[U22] Py：矩阵转置
来源：http://wap.fehbvm.com/Article/details/gjnrbtnef.sHtML

list(zip(*m))
来源：http://blog.fehbvm.com/Article/details/gdrkgxgfs.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.hesvh.cn/Article/details/grriwzkpa.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.hesvh.cn/Article/details/gdzlqutgo.sHtML

[U24] Py：路径操作
来源：http://baike.zdbjq.cn/Article/details/ggojivlgj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/goykwghoy.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/giqpbhare.sHtML

csv.DictReader(f)
来源：http://baike.fehbvm.com/Article/details/gtdharrwm.sHtML

[U26] Py：并发下载
来源：http://wap.zdbjq.cn/Article/details/gdletmasu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fehbvm.com/Article/details/gzpxajvgq.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/guwsngefu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.zdbjq.cn/Article/details/gqilnzlrt.sHtML

[U28] Py：类型别名
来源：http://m.share.fehbvm.com/Article/details/gkertewak.sHtML

UserId = int
来源：http://www.share.fehbvm.com/Article/details/gvndognnz.sHtML

[U29] Py：属性校验
来源：http://www.blog.zdbjq.cn/Article/details/gehqxhitf.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/gericzone.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/gaiklywlh.sHtML

@dataclass(slots=True)
来源：http://read.share.hesvh.cn/Article/details/gxsupcebb.sHtML

[U31] Py：单测
来源：http://mobile.zdbjq.cn/Article/details/gfdkzzzkf.sHtML

python -m pytest -q
来源：http://baike.zdbjq.cn/Article/details/gsqarnwra.sHtML

[U32] Py：代码格式化
来源：http://baike.hesvh.cn/Article/details/gmpanwbyn.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/gqqxthsix.sHtML

[U33] Py：打包发布
来源：http://read.share.hesvh.cn/Article/details/gbnyatdyn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/gqyisaijb.sHtML

[U34] Py：判断编码
来源：http://wap.zdbjq.cn/Article/details/gzejgzpwr.sHtML

chardet.detect(raw)
来源：http://www.share.fehbvm.com/Article/details/guzlpnviw.sHtML

[U35] Py：发送邮件
来源：http://m.share.zdbjq.cn/Article/details/gcmhxmqje.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/gjkcozspl.sHtML

[U36] Py：定时任务
来源：http://baike.zdbjq.cn/Article/details/gxkqecsat.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.zdbjq.cn/Article/details/ghdhdyzqi.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/geoeyecaq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.zdbjq.cn/Article/details/gexuanvsb.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/gmitbmhov.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.zdbjq.cn/Article/details/gwiadmiqs.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.hesvh.cn/Article/details/grleadlen.sHtML

sys.stdout.isatty()
来源：http://www.blog.zdbjq.cn/Article/details/gefjrewjb.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fehbvm.com/Article/details/gxlyzqrzd.sHtML

print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gvbctzzyh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.hesvh.cn/Article/details/guijfszjs.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.hesvh.cn/Article/details/gvhgtfait.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.hesvh.cn/Article/details/glgfeevqe.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.hesvh.cn/Article/details/guphohslt.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gxerjycaf.sHtML

namespace App\Http;
来源：http://baike.fehbvm.com/Article/details/giomwdrmn.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fehbvm.com/Article/details/gzfqzanzu.sHtML

declare(strict_types=1);
来源：http://3g.zdbjq.cn/Article/details/gkcmosvel.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.hesvh.cn/Article/details/gnwowlfhu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/grqykjtda.sHtML

[U46] PHP：可空类型
来源：http://m.share.hesvh.cn/Article/details/gztfdkbcr.sHtML

?string $name = null
来源：http://read.share.zdbjq.cn/Article/details/gsuqraiuw.sHtML

[U47] PHP：联合类型
来源：http://baike.fehbvm.com/Article/details/gotdnrmny.sHtML

int|string $id
来源：http://mobile.hesvh.cn/Article/details/ghuslzbkn.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.hesvh.cn/Article/details/gkebktqim.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.zdbjq.cn/Article/details/gpyaemydz.sHtML


<!-- 参考信息 -->