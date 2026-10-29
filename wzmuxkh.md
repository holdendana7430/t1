代发 wailian999

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gavhdbbas.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gzxdbykng.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gpgubkmif.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/gmqkejsvk.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/giivsmhtr.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gwvwcttia.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/gehdjlwsb.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/gqrcgnvsb.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gshwinmje.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gytvudatw.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/gdkknujuc.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/glllsvosr.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/gfwzusygz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/gvsundywv.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/gefgeujhg.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gpdadbpvu.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gfhzsxvdb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/gwsqjpzeu.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gdyieatxx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gctrcaktz.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gjhxzikny.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/glffwgckm.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/gtcmiexno.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gztpwhrqy.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/gdvolqdbv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/grbtfislu.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gfvdptwlz.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/gwwfhtdir.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/glbfagrsm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/glmxnourv.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gfgqmbfsb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/golakqzxz.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gblslzbxg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/gnowpznfh.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/ggcepcnqo.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gybyrbsjb.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gresyyyfd.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/gwlimracp.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/gttlwdcsh.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gdddvtice.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/glkbjwfhp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fehbvm.com/Article/details/gyaljmlir.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/glystwtqb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gmbwibptz.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gzlxuhhor.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/gggbehrxs.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gnbtmitgg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/gegmlhjes.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/gebpkeeho.sHtML

[S49] C++：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gawjeonoj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/ghkjtluey.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/gmsorjxwa.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/gyipbdhtj.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/gklhfelgh.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gatbwvpjr.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/gyexlrbuj.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gdoywioao.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/grefljmxy.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gxlzigbng.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gtylfbqut.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/gycidunua.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fehbvm.com/Article/details/gjguosjao.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gsrmmexwz.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/gpjvljpbk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/gxbgtofca.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gsybavfif.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gyiutslsz.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gqkxeluin.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/gptpgisgw.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gpaowtxgm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gtgtqmokb.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/gxtjniizh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/gzxdybiys.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gepqmmcrf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gbabcfhxi.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmjvojkpz.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gtmxankft.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gdfanuxyu.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/gvcoqpeql.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/gtdxdqmes.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gggpabshh.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/grrntgcsu.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gitxnnoer.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/gwdzvckpp.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/gcqjcaggs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/getokrefh.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/gkfvygnlb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gfohhjiar.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/gzdcqnzth.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/gwiicosky.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gwcnxjehn.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/gpzslzvmm.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/gxhpvubem.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/gxhoaupmn.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/gqmjqrepq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/gajkgocgl.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gqvmyqxrm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gwehibbrh.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/glkonjcdx.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gtwlgvyey.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/gquenljdw.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/gjczyncaa.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gzujfsrln.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/grwggruwt.sHtML

[T15] Kotlin：接口
来源：http://blog.hesvh.cn/Article/details/gifzwrzpv.sHtML

interface Shape { fun area(): Double }
来源：http://3g.hesvh.cn/Article/details/gvtbvjpkq.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gxhmiqwjj.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gbxfbivcc.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/gsuabokif.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gtarzaaoz.sHtML

[T18] Swift：字符串插值
来源：http://wap.hesvh.cn/Article/details/glrttbpxc.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/ggutzquba.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fehbvm.com/Article/details/gjmbjgjnv.sHtML

if let n = opt { print(n) }
来源：http://mobile.zdbjq.cn/Article/details/gbgpduxfb.sHtML

[T20] Swift：数组操作
来源：http://www.share.fehbvm.com/Article/details/gqffukgeg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/gapmogajh.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/gllmjwpux.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gawybjrjz.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/gxofbelha.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/gknrwigyu.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gfdarcwcd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/gfqmejudb.sHtML

[T24] Swift：闭包
来源：http://blog.hesvh.cn/Article/details/gxkbxqrii.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gyheqwigw.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/gsyktslaq.sHtML

struct P { var x: Int }
来源：http://mobile.fehbvm.com/Article/details/gpwfryiih.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/gzktirrwa.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/gineqbedh.sHtML

[T27] Swift：错误处理
来源：http://blog.fehbvm.com/Article/details/gytcsltqu.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/gbkhesanl.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gbyhgflgg.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/gifkfhrwl.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.zdbjq.cn/Article/details/goediftot.sHtML

guard let x = opt else { return }
来源：http://www.blog.zdbjq.cn/Article/details/gtdazplzp.sHtML

[T30] Swift：协议
来源：http://mobile.fehbvm.com/Article/details/gomcnthfn.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/gprpjygbv.sHtML

[T31] Lua：Hello World
来源：http://3g.zdbjq.cn/Article/details/gjjqevmai.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gfjpwkvfy.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/gdgfwchhx.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gknjiqviq.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/gsiuzmlaw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.zdbjq.cn/Article/details/gnxxljmeb.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/gezpduqcm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/ghzfbkiyk.sHtML

[T35] Lua：字典表
来源：http://mobile.fehbvm.com/Article/details/grfzdjrjt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/guvciulaq.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/gzxcscmoj.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/gsoitqegg.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gimrlorxr.sHtML

"a" .. "b"
来源：http://3g.fehbvm.com/Article/details/grntzhzia.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/gjzfkziee.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/gflkzuvdp.sHtML

[T39] Lua：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gpitrjcrl.sHtML

string.find(s, "%d+")
来源：http://www.blog.fehbvm.com/Article/details/gfftpjdsg.sHtML

[T40] Lua：元表
来源：http://www.blog.hesvh.cn/Article/details/geyywmltl.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/gmdryhugl.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gnmgbwzno.sHtML

print "Hello\n";
来源：http://wap.hesvh.cn/Article/details/gdkeoaxzz.sHtML

[T42] Perl：变量类型
来源：http://blog.zdbjq.cn/Article/details/gqueowrak.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fehbvm.com/Article/details/gheugsudw.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/givxrwucm.sHtML

"值: $a"
来源：http://read.share.zdbjq.cn/Article/details/gwibhjwab.sHtML

[T44] Perl：条件
来源：http://mobile.zdbjq.cn/Article/details/gcijocses.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.hesvh.cn/Article/details/gaqnexacp.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/gljysgxhv.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/gdreacjce.sHtML

[T46] Perl：哈希操作
来源：http://3g.zdbjq.cn/Article/details/gcnwqojss.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fehbvm.com/Article/details/gaxhzjzrf.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gktladhtz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.hesvh.cn/Article/details/gbrutmjwx.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/gvowmvbns.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.zdbjq.cn/Article/details/glehcqoiq.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/giwvaiyge.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gtapltnnm.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gmkgglrmn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.hesvh.cn/Article/details/gkiqnhafu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/gqzuifgjy.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/gakzsgxgj.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/grimtjomw.sHtML

[T52] Scala：变量
来源：http://blog.hesvh.cn/Article/details/gjlqmglnp.sHtML

val a = 1;  var b = 2
来源：http://mobile.hesvh.cn/Article/details/gpgatpaln.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gimhbozmj.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/gukorkfyn.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/govlmcqkg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/gqlaxjshb.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/grmlzogip.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.hesvh.cn/Article/details/gpcbfatgr.sHtML

[T56] Scala：样例类
来源：http://m.share.zdbjq.cn/Article/details/gujpcszyq.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gqpfinpgk.sHtML

[T57] Scala：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gidrkkumr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gdmaqpjmn.sHtML

[T58] Scala：函数定义
来源：http://blog.zdbjq.cn/Article/details/gxblrjsmz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.hesvh.cn/Article/details/giehynxuh.sHtML

[T59] Scala：循环
来源：http://m.share.fehbvm.com/Article/details/gkegaygii.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/gqqownyfx.sHtML

[T60] Scala：折叠
来源：http://blog.zdbjq.cn/Article/details/grrqroyis.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fehbvm.com/Article/details/gfgmsdbsv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjfqaybxw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gjetlwosi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/goqvwwzkv.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fehbvm.com/Article/details/gkwauhkcd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/gvqccmpkp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/giqjldylh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/gaxrdfqpg.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fehbvm.com/Article/details/gagauubnq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.zdbjq.cn/Article/details/gwlnobbmo.sHtML

[U04] Py：变量调试打印
来源：http://3g.hesvh.cn/Article/details/gbgiebqts.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gxtydvtmi.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.zdbjq.cn/Article/details/ghueflsjw.sHtML

list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/growflqcc.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gdjthmkyn.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/ggcgzhuyc.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.hesvh.cn/Article/details/gnemiauwc.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/gdohrbfsh.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.hesvh.cn/Article/details/gtpjzhbwm.sHtML

[y for x in nested for y in x]
来源：http://read.share.zdbjq.cn/Article/details/gdzlequsd.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.zdbjq.cn/Article/details/gswxsbrmy.sHtML

max(d, key=d.get)
来源：http://www.m.share.zdbjq.cn/Article/details/gdshdbxuz.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.hesvh.cn/Article/details/gjfnsdvac.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.zdbjq.cn/Article/details/ghptynqkk.sHtML

[U11] Py：生成器表达式
来源：http://www.share.zdbjq.cn/Article/details/gisoyvcxx.sHtML

(x * 2 for x in arr)
来源：http://3g.zdbjq.cn/Article/details/ghbokiuxn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/gjkzqdiek.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/goowlycno.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/geumxlndk.sHtML

deque(maxlen=10)
来源：http://baike.zdbjq.cn/Article/details/grhknbgwt.sHtML

[U14] Py：分组收集到列表
来源：http://blog.hesvh.cn/Article/details/gefokvvsy.sHtML

defaultdict(list)
来源：http://m.share.zdbjq.cn/Article/details/gpbhdfocf.sHtML

[U15] Py：高精度计时
来源：http://read.share.hesvh.cn/Article/details/ggiqzeqip.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/gfafduemx.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.zdbjq.cn/Article/details/gqoniigms.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.hesvh.cn/Article/details/gukkyrpkk.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.hesvh.cn/Article/details/guaabjbfm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fehbvm.com/Article/details/gvtjvivqg.sHtML

[U18] Py：预编译正则
来源：http://www.share.zdbjq.cn/Article/details/gjqykabix.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/ghnfwibpa.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/gfgvpmquq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fehbvm.com/Article/details/glslgxzos.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/grksprsxn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fehbvm.com/Article/details/gcvbknpsk.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.zdbjq.cn/Article/details/ggbfwmjyt.sHtML

@contextlib.contextmanager
来源：http://baike.zdbjq.cn/Article/details/gizlbklta.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fehbvm.com/Article/details/gbjakyqvq.sHtML

list(zip(*m))
来源：http://m.share.fehbvm.com/Article/details/ghiucqhmn.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fehbvm.com/Article/details/gdxdpcefw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.hesvh.cn/Article/details/gzxrubdzu.sHtML

[U24] Py：路径操作
来源：http://mobile.fehbvm.com/Article/details/gjqmntiue.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gjqvphygd.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.hesvh.cn/Article/details/gcanouvvo.sHtML

csv.DictReader(f)
来源：http://baike.hesvh.cn/Article/details/gtohdcjst.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/ghwvwgemh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.zdbjq.cn/Article/details/gmlvppqcb.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.zdbjq.cn/Article/details/ghztbowqt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.zdbjq.cn/Article/details/gectqucnz.sHtML

[U28] Py：类型别名
来源：http://mobile.zdbjq.cn/Article/details/gzznfxxbp.sHtML

UserId = int
来源：http://3g.hesvh.cn/Article/details/guhazoepy.sHtML

[U29] Py：属性校验
来源：http://baike.zdbjq.cn/Article/details/gamwdooju.sHtML

@property 与 @x.setter 配合
来源：http://3g.fehbvm.com/Article/details/ghimxufvm.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/glgbgkgpd.sHtML

@dataclass(slots=True)
来源：http://blog.fehbvm.com/Article/details/gxlruciwa.sHtML

[U31] Py：单测
来源：http://baike.zdbjq.cn/Article/details/ggngenugb.sHtML

python -m pytest -q
来源：http://m.share.fehbvm.com/Article/details/gnbdcugzu.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/gugayztbf.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.zdbjq.cn/Article/details/ghsbluytg.sHtML

[U33] Py：打包发布
来源：http://blog.hesvh.cn/Article/details/gmlzxbwgt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.zdbjq.cn/Article/details/getpzfaip.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/gehhkbpaw.sHtML

chardet.detect(raw)
来源：http://wap.hesvh.cn/Article/details/gfzhwmfts.sHtML

[U35] Py：发送邮件
来源：http://3g.zdbjq.cn/Article/details/gukndawpz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.hesvh.cn/Article/details/goynpzcqp.sHtML

[U36] Py：定时任务
来源：http://mobile.hesvh.cn/Article/details/gsunhwldn.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.zdbjq.cn/Article/details/gxahzscou.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fehbvm.com/Article/details/gsvynyyof.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fehbvm.com/Article/details/grnnjgmeq.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.hesvh.cn/Article/details/gnkoqullh.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fehbvm.com/Article/details/gcytigdke.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.zdbjq.cn/Article/details/gbfjgqjcd.sHtML

sys.stdout.isatty()
来源：http://blog.fehbvm.com/Article/details/gmdfuwjjt.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.hesvh.cn/Article/details/gsxeruplo.sHtML

print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gtmigerpz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.hesvh.cn/Article/details/gnobrwkjp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fehbvm.com/Article/details/glhshzdvi.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.hesvh.cn/Article/details/gzaxeluzy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/glzzhgixf.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.hesvh.cn/Article/details/goerifvux.sHtML

namespace App\Http;
来源：http://wap.zdbjq.cn/Article/details/gbsynerle.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.hesvh.cn/Article/details/ghnqodksb.sHtML

declare(strict_types=1);
来源：http://3g.fehbvm.com/Article/details/gpejmyvmf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fehbvm.com/Article/details/grdzbgyuu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gchpishim.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fehbvm.com/Article/details/gfryahmiq.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/gdibhtxox.sHtML

[U47] PHP：联合类型
来源：http://3g.hesvh.cn/Article/details/gbzpukoun.sHtML

int|string $id
来源：http://mobile.hesvh.cn/Article/details/gsvdmoksk.sHtML

[U48] PHP：纯枚举
来源：http://baike.fehbvm.com/Article/details/gepaphhlb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fehbvm.com/Article/details/gbwfvnfhu.sHtML

[U49] PHP：只读属性
来源：http://mobile.fehbvm.com/Article/details/gmpzmsorz.sHtML

public readonly string $name
来源：http://www.blog.zdbjq.cn/Article/details/gajsfcpov.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/gayoddzzb.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.zdbjq.cn/Article/details/gssxhwysj.sHtML


<!-- 参考信息 -->