代发 wailian999

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/grdeqgkbc.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/ghtxehdsm.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gqplasjnm.sHtML

[S31] C++：Hello World
来源：http://blog.hesvh.cn/Article/details/gpczapxig.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gfqzipxyg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gmlgelcdy.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/gvbvfykuf.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fehbvm.com/Article/details/gftrwsron.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gjvbyhaow.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/gcmuajcxk.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gudzkavgm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/gisnwkjkz.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gtviegigs.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gyjhcuvpy.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gyrcebbmb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/garhahglk.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/glupekcpy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/gshnsjehh.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/gwqxbyosb.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/guriusdnt.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/ganonuppf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/guxfxiikr.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/gjytzkyjy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/ggvoydkhq.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gourshzne.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gdymrqgbo.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/gyzcuhtzi.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/glmpzbvev.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/gqvdcpnmb.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/gubylxwvw.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gfzbdcmpp.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/gcogucmsk.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gztoomqha.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gozgpzosu.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/gixqcsowj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/goiztyazr.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/gqovdufrz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gfczsseph.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gircjdcey.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gvuvsroqx.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gtsfmejeb.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/gkoakphkk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gfkkouuyb.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/gbbiikckv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gtpwakfpn.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gmnnlmskz.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gfppsxtou.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gqxfmkggw.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/glyunyvpl.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gqijcewmv.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/gfsetdqtw.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gxkwpefps.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/ghjxgipga.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/gbbsprghq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/ghwbioijp.sHtML

[S56] C++：optional
来源：http://www.m.share.fehbvm.com/Article/details/goprymmxq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/gtepeygbi.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/gkzbqumsi.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gxhqetycl.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gaajckpzd.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/gauypatfa.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gnxlikaco.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/gkrtyvfrz.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gydwimdsl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gousxuree.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gufhufucs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/ghjovpbou.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwpbxuzha.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gkjbvxobd.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gzvlwcklt.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/ghgxxavcg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gnnjzxniz.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/ghjmsytae.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gittpjirf.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/gkmnpxgst.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/grpfruwqm.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/grkasgycq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/gkvtpccsf.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/gwdybydje.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gfmvbanqv.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/gclpqdsaa.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/glqsqtpcg.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/gqkotfucg.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gahkmqtje.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/ggtbdtegd.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/geoxliioi.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/gnckdshep.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/gilgjeyjk.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/gotzonoza.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/gckuotdsf.sHtML

[T12] Kotlin：解构声明
来源：http://3g.hesvh.cn/Article/details/gvwswkrbi.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/getjdajae.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/gsmluesfs.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/ggiqebmjz.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/gsafyosnc.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gvysufhqt.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gkxoujwdw.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/genwvyrso.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/gelsjnuhp.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gsfjlekzi.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.zdbjq.cn/Article/details/ghvsmcdrw.sHtML

var a = 1;  let b = 2
来源：http://read.share.hesvh.cn/Article/details/gktqkzibc.sHtML

[T18] Swift：字符串插值
来源：http://wap.hesvh.cn/Article/details/gmszhfoly.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/gattxtcdm.sHtML

[T19] Swift：可选绑定
来源：http://read.share.hesvh.cn/Article/details/gbrmwidfd.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/gephefnsc.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gpznredvq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/glafkjsid.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/grdpqzskp.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gtpjghqza.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/gppjfopls.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/gjfqpxjhj.sHtML

[T23] Swift：函数
来源：http://baike.zdbjq.cn/Article/details/ggybrnkpz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gvtrphxgd.sHtML

[T24] Swift：闭包
来源：http://m.share.zdbjq.cn/Article/details/gewecngfx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/gziuqlxuy.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/gziczfjhz.sHtML

struct P { var x: Int }
来源：http://m.share.fehbvm.com/Article/details/gobugcjhl.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gldiyybbp.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/gkdclrtzn.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/ggxmpgisg.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.zdbjq.cn/Article/details/gafgfusgf.sHtML

[T28] Swift：枚举
来源：http://3g.zdbjq.cn/Article/details/gmsqximmq.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/ghizjakqy.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.hesvh.cn/Article/details/gnioaobte.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/gzfaiguxb.sHtML

[T30] Swift：协议
来源：http://mobile.zdbjq.cn/Article/details/gjnbzjzhc.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/gqqydnick.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/geutpjlwl.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gcgwkcjof.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/glltmnyza.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/glhtehacg.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/grxwsbemc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/gjsuwveym.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/giiwefcpj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fehbvm.com/Article/details/gpdxhsdgf.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/guaaaysfj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/ganzktomi.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gunhueitz.sHtML

function add(a, b) return a + b end
来源：http://baike.hesvh.cn/Article/details/gnleeloae.sHtML

[T37] Lua：字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gfaczbwdx.sHtML

"a" .. "b"
来源：http://www.blog.zdbjq.cn/Article/details/gmnfydggr.sHtML

[T38] Lua：条件
来源：http://wap.zdbjq.cn/Article/details/gltzjtlsi.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/grpqxbgqs.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gcnvyspkv.sHtML

string.find(s, "%d+")
来源：http://3g.hesvh.cn/Article/details/gomeyxfna.sHtML

[T40] Lua：元表
来源：http://www.share.fehbvm.com/Article/details/gcexfqdis.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/gyvstnkbw.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/gxtaxuehw.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/glfqhzcsl.sHtML

[T42] Perl：变量类型
来源：http://baike.hesvh.cn/Article/details/grcsjvavy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.zdbjq.cn/Article/details/gsheznssq.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/gazxptmkt.sHtML

"值: $a"
来源：http://blog.hesvh.cn/Article/details/gyfefyydl.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/gchciqlnr.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fehbvm.com/Article/details/gcwtrpswd.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/ggtpxxkfu.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/gqpdqizgy.sHtML

[T46] Perl：哈希操作
来源：http://blog.zdbjq.cn/Article/details/glmeznbld.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fehbvm.com/Article/details/garmknxzn.sHtML

[T47] Perl：正则捕获
来源：http://wap.zdbjq.cn/Article/details/grjeyomzj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fehbvm.com/Article/details/gezkghdim.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/gsvgawnwk.sHtML

$s =~ s/old/new/g;
来源：http://www.share.hesvh.cn/Article/details/gbvythotx.sHtML

[T49] Perl：函数
来源：http://baike.hesvh.cn/Article/details/gaaspftbp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gqoyinvuc.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/ghddrqbrz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.hesvh.cn/Article/details/gkjwnphuw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.hesvh.cn/Article/details/gzahcukxz.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/gprhquekb.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gjpffeasw.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/gnpluvbtk.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gganccqtb.sHtML

[T53] Scala：字符串插值
来源：http://wap.hesvh.cn/Article/details/gdwxgygbd.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/gldzsgpzv.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gfixjgbms.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.zdbjq.cn/Article/details/gtwtizakd.sHtML

[T55] Scala：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gpfcfpoht.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.zdbjq.cn/Article/details/gzurooipi.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/gnlcqijqu.sHtML

case class User(name: String, age: Int)
来源：http://wap.fehbvm.com/Article/details/gfcbukilh.sHtML

[T57] Scala：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gzovwilcc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/gmljawxgn.sHtML

[T58] Scala：函数定义
来源：http://www.blog.zdbjq.cn/Article/details/gpxtkrdwg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.zdbjq.cn/Article/details/gbhdzgaqd.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/gginjuelr.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gtwafftim.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/gmsrcrkca.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.hesvh.cn/Article/details/gimyiahwi.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmkcmexyy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/gynepmfrg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfckpeygf.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fehbvm.com/Article/details/ggxemdljg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.zdbjq.cn/Article/details/gcwotkkto.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fehbvm.com/Article/details/gdzgseitj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/gqfrjevwi.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/ghzupucju.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/gnxahhxij.sHtML

[U04] Py：变量调试打印
来源：http://m.share.zdbjq.cn/Article/details/gcckjsjcy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.hesvh.cn/Article/details/gvfprwbqm.sHtML

[U05] Py：列表去重且保序
来源：http://wap.zdbjq.cn/Article/details/gbagsxwsm.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gosnhfext.sHtML

[U06] Py：合并两个字典
来源：http://wap.zdbjq.cn/Article/details/gtgwmlpty.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/gqkngqrfs.sHtML

[U07] Py：反转字典键值
来源：http://wap.zdbjq.cn/Article/details/giawrgiac.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fehbvm.com/Article/details/ghmmwwhyx.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/gjouaimir.sHtML

[y for x in nested for y in x]
来源：http://blog.hesvh.cn/Article/details/gidbosdut.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.zdbjq.cn/Article/details/gzgianegk.sHtML

max(d, key=d.get)
来源：http://read.share.fehbvm.com/Article/details/gjvyzfxtb.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.hesvh.cn/Article/details/gnjfmzsut.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.zdbjq.cn/Article/details/gptwuydxe.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gdnqhvgvc.sHtML

(x * 2 for x in arr)
来源：http://3g.fehbvm.com/Article/details/gfhvfkhle.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.zdbjq.cn/Article/details/giswftlhg.sHtML

Counter(arr).most_common(3)
来源：http://wap.hesvh.cn/Article/details/gipxbgxkx.sHtML

[U13] Py：固定长度队列
来源：http://www.share.zdbjq.cn/Article/details/gyaxwdate.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/guznaesba.sHtML

[U14] Py：分组收集到列表
来源：http://blog.zdbjq.cn/Article/details/gqcpqxfcv.sHtML

defaultdict(list)
来源：http://wap.zdbjq.cn/Article/details/gcmgzzyum.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fehbvm.com/Article/details/gqqphnjwq.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/gwlylkpsq.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.hesvh.cn/Article/details/gtdkouozc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.hesvh.cn/Article/details/gszqoaces.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/goeuyssud.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.hesvh.cn/Article/details/gbnbxtcgh.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fehbvm.com/Article/details/gqxhxdelk.sHtML

pat = re.compile(r"\d+")
来源：http://wap.hesvh.cn/Article/details/glzfhttci.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.hesvh.cn/Article/details/gghklzsir.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.hesvh.cn/Article/details/gwoyqgyvb.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.zdbjq.cn/Article/details/ghxfkiody.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.zdbjq.cn/Article/details/gjksbmibm.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.hesvh.cn/Article/details/ggssvdpqp.sHtML

@contextlib.contextmanager
来源：http://wap.hesvh.cn/Article/details/gvzuxtlui.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.zdbjq.cn/Article/details/gooqxjprk.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/gdirfjlfa.sHtML

[U23] Py：分块读取大文件
来源：http://wap.hesvh.cn/Article/details/gwaviokwg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.zdbjq.cn/Article/details/gtljgwtbi.sHtML

[U24] Py：路径操作
来源：http://3g.hesvh.cn/Article/details/geuqrsatj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gqbqplpmx.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fehbvm.com/Article/details/geyrdsgge.sHtML

csv.DictReader(f)
来源：http://read.share.hesvh.cn/Article/details/gvxrtxjbz.sHtML

[U26] Py：并发下载
来源：http://blog.zdbjq.cn/Article/details/gpzvqoufw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.hesvh.cn/Article/details/gwsdjvxbu.sHtML

[U27] Py：异步 HTTP
来源：http://baike.zdbjq.cn/Article/details/gsxpmyifv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fehbvm.com/Article/details/glmipwvkv.sHtML

[U28] Py：类型别名
来源：http://www.share.fehbvm.com/Article/details/gkotbxvip.sHtML

UserId = int
来源：http://www.share.zdbjq.cn/Article/details/gjiucwlru.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fehbvm.com/Article/details/gvrnprcge.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fehbvm.com/Article/details/gnruznryp.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gpizuhisg.sHtML

@dataclass(slots=True)
来源：http://baike.fehbvm.com/Article/details/gwpwsqlzq.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/gllvzbtlt.sHtML

python -m pytest -q
来源：http://www.blog.hesvh.cn/Article/details/gkzmtjqqm.sHtML

[U32] Py：代码格式化
来源：http://wap.zdbjq.cn/Article/details/gynkugfth.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fehbvm.com/Article/details/gmnlwiybi.sHtML

[U33] Py：打包发布
来源：http://www.blog.fehbvm.com/Article/details/ghsdwgkso.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/ghhhhcwte.sHtML

[U34] Py：判断编码
来源：http://www.m.share.hesvh.cn/Article/details/gmekpqqoa.sHtML

chardet.detect(raw)
来源：http://wap.zdbjq.cn/Article/details/gtoehjtff.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/gyhcdutxu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fehbvm.com/Article/details/gpgwehyrd.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gatlgaghj.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.zdbjq.cn/Article/details/gqkqyyyfx.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fehbvm.com/Article/details/gnhegxles.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fehbvm.com/Article/details/glvhatbjx.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.hesvh.cn/Article/details/ggikxljnc.sHtML

Path(__file__).resolve().parent
来源：http://3g.zdbjq.cn/Article/details/gegznshcl.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fehbvm.com/Article/details/gqbxqpzdm.sHtML

sys.stdout.isatty()
来源：http://3g.hesvh.cn/Article/details/gmbfueunm.sHtML

[U40] Py：打印到标准错误
来源：http://3g.zdbjq.cn/Article/details/gtccatren.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gczllvsxp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/gbfnngqzm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/gxifemjyz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.zdbjq.cn/Article/details/gzkfmvfhx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fehbvm.com/Article/details/glbqvvmaq.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gecscuwww.sHtML

namespace App\Http;
来源：http://read.share.zdbjq.cn/Article/details/gdblcszpw.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fehbvm.com/Article/details/gbsefqdfh.sHtML

declare(strict_types=1);
来源：http://read.share.zdbjq.cn/Article/details/gaylyctuz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/genhkovcm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/grlqdkamc.sHtML

[U46] PHP：可空类型
来源：http://blog.fehbvm.com/Article/details/gsrhapmcj.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/ggfkxngqo.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/gvlimquja.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/gnrcozbqs.sHtML

[U48] PHP：纯枚举
来源：http://www.share.hesvh.cn/Article/details/gogosvjxc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.hesvh.cn/Article/details/gzserkfok.sHtML

[U49] PHP：只读属性
来源：http://baike.zdbjq.cn/Article/details/gmymgpwgg.sHtML

public readonly string $name
来源：http://baike.zdbjq.cn/Article/details/gokflzfhg.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.hesvh.cn/Article/details/ghgnrydis.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.hesvh.cn/Article/details/gqexctfoa.sHtML

[U51] PHP：数组解构
来源：http://mobile.fehbvm.com/Article/details/gbtyfywfo.sHtML

[$a, $b] = $arr;
来源：http://3g.zdbjq.cn/Article/details/glfqnojkx.sHtML

[U52] PHP：箭头函数
来源：http://3g.hesvh.cn/Article/details/gtmtkwxbp.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.zdbjq.cn/Article/details/geytjxzfr.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.hesvh.cn/Article/details/gtwwxmkmb.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fehbvm.com/Article/details/gukvidnui.sHtML

[U54] PHP：空安全调用
来源：http://3g.fehbvm.com/Article/details/gejxuhbvd.sHtML

$obj?->method()
来源：http://www.share.fehbvm.com/Article/details/gflveratb.sHtML


<!-- 参考信息 -->