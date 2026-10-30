代发 wailian999

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gsqjjeyih.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gveyrfagb.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gcqewspft.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gyeubvfoh.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gajdvmncb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtnhmdcc.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gdvewizlz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfxpxyoxy.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/ghnliabqw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvblcqdv.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gtefudavr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpwyalqj.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gaglgsulr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbnredrg.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gxbkgzxhm.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gvlbgfxkq.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxhkffkl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/grmuucjtr.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gcozxfmfn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gpaglbcol.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gkilbpaot.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsxizmig.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gputeyzwv.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gkijrekbw.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/goocaqlse.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/glgpaward.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/ghglqwovq.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gruybypxn.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdifwwfz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggwtnunp.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gruhzgkkd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gctorzjnq.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gznduofuu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagpielgm.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkqfqhjd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/goffvuqxx.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gioalpsby.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/ghxsiisah.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/goyztoqat.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxxefbue.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gcccsbxno.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gsyjiszor.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gvdndftxw.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyliguqh.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggragaaot.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubafmdgq.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjoiiios.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gcisukswm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecmdohbg.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gtlohijnz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqdwknxh.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygjhfcjl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdjhffcz.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gomztwqzw.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gznsoemwx.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/grvevnfsa.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gslsnynkk.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/grhsxmunf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gcoyrfudp.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gberjsygf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnpnpgmk.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gtgjvrexo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcdyfcob.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglyczisf.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhpwamok.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtglinlcu.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/ghukjjapw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gwfvufruo.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/gswxfppvt.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsycbdvgf.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gubipmnfg.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/geynuqknm.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqmdovuh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gmrpjfxma.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrcbbuik.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gfjkiivzg.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/glktwelcc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gzidysrbq.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gxhxwudfr.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzgsyxqb.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/gkarutmxn.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gotklnivz.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyibhiss.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzodmobg.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gsjnwfimj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjxdhtol.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvsnjmxe.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrewnydn.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjwqhzup.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gujwodrgl.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gycxoresj.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/groqzpygi.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjtsypmm.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gqdieyrvw.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbjpsfyx.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxasijsk.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwzvusfi.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvvdtecb.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/garjgyznt.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdirjpqfn.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubxepdpl.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbxigdcw.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlvxmiki.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcyyvgzr.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gzaviegfy.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/gdnspoqib.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrqsnxrz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gqasrhufc.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gshmcycxo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdvnvwdr.sHtML

[T24] Swift：闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/gsiyhuvxu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gloroigux.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcksfmfwm.sHtML

struct P { var x: Int }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghodfhqin.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/gkkvkrpbg.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosbulujv.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacighhse.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garlfrkfo.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gmyxnfgyg.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgancfqy.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/gwbexivph.sHtML

guard let x = opt else { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvfkwkez.sHtML

[T30] Swift：协议
来源：http://blog.fanxiaobao.xyz/Article/details/gwnftywto.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/ghbowfrhf.sHtML

[T31] Lua：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/ghiiixdnm.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/giyyudxuc.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gnzpqxakj.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkoxffexp.sHtML

[T33] Lua：表（数组）
来源：http://baike.fanxiaobao.xyz/Article/details/ghnqdqlwj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtmppixm.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/gjknguxsl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fanxiaobao.xyz/Article/details/gefhtjrgr.sHtML

[T35] Lua：字典表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydgjmzit.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvpeoljq.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gaentgnxw.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fanxiaobao.xyz/Article/details/grklqpafr.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gguoziyep.sHtML

"a" .. "b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrqrrsre.sHtML

[T38] Lua：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxzdjemb.sHtML

if x > 0 then print("正") end
来源：http://wap.fanxiaobao.xyz/Article/details/gxhakturx.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwseatgi.sHtML

string.find(s, "%d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gzgbjywsa.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/gfoczzwam.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fanxiaobao.xyz/Article/details/gruhkjrpb.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbcdtomp.sHtML

print "Hello\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gebjkipee.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsquvaywk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsenjzaxy.sHtML

[T43] Perl：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gvjeohvxx.sHtML

"值: $a"
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfszbnrj.sHtML

[T44] Perl：条件
来源：http://baike.fanxiaobao.xyz/Article/details/grzvtunup.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gotkkngjl.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcfdwpix.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gffqsozzm.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geygewlaz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbreauey.sHtML

[T47] Perl：正则捕获
来源：http://baike.fanxiaobao.xyz/Article/details/gyivtzdjy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkisbnbv.sHtML

[T48] Perl：正则替换
来源：http://baike.fanxiaobao.xyz/Article/details/gvjavwzyl.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fanxiaobao.xyz/Article/details/gefsblrhp.sHtML

[T49] Perl：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gioeervsq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdwkpkix.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbeutvfo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fanxiaobao.xyz/Article/details/gvkvlrnbi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkolthiuf.sHtML

[T51] Scala：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gnalperxu.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/geqtwzpaw.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/glisawunc.sHtML

val a = 1;  var b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gjuwqtdpn.sHtML

[T53] Scala：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gdusirwne.sHtML

s"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gfwmauzyc.sHtML

[T54] Scala：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gfytofwia.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbkqswlg.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gebokazmh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnduihvqu.sHtML

[T56] Scala：样例类
来源：http://www.share.fanxiaobao.xyz/Article/details/gaylpxqjh.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/glcyewrgi.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnsfhhri.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnbhaapm.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gynzsbktf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fanxiaobao.xyz/Article/details/ggqxemmha.sHtML

[T59] Scala：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjaoivgt.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gmoprveue.sHtML

[T60] Scala：折叠
来源：http://baike.fanxiaobao.xyz/Article/details/gihcysfen.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fanxiaobao.xyz/Article/details/gfcsgddvh.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gqcbzcioc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuvacunp.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgltrbma.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqgehdus.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuqdzqye.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/gjtbszgcx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fanxiaobao.xyz/Article/details/guuumfgni.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxzaihbb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhmuggan.sHtML

[U04] Py：变量调试打印
来源：http://blog.fanxiaobao.xyz/Article/details/gazrhfwap.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fanxiaobao.xyz/Article/details/gskkwljri.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/gyntivgmr.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gqjpsrlhz.sHtML

[U06] Py：合并两个字典
来源：http://blog.fanxiaobao.xyz/Article/details/gigazygrp.sHtML

{**a, **b}
来源：http://wap.fanxiaobao.xyz/Article/details/gwxauejvw.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhqexqzv.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjglgdeg.sHtML

[U08] Py：展平二维列表
来源：http://3g.fanxiaobao.xyz/Article/details/gmdzuawle.sHtML

[y for x in nested for y in x]
来源：http://wap.fanxiaobao.xyz/Article/details/gavzqcefv.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkcltvug.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqscnsyyu.sHtML

[U10] Py：按值排序字典
来源：http://baike.fanxiaobao.xyz/Article/details/gsdcujpch.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnyorgpr.sHtML

[U11] Py：生成器表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gsidouekw.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnosmeqqx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fanxiaobao.xyz/Article/details/gyazwvhya.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpwmhvxr.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfspzuyj.sHtML

deque(maxlen=10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwehlmbpu.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fanxiaobao.xyz/Article/details/gkyrorhkt.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/geugowpol.sHtML

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/gylvsitgs.sHtML

t = time.perf_counter()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpqrmxys.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/gxklabbsr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofodgkoh.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemdumeke.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtgyfzrb.sHtML

[U18] Py：预编译正则
来源：http://wap.fanxiaobao.xyz/Article/details/gglaqxuep.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/ggqixikpk.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fanxiaobao.xyz/Article/details/ggnruxiff.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/gfenlgqgp.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlabrmub.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbhrehot.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fanxiaobao.xyz/Article/details/goiyavzdj.sHtML

@contextlib.contextmanager
来源：http://3g.fanxiaobao.xyz/Article/details/grdocdkoi.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhkanpmf.sHtML

list(zip(*m))
来源：http://wap.fanxiaobao.xyz/Article/details/grcxohhwt.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/gsbocjfuw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fanxiaobao.xyz/Article/details/gftknvbwt.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gfvlcfldn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/grrljqaig.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/gogjcxyne.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfhhndhd.sHtML

[U26] Py：并发下载
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwdbtwxx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmjwjaxb.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/girvqbzya.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgtzsycp.sHtML

[U28] Py：类型别名
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrtewuzk.sHtML

UserId = int
来源：http://mobile.fanxiaobao.xyz/Article/details/gntrggeqz.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzipnsjnt.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/gqdjzceoe.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/glcsmwzxt.sHtML

@dataclass(slots=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gratiblyz.sHtML

[U31] Py：单测
来源：http://blog.fanxiaobao.xyz/Article/details/geaoxfmvb.sHtML

python -m pytest -q
来源：http://3g.fanxiaobao.xyz/Article/details/gnlujwpql.sHtML

[U32] Py：代码格式化
来源：http://blog.fanxiaobao.xyz/Article/details/grswlqrvm.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fanxiaobao.xyz/Article/details/gwfggqmrc.sHtML

[U33] Py：打包发布
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscleerdp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspefbmei.sHtML

[U34] Py：判断编码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzescxmx.sHtML

chardet.detect(raw)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggussieic.sHtML

[U35] Py：发送邮件
来源：http://m.share.fanxiaobao.xyz/Article/details/grjulacnr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fanxiaobao.xyz/Article/details/gaalfnltc.sHtML

[U36] Py：定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gsbdhmwbp.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fanxiaobao.xyz/Article/details/gfhnklbxo.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gosvndlkc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fanxiaobao.xyz/Article/details/gzqevhbky.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fanxiaobao.xyz/Article/details/ghojmyxhc.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fanxiaobao.xyz/Article/details/gnslizkjr.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxwqcmfj.sHtML

sys.stdout.isatty()
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgzthvgl.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fanxiaobao.xyz/Article/details/ggpegunra.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gohmukykf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gjroqgytr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fanxiaobao.xyz/Article/details/geadwzfkj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fanxiaobao.xyz/Article/details/grnhxutnm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gifhdqslz.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/ghqqesdli.sHtML

namespace App\Http;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqoswgwz.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gordmgqwz.sHtML

declare(strict_types=1);
来源：http://www.share.fanxiaobao.xyz/Article/details/goinzpmrm.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdjytibw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjmwkyvuf.sHtML

[U46] PHP：可空类型
来源：http://wap.fanxiaobao.xyz/Article/details/gubuewprn.sHtML

?string $name = null
来源：http://baike.fanxiaobao.xyz/Article/details/ggbhgrufe.sHtML

[U47] PHP：联合类型
来源：http://3g.fanxiaobao.xyz/Article/details/gqxmjxtpx.sHtML

int|string $id
来源：http://3g.fanxiaobao.xyz/Article/details/gwyheurqx.sHtML

[U48] PHP：纯枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gtycnziba.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnsxpgevz.sHtML

[U49] PHP：只读属性
来源：http://mobile.fanxiaobao.xyz/Article/details/gltjsythq.sHtML

public readonly string $name
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgzvczes.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fanxiaobao.xyz/Article/details/gigvnseve.sHtML

public function __construct(private int $id) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gizmerzjx.sHtML

[U51] PHP：数组解构
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqapdaop.sHtML

[$a, $b] = $arr;
来源：http://blog.fanxiaobao.xyz/Article/details/gutbmycuj.sHtML

[U52] PHP：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gzwyyoyfu.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gsuodbghl.sHtML

[U53] PHP：空合并运算符
来源：http://baike.fanxiaobao.xyz/Article/details/gxnzfrfrn.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fanxiaobao.xyz/Article/details/grlxoapwq.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyhnvnfi.sHtML

$obj?->method()
来源：http://blog.fanxiaobao.xyz/Article/details/gddfpcqdn.sHtML

[U55] PHP：match 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gxrjfyzsz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/gizdolkad.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyzjzvxh.sHtML

f(a: 1, b: 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gwaoxztua.sHtML


<!-- 参考信息 -->