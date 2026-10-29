代发 wailian999

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/gsydqvqdr.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/gjeoxyqkr.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gfpfvgtow.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/gnqrivfbt.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/ghcigadof.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gjlobvcmq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/gplrhgdsn.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gshlnibpj.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gexnsjjov.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/ghivnsjnw.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/grzewsujs.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gqppnmlfn.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/ghjvxwlmw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/gxmbtoisg.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/guigrtgsw.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gmnkuspey.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/gcfprgwai.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/gwwkvcwxr.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gituhzeiv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gukbvtjtc.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gljmlbcjz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/geyyjsgxj.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/gvqpvicea.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gyoterqfd.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/gaznqlvzr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gejkpcsxg.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/ghczwmnbb.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/glovyohxx.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/gefslshrj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/geyrjkxva.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/gdilratyu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/guacfgsfg.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/gpdogfdlj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gdodmnzgg.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gynjjnrfz.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/grejfiibk.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/giloorklu.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gwuudepes.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gbguwofsl.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/grzymusrc.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/gelepngdo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gobfjsjft.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/guvhunxup.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/gfoxsxhmy.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/gpsttbtsj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/geptxschi.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gylwpkmiq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gesqvsoep.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/gdkbzjbls.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/glnpmscfv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/glwtusfbm.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/gxlclweub.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gyomhtott.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/goqkrkbkx.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/gdsedcchf.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gduswldup.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gjpprbuoq.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gdoqlnqve.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/girpzaebm.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/ghskflkcz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/ghgtbllkf.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/gmmengekd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gtcwldlsk.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/gfoukhmev.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/gtrxqzxnp.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/ghhbcgyos.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gavrssaqx.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/gdlvypxxb.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/gmibybchd.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/gvpuetjco.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gzhcgknre.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/gysiihblf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fehbvm.com/Article/details/gycryyfxs.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjzopjqkv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gkdgsznle.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxgbiwdfk.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gbexskkmx.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gwytibbuw.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/gsaxxogtg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gjbwauoqu.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.hesvh.cn/Article/details/giukdltuc.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gorgcjufr.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gdvzpjobl.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/glmxindks.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gocroplrg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gsdsjcrge.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/gvqikhxsf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gawhikxtn.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gobfxvmdy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/gaequczwk.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/gycvshnwz.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/gdaaamokr.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/glqrmyjhr.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/goytxiwpf.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/gbtyqecct.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gwrclgtdd.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/gdeollzzo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fehbvm.com/Article/details/gzszoeixl.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/gdbhsdmwx.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gcmzudyfa.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.zdbjq.cn/Article/details/gxazauphz.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gcuhfgiyw.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gjvyetfss.sHtML

for (i in 1..10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/glqpbpqqy.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/ggvejwend.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/gfeqnalsv.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gfqklnuvy.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/grtbfrdbd.sHtML

[T17] Swift：变量与常量
来源：http://baike.hesvh.cn/Article/details/gkkzbzxqs.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gbkyqzohh.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gonbgiofs.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/gitwohzzf.sHtML

[T19] Swift：可选绑定
来源：http://3g.fehbvm.com/Article/details/gqxljisiv.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/gwcsifuvw.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gtawitmug.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gyjizhzfy.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/gbwlclird.sHtML

for x in a { print(x) }
来源：http://www.m.share.zdbjq.cn/Article/details/gfllpzeoj.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/gqyvsecxz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/gsrgzlayv.sHtML

[T23] Swift：函数
来源：http://baike.fehbvm.com/Article/details/gyidwuiav.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/guaawbyek.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/gsiqmvhkg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gsuqkfllu.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gysiktglg.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gumjjhyqb.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gyipmkzii.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/gwgthepeh.sHtML

[T27] Swift：错误处理
来源：http://mobile.zdbjq.cn/Article/details/gtpfrnnvm.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/goyxydvey.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/geqqthrqr.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/giwpnxzru.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.hesvh.cn/Article/details/gvymsiupb.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/gxzywntnk.sHtML

[T30] Swift：协议
来源：http://baike.zdbjq.cn/Article/details/gyobgmkke.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/gwkvnxcsa.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gqnfuqogp.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gglukucbq.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/gvzqlcvkz.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/ghsjmqrub.sHtML

[T33] Lua：表（数组）
来源：http://wap.hesvh.cn/Article/details/gyrpasetl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/gxgrgbqdu.sHtML

[T34] Lua：遍历表
来源：http://mobile.zdbjq.cn/Article/details/gcurzivmk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fehbvm.com/Article/details/gzmtvvrul.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gforksmqd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gwgfmokap.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/gbfqfxhiv.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/gycokowjq.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gydtzgnzl.sHtML

"a" .. "b"
来源：http://www.blog.hesvh.cn/Article/details/glwzormou.sHtML

[T38] Lua：条件
来源：http://read.share.fehbvm.com/Article/details/guinhopjw.sHtML

if x > 0 then print("正") end
来源：http://www.share.hesvh.cn/Article/details/gnntjxoqg.sHtML

[T39] Lua：模式匹配
来源：http://wap.hesvh.cn/Article/details/gurszozpc.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/gnstvejso.sHtML

[T40] Lua：元表
来源：http://3g.zdbjq.cn/Article/details/gxmdbxqxz.sHtML

setmetatable({}, { __index = base })
来源：http://3g.zdbjq.cn/Article/details/gwrruglhk.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gfnomnkel.sHtML

print "Hello\n";
来源：http://www.share.zdbjq.cn/Article/details/gdrdnnprd.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/ghcdzdmil.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.hesvh.cn/Article/details/gbywlgacr.sHtML

[T43] Perl：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gxsyrokzf.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/gjwvsbkol.sHtML

[T44] Perl：条件
来源：http://mobile.fehbvm.com/Article/details/gaqpjmhnl.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.zdbjq.cn/Article/details/glbkvfbjn.sHtML

[T45] Perl：数组遍历
来源：http://read.share.hesvh.cn/Article/details/goetwwqca.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.hesvh.cn/Article/details/ggjtykxuz.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fehbvm.com/Article/details/gyphrguqd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fehbvm.com/Article/details/gjnkdzcrg.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fehbvm.com/Article/details/gtywgdlsg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.hesvh.cn/Article/details/glvfoygbr.sHtML

[T48] Perl：正则替换
来源：http://wap.fehbvm.com/Article/details/gnbqiskko.sHtML

$s =~ s/old/new/g;
来源：http://3g.hesvh.cn/Article/details/gwvwacqxm.sHtML

[T49] Perl：函数
来源：http://www.share.zdbjq.cn/Article/details/gokeuuvsy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gyospozen.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gbmlouhmg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/gzprffgpg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/grlcfrowo.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gwrnqarcp.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gnwlnokbv.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/gqlluauda.sHtML

val a = 1;  var b = 2
来源：http://read.share.fehbvm.com/Article/details/gkkavbaxf.sHtML

[T53] Scala：字符串插值
来源：http://m.share.hesvh.cn/Article/details/grfnmnoyu.sHtML

s"值: $b"
来源：http://read.share.hesvh.cn/Article/details/ggvcfkbpa.sHtML

[T54] Scala：集合映射
来源：http://3g.zdbjq.cn/Article/details/gpzrrvbjt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.hesvh.cn/Article/details/gsiioehig.sHtML

[T55] Scala：集合过滤
来源：http://blog.hesvh.cn/Article/details/geenrigvl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/gabawtswq.sHtML

[T56] Scala：样例类
来源：http://3g.hesvh.cn/Article/details/gockbzdlb.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gplclvpjc.sHtML

[T57] Scala：模式匹配
来源：http://wap.hesvh.cn/Article/details/gbwzyvipx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.hesvh.cn/Article/details/gpybijrsg.sHtML

[T58] Scala：函数定义
来源：http://3g.fehbvm.com/Article/details/ggfmvxzpu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fehbvm.com/Article/details/gcpxygkla.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/gxzajmods.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gkhcczlcj.sHtML

[T60] Scala：折叠
来源：http://3g.hesvh.cn/Article/details/gnlzaxiez.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/gjwweijsn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmvtcctds.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/gfsfyqohw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxotapwyw.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.zdbjq.cn/Article/details/gagvxhexo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/gjpznqhjb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.zdbjq.cn/Article/details/gxmvoqwyt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.zdbjq.cn/Article/details/gaughuyjm.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gnhzqrvna.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.hesvh.cn/Article/details/grpyaagyv.sHtML

[U04] Py：变量调试打印
来源：http://m.share.zdbjq.cn/Article/details/gyplvefmb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gcoqzokdy.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/ghdtqzgje.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gmtawdxce.sHtML

[U06] Py：合并两个字典
来源：http://wap.hesvh.cn/Article/details/gunhutzpt.sHtML

{**a, **b}
来源：http://blog.zdbjq.cn/Article/details/gllqmoyjc.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/gfyzrbzvf.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fehbvm.com/Article/details/gtdfsrywp.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/gyyvmhdaf.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fehbvm.com/Article/details/gkyjfatjw.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fehbvm.com/Article/details/gotvgxwck.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/gkdqrmkie.sHtML

[U10] Py：按值排序字典
来源：http://baike.hesvh.cn/Article/details/gatbsefso.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/gfxqkmrwy.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/govvozoma.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/gmghbnxxh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.hesvh.cn/Article/details/gbobxhzbb.sHtML

Counter(arr).most_common(3)
来源：http://m.share.hesvh.cn/Article/details/gguiqxbui.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fehbvm.com/Article/details/gwmuqjucq.sHtML

deque(maxlen=10)
来源：http://wap.zdbjq.cn/Article/details/gkychdkhg.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.zdbjq.cn/Article/details/gejrsojce.sHtML

defaultdict(list)
来源：http://www.share.hesvh.cn/Article/details/gqiekonej.sHtML

[U15] Py：高精度计时
来源：http://mobile.hesvh.cn/Article/details/gomlumxta.sHtML

t = time.perf_counter()
来源：http://www.m.share.hesvh.cn/Article/details/gabcrwwoy.sHtML

[U16] Py：命令行参数解析
来源：http://baike.hesvh.cn/Article/details/gfmojgzgk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fehbvm.com/Article/details/gzocodltm.sHtML

[U17] Py：初始化日志
来源：http://mobile.fehbvm.com/Article/details/giqwxhnha.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/gvlmwdemr.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/gqtglrarj.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/gjlkapcmg.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.hesvh.cn/Article/details/gixeinjsr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/gxbuexmki.sHtML

[U20] Py：缓存函数结果
来源：http://wap.zdbjq.cn/Article/details/goqmjkdmb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/gofpuevju.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.hesvh.cn/Article/details/gbanyrlxd.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/gtqytpnbz.sHtML

[U22] Py：矩阵转置
来源：http://mobile.hesvh.cn/Article/details/gkbcolmwo.sHtML

list(zip(*m))
来源：http://read.share.fehbvm.com/Article/details/gfbqjnylf.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/gjoiqpczc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/grgvxiufh.sHtML

[U24] Py：路径操作
来源：http://www.blog.fehbvm.com/Article/details/glmlxkdqp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gtaunxwgh.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.zdbjq.cn/Article/details/giqhgyefa.sHtML

csv.DictReader(f)
来源：http://www.share.fehbvm.com/Article/details/gohztjstz.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/gtmnssphg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fehbvm.com/Article/details/grrfqlaok.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.zdbjq.cn/Article/details/gyuxydteu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.zdbjq.cn/Article/details/gdauqwxdl.sHtML

[U28] Py：类型别名
来源：http://blog.hesvh.cn/Article/details/godfqkdzb.sHtML

UserId = int
来源：http://www.blog.hesvh.cn/Article/details/gfaaljvvs.sHtML

[U29] Py：属性校验
来源：http://www.share.hesvh.cn/Article/details/ggeympabw.sHtML

@property 与 @x.setter 配合
来源：http://3g.hesvh.cn/Article/details/glofxibxo.sHtML

[U30] Py：数据类
来源：http://m.share.hesvh.cn/Article/details/gkrruefmo.sHtML

@dataclass(slots=True)
来源：http://wap.hesvh.cn/Article/details/gtugaadaf.sHtML

[U31] Py：单测
来源：http://www.share.zdbjq.cn/Article/details/gmdowhyep.sHtML

python -m pytest -q
来源：http://www.blog.hesvh.cn/Article/details/ggpmufgsz.sHtML

[U32] Py：代码格式化
来源：http://mobile.zdbjq.cn/Article/details/gpyfqdtkx.sHtML

ruff format . && ruff check --fix .
来源：http://3g.hesvh.cn/Article/details/gitjihzvp.sHtML

[U33] Py：打包发布
来源：http://blog.hesvh.cn/Article/details/gxxukdxee.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fehbvm.com/Article/details/gjdjnawrp.sHtML

[U34] Py：判断编码
来源：http://www.m.share.hesvh.cn/Article/details/grtuhumti.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/gtwlbippf.sHtML

[U35] Py：发送邮件
来源：http://www.share.fehbvm.com/Article/details/galehzaga.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.hesvh.cn/Article/details/gwirieush.sHtML

[U36] Py：定时任务
来源：http://baike.fehbvm.com/Article/details/gsnsxnptg.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.zdbjq.cn/Article/details/grognuill.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.zdbjq.cn/Article/details/gebsbqmza.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.hesvh.cn/Article/details/genfxnqmy.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fehbvm.com/Article/details/gbgvcuycs.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.zdbjq.cn/Article/details/gvqodzofz.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.zdbjq.cn/Article/details/gkfmcvtjf.sHtML

sys.stdout.isatty()
来源：http://baike.hesvh.cn/Article/details/gosjstrsk.sHtML

[U40] Py：打印到标准错误
来源：http://blog.zdbjq.cn/Article/details/gpjunhbqc.sHtML

print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gffgivgoz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.hesvh.cn/Article/details/gvewfnazq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.zdbjq.cn/Article/details/gjleoibti.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.zdbjq.cn/Article/details/gfzwqstoe.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/goqbdcvez.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.zdbjq.cn/Article/details/gciotlkjb.sHtML

namespace App\Http;
来源：http://www.m.share.fehbvm.com/Article/details/gqjcjzrap.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/gxzsqtwar.sHtML

declare(strict_types=1);
来源：http://www.blog.fehbvm.com/Article/details/gkoaeybhg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.zdbjq.cn/Article/details/ghktnganr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gsojcdpxa.sHtML

[U46] PHP：可空类型
来源：http://www.share.zdbjq.cn/Article/details/gprcrrpxn.sHtML

?string $name = null
来源：http://wap.fehbvm.com/Article/details/gceuiupvh.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fehbvm.com/Article/details/gevplampa.sHtML

int|string $id
来源：http://www.share.zdbjq.cn/Article/details/geiolucbe.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fehbvm.com/Article/details/gaswenfim.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.zdbjq.cn/Article/details/gipoydwop.sHtML

[U49] PHP：只读属性
来源：http://www.blog.zdbjq.cn/Article/details/gretxcusf.sHtML

public readonly string $name
来源：http://read.share.fehbvm.com/Article/details/giabhpzsv.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/gcapbgfvs.sHtML

public function __construct(private int $id) {}
来源：http://wap.fehbvm.com/Article/details/gfjbparat.sHtML


<!-- 参考信息 -->