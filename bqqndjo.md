代发 wailian999

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/gghekfuxf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gjsazndpg.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/glitwybem.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/geuhjggis.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/gvouoofab.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gyfvifiav.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gayelyysr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gthwejumu.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gnrrcnehd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gayskbtgl.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/gxgjssiey.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gtuzlbaeo.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gjgjoqdlz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/grnhbxclo.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gwbpyaxfw.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/gozoghrnd.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/glpjpknzj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/gmtkgvxlu.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gcvglirsw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/gxwjikano.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gwxkmcbxk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/grwkrnbbu.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/gygsoaldb.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gudkurcwk.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gitdmukkl.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/gfoyqasij.sHtML

[S44] C++：引用传参
来源：http://www.blog.hesvh.cn/Article/details/gxnkprnyl.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/gicjdwzfe.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/gltwylhaj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gajsrwhgf.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/guwtaggrj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gnntmhske.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/gojtrxffp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/grfaryhop.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gqpusdsbe.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/gbxgpuxss.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gimnisrvc.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gtppxtiqg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gxkngcyft.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gplyueylr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gjmomfxyi.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/gnvljjvxa.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gpejppprt.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/gjfdcfuip.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gvvgbsros.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/gsnrynbmb.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/gtuwxxfkg.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gdtwwkpca.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gnachudqr.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/gcemxqllk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/geovqmqrg.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/gcudhqupt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/gmlhhqius.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/gwtapdwcp.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/grarsuhep.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/gqtmrfabf.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fehbvm.com/Article/details/glltftigb.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gnpgzbhsm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/gecyapgel.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/ggjkypyxs.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gqggqkxfs.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/guazpoggc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gfmzahdsd.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfdrdofuu.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/gnhfwzovt.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/ggsqhikjx.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/gliuvflum.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/grgnmswhw.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gojfgodei.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gvtsjyqez.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/ggdmylwtx.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/gricqqkhf.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/gnqvzgfcm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/gwkyfdmrz.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/govdhszrj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gondpupqt.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gqvmiotil.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/gbzbcgjff.sHtML

[T08] Kotlin：数据类
来源：http://wap.fehbvm.com/Article/details/glutxqudg.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/gnfzdgzhb.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/gxlgjzekf.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/gmkdsgwav.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gozdqxelp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/getijvrxs.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/gtcugvgwz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/gqwsvcosb.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gwmrofsmz.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gchxvvqlw.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/gynmenoha.sHtML

val m = mapOf("a" to 1)
来源：http://wap.hesvh.cn/Article/details/galmnirgk.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/gjutytgch.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gepylxmfb.sHtML

[T15] Kotlin：接口
来源：http://m.share.hesvh.cn/Article/details/gnbclwddf.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/gzemisngu.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gvroicayu.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gddanfvmh.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gjhjivkka.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/gpkwjabcz.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gslhblrwf.sHtML

"值: \(b)"
来源：http://www.m.share.hesvh.cn/Article/details/gdnggkzsq.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/gixkkhnvu.sHtML

if let n = opt { print(n) }
来源：http://blog.fehbvm.com/Article/details/ghcrngude.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/gysulkhvy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/gaqliovok.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/geivuomxv.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/gipaxnllw.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gcbgtwlgt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.zdbjq.cn/Article/details/gybtartto.sHtML

[T23] Swift：函数
来源：http://m.share.zdbjq.cn/Article/details/gjalfeecu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gqtputnqx.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/gayebdlqo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gdfweqolr.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/gnwwioguk.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/gcmffdxow.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/gwkqctouz.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/gzsaeejwi.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/gcrdyfufj.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/gvuikqsdg.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gcbbvdgvj.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/gtbaphlwd.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/gpztqorkj.sHtML

guard let x = opt else { return }
来源：http://baike.fehbvm.com/Article/details/gzywiukql.sHtML

[T30] Swift：协议
来源：http://3g.hesvh.cn/Article/details/gcqqeegkz.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/gioppjhvl.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/garfwcahl.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/ggpjvamuu.sHtML

[T32] Lua：局部变量
来源：http://baike.fehbvm.com/Article/details/gylhqpykb.sHtML

local a = 1
来源：http://www.share.fehbvm.com/Article/details/gywhcipzi.sHtML

[T33] Lua：表（数组）
来源：http://m.share.hesvh.cn/Article/details/guadoejev.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fehbvm.com/Article/details/gbwrdmvoo.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gomzfnpkc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.zdbjq.cn/Article/details/gtxsdtdyk.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gupldeatg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gfvkpidre.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/gfnnyeplc.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/geaghbrem.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/gghbelmiz.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/gadxrnyhq.sHtML

[T38] Lua：条件
来源：http://read.share.zdbjq.cn/Article/details/ggserybwo.sHtML

if x > 0 then print("正") end
来源：http://mobile.fehbvm.com/Article/details/giuoyxedz.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/gmztebwmu.sHtML

string.find(s, "%d+")
来源：http://m.share.zdbjq.cn/Article/details/gkuuchttj.sHtML

[T40] Lua：元表
来源：http://3g.hesvh.cn/Article/details/gcvcbgqjl.sHtML

setmetatable({}, { __index = base })
来源：http://baike.zdbjq.cn/Article/details/grwunytkg.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gpkzkhctd.sHtML

print "Hello\n";
来源：http://baike.hesvh.cn/Article/details/gbbxltdsu.sHtML

[T42] Perl：变量类型
来源：http://read.share.fehbvm.com/Article/details/gopbvgify.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/ggpitleio.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/guyfvwwtf.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/gahkrpyig.sHtML

[T44] Perl：条件
来源：http://mobile.fehbvm.com/Article/details/gsnypypwv.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/gvjsikfka.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/gqyhgbrkj.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/ghcocgsom.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/gjcklyalj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.hesvh.cn/Article/details/gyrtgrnzk.sHtML

[T47] Perl：正则捕获
来源：http://m.share.hesvh.cn/Article/details/gyrqnxvcy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.hesvh.cn/Article/details/gichzcylb.sHtML

[T48] Perl：正则替换
来源：http://3g.hesvh.cn/Article/details/ggdiwafxe.sHtML

$s =~ s/old/new/g;
来源：http://read.share.hesvh.cn/Article/details/gqfndlbjs.sHtML

[T49] Perl：函数
来源：http://www.share.fehbvm.com/Article/details/guqakglbd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gjhijqtee.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/ggymrtjfr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/ggrmpugmv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gxbqgeomv.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gncmmavjx.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gbgupikla.sHtML

[T52] Scala：变量
来源：http://blog.zdbjq.cn/Article/details/ghltdjdyl.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/gtrhmkvib.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gczjqggvw.sHtML

s"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gcdbdzmix.sHtML

[T54] Scala：集合映射
来源：http://www.share.hesvh.cn/Article/details/goiidxvha.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/gkrfckdjw.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gxdwokwjl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fehbvm.com/Article/details/ggttnrbci.sHtML

[T56] Scala：样例类
来源：http://blog.zdbjq.cn/Article/details/glydhzspm.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gnzraebcw.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gxjgshscx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/ghmxgfxxm.sHtML

[T58] Scala：函数定义
来源：http://wap.zdbjq.cn/Article/details/gphxwpgui.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/gvfvqguuy.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/gugjsubla.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fehbvm.com/Article/details/guxxgsekd.sHtML

[T60] Scala：折叠
来源：http://m.share.zdbjq.cn/Article/details/gtamrtees.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.hesvh.cn/Article/details/gupwfcxap.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghuiyyukm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gzyemtfqm.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gobhigeng.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fehbvm.com/Article/details/gtmfgwani.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.hesvh.cn/Article/details/gzkuaymla.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/gzgagsisu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/ghkxexwbw.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/gcgjcswsi.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/gkehmvklk.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gulyrwsgq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.hesvh.cn/Article/details/gnucxcmii.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.zdbjq.cn/Article/details/goqezxfjn.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/grdqezoge.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/gdbbqosfa.sHtML

{**a, **b}
来源：http://mobile.zdbjq.cn/Article/details/gbglyfdnf.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/gnqfvubsg.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.hesvh.cn/Article/details/glddsywad.sHtML

[U08] Py：展平二维列表
来源：http://www.share.zdbjq.cn/Article/details/gxiazrxxs.sHtML

[y for x in nested for y in x]
来源：http://read.share.zdbjq.cn/Article/details/grueshqum.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.zdbjq.cn/Article/details/gfwgjcalb.sHtML

max(d, key=d.get)
来源：http://3g.fehbvm.com/Article/details/glscoxeer.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/gerjygjyb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.hesvh.cn/Article/details/gdimtbyva.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fehbvm.com/Article/details/gymqpqjva.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/gxrulzxlb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.zdbjq.cn/Article/details/giejircyz.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/gtbztvbut.sHtML

[U13] Py：固定长度队列
来源：http://mobile.hesvh.cn/Article/details/gvknykmgw.sHtML

deque(maxlen=10)
来源：http://m.share.zdbjq.cn/Article/details/gbaceucgs.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fehbvm.com/Article/details/gtefyobcp.sHtML

defaultdict(list)
来源：http://wap.zdbjq.cn/Article/details/glevwzfks.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/gacfkykhd.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/gmshodvog.sHtML

[U16] Py：命令行参数解析
来源：http://3g.hesvh.cn/Article/details/gmxdfxhmd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fehbvm.com/Article/details/grwxwvndg.sHtML

[U17] Py：初始化日志
来源：http://3g.hesvh.cn/Article/details/gbdxpxnss.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fehbvm.com/Article/details/gbrbapamf.sHtML

[U18] Py：预编译正则
来源：http://mobile.fehbvm.com/Article/details/gigfzvwni.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gmxoeudua.sHtML

[U19] Py：正则替换带回调
来源：http://baike.hesvh.cn/Article/details/gwkxdcefk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fehbvm.com/Article/details/gtilyivfi.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/gtwphnapz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fehbvm.com/Article/details/gslixgjuu.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.zdbjq.cn/Article/details/gkvmepivp.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/gtkigobgc.sHtML

[U22] Py：矩阵转置
来源：http://blog.zdbjq.cn/Article/details/guyteybjd.sHtML

list(zip(*m))
来源：http://baike.hesvh.cn/Article/details/grjhevnne.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fehbvm.com/Article/details/gtswwukco.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fehbvm.com/Article/details/ghnaqtoei.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/gsdnjjvys.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gwjzxmfec.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.zdbjq.cn/Article/details/gqbyyasfd.sHtML

csv.DictReader(f)
来源：http://m.share.hesvh.cn/Article/details/gvidampdl.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/glfxonghq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fehbvm.com/Article/details/gvcjoeeso.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fehbvm.com/Article/details/gomqioayf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.zdbjq.cn/Article/details/guiqqszav.sHtML

[U28] Py：类型别名
来源：http://www.blog.zdbjq.cn/Article/details/gnozuhfff.sHtML

UserId = int
来源：http://www.share.fehbvm.com/Article/details/gsukwzuiz.sHtML

[U29] Py：属性校验
来源：http://blog.zdbjq.cn/Article/details/gosqwltmb.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fehbvm.com/Article/details/giojlfadp.sHtML

[U30] Py：数据类
来源：http://www.share.fehbvm.com/Article/details/gxyqejgmf.sHtML

@dataclass(slots=True)
来源：http://baike.hesvh.cn/Article/details/gaxprqeht.sHtML

[U31] Py：单测
来源：http://baike.fehbvm.com/Article/details/gctgkehqn.sHtML

python -m pytest -q
来源：http://3g.hesvh.cn/Article/details/ggusbmmcj.sHtML

[U32] Py：代码格式化
来源：http://blog.hesvh.cn/Article/details/gwzpkqxfr.sHtML

ruff format . && ruff check --fix .
来源：http://3g.hesvh.cn/Article/details/geizbapgr.sHtML

[U33] Py：打包发布
来源：http://www.blog.fehbvm.com/Article/details/gtmrdkgyu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fehbvm.com/Article/details/gknvpzkqj.sHtML

[U34] Py：判断编码
来源：http://m.share.hesvh.cn/Article/details/gttsmdnle.sHtML

chardet.detect(raw)
来源：http://blog.fehbvm.com/Article/details/gxhdkpxrj.sHtML

[U35] Py：发送邮件
来源：http://wap.zdbjq.cn/Article/details/gmaalqsrl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fehbvm.com/Article/details/gzteantok.sHtML

[U36] Py：定时任务
来源：http://baike.zdbjq.cn/Article/details/gyfqcwdtw.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fehbvm.com/Article/details/gmmyybixq.sHtML

[U37] Py：读写 Excel
来源：http://m.share.zdbjq.cn/Article/details/gztkgxdio.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.hesvh.cn/Article/details/ghsjqvyad.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fehbvm.com/Article/details/gnioehkqe.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.hesvh.cn/Article/details/gwvhcuezo.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.zdbjq.cn/Article/details/gxzihczij.sHtML

sys.stdout.isatty()
来源：http://wap.zdbjq.cn/Article/details/gpuwuddxg.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.zdbjq.cn/Article/details/gojktfqbp.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gmthgciwt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.hesvh.cn/Article/details/gbgyqagva.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.hesvh.cn/Article/details/gabeeuvej.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/gpctlsrdv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/gtooiqlur.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/gvajjsitn.sHtML

namespace App\Http;
来源：http://m.share.fehbvm.com/Article/details/gdtzyhscq.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fehbvm.com/Article/details/gjhitkeqd.sHtML

declare(strict_types=1);
来源：http://baike.fehbvm.com/Article/details/gpjrvsfcq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fehbvm.com/Article/details/gufprppoh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gsrhovylx.sHtML

[U46] PHP：可空类型
来源：http://www.blog.hesvh.cn/Article/details/ggkezwmka.sHtML

?string $name = null
来源：http://www.m.share.fehbvm.com/Article/details/gwqrswklc.sHtML

[U47] PHP：联合类型
来源：http://www.share.fehbvm.com/Article/details/grefyyquh.sHtML

int|string $id
来源：http://www.blog.hesvh.cn/Article/details/gsbuvjqrx.sHtML

[U48] PHP：纯枚举
来源：http://read.share.hesvh.cn/Article/details/gvphxkcur.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.hesvh.cn/Article/details/gccydjulh.sHtML

[U49] PHP：只读属性
来源：http://3g.hesvh.cn/Article/details/gusjsasmf.sHtML

public readonly string $name
来源：http://3g.zdbjq.cn/Article/details/gdkrtjpxv.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fehbvm.com/Article/details/ghrbqxfsh.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/gsknwjmpm.sHtML

[U51] PHP：数组解构
来源：http://3g.zdbjq.cn/Article/details/gpikpvsfz.sHtML

[$a, $b] = $arr;
来源：http://wap.hesvh.cn/Article/details/gfsdzwjgy.sHtML

[U52] PHP：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gtnvuzbcn.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.zdbjq.cn/Article/details/glwolqkdr.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/gghlgfayl.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fehbvm.com/Article/details/goitwcvlb.sHtML

[U54] PHP：空安全调用
来源：http://blog.hesvh.cn/Article/details/gzzsqwwac.sHtML

$obj?->method()
来源：http://mobile.fehbvm.com/Article/details/gidnytxgn.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fehbvm.com/Article/details/gtsaockuo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/gqmhrdhcz.sHtML

[U56] PHP：命名参数
来源：http://mobile.fehbvm.com/Article/details/gpgntvhxl.sHtML

f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gthffdkkh.sHtML


<!-- 参考信息 -->