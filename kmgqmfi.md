代发 wailian999

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/gtmoiytga.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gxxkaorhs.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/gneqqzzgi.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gjwqmfowc.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/gzxzdtovw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fehbvm.com/Article/details/gksdayssf.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/gmpjkyuhg.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/golrhtfjf.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/geotjkkgu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/gxfwsvfbu.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gvcukpies.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fehbvm.com/Article/details/gzzrlivlb.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/gsoghbobr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gilgfniht.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/gktmdvpdm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gnuhaokat.sHtML

[S37] C++：set
来源：http://3g.zdbjq.cn/Article/details/gkxrwkymk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gwfqbvxnw.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gflcgxwlu.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gsuyizjxl.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/gwvjhojim.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gkszatzya.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gzjxtikyy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gusnoplci.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gllvqyemb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/gxwowjcjr.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gzhmuznwn.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/gsxnjxbvg.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/ggskygxfo.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/gvxaexkjm.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/ghbzfpsvm.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/giqhazmco.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/gfnauvysx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gelovswuh.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/gjsexdzac.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/ghvyruxbt.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/geaoombcu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjmgvwwfy.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gfyfjciqk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gutszamwa.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gfhccgwpa.sHtML

[S49] C++：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gqqjnunqh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/glvaphwaa.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gtfrnqzun.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gvvkwoxwh.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/gwnqpbvoe.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gethdanku.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/gprxkxhro.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gtufznncg.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gpelztfxm.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.hesvh.cn/Article/details/ggzygshxh.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/gcytophdx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/giqnidfkv.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gtdyjddmf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/ghpmahydx.sHtML

[S56] C++：optional
来源：http://www.m.share.fehbvm.com/Article/details/grefzugui.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/gyjsfgvft.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gpkdxapqe.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gvmpdppdk.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/gczwhctzo.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/geumsmner.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gfprhoffx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/gtoafbhqb.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/ggrbtrijt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/glvhuzayp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grtnxzkcl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gpbzcryqm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggjcbossr.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gbnizywho.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/guqvurvqq.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/geyjblgiq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/gtbveneqw.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/gmuuxjuqf.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gkrzdvgoy.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/grorebnsa.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gexgfavgr.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/gzmxuxwod.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gysmxnmzo.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/glcilzvll.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gcobladve.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gktbehlxk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/gevmqbeml.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gtjseoxll.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/giwjahotv.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.hesvh.cn/Article/details/gibyopdvw.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gadscleec.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gckowmaew.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/gxnpzkovc.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/gtutgpgwi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/gokldtdnk.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gvlvwepcm.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gwvfgkqsc.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.zdbjq.cn/Article/details/glqblcmuo.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/gbttglaps.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gylmnejbg.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gjcgjfohm.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gjrpngxkz.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gyefnlayb.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/grkmndsyh.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/grxjtanpf.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/goojipcmu.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/grogdkedt.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/guknbnujp.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gnzeowxyl.sHtML

[T19] Swift：可选绑定
来源：http://3g.hesvh.cn/Article/details/gswxqcivw.sHtML

if let n = opt { print(n) }
来源：http://blog.fehbvm.com/Article/details/grehbxdci.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/ggdsyxrph.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/guqoibxuq.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/gyjtpamxn.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/gnhcalobn.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/gmbccpfpx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/gtmdhnaed.sHtML

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/giqwqtyxo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/gjwywmdfx.sHtML

[T24] Swift：闭包
来源：http://wap.hesvh.cn/Article/details/gwqynpook.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gtrkzinpq.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/giuqnsgeo.sHtML

struct P { var x: Int }
来源：http://m.share.fehbvm.com/Article/details/gwfwumdwg.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/gjewfhbgu.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/gycsbimoh.sHtML

[T27] Swift：错误处理
来源：http://mobile.hesvh.cn/Article/details/gclmimxyw.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/gzfsdmsxw.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gotdzpetl.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gnpatjzil.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gtldruqvy.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/gdamaixwe.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/gpitqmmum.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.hesvh.cn/Article/details/ghnwgoldo.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gfjuzjjmc.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gpnlsurgb.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/goprdeqfp.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/gyjhheakq.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fehbvm.com/Article/details/gnqjqmjdv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/gibkomwqj.sHtML

[T34] Lua：遍历表
来源：http://wap.fehbvm.com/Article/details/gekcvsuao.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/gqfphqqra.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gnmavqnrq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/gnszesebt.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/gmrnvvvbg.sHtML

function add(a, b) return a + b end
来源：http://read.share.zdbjq.cn/Article/details/gnrmtqrzs.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gwjudfnni.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/gqlmsnjkq.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/glxqyhrap.sHtML

if x > 0 then print("正") end
来源：http://www.share.hesvh.cn/Article/details/gngdngewl.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/goaojphmz.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/gzcaaoeyz.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/gwznwozmj.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/gxrupbdug.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/gasncutgz.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/gelozozsd.sHtML

[T42] Perl：变量类型
来源：http://read.share.fehbvm.com/Article/details/gnvoktask.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fehbvm.com/Article/details/gqxrhfwqs.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gmghxnmtb.sHtML

"值: $a"
来源：http://www.blog.zdbjq.cn/Article/details/gieqzoklj.sHtML

[T44] Perl：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gcxeckihj.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.zdbjq.cn/Article/details/gfikjrbum.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/gqcxkblwu.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.zdbjq.cn/Article/details/gixrpykok.sHtML

[T46] Perl：哈希操作
来源：http://mobile.hesvh.cn/Article/details/gciffubpt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.hesvh.cn/Article/details/ggmwbvgix.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/gsmwbgryh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.zdbjq.cn/Article/details/gnpgyvbxf.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/gblcfbmsd.sHtML

$s =~ s/old/new/g;
来源：http://baike.hesvh.cn/Article/details/gdtwbehff.sHtML

[T49] Perl：函数
来源：http://www.share.hesvh.cn/Article/details/genxokrpu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gycswqasl.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gppoleqwb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/gkqiooamc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/grusulkrd.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/guheltxxf.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gniquhtjw.sHtML

[T52] Scala：变量
来源：http://m.share.hesvh.cn/Article/details/ghyfuofyo.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/gvjnznlnb.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fehbvm.com/Article/details/getisqdwv.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/gjeqoiibo.sHtML

[T54] Scala：集合映射
来源：http://3g.hesvh.cn/Article/details/ggwcvglsd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gaaeyjlcz.sHtML

[T55] Scala：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gweugkbmg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fehbvm.com/Article/details/gmogdnbxl.sHtML

[T56] Scala：样例类
来源：http://baike.zdbjq.cn/Article/details/grsdboqcu.sHtML

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gehcbwrzl.sHtML

[T57] Scala：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gdhitxwuf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.hesvh.cn/Article/details/grzeujywt.sHtML

[T58] Scala：函数定义
来源：http://mobile.zdbjq.cn/Article/details/gcodnusen.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.hesvh.cn/Article/details/gunpjamdx.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gufrqnhla.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gllnrnqvl.sHtML

[T60] Scala：折叠
来源：http://baike.hesvh.cn/Article/details/gktebwjmg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/guswfrbfb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghjqgapxd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gmzqyuzbv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnxrmjhdi.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.zdbjq.cn/Article/details/gypepcuim.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fehbvm.com/Article/details/gpdnuruvs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/gslcxvlgf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.hesvh.cn/Article/details/gqbmpmnaw.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fehbvm.com/Article/details/geovxagns.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fehbvm.com/Article/details/gjpptqhkg.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gijfefjod.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.hesvh.cn/Article/details/gxytbenxy.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.hesvh.cn/Article/details/glggqxwgl.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gtvarwcca.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.zdbjq.cn/Article/details/gtqocmgdv.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/gwmosuksl.sHtML

[U07] Py：反转字典键值
来源：http://mobile.zdbjq.cn/Article/details/gqmnqylll.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/ggcnfyptx.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.zdbjq.cn/Article/details/grtrialtf.sHtML

[y for x in nested for y in x]
来源：http://blog.hesvh.cn/Article/details/gkuntxpuy.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.hesvh.cn/Article/details/gwmpehtwh.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/glkplkggh.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fehbvm.com/Article/details/gpwopbbqe.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/gxuatmyib.sHtML

[U11] Py：生成器表达式
来源：http://m.share.zdbjq.cn/Article/details/gqualzrkv.sHtML

(x * 2 for x in arr)
来源：http://blog.fehbvm.com/Article/details/gdtwwxwvh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/gbqdjcrko.sHtML

Counter(arr).most_common(3)
来源：http://3g.fehbvm.com/Article/details/glgraxucx.sHtML

[U13] Py：固定长度队列
来源：http://3g.zdbjq.cn/Article/details/gxvwxcils.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/gutxsjqwx.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/gkoacktbs.sHtML

defaultdict(list)
来源：http://3g.hesvh.cn/Article/details/ggdnwsimi.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/gkgwgooas.sHtML

t = time.perf_counter()
来源：http://www.m.share.fehbvm.com/Article/details/geokhvsto.sHtML

[U16] Py：命令行参数解析
来源：http://baike.zdbjq.cn/Article/details/gcboognne.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.zdbjq.cn/Article/details/ghnttdzwz.sHtML

[U17] Py：初始化日志
来源：http://www.share.zdbjq.cn/Article/details/gcxkwocrc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fehbvm.com/Article/details/gyyfshskr.sHtML

[U18] Py：预编译正则
来源：http://read.share.zdbjq.cn/Article/details/gavjahlci.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/gbwwylfgk.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.zdbjq.cn/Article/details/gghygtqsp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fehbvm.com/Article/details/gfekudlww.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fehbvm.com/Article/details/gadfojbrg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.zdbjq.cn/Article/details/ggbsdraiw.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.hesvh.cn/Article/details/gceqzwcpu.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/gehijxesq.sHtML

[U22] Py：矩阵转置
来源：http://wap.fehbvm.com/Article/details/gvrgggode.sHtML

list(zip(*m))
来源：http://baike.fehbvm.com/Article/details/gohdenjlm.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/gfvvjllsp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.zdbjq.cn/Article/details/ghrhyjteo.sHtML

[U24] Py：路径操作
来源：http://m.share.zdbjq.cn/Article/details/grdqpnfha.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/grjogwxwx.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fehbvm.com/Article/details/gqtrwdcha.sHtML

csv.DictReader(f)
来源：http://mobile.fehbvm.com/Article/details/gftfhxnnf.sHtML

[U26] Py：并发下载
来源：http://3g.fehbvm.com/Article/details/grozudrzf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/gxfjrxqqy.sHtML

[U27] Py：异步 HTTP
来源：http://wap.hesvh.cn/Article/details/gqbqfetig.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.zdbjq.cn/Article/details/gamrtxmcw.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/gtrrmrmrk.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/gyuhxytvv.sHtML

[U29] Py：属性校验
来源：http://www.m.share.hesvh.cn/Article/details/gtsruaibt.sHtML

@property 与 @x.setter 配合
来源：http://wap.hesvh.cn/Article/details/gjahqeiaf.sHtML

[U30] Py：数据类
来源：http://read.share.hesvh.cn/Article/details/ggkiqiyml.sHtML

@dataclass(slots=True)
来源：http://mobile.zdbjq.cn/Article/details/gngiromtt.sHtML

[U31] Py：单测
来源：http://www.share.hesvh.cn/Article/details/giollbyuv.sHtML

python -m pytest -q
来源：http://mobile.fehbvm.com/Article/details/gmdecgdmj.sHtML

[U32] Py：代码格式化
来源：http://3g.hesvh.cn/Article/details/glurulwub.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.hesvh.cn/Article/details/gyqrtwwon.sHtML

[U33] Py：打包发布
来源：http://3g.zdbjq.cn/Article/details/glitxuaii.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fehbvm.com/Article/details/gnaveabrf.sHtML

[U34] Py：判断编码
来源：http://wap.zdbjq.cn/Article/details/gzwzmidwr.sHtML

chardet.detect(raw)
来源：http://baike.fehbvm.com/Article/details/gfuylrsot.sHtML

[U35] Py：发送邮件
来源：http://www.share.fehbvm.com/Article/details/gcmjqvswh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.zdbjq.cn/Article/details/gdmzwccqo.sHtML

[U36] Py：定时任务
来源：http://mobile.zdbjq.cn/Article/details/gletnjgrm.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.hesvh.cn/Article/details/gbpaaxfkb.sHtML

[U37] Py：读写 Excel
来源：http://baike.fehbvm.com/Article/details/gkupkrgxw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.zdbjq.cn/Article/details/gaesnoicb.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.hesvh.cn/Article/details/gionrzdob.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.zdbjq.cn/Article/details/gejqaarmq.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.zdbjq.cn/Article/details/gwojkecua.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/gcmobpcph.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.zdbjq.cn/Article/details/gxzqxdhuf.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gliabvbfs.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/getsagljf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/gcmskpsqt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.zdbjq.cn/Article/details/gkovaqkdk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.hesvh.cn/Article/details/glrlhydvw.sHtML

[U43] PHP：声明命名空间
来源：http://3g.zdbjq.cn/Article/details/gqtclwuof.sHtML

namespace App\Http;
来源：http://www.m.share.fehbvm.com/Article/details/gewhcvlnr.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fehbvm.com/Article/details/gruzcycqx.sHtML

declare(strict_types=1);
来源：http://read.share.fehbvm.com/Article/details/gmxgzovua.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.hesvh.cn/Article/details/gbozvxwpe.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/glwrsssqj.sHtML

[U46] PHP：可空类型
来源：http://baike.fehbvm.com/Article/details/gjrhvkwqe.sHtML

?string $name = null
来源：http://www.share.fehbvm.com/Article/details/gqkdhgggr.sHtML

[U47] PHP：联合类型
来源：http://baike.zdbjq.cn/Article/details/gcapfcpuh.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/gcerakygb.sHtML

[U48] PHP：纯枚举
来源：http://wap.hesvh.cn/Article/details/gtngfaljn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.hesvh.cn/Article/details/gikgtpkuh.sHtML

[U49] PHP：只读属性
来源：http://www.blog.zdbjq.cn/Article/details/gnjwejqbt.sHtML

public readonly string $name
来源：http://www.share.zdbjq.cn/Article/details/gdfdmpuok.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fehbvm.com/Article/details/gmcldlyji.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/gaknccvcv.sHtML

[U51] PHP：数组解构
来源：http://baike.zdbjq.cn/Article/details/gaoieldye.sHtML

[$a, $b] = $arr;
来源：http://www.blog.hesvh.cn/Article/details/gnvawmuvz.sHtML

[U52] PHP：箭头函数
来源：http://baike.zdbjq.cn/Article/details/ghoeneyiw.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fehbvm.com/Article/details/ghiewvwff.sHtML

[U53] PHP：空合并运算符
来源：http://baike.fehbvm.com/Article/details/gxtesiszk.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.zdbjq.cn/Article/details/gjjjursxi.sHtML

[U54] PHP：空安全调用
来源：http://m.share.hesvh.cn/Article/details/gthzsspuc.sHtML

$obj?->method()
来源：http://www.m.share.hesvh.cn/Article/details/gtxahpiiq.sHtML


<!-- 参考信息 -->