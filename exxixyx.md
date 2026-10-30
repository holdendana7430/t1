代发 wailian999

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gduhjwdpx.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gptpoqnat.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwhkkaab.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gqbvjrdes.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/ganeyrcgp.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gkskvlhxu.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gosbalbjs.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gzsgbhbfq.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjatkhxn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gllicbbyh.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/goxjnremj.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmyfoenn.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyhkainu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/giluuqfra.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gnixmnieb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtacaviut.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpsdawzl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gxrprthzf.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqwretax.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/geycuxugh.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gzfcpttmi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobabhfjl.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gwglfxljn.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gpriwudcm.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gnhmgjlhf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gedzomisw.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogwcedwj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykqxnrme.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gkzuvnbbg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gruhjralq.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmeeiarv.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfeuvsskx.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkgprmot.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/glvurzvty.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmrhfojz.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmmhtxjn.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gunibqcdi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/giduytmpx.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/groenqiyh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gntkkxfcx.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gfyhaleiz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxqqjljaa.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzelcoav.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqbaqbtn.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzwbupdb.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gnykzilnc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gvlimfdod.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/grvmoihxn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/glmfevuhz.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gkkdiyout.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjiteoedo.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gufonpfmf.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/griqrvsmi.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gnrxituui.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmkonxpu.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpwiswsq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/geyfgyxtb.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzqojbkc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafcyycmq.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjavolvmj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqykjwtun.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrbcuunb.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsznpmoxd.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gygkjuxew.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gkhdfslhj.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gpezifcrq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpkehthi.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gqklbzajp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/grmnnawsx.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gpighljoo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsqovleo.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gckxtspwz.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/guuicigon.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gmislaimb.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjgbuxiw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpctcupl.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpizgyam.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gcfzhdqex.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gutfpgoum.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnujjfmt.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gvkotsini.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/gnomhnuuc.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gksqihltp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzeqpfnb.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnvrmrow.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyahhdker.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbjzjpwg.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gjsbwhldj.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gvumgntdu.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvznazuav.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtguvxvua.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/gwnydbaed.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxlmzhzj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgfofhix.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gxubzxjbq.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/glxcwhdfq.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzqmdehu.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnymcihxx.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkltzjkv.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdkvyenx.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyywwmuv.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gopwmrrrr.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxfnldso.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbpcpodq.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/gqqaqtnex.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gczzeidue.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgjltunc.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtmdnfyv.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbmxymtz.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizwstipz.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgrqrcyd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fanxiaobao.xyz/Article/details/gvpbfssku.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmuhedcj.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gnizaibhh.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/ghwngwfwy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfncemho.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gjnjyexqr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzaqoogj.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gbfvnclts.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjopkojqe.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/gqunfvybo.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwmzjmaq.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfejlduk.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqxuxhef.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gshylarvv.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnquhngd.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/glnpupcvp.sHtML

enum Color { case red, green }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnutvvayh.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwhcoutw.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhnpazwj.sHtML

[T30] Swift：协议
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxjektzl.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gcxkslyry.sHtML

[T31] Lua：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxdybgbi.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfeucozq.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gzdtgntzb.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/giztalgwz.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gksibphom.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwilhrju.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/gguxflwzo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fanxiaobao.xyz/Article/details/gbceiqlxa.sHtML

[T35] Lua：字典表
来源：http://3g.fanxiaobao.xyz/Article/details/gmygvyphh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gcuxnhnum.sHtML

[T36] Lua：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/grzctnmcg.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglkkdkry.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gojoqgbrj.sHtML

"a" .. "b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrwjfjnp.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/ggltvaaey.sHtML

if x > 0 then print("正") end
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyfqrmqj.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gttrfokad.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gpvjfowco.sHtML

[T40] Lua：元表
来源：http://blog.fanxiaobao.xyz/Article/details/gahlrxrjy.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzzwxens.sHtML

[T41] Perl：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gvqsgyqpz.sHtML

print "Hello\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gouwvswql.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudelzjhr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgnporyr.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghslsbykm.sHtML

"值: $a"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzuytiwmw.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsdxwyhe.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzefltfws.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giretvhxs.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcqfyiyg.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmziqalnu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwagvlwlm.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fanxiaobao.xyz/Article/details/gxktiggzg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmeraunyn.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/glpmtckfj.sHtML

$s =~ s/old/new/g;
来源：http://wap.fanxiaobao.xyz/Article/details/gutyhjvsy.sHtML

[T49] Perl：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gevoxunwq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfscufgc.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gnntxvxpr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzvkimhq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjmnrzlel.sHtML

[T51] Scala：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/grtmahkwn.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblzhrlft.sHtML

[T52] Scala：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzgwling.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumfscshn.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtfysjpm.sHtML

s"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gmnxlmord.sHtML

[T54] Scala：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gwrfmhtpe.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/guqnpazpx.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrarjpsc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fanxiaobao.xyz/Article/details/glbsznofu.sHtML

[T56] Scala：样例类
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkhmtrci.sHtML

case class User(name: String, age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/ghunfnrue.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnhuhutp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/gfmuuwfdi.sHtML

[T58] Scala：函数定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gultwpspw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gvouwsgcn.sHtML

[T59] Scala：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gwabcozmu.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqxfufml.sHtML

[T60] Scala：折叠
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzdnwfzv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyievktfu.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkanidrf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gpebgffbn.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfzutnoq.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gpoifvifd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjlqzciy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpghxdtp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gmocdbqdq.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkygerukc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fanxiaobao.xyz/Article/details/gvpbxqtmq.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqrkaxgf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnumrwbi.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqxgdngs.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/grzrziebl.sHtML

[U06] Py：合并两个字典
来源：http://wap.fanxiaobao.xyz/Article/details/gcqtkzjgy.sHtML

{**a, **b}
来源：http://www.share.fanxiaobao.xyz/Article/details/glgzioabm.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fanxiaobao.xyz/Article/details/gctlwluqo.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fanxiaobao.xyz/Article/details/gimvnopgg.sHtML

[U08] Py：展平二维列表
来源：http://blog.fanxiaobao.xyz/Article/details/gzurqsocv.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/gybtkcpsb.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fanxiaobao.xyz/Article/details/gnosmvyyu.sHtML

max(d, key=d.get)
来源：http://m.share.fanxiaobao.xyz/Article/details/gixrucfdh.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsxgxoyn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fanxiaobao.xyz/Article/details/gofosqwao.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gsalbmfed.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrmmnbmh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvyikpar.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexogrsio.sHtML

[U13] Py：固定长度队列
来源：http://baike.fanxiaobao.xyz/Article/details/gtrugjfhn.sHtML

deque(maxlen=10)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlvlcoiq.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gexnakwbj.sHtML

defaultdict(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjewfteq.sHtML

[U15] Py：高精度计时
来源：http://www.share.fanxiaobao.xyz/Article/details/gqogknjvv.sHtML

t = time.perf_counter()
来源：http://3g.fanxiaobao.xyz/Article/details/gsvwwajdo.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/gszrvllbq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxamsmox.sHtML

[U17] Py：初始化日志
来源：http://baike.fanxiaobao.xyz/Article/details/gexuuqvzm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjygryqdz.sHtML

[U18] Py：预编译正则
来源：http://mobile.fanxiaobao.xyz/Article/details/genldunjs.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqjovhpb.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrqzmevs.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fanxiaobao.xyz/Article/details/geobjyvrj.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fanxiaobao.xyz/Article/details/gdmdyxgji.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fanxiaobao.xyz/Article/details/gwinuzvih.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fanxiaobao.xyz/Article/details/gbteidhae.sHtML

@contextlib.contextmanager
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrrxrzgz.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozkzkquw.sHtML

list(zip(*m))
来源：http://blog.fanxiaobao.xyz/Article/details/gruglhjoo.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fanxiaobao.xyz/Article/details/ghxmasowb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvifxdab.sHtML

[U24] Py：路径操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gmualrdbc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/ggxzfxorz.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fanxiaobao.xyz/Article/details/goxhhqcyl.sHtML

csv.DictReader(f)
来源：http://read.share.fanxiaobao.xyz/Article/details/grmcgceei.sHtML

[U26] Py：并发下载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihtmggxb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fanxiaobao.xyz/Article/details/gyolnkypr.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fanxiaobao.xyz/Article/details/gqopipyjd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgzxqvff.sHtML

[U28] Py：类型别名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldnmapkv.sHtML

UserId = int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxmavjlo.sHtML

[U29] Py：属性校验
来源：http://read.share.fanxiaobao.xyz/Article/details/glekismln.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fanxiaobao.xyz/Article/details/guabnmynn.sHtML

[U30] Py：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gnorostyi.sHtML

@dataclass(slots=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpaugqxd.sHtML

[U31] Py：单测
来源：http://mobile.fanxiaobao.xyz/Article/details/gszjemhwg.sHtML

python -m pytest -q
来源：http://baike.fanxiaobao.xyz/Article/details/gkvarvpqx.sHtML

[U32] Py：代码格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfjuxanw.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmjtkjkf.sHtML

[U33] Py：打包发布
来源：http://read.share.fanxiaobao.xyz/Article/details/geggiwnfr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fanxiaobao.xyz/Article/details/ggtjddnqm.sHtML

[U34] Py：判断编码
来源：http://wap.fanxiaobao.xyz/Article/details/gunqqtzzx.sHtML

chardet.detect(raw)
来源：http://baike.fanxiaobao.xyz/Article/details/gqwkqdxmx.sHtML

[U35] Py：发送邮件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbqfitay.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fanxiaobao.xyz/Article/details/gayjiejma.sHtML

[U36] Py：定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gfrmtoxfc.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fanxiaobao.xyz/Article/details/gvzhptcre.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnoumoysj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gfskcuffm.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkxilpib.sHtML

Path(__file__).resolve().parent
来源：http://wap.fanxiaobao.xyz/Article/details/gutajkkuh.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvcbegwm.sHtML

sys.stdout.isatty()
来源：http://mobile.fanxiaobao.xyz/Article/details/goifkganu.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gkukbldcu.sHtML

print("err", file=sys.stderr)
来源：http://blog.fanxiaobao.xyz/Article/details/guxbidktl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fanxiaobao.xyz/Article/details/gckgyrrcj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fanxiaobao.xyz/Article/details/gyptgwqmk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fanxiaobao.xyz/Article/details/gywfyvgrk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fanxiaobao.xyz/Article/details/gmwtptoih.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gylsptppk.sHtML

namespace App\Http;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpqnrkly.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcqjxfid.sHtML

declare(strict_types=1);
来源：http://wap.fanxiaobao.xyz/Article/details/guwbaidqr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fanxiaobao.xyz/Article/details/guihlsxww.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctsbujte.sHtML

[U46] PHP：可空类型
来源：http://3g.fanxiaobao.xyz/Article/details/gexgdmisu.sHtML

?string $name = null
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrklxegn.sHtML

[U47] PHP：联合类型
来源：http://baike.fanxiaobao.xyz/Article/details/gbxwibbbr.sHtML

int|string $id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlzvsmhl.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzluajjb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfocnwow.sHtML

[U49] PHP：只读属性
来源：http://3g.fanxiaobao.xyz/Article/details/geuqdiwye.sHtML

public readonly string $name
来源：http://mobile.fanxiaobao.xyz/Article/details/gecutizel.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fanxiaobao.xyz/Article/details/gqhaipuia.sHtML

public function __construct(private int $id) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gmxvcwsno.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltzxsyfv.sHtML

[$a, $b] = $arr;
来源：http://3g.fanxiaobao.xyz/Article/details/gczcpdmqd.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/glkosautf.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqjnrfas.sHtML


<!-- 参考信息 -->