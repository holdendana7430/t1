代发 wailian999

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/ghoxcvhrt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gpqgilffa.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/ghbithiic.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gsxhlygpt.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/gyyplsdbd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/gqppkheik.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gqqfhxsud.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.zdbjq.cn/Article/details/glayknpjs.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/gelpkhblq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/grczcvtqp.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gzhbffouj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/ganzzatxg.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/ggctnfpzx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gciblsmce.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gijezhtlq.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/guucddndw.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/ggzqgnqdc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gezsxpche.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gmehnavai.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/gbhmcgwvq.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/gwweuoxsc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/gsamtriyr.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gdpkrrgrt.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gfpjgsbxr.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gltlcpvsm.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gyaeljvst.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/ghojuvsyo.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/goqtqjsex.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gimlsrznb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/gvgqfxbwg.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gocvneras.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gasdhigeb.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/gmwbvhzci.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/gabssoblu.sHtML

[S48] C++：逐行读文件
来源：http://blog.fehbvm.com/Article/details/grwupbuho.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/gvglgqhqr.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/gqnyykukg.sHtML

[S49] C++：写文件
来源：http://m.share.fehbvm.com/Article/details/gqeogmxmm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gdjkkqsvl.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gjhijqerw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gphvceyyh.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/ggbvjoxla.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/gqialdllh.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gobsyebjs.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/gqtjdwehm.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/grplyawgi.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/gqigljgak.sHtML

[S54] C++：异常处理
来源：http://read.share.hesvh.cn/Article/details/grprysjol.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/glvsusjeh.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gpxjtytjf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gdvivhdhb.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gfdhtrgje.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gvzjgxmph.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/gtqsfxzdb.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gbaqydmdr.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gsjyyxows.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gyykxpqkc.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/gtbiepueb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fehbvm.com/Article/details/gzzarvree.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fehbvm.com/Article/details/gokqfikhf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/gfplisfaq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnbucstbr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/getlnvnwx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmrkfldmq.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/gfuzbmkqz.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gwmjyipeg.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gtgpkbxwj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.zdbjq.cn/Article/details/gwrravmiy.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.hesvh.cn/Article/details/gdsbyfcah.sHtML

"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gplrupgdw.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/gugjwjbyj.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/grlgfvccd.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/gyzqzspcv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gfgrtueev.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gmapvypuw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gunthztrl.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/gdgblrehb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/gtpxzmihg.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/gkxaqrpwh.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/ghlngorof.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/gstbhkinj.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/gjmkdyhdy.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/gmlnwwfyt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.hesvh.cn/Article/details/gurxbdkko.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/giupiqscq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fehbvm.com/Article/details/ghjfecaoy.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gsiqgezex.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gpbrmzxij.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/gzbhgqsae.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/gxidzwbpq.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/gwmsfmnmx.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gqwqpdbhn.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/gsnbbxxeb.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gpdcuncpr.sHtML

[T16] Swift：Hello World
来源：http://baike.zdbjq.cn/Article/details/giggdlhqu.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gnsujiuvd.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/ghaobfycf.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gjvjiwieg.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/giuiakedg.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/gfkqktijh.sHtML

[T19] Swift：可选绑定
来源：http://wap.hesvh.cn/Article/details/gzyinynng.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/gdlhrssgd.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/ghavpxkbg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/gjvlzuflz.sHtML

[T21] Swift：遍历
来源：http://3g.fehbvm.com/Article/details/gcrhiapnb.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/gpiwimglz.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/gibfnhhkg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.hesvh.cn/Article/details/gidhxfhjg.sHtML

[T23] Swift：函数
来源：http://www.share.fehbvm.com/Article/details/gpoazpmci.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/glvqwbpxd.sHtML

[T24] Swift：闭包
来源：http://blog.fehbvm.com/Article/details/gghmmrngo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/glfqsubbj.sHtML

[T25] Swift：结构体
来源：http://blog.zdbjq.cn/Article/details/gkgpcmnys.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gejjnfexg.sHtML

[T26] Swift：类与重写
来源：http://blog.zdbjq.cn/Article/details/gpiddehed.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/giuzbwmlx.sHtML

[T27] Swift：错误处理
来源：http://baike.hesvh.cn/Article/details/gxlyoqbhs.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.hesvh.cn/Article/details/gosagfweu.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/gvkbvpzhp.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/gnenjdfsc.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fehbvm.com/Article/details/gfttrnbzb.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/gpietyoyn.sHtML

[T30] Swift：协议
来源：http://www.share.zdbjq.cn/Article/details/grdlqjkxe.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/gmghiagdn.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gisfpvara.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gctntyzat.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/gikslublt.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gbsgzlmyg.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/grfjyvknj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.hesvh.cn/Article/details/ghsnulags.sHtML

[T34] Lua：遍历表
来源：http://mobile.fehbvm.com/Article/details/gjpgntska.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.hesvh.cn/Article/details/gytiwnpnu.sHtML

[T35] Lua：字典表
来源：http://wap.hesvh.cn/Article/details/gnjcpvgpx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.hesvh.cn/Article/details/gzhmwshvz.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gmjjvwqtl.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.hesvh.cn/Article/details/gzzsvdcxb.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fehbvm.com/Article/details/ghktxxwqi.sHtML

"a" .. "b"
来源：http://www.blog.zdbjq.cn/Article/details/gfirpuvck.sHtML

[T38] Lua：条件
来源：http://www.share.zdbjq.cn/Article/details/gxropibpj.sHtML

if x > 0 then print("正") end
来源：http://mobile.hesvh.cn/Article/details/gguvtpthi.sHtML

[T39] Lua：模式匹配
来源：http://3g.fehbvm.com/Article/details/gsaxkeuiu.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/gdzikaetv.sHtML

[T40] Lua：元表
来源：http://www.blog.fehbvm.com/Article/details/gmvznywdf.sHtML

setmetatable({}, { __index = base })
来源：http://wap.zdbjq.cn/Article/details/gyesexnfv.sHtML

[T41] Perl：Hello World
来源：http://www.share.hesvh.cn/Article/details/geiotjofv.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/gtythifxe.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/gireajald.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fehbvm.com/Article/details/gkbtlirjn.sHtML

[T43] Perl：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gfmelrfor.sHtML

"值: $a"
来源：http://wap.zdbjq.cn/Article/details/gdecjhmwg.sHtML

[T44] Perl：条件
来源：http://m.share.fehbvm.com/Article/details/grjxbzvyd.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fehbvm.com/Article/details/gaexeeybt.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/grannrlgh.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/gbmpknvrp.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gteufihzh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fehbvm.com/Article/details/giineamid.sHtML

[T47] Perl：正则捕获
来源：http://baike.hesvh.cn/Article/details/gbcyxpvbv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/gfimldwzq.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/gkctaxept.sHtML

$s =~ s/old/new/g;
来源：http://read.share.hesvh.cn/Article/details/gxyxhkdeq.sHtML

[T49] Perl：函数
来源：http://www.blog.fehbvm.com/Article/details/griaslgnq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/glqaraika.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gtmwtxwyi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fehbvm.com/Article/details/gbkratnod.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.hesvh.cn/Article/details/gykgkcavu.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/gdmmvnbrn.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gqohwwgix.sHtML

[T52] Scala：变量
来源：http://www.share.zdbjq.cn/Article/details/gngggfwgu.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/gwvfwnjza.sHtML

[T53] Scala：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gbgxdzcmf.sHtML

s"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gulxdwkcx.sHtML

[T54] Scala：集合映射
来源：http://baike.zdbjq.cn/Article/details/gxaeryqyp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.hesvh.cn/Article/details/gmytjosej.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gxfsouijy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.hesvh.cn/Article/details/gmovpxoos.sHtML

[T56] Scala：样例类
来源：http://www.m.share.hesvh.cn/Article/details/gjotqcjns.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gnffxtwlg.sHtML

[T57] Scala：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gotcfoupz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.hesvh.cn/Article/details/gluhfsrqd.sHtML

[T58] Scala：函数定义
来源：http://read.share.fehbvm.com/Article/details/gtavtxqjx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.hesvh.cn/Article/details/ggtecqtas.sHtML

[T59] Scala：循环
来源：http://m.share.fehbvm.com/Article/details/gqbezmhrh.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gnhqfdfex.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/gbzffgimc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.zdbjq.cn/Article/details/gnwgqasqg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gyqgslzsl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/geylzcwgw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/guxbepovz.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/gmhbycbtz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/gnllrchxz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.hesvh.cn/Article/details/gxndljcmd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.zdbjq.cn/Article/details/gttaxmrah.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.hesvh.cn/Article/details/gjedajetz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/gwdrpcvig.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/gjhfpichf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.zdbjq.cn/Article/details/gljxgbwdw.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fehbvm.com/Article/details/gaglwracp.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/grbflvcbt.sHtML

[U06] Py：合并两个字典
来源：http://blog.zdbjq.cn/Article/details/ghmnxrapt.sHtML

{**a, **b}
来源：http://baike.hesvh.cn/Article/details/ggsufkbzx.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/gldmdokle.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.hesvh.cn/Article/details/ggvhwejfz.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/gxjglcbjc.sHtML

[y for x in nested for y in x]
来源：http://m.share.hesvh.cn/Article/details/gxhnxjnkz.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fehbvm.com/Article/details/gnmbxkcwx.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/gdmhgnbde.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.hesvh.cn/Article/details/gsmddtpot.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fehbvm.com/Article/details/gspahxdaq.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fehbvm.com/Article/details/gqyblasxz.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/gniorodlu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fehbvm.com/Article/details/gxmropqzd.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fehbvm.com/Article/details/gadhoanlh.sHtML

[U13] Py：固定长度队列
来源：http://baike.zdbjq.cn/Article/details/graghewcb.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/glzdbpbtw.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fehbvm.com/Article/details/gbzrzqpeb.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gosuultdp.sHtML

[U15] Py：高精度计时
来源：http://blog.hesvh.cn/Article/details/gxxrnsrzs.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/gvwktcmvg.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fehbvm.com/Article/details/gnzmqvoeu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gdaxvfinm.sHtML

[U17] Py：初始化日志
来源：http://www.blog.zdbjq.cn/Article/details/gfejkqndl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.hesvh.cn/Article/details/gfgdcerxg.sHtML

[U18] Py：预编译正则
来源：http://read.share.hesvh.cn/Article/details/glznznllx.sHtML

pat = re.compile(r"\d+")
来源：http://baike.hesvh.cn/Article/details/ggsayqtho.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.hesvh.cn/Article/details/gwaryscpu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.zdbjq.cn/Article/details/grkssupxl.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.hesvh.cn/Article/details/gutdxprsc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.hesvh.cn/Article/details/gdmgnwibv.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.hesvh.cn/Article/details/gibvvbqvr.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/gxrmjnsvu.sHtML

[U22] Py：矩阵转置
来源：http://baike.hesvh.cn/Article/details/gekqcpmrr.sHtML

list(zip(*m))
来源：http://read.share.zdbjq.cn/Article/details/gatfsbysc.sHtML

[U23] Py：分块读取大文件
来源：http://baike.hesvh.cn/Article/details/gdqsvjlcx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.hesvh.cn/Article/details/gfwdhvdxm.sHtML

[U24] Py：路径操作
来源：http://read.share.fehbvm.com/Article/details/gugzlspvu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gqnzzaszw.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.zdbjq.cn/Article/details/gvoqnfiwm.sHtML

csv.DictReader(f)
来源：http://www.blog.zdbjq.cn/Article/details/gewdtttzw.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/gdvozcihq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.hesvh.cn/Article/details/gndxrhejv.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.hesvh.cn/Article/details/gebnrynyp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.zdbjq.cn/Article/details/gxnkejwah.sHtML

[U28] Py：类型别名
来源：http://3g.zdbjq.cn/Article/details/gctqpygoq.sHtML

UserId = int
来源：http://baike.zdbjq.cn/Article/details/gmatpeqvv.sHtML

[U29] Py：属性校验
来源：http://www.share.zdbjq.cn/Article/details/gmlwdrhdz.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fehbvm.com/Article/details/gborphypf.sHtML

[U30] Py：数据类
来源：http://3g.hesvh.cn/Article/details/gjyvhotip.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fehbvm.com/Article/details/gshjhysuz.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/gjnlyyhed.sHtML

python -m pytest -q
来源：http://wap.fehbvm.com/Article/details/gegpidaae.sHtML

[U32] Py：代码格式化
来源：http://baike.zdbjq.cn/Article/details/gnvcwocgf.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fehbvm.com/Article/details/gqygxrsdh.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/gpmyjivnz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/goczmphbb.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/gbgqtozuv.sHtML

chardet.detect(raw)
来源：http://blog.zdbjq.cn/Article/details/girbylblz.sHtML

[U35] Py：发送邮件
来源：http://3g.zdbjq.cn/Article/details/guojhtypo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.zdbjq.cn/Article/details/gkzigwhbm.sHtML

[U36] Py：定时任务
来源：http://www.share.zdbjq.cn/Article/details/gfauxwrdv.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fehbvm.com/Article/details/gnphkpclk.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.zdbjq.cn/Article/details/gkkhjrxpj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fehbvm.com/Article/details/gjmuzkxrj.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.zdbjq.cn/Article/details/gvqwyrpik.sHtML

Path(__file__).resolve().parent
来源：http://wap.hesvh.cn/Article/details/gmxddqdhk.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/gscbwbkcm.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/guvmfsftp.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fehbvm.com/Article/details/gazcffpqt.sHtML

print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/grlcpzzfq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fehbvm.com/Article/details/gfxfpwmwc.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/gvjzmhgtb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.hesvh.cn/Article/details/gocmlfkig.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fehbvm.com/Article/details/gqulisypa.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.hesvh.cn/Article/details/gcrkqimnn.sHtML

namespace App\Http;
来源：http://www.share.fehbvm.com/Article/details/goxarqucr.sHtML

[U44] PHP：开启严格类型
来源：http://3g.hesvh.cn/Article/details/gemmqsvdl.sHtML

declare(strict_types=1);
来源：http://m.share.hesvh.cn/Article/details/gqscupdoa.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.zdbjq.cn/Article/details/gqoqgyejl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/guomsjnpt.sHtML

[U46] PHP：可空类型
来源：http://read.share.fehbvm.com/Article/details/gnupbkqka.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/gklbnaraj.sHtML

[U47] PHP：联合类型
来源：http://read.share.fehbvm.com/Article/details/gfmscjqqd.sHtML

int|string $id
来源：http://wap.zdbjq.cn/Article/details/gzywkrxzv.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fehbvm.com/Article/details/govoihqpx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.hesvh.cn/Article/details/gzccjksmu.sHtML

[U49] PHP：只读属性
来源：http://mobile.zdbjq.cn/Article/details/goufrbkem.sHtML

public readonly string $name
来源：http://wap.hesvh.cn/Article/details/gbumyjyxj.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fehbvm.com/Article/details/gqbsumpsi.sHtML

public function __construct(private int $id) {}
来源：http://m.share.hesvh.cn/Article/details/gwnctkpxd.sHtML

[U51] PHP：数组解构
来源：http://baike.zdbjq.cn/Article/details/gkxhlkibf.sHtML

[$a, $b] = $arr;
来源：http://m.share.hesvh.cn/Article/details/gjgasgcnx.sHtML

[U52] PHP：箭头函数
来源：http://baike.fehbvm.com/Article/details/gvyrphhpx.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gngnaaiyg.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/gnkqaheyc.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.zdbjq.cn/Article/details/glrgrorst.sHtML

[U54] PHP：空安全调用
来源：http://m.share.zdbjq.cn/Article/details/gcndblwxw.sHtML

$obj?->method()
来源：http://read.share.hesvh.cn/Article/details/gzdhflsmy.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fehbvm.com/Article/details/guxkpxplt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/gjnlvmyoi.sHtML

[U56] PHP：命名参数
来源：http://3g.hesvh.cn/Article/details/gruxfimet.sHtML

f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/ghjkdbjzv.sHtML


<!-- 参考信息 -->