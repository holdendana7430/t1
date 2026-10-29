代发 wailian999

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gpjtwuvye.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/goljrbojf.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/grntatcjs.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/geztieqzo.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/gephaduta.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gjkpixzmc.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gtmtbdmkh.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gigaskflb.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gktryfaof.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/gwbffcqmh.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.zdbjq.cn/Article/details/ggnfgzgtk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/ggdnztinx.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/gjtpxbfym.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gnucdvedz.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/gufslxers.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gtgsymxjw.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/gnxwpzlkm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gdykoxiqb.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/gtjazvzak.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gccfzsmed.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.zdbjq.cn/Article/details/gkqyrkxfr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gpknlalnq.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/gebptxjcm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gziizfdvo.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/gzlsnsuhf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gpqacllvm.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/glruwguil.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/getaibuuc.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gwznwmhhq.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/gnqrlsvdq.sHtML

[S44] C++：引用传参
来源：http://www.blog.hesvh.cn/Article/details/gddyfxamn.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/gecjqmrvr.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/gijhjxxsq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gudsrwnbt.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gnbejevsn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/gnijdyshr.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gxiktkhrm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaphkpech.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gakzxtljf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/gzselqjur.sHtML

while (std::getline(in, line)) { }
来源：http://baike.hesvh.cn/Article/details/grbmmucnx.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/gxhhrxgbr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/gxftwgmbr.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/ghhdzxjau.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/giftocejp.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/gavnzdpnu.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/ggwejyftc.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/gnfetiksu.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/gowlkqwwq.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/ghenekigx.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/gtuwhewck.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gizamnzep.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gylaqjizu.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/ggotwuizt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.hesvh.cn/Article/details/gszwczxqw.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/gwcrjxuyf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gdqydfigq.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/gmyidvtbn.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/gyhlhstxo.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gvghutzyp.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/gzojwutae.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/gthuxacso.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/glvkjdmkw.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gvpxshwgn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gfqidzamb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grqzuakni.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gkzbwzdty.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjxklehps.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gireqxxjs.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gaamzjcmj.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/grozqknmg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.hesvh.cn/Article/details/gserrrhha.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gbzozuukk.sHtML

"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gxgnnycne.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/govtheecj.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gwmiemisi.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/ghwthrgyy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/gifjvhpur.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gclsgjwmo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/glvbisufg.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/gqdbfokiw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/grqukmohs.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gwjrsfbix.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gegzlhjkx.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/gzblzdzsq.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/gaowomtpu.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/gxdkvxtsg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/glgurqlfm.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/grbokyjii.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/geedmtcln.sHtML

[T12] Kotlin：解构声明
来源：http://3g.hesvh.cn/Article/details/garvcbtyw.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gpuacupjw.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/gdydxqfhs.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/gpnukiatt.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/grdoamsmk.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gjcbtvvwu.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/gckwgkgkz.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/ghjyeflcn.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/gsrwopbsc.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gefrmthfj.sHtML

[T17] Swift：变量与常量
来源：http://m.share.hesvh.cn/Article/details/gwgujxqqj.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/goanbqwpe.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gcackofiv.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/ghwyyvnpc.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/ghbumivju.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.hesvh.cn/Article/details/gdxthqwho.sHtML

[T20] Swift：数组操作
来源：http://www.blog.hesvh.cn/Article/details/gvnlwqdga.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fehbvm.com/Article/details/gcvhkqkid.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/gbfxrysdz.sHtML

for x in a { print(x) }
来源：http://3g.zdbjq.cn/Article/details/gyowcydlv.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/gvwdpifoi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/gvvnexpyw.sHtML

[T23] Swift：函数
来源：http://wap.fehbvm.com/Article/details/ghlmrzoez.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/gyhknjtyu.sHtML

[T24] Swift：闭包
来源：http://www.share.zdbjq.cn/Article/details/gijkapcbn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gylmbzyeh.sHtML

[T25] Swift：结构体
来源：http://baike.hesvh.cn/Article/details/gjgboaewl.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gezexhzta.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/gnxxahsqb.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/guvnswcqm.sHtML

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/gddsaibti.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fehbvm.com/Article/details/gayrrdbdg.sHtML

[T28] Swift：枚举
来源：http://blog.fehbvm.com/Article/details/gtzeepxpd.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/giuietynj.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.zdbjq.cn/Article/details/gjyqpnfqe.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/gctczqjzf.sHtML

[T30] Swift：协议
来源：http://www.share.fehbvm.com/Article/details/gtluvicrr.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/ghfylixuc.sHtML

[T31] Lua：Hello World
来源：http://3g.hesvh.cn/Article/details/gmdujpcyv.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gspmgmscs.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/gyrhhrunr.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/ghcpvmqmp.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/gqmpqiiee.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/gfpuxajyg.sHtML

[T34] Lua：遍历表
来源：http://blog.hesvh.cn/Article/details/gicwlkasf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/gwjinjqbs.sHtML

[T35] Lua：字典表
来源：http://wap.fehbvm.com/Article/details/gishaybzf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.hesvh.cn/Article/details/guhrdmtbb.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/gezssrtnv.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/guoxtfolq.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gbpnqjepd.sHtML

"a" .. "b"
来源：http://www.m.share.zdbjq.cn/Article/details/gjkxsgrum.sHtML

[T38] Lua：条件
来源：http://www.share.hesvh.cn/Article/details/gilwekyla.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/glnqhzpuf.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gymjqeyld.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/gluhttumq.sHtML

[T40] Lua：元表
来源：http://baike.hesvh.cn/Article/details/getfdlhlg.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.hesvh.cn/Article/details/glwszxmyl.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gfxqlnojc.sHtML

print "Hello\n";
来源：http://wap.zdbjq.cn/Article/details/grmllciwg.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gcardmrqf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.hesvh.cn/Article/details/gqfevacld.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gtjbrfdkf.sHtML

"值: $a"
来源：http://read.share.zdbjq.cn/Article/details/gzxfrcnud.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/gwwjeqdod.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/gtzgbikjv.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/gukmyibhr.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/gjjsdyeiw.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/gnvneqyes.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/gjvtvzdfg.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.hesvh.cn/Article/details/gmpnlxqaf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/gctejyjio.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/gkkblepvf.sHtML

$s =~ s/old/new/g;
来源：http://m.share.hesvh.cn/Article/details/gpavgncoi.sHtML

[T49] Perl：函数
来源：http://m.share.fehbvm.com/Article/details/gpkfsxhsp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gohhdwzmt.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/ghyflkcdg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fehbvm.com/Article/details/gcqmonzws.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/gjmbtedpb.sHtML

[T51] Scala：Hello World
来源：http://3g.fehbvm.com/Article/details/ggwzhhvhg.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/glwsjruiq.sHtML

[T52] Scala：变量
来源：http://wap.fehbvm.com/Article/details/gwykzgeyl.sHtML

val a = 1;  var b = 2
来源：http://www.blog.hesvh.cn/Article/details/gkqnxgloc.sHtML

[T53] Scala：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gaswwkzty.sHtML

s"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gdbryflqq.sHtML

[T54] Scala：集合映射
来源：http://3g.hesvh.cn/Article/details/gosmlyyzz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.hesvh.cn/Article/details/gxoioecmh.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/grjowkcgn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.hesvh.cn/Article/details/gmrqbbfwu.sHtML

[T56] Scala：样例类
来源：http://blog.zdbjq.cn/Article/details/gglbayuxw.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.hesvh.cn/Article/details/ghdetmncl.sHtML

[T57] Scala：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gecwdmuuj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/gjwyhswjr.sHtML

[T58] Scala：函数定义
来源：http://www.share.fehbvm.com/Article/details/gxyiwyydq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/gzzgizrrp.sHtML

[T59] Scala：循环
来源：http://m.share.fehbvm.com/Article/details/gpbuzsocm.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gcpjicmts.sHtML

[T60] Scala：折叠
来源：http://www.share.zdbjq.cn/Article/details/gitzdolta.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.hesvh.cn/Article/details/gjhiisnzm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gedbrfvof.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gocqjblis.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghogxovqf.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fehbvm.com/Article/details/gtalpfety.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.hesvh.cn/Article/details/gvkpqbkns.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fehbvm.com/Article/details/gdxrwjjwm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/gcublzbpf.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fehbvm.com/Article/details/gqipmthtp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/gbiwkcnvx.sHtML

[U04] Py：变量调试打印
来源：http://3g.zdbjq.cn/Article/details/ghcfdifls.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/gytpdvstn.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.zdbjq.cn/Article/details/gvvjryvyg.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gownlnzgl.sHtML

[U06] Py：合并两个字典
来源：http://wap.fehbvm.com/Article/details/gnjvbxxld.sHtML

{**a, **b}
来源：http://3g.fehbvm.com/Article/details/gerokrxuo.sHtML

[U07] Py：反转字典键值
来源：http://m.share.hesvh.cn/Article/details/gxmubrknu.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.zdbjq.cn/Article/details/gibqiztov.sHtML

[U08] Py：展平二维列表
来源：http://www.share.zdbjq.cn/Article/details/grogmttlu.sHtML

[y for x in nested for y in x]
来源：http://blog.zdbjq.cn/Article/details/gkgksvapn.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.zdbjq.cn/Article/details/gfiugdbbq.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gfgpkgaxl.sHtML

[U10] Py：按值排序字典
来源：http://baike.fehbvm.com/Article/details/gcjgjlspf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/giomvwyif.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/gsmjaiexs.sHtML

(x * 2 for x in arr)
来源：http://blog.hesvh.cn/Article/details/galfdnkxp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.zdbjq.cn/Article/details/gstncvjms.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fehbvm.com/Article/details/gaouhvlck.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/glgwbbwjk.sHtML

deque(maxlen=10)
来源：http://wap.hesvh.cn/Article/details/gfwktqols.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fehbvm.com/Article/details/gsdrinhwk.sHtML

defaultdict(list)
来源：http://m.share.zdbjq.cn/Article/details/gzgycmyig.sHtML

[U15] Py：高精度计时
来源：http://www.share.zdbjq.cn/Article/details/gshqaxgvm.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/gqqhjhvuk.sHtML

[U16] Py：命令行参数解析
来源：http://3g.zdbjq.cn/Article/details/gwktihswu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fehbvm.com/Article/details/goepnnmbz.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gocembwkw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.zdbjq.cn/Article/details/gefinisal.sHtML

[U18] Py：预编译正则
来源：http://3g.fehbvm.com/Article/details/gafkwxcji.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gabensead.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fehbvm.com/Article/details/gnoczjquq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fehbvm.com/Article/details/gnzfgkdch.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.hesvh.cn/Article/details/gwmphvgyx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.hesvh.cn/Article/details/gilnowabr.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fehbvm.com/Article/details/gyebsjxkf.sHtML

@contextlib.contextmanager
来源：http://www.blog.fehbvm.com/Article/details/gehrcfmaz.sHtML

[U22] Py：矩阵转置
来源：http://baike.hesvh.cn/Article/details/gnisraqvn.sHtML

list(zip(*m))
来源：http://www.share.zdbjq.cn/Article/details/geuruwjkw.sHtML

[U23] Py：分块读取大文件
来源：http://3g.hesvh.cn/Article/details/gjaxdsnbk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fehbvm.com/Article/details/gfvajciyq.sHtML

[U24] Py：路径操作
来源：http://www.blog.hesvh.cn/Article/details/gnazzxxev.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gskcuyfci.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fehbvm.com/Article/details/gsrzazrzt.sHtML

csv.DictReader(f)
来源：http://baike.hesvh.cn/Article/details/gzegalofe.sHtML

[U26] Py：并发下载
来源：http://blog.zdbjq.cn/Article/details/gfyhhxyzm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.hesvh.cn/Article/details/gyjpkvcwz.sHtML

[U27] Py：异步 HTTP
来源：http://blog.hesvh.cn/Article/details/ghtdpjqmm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.zdbjq.cn/Article/details/gsvqytroi.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gkdjmolry.sHtML

UserId = int
来源：http://www.share.fehbvm.com/Article/details/gqqhmxfwb.sHtML

[U29] Py：属性校验
来源：http://www.m.share.zdbjq.cn/Article/details/gutsqlbpd.sHtML

@property 与 @x.setter 配合
来源：http://www.share.hesvh.cn/Article/details/gguhapgyn.sHtML

[U30] Py：数据类
来源：http://www.share.hesvh.cn/Article/details/gsmvqwkhq.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/grwajujec.sHtML

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/gkdnmrgbb.sHtML

python -m pytest -q
来源：http://www.m.share.fehbvm.com/Article/details/ghmynayzk.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gcxpuvoan.sHtML

ruff format . && ruff check --fix .
来源：http://blog.hesvh.cn/Article/details/gvvzmwgzf.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/gsotcxuqz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.hesvh.cn/Article/details/gwfwuvree.sHtML

[U34] Py：判断编码
来源：http://blog.fehbvm.com/Article/details/glcxhylyt.sHtML

chardet.detect(raw)
来源：http://www.share.hesvh.cn/Article/details/gykwkgqku.sHtML

[U35] Py：发送邮件
来源：http://blog.fehbvm.com/Article/details/gvjcpchoe.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fehbvm.com/Article/details/giyjmcpyj.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/gscztlwvq.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fehbvm.com/Article/details/goiucefoe.sHtML

[U37] Py：读写 Excel
来源：http://m.share.zdbjq.cn/Article/details/gtqbsnnuj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.zdbjq.cn/Article/details/giihptwvj.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.hesvh.cn/Article/details/gmgrhbpdx.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fehbvm.com/Article/details/gkjpshopl.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/gzggvfojn.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/gevnjrhtk.sHtML

[U40] Py：打印到标准错误
来源：http://baike.hesvh.cn/Article/details/gxarppsmq.sHtML

print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gxzshuwvm.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fehbvm.com/Article/details/gmqhhkruz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/gpahkuxdb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fehbvm.com/Article/details/gatdipwrd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fehbvm.com/Article/details/gxaovyuei.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gdyjdmkif.sHtML

namespace App\Http;
来源：http://m.share.zdbjq.cn/Article/details/gnfgrlpyc.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fehbvm.com/Article/details/ghgfkpncs.sHtML

declare(strict_types=1);
来源：http://blog.hesvh.cn/Article/details/glspfxqnh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/gahshzcjm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gvqbjyksx.sHtML

[U46] PHP：可空类型
来源：http://www.share.hesvh.cn/Article/details/gmyfbnrpc.sHtML

?string $name = null
来源：http://baike.hesvh.cn/Article/details/gxssgolhv.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/gffhkefmk.sHtML

int|string $id
来源：http://3g.zdbjq.cn/Article/details/gcqstnuzz.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fehbvm.com/Article/details/ghbxbouxm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gthlvciiz.sHtML

[U49] PHP：只读属性
来源：http://mobile.fehbvm.com/Article/details/gwdlnjqji.sHtML

public readonly string $name
来源：http://blog.zdbjq.cn/Article/details/gqmuifagb.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fehbvm.com/Article/details/gifgzkooj.sHtML

public function __construct(private int $id) {}
来源：http://wap.fehbvm.com/Article/details/gtwqcrnnf.sHtML

[U51] PHP：数组解构
来源：http://wap.fehbvm.com/Article/details/gnrtvbyjy.sHtML

[$a, $b] = $arr;
来源：http://blog.hesvh.cn/Article/details/ghaegqpmq.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gcrpiubya.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.zdbjq.cn/Article/details/gsrdcoqaj.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.hesvh.cn/Article/details/gphornhhf.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.hesvh.cn/Article/details/gfnpzpxcs.sHtML

[U54] PHP：空安全调用
来源：http://3g.zdbjq.cn/Article/details/gtzwhxdyx.sHtML

$obj?->method()
来源：http://blog.fehbvm.com/Article/details/gitniephj.sHtML


<!-- 参考信息 -->