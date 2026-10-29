代发 wailian999

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/gxoyhrulp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/gvuvqkgfy.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gdpicscgw.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gcedoaszw.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/glisddjky.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fehbvm.com/Article/details/gubiioxgs.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/gfhoizppx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gwvbwrzpk.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/gvikjrhby.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/guyvzzphz.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/gmcethqtt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/giexlxpna.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/ghclkeoog.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/gkjmjtsdo.sHtML

[S38] C++：排序
来源：http://3g.zdbjq.cn/Article/details/gilugodqp.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gedoyftni.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gelzyjnch.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gttypcrvw.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gqafkwjpi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gpnxqfqlk.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/grdwgzvmp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gibmomkdg.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gwdgvbfyn.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gulawcraf.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/gdbyoxkhq.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gzlevbabn.sHtML

[S44] C++：引用传参
来源：http://mobile.hesvh.cn/Article/details/gzgvjxtyr.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/geiebckiu.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gtmkmaqop.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gxzcfjcng.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gkhaskeat.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/glougyieq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gvtxjxhjn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/giiyewhrm.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gufrtgdnw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/gvblhgbuh.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/grpestaia.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/gzjpwvhcn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/gyamrvvhz.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/geoweosma.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gxtqgcjcf.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gyvhubrnd.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/gxwqmrwxj.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/glayxpygk.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gnuvmadqe.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gukjakdxa.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gfoofavao.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/giwoxvlgm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/gjxzraxul.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/gujvghunl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/groooolxq.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gdldwnqde.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/gqyoamttc.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/gbsmfzfzm.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/gchuvckku.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gejjtwutk.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gjktzzkug.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/gawiurcox.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gfbjqghhv.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/gitugmucs.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/gzjbmimzo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gynnfsehf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gyujdifng.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gngmepfxg.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gsrnckeua.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gsqzwcqlm.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/gkmrsgprm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/gtfuhktek.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/gcgwdpkjy.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/grvoxdhlh.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gpqixbgmt.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/ghsqybizc.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/gznnrbtca.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/gtxykzlyn.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gkdcsmqxy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/glmvmxwyt.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gngurwuaf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/gsdzjnrgx.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gkbxfcvgo.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/gtpibgmtv.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/ghaowctka.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/ggtqkvntc.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/gnfqaljrz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/gnrotpacx.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/gnuzbdxqf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fehbvm.com/Article/details/gqbugdcgm.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/gvmrvufes.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gpvxqzdou.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/gxbfvwonl.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gpudizmug.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/goxjwfnrh.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gdsfezjdx.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/gflfrkons.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gncqzqlqy.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gaoeatkjy.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/ggxysndcn.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gcdgdctbu.sHtML

var a = 1;  let b = 2
来源：http://mobile.zdbjq.cn/Article/details/grhvkyoca.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gwdsucegn.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gpueizdsr.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gmtsxsmag.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gcbxobvle.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gjjincijl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/ggzmedlte.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/gzxneiyeg.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gblufdppv.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/gfuliekpz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/gajftzwri.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gazxcsvkh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.zdbjq.cn/Article/details/gjummkslt.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/gjbqfozaj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/ghnsnqtze.sHtML

[T25] Swift：结构体
来源：http://mobile.zdbjq.cn/Article/details/gkhtpzgdw.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gitzfmqoy.sHtML

[T26] Swift：类与重写
来源：http://blog.zdbjq.cn/Article/details/gazqtwuzn.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/gchfrfncl.sHtML

[T27] Swift：错误处理
来源：http://blog.fehbvm.com/Article/details/grmhqoytm.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.zdbjq.cn/Article/details/giakmowfp.sHtML

[T28] Swift：枚举
来源：http://baike.fehbvm.com/Article/details/ghufxkwzm.sHtML

enum Color { case red, green }
来源：http://www.blog.zdbjq.cn/Article/details/glbiintni.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/ghmkztrxq.sHtML

guard let x = opt else { return }
来源：http://www.blog.fehbvm.com/Article/details/gaujevepj.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gcefagrne.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fehbvm.com/Article/details/ggcmeqmqo.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/gxieogrqn.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/godejdyds.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/gpxuntmad.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/guyztpoya.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/guicclfzo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/gdypnyhhz.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gnmjbtewg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.hesvh.cn/Article/details/gdzaegnhn.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/gmrignwhq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.zdbjq.cn/Article/details/gyiwvedhy.sHtML

[T36] Lua：函数
来源：http://read.share.hesvh.cn/Article/details/gbxrteopd.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/gckaloxha.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gaqeqiqwv.sHtML

"a" .. "b"
来源：http://www.m.share.fehbvm.com/Article/details/gyuffmcpp.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/gljhpdhdr.sHtML

if x > 0 then print("正") end
来源：http://www.blog.hesvh.cn/Article/details/ggjqyzlpp.sHtML

[T39] Lua：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gubfjmvxb.sHtML

string.find(s, "%d+")
来源：http://baike.zdbjq.cn/Article/details/gphtplxpp.sHtML

[T40] Lua：元表
来源：http://www.share.zdbjq.cn/Article/details/gahggloth.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/gmiwlhhvw.sHtML

[T41] Perl：Hello World
来源：http://www.share.fehbvm.com/Article/details/gvjagwxuk.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/gqawcpdjw.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/gydthylov.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.zdbjq.cn/Article/details/gggwdlamh.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gjndymwem.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/gddmtrbnn.sHtML

[T44] Perl：条件
来源：http://baike.hesvh.cn/Article/details/gqmtgnwed.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.hesvh.cn/Article/details/gsnjidyjt.sHtML

[T45] Perl：数组遍历
来源：http://www.share.hesvh.cn/Article/details/gvetgxicb.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.hesvh.cn/Article/details/gfsfaicye.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/gjlojubel.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.zdbjq.cn/Article/details/gpcosazrn.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gskowtbfo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/guyqjdkig.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/gzvkasqfc.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.zdbjq.cn/Article/details/gnastokoc.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/goqwegnml.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gzgtfvxuj.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gqizuhdgq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/gjjlqgevh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/gmkxpwjbq.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gsrrdwapm.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gbmnamrzv.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/gcbxmstqc.sHtML

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/giqknuhyh.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/gzyesigfk.sHtML

s"值: $b"
来源：http://baike.hesvh.cn/Article/details/gymwzwqhs.sHtML

[T54] Scala：集合映射
来源：http://m.share.fehbvm.com/Article/details/giylnhkrm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/genwsclwx.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/gsilshdsz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fehbvm.com/Article/details/gbcbhfwzo.sHtML

[T56] Scala：样例类
来源：http://baike.hesvh.cn/Article/details/gesrrhvha.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fehbvm.com/Article/details/gdinzeiou.sHtML

[T57] Scala：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gnwstyktj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/gojqirsoe.sHtML

[T58] Scala：函数定义
来源：http://m.share.zdbjq.cn/Article/details/ghpljrjtx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fehbvm.com/Article/details/ggvkfucmx.sHtML

[T59] Scala：循环
来源：http://www.m.share.hesvh.cn/Article/details/ggwgmejat.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gjmsopzew.sHtML

[T60] Scala：折叠
来源：http://www.share.fehbvm.com/Article/details/gcyawojny.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fehbvm.com/Article/details/gaqrmanrm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gilvjstgk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gyfvbfokx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtqzrjklf.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fehbvm.com/Article/details/geptpxzdb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/gjakfrcvb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.hesvh.cn/Article/details/glixqocus.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/gkdklcdba.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.zdbjq.cn/Article/details/gpmwzdcfz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.hesvh.cn/Article/details/gqhxejziv.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/gsypkyphf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/gmnwyllop.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/gclizarqx.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gdmtgrnzh.sHtML

[U06] Py：合并两个字典
来源：http://wap.zdbjq.cn/Article/details/grxyktffl.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/gngtyfuge.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/gtuahushe.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/gisondfgu.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/gxcfxeoog.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/gqevhqvdi.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.hesvh.cn/Article/details/gbfeluscg.sHtML

max(d, key=d.get)
来源：http://blog.fehbvm.com/Article/details/gdobincds.sHtML

[U10] Py：按值排序字典
来源：http://read.share.zdbjq.cn/Article/details/gxxbklmxv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.hesvh.cn/Article/details/gaejwujqy.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gcksjylch.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fehbvm.com/Article/details/glbwowabf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/gogmqsnxw.sHtML

Counter(arr).most_common(3)
来源：http://mobile.hesvh.cn/Article/details/glxtvbnuk.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fehbvm.com/Article/details/grhusoccm.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/gegltarrf.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/grfdtlyvk.sHtML

defaultdict(list)
来源：http://www.share.hesvh.cn/Article/details/gxpagreum.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/gycmzqrjy.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/grhjgnzio.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fehbvm.com/Article/details/gdxapbkpf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.hesvh.cn/Article/details/gjlsoqtdp.sHtML

[U17] Py：初始化日志
来源：http://m.share.zdbjq.cn/Article/details/gdivqzroc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.zdbjq.cn/Article/details/gmhmfabxz.sHtML

[U18] Py：预编译正则
来源：http://m.share.zdbjq.cn/Article/details/gihhmsuli.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/gzocrggyk.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.zdbjq.cn/Article/details/ghlugtpqy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fehbvm.com/Article/details/gefexddei.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/gsuaapebc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fehbvm.com/Article/details/gjrhxrzwm.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.zdbjq.cn/Article/details/gdsazdcms.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fehbvm.com/Article/details/gyecorzjp.sHtML

[U22] Py：矩阵转置
来源：http://blog.zdbjq.cn/Article/details/gxsffalij.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/gqqrmjnwu.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fehbvm.com/Article/details/gnoclkhjy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.hesvh.cn/Article/details/gzigeacpm.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/gdbmzldjg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gkcbipqoc.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/givswmbdd.sHtML

csv.DictReader(f)
来源：http://www.share.hesvh.cn/Article/details/gzromhuii.sHtML

[U26] Py：并发下载
来源：http://www.share.fehbvm.com/Article/details/gragpskct.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fehbvm.com/Article/details/gpormgwgk.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.zdbjq.cn/Article/details/gxniihtsj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.hesvh.cn/Article/details/golzqdarp.sHtML

[U28] Py：类型别名
来源：http://mobile.fehbvm.com/Article/details/glvwbeygj.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/gkbsrxmhb.sHtML

[U29] Py：属性校验
来源：http://baike.hesvh.cn/Article/details/gxtgpmbfh.sHtML

@property 与 @x.setter 配合
来源：http://read.share.hesvh.cn/Article/details/gjwtvqpcz.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/gdwhyepmn.sHtML

@dataclass(slots=True)
来源：http://www.share.zdbjq.cn/Article/details/gfowcdtfx.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/gwkbdluiy.sHtML

python -m pytest -q
来源：http://baike.fehbvm.com/Article/details/gdbhpubux.sHtML

[U32] Py：代码格式化
来源：http://m.share.fehbvm.com/Article/details/gdkwstxgh.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.zdbjq.cn/Article/details/giymvaxle.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fehbvm.com/Article/details/glbwkfwpv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.zdbjq.cn/Article/details/gedgcfvcn.sHtML

[U34] Py：判断编码
来源：http://m.share.hesvh.cn/Article/details/gejpkcjfq.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/gpzwtrinm.sHtML

[U35] Py：发送邮件
来源：http://www.share.fehbvm.com/Article/details/glnonbjjt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.zdbjq.cn/Article/details/gsakqyedy.sHtML

[U36] Py：定时任务
来源：http://www.blog.fehbvm.com/Article/details/gntrxqxbe.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/gytiaiwkc.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/gtghqlvvu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.zdbjq.cn/Article/details/glxtqzugl.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.zdbjq.cn/Article/details/gnpkewmhx.sHtML

Path(__file__).resolve().parent
来源：http://baike.hesvh.cn/Article/details/gymalvvki.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.zdbjq.cn/Article/details/gydmlszvb.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/ggowpnzxi.sHtML

[U40] Py：打印到标准错误
来源：http://3g.hesvh.cn/Article/details/gqptynxgv.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gnwoqjdcf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.hesvh.cn/Article/details/gzyvylhmf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fehbvm.com/Article/details/gzcvjirit.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.zdbjq.cn/Article/details/gjmpkuaeh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.zdbjq.cn/Article/details/gbttkutej.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fehbvm.com/Article/details/goojeajym.sHtML

namespace App\Http;
来源：http://www.share.hesvh.cn/Article/details/gizuvmalf.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fehbvm.com/Article/details/gkezixgvw.sHtML

declare(strict_types=1);
来源：http://wap.zdbjq.cn/Article/details/gqlgbqnds.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fehbvm.com/Article/details/gmoxpogtv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gsgciagmr.sHtML

[U46] PHP：可空类型
来源：http://wap.zdbjq.cn/Article/details/gwtcrwryg.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/gypfaaljk.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/gfprelpvb.sHtML

int|string $id
来源：http://3g.hesvh.cn/Article/details/gydivieah.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fehbvm.com/Article/details/gxjgfxvcu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/gwvgubtni.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fehbvm.com/Article/details/gswmgrgkw.sHtML

public readonly string $name
来源：http://m.share.zdbjq.cn/Article/details/gmuutsfvn.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fehbvm.com/Article/details/gunferafh.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.hesvh.cn/Article/details/ggzcqwgqq.sHtML

[U51] PHP：数组解构
来源：http://www.share.fehbvm.com/Article/details/gyumejdig.sHtML

[$a, $b] = $arr;
来源：http://3g.zdbjq.cn/Article/details/gtqkhlbzm.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gaqmuxlsw.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fehbvm.com/Article/details/gtqlqfzqw.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fehbvm.com/Article/details/gbdraqjpr.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fehbvm.com/Article/details/gqczvswou.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fehbvm.com/Article/details/ghbreudee.sHtML

$obj?->method()
来源：http://baike.fehbvm.com/Article/details/gpmznevas.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fehbvm.com/Article/details/gisxtbhjy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.zdbjq.cn/Article/details/gihdjriwc.sHtML

[U56] PHP：命名参数
来源：http://m.share.zdbjq.cn/Article/details/gtzycvott.sHtML

f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gmfwtaaxm.sHtML


<!-- 参考信息 -->