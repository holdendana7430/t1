代发 wailian999

#ifndef X_H
来源：http://blog.hesvh.cn/Article/details/gftndnfdp.sHtML

#define X_H
来源：http://www.share.zdbjq.cn/Article/details/gecuuvine.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/gmzioguxq.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gsicmoatf.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/grksyormi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gxcpykeab.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gxasjnrxi.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/ganugiiim.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gjlnauliw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gesjdeqwt.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/giayiyscz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/gjpabmemp.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gzelcjjas.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gxwbperzl.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gpmktqklo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gfhaapdxg.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/ghqhphjzz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/glnwuxtyg.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/goihcdxdy.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/girjjytix.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/gpxpcjile.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.zdbjq.cn/Article/details/gwcdkojsi.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gfiyknuna.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gjqongnwn.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gkiplhvut.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gafsjalpt.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gnecygpkz.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gkcgpfvir.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gckigozqg.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fehbvm.com/Article/details/ghvcsqsxe.sHtML

[S44] C++：引用传参
来源：http://read.share.zdbjq.cn/Article/details/gfomzxqnu.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gwigpcbzv.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/gamisahcf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/gjgxturtd.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/giiucwhfo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gzwzaxdlq.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gkbnhkvaq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/gjirtjtyb.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gapigdnve.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/guedbwvnl.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gvhbwnlbv.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gzerfytud.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gbztyrxbk.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gtazbytui.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gcjoyytbc.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gwtzvlufn.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/gbsiphgfq.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gdvrjrdyy.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gfxchchdo.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/ggkaqkwsb.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gsljrikmj.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/gnmnqpjjp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/gqonnrpbo.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/gtiahfpuv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gdpyhiqyq.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gxzvsnswu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.hesvh.cn/Article/details/goevtjguy.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gveruzqpb.sHtML

constexpr int N = 10;
来源：http://baike.fehbvm.com/Article/details/gsprqbezp.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gemanutip.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gozltoklh.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/gghjhzlde.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/gsamdqgcw.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/guulzanau.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fehbvm.com/Article/details/gtotjgale.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxcpndycc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/grnvdiekv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gknbkbpfy.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/ghyyxkamh.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/giecmnhtj.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gfhlhjmps.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gmrspqlyt.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/gzxqqvbwr.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/gxjxrbsis.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/ghklnkrxl.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/ghppnsxxm.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/geqgsdmvj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/getatyfsv.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gmamutnau.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gxbhdzuwy.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/gsjnrvilm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/gnubcvsii.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/gpexneqfg.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gzncgahhs.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/gztjuqaih.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gevdfgxmu.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/gfhwffamf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gefighreg.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gokomtcjn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gjgvvionk.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gpikzwgau.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gvkoygkcy.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/gkzppnipx.sHtML

val m = mapOf("a" to 1)
来源：http://wap.hesvh.cn/Article/details/grduwajpj.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gdnokuxsj.sHtML

for (i in 1..10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gvmgopamc.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/girkvemad.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/ghhjqsdpp.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/guoviymne.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gepgehqyu.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fehbvm.com/Article/details/gdmqgjwlr.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/gbusnnnuh.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/gcgkxzyvf.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/gdqjmecfa.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gimnorwbs.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.hesvh.cn/Article/details/gtdcrksgy.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/gtwqvbsvm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/gwtilfyst.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/glpusonpd.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/gzftfligu.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/gpnvjfoaz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gakfzlfqh.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gohpwbdsh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/ghpttraoj.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/gsjzrkbyq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gidemdhwk.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/gaajyulbw.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/geicrgpop.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/gifnwylpu.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/gmmfhrrgu.sHtML

[T27] Swift：错误处理
来源：http://mobile.fehbvm.com/Article/details/grimamcmn.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/giyjhkscy.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gqkifefux.sHtML

enum Color { case red, green }
来源：http://www.blog.hesvh.cn/Article/details/grultwarh.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/gmsikhepc.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/godclmctl.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/gcbggsclg.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/gyjogzpbp.sHtML

[T31] Lua：Hello World
来源：http://www.share.hesvh.cn/Article/details/ghumijoam.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gzfhwvhhp.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gilhchibv.sHtML

local a = 1
来源：http://www.m.share.hesvh.cn/Article/details/ghpwuitap.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fehbvm.com/Article/details/gmxfoyzjp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.zdbjq.cn/Article/details/gvorjfhzn.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gklfstaal.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/gygcxcntw.sHtML

[T35] Lua：字典表
来源：http://wap.zdbjq.cn/Article/details/goupdrxkp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/gvccqzrql.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/ghupgrqgk.sHtML

function add(a, b) return a + b end
来源：http://baike.zdbjq.cn/Article/details/gbdbpsyas.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gkwmwuzsp.sHtML

"a" .. "b"
来源：http://read.share.zdbjq.cn/Article/details/gysngzqhx.sHtML

[T38] Lua：条件
来源：http://mobile.zdbjq.cn/Article/details/giniuoqcc.sHtML

if x > 0 then print("正") end
来源：http://mobile.hesvh.cn/Article/details/gdmawunsn.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gyaerwexs.sHtML

string.find(s, "%d+")
来源：http://m.share.zdbjq.cn/Article/details/gceplcbzc.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/giqdjnlrx.sHtML

setmetatable({}, { __index = base })
来源：http://3g.zdbjq.cn/Article/details/gguttczxo.sHtML

[T41] Perl：Hello World
来源：http://wap.zdbjq.cn/Article/details/gosuwrifm.sHtML

print "Hello\n";
来源：http://read.share.hesvh.cn/Article/details/gebdbatem.sHtML

[T42] Perl：变量类型
来源：http://wap.hesvh.cn/Article/details/gjvmaweil.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gyuvwyebu.sHtML

[T43] Perl：字符串插值
来源：http://wap.zdbjq.cn/Article/details/ghuafvfca.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/gioptvxva.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/gomqayqoe.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/gwoefhbwh.sHtML

[T45] Perl：数组遍历
来源：http://baike.fehbvm.com/Article/details/gczbazxxb.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.zdbjq.cn/Article/details/gomingmra.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/gallhxyno.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fehbvm.com/Article/details/gcwsqxomx.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/gdpdlnnnn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/gfwcoybhz.sHtML

[T48] Perl：正则替换
来源：http://baike.hesvh.cn/Article/details/gfpmeagtj.sHtML

$s =~ s/old/new/g;
来源：http://read.share.hesvh.cn/Article/details/gmqtxqtmc.sHtML

[T49] Perl：函数
来源：http://3g.zdbjq.cn/Article/details/glnoortdu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gjohvliuj.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gliqqyvfn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.zdbjq.cn/Article/details/glmfoyiqq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/gpavcptlz.sHtML

[T51] Scala：Hello World
来源：http://wap.zdbjq.cn/Article/details/gshpdsqnh.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gtllnlmme.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/gwmxrojln.sHtML

val a = 1;  var b = 2
来源：http://read.share.fehbvm.com/Article/details/gjtpzxhjv.sHtML

[T53] Scala：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gaixkdmcd.sHtML

s"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gzsbylcxj.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gfbenwpzc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/gfwostlum.sHtML

[T55] Scala：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gtvboitvm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.hesvh.cn/Article/details/gsiikvkid.sHtML

[T56] Scala：样例类
来源：http://www.blog.fehbvm.com/Article/details/guaesqlib.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/glbzwlzbp.sHtML

[T57] Scala：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gflyixjjg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/ggghuolvo.sHtML

[T58] Scala：函数定义
来源：http://mobile.zdbjq.cn/Article/details/gjkduttce.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.zdbjq.cn/Article/details/ggcykwuso.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/gzowomhqs.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gxugkburw.sHtML

[T60] Scala：折叠
来源：http://baike.zdbjq.cn/Article/details/ggntusykv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/gaohzdkft.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkrkkhhee.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gzkystnju.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwcchjsgy.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.hesvh.cn/Article/details/gcgqqjqio.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/gvqpcbtju.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.zdbjq.cn/Article/details/gbpkqeajg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.hesvh.cn/Article/details/gkrptqbhw.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gjfosozyp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/gwemlaxfk.sHtML

[U04] Py：变量调试打印
来源：http://www.share.zdbjq.cn/Article/details/glqaxvbvf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gfhomgrhq.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.zdbjq.cn/Article/details/gjfccrodb.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/ggqyplaoa.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/gcgniqwzv.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/gdnvhpyas.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fehbvm.com/Article/details/gnmgjgfas.sHtML

{v: k for k, v in d.items()}
来源：http://baike.hesvh.cn/Article/details/gcsasjhfj.sHtML

[U08] Py：展平二维列表
来源：http://m.share.zdbjq.cn/Article/details/grtdxcyvz.sHtML

[y for x in nested for y in x]
来源：http://blog.hesvh.cn/Article/details/gbjdidbxz.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fehbvm.com/Article/details/gzdkdueed.sHtML

max(d, key=d.get)
来源：http://3g.hesvh.cn/Article/details/ghcvopmxt.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fehbvm.com/Article/details/gbwlpieop.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/gzbriktjs.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/guuieesgq.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/gufadspaj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.hesvh.cn/Article/details/glpxotkjm.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/grdrdxaag.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fehbvm.com/Article/details/gunyjizfd.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/gsrqyeook.sHtML

[U14] Py：分组收集到列表
来源：http://3g.hesvh.cn/Article/details/gdlgmljkz.sHtML

defaultdict(list)
来源：http://blog.fehbvm.com/Article/details/gobwfmwnj.sHtML

[U15] Py：高精度计时
来源：http://baike.hesvh.cn/Article/details/guqfzctve.sHtML

t = time.perf_counter()
来源：http://www.m.share.hesvh.cn/Article/details/gonwkqqoy.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/gnzsjnvgh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.zdbjq.cn/Article/details/gohkujikb.sHtML

[U17] Py：初始化日志
来源：http://www.share.fehbvm.com/Article/details/gxgjvrqqk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.zdbjq.cn/Article/details/ggnooeffp.sHtML

[U18] Py：预编译正则
来源：http://www.blog.hesvh.cn/Article/details/grfqbuzry.sHtML

pat = re.compile(r"\d+")
来源：http://3g.hesvh.cn/Article/details/gvacnbjii.sHtML

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/gnelpjytw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.hesvh.cn/Article/details/gcjdxlfcv.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fehbvm.com/Article/details/gakzgswzr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fehbvm.com/Article/details/gidcdgprc.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.zdbjq.cn/Article/details/gmkjrqnop.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/gwyzrwyyi.sHtML

[U22] Py：矩阵转置
来源：http://3g.zdbjq.cn/Article/details/gtfyqzatj.sHtML

list(zip(*m))
来源：http://baike.hesvh.cn/Article/details/genlfobjq.sHtML

[U23] Py：分块读取大文件
来源：http://blog.hesvh.cn/Article/details/gdlsvdzkl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.zdbjq.cn/Article/details/ginwiirxx.sHtML

[U24] Py：路径操作
来源：http://mobile.fehbvm.com/Article/details/gkvzumhze.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gducjlklk.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fehbvm.com/Article/details/gthszjgwt.sHtML

csv.DictReader(f)
来源：http://www.share.zdbjq.cn/Article/details/gtymdzklj.sHtML

[U26] Py：并发下载
来源：http://www.blog.zdbjq.cn/Article/details/gjtpvwqcj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/guypmyuhf.sHtML

[U27] Py：异步 HTTP
来源：http://baike.hesvh.cn/Article/details/gvwwfkwrt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.zdbjq.cn/Article/details/gfvjdbrjm.sHtML

[U28] Py：类型别名
来源：http://www.blog.hesvh.cn/Article/details/gtavnzuav.sHtML

UserId = int
来源：http://www.m.share.fehbvm.com/Article/details/gyxnkfmyb.sHtML

[U29] Py：属性校验
来源：http://mobile.fehbvm.com/Article/details/gjuxicxmq.sHtML

@property 与 @x.setter 配合
来源：http://read.share.zdbjq.cn/Article/details/grqqshtng.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/gemysdkhi.sHtML

@dataclass(slots=True)
来源：http://3g.fehbvm.com/Article/details/gcqhdguys.sHtML

[U31] Py：单测
来源：http://www.share.fehbvm.com/Article/details/gvapjybfq.sHtML

python -m pytest -q
来源：http://mobile.fehbvm.com/Article/details/gixjwoqns.sHtML

[U32] Py：代码格式化
来源：http://m.share.fehbvm.com/Article/details/giqqyfiih.sHtML

ruff format . && ruff check --fix .
来源：http://blog.zdbjq.cn/Article/details/gvvurfjwj.sHtML

[U33] Py：打包发布
来源：http://mobile.zdbjq.cn/Article/details/gpyuutayi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.zdbjq.cn/Article/details/goslbxdmn.sHtML

[U34] Py：判断编码
来源：http://3g.zdbjq.cn/Article/details/gjyodoioa.sHtML

chardet.detect(raw)
来源：http://mobile.zdbjq.cn/Article/details/gtwuzigmh.sHtML

[U35] Py：发送邮件
来源：http://www.blog.zdbjq.cn/Article/details/gdjeciewp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fehbvm.com/Article/details/ghqzjnsqx.sHtML

[U36] Py：定时任务
来源：http://3g.hesvh.cn/Article/details/ggbaqctzc.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/gdizizcjk.sHtML

[U37] Py：读写 Excel
来源：http://mobile.zdbjq.cn/Article/details/gsppcqbxf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.zdbjq.cn/Article/details/gljktcszg.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.hesvh.cn/Article/details/gshbamzsh.sHtML

Path(__file__).resolve().parent
来源：http://wap.zdbjq.cn/Article/details/gbgflfnlj.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/gfepzlhyb.sHtML

sys.stdout.isatty()
来源：http://www.m.share.hesvh.cn/Article/details/gvfqwbqvx.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/gdhtqraky.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/galpwguyx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.zdbjq.cn/Article/details/gvwwwbjbp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.hesvh.cn/Article/details/gplmoksfo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fehbvm.com/Article/details/gsuffhftt.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fehbvm.com/Article/details/gpccivlkm.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fehbvm.com/Article/details/glaehwxdb.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/gdqnvtcob.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fehbvm.com/Article/details/gxazknllu.sHtML

declare(strict_types=1);
来源：http://m.share.zdbjq.cn/Article/details/gtnphlpku.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/gziccbqdy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gamzypuhm.sHtML

[U46] PHP：可空类型
来源：http://read.share.hesvh.cn/Article/details/girgphqyy.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/gewngqikk.sHtML

[U47] PHP：联合类型
来源：http://3g.hesvh.cn/Article/details/gfrukqksu.sHtML

int|string $id
来源：http://www.blog.hesvh.cn/Article/details/gctqsmclb.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/gfchmhzrg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.zdbjq.cn/Article/details/gvzqxoxlb.sHtML

[U49] PHP：只读属性
来源：http://mobile.hesvh.cn/Article/details/gnptqvjsi.sHtML

public readonly string $name
来源：http://baike.zdbjq.cn/Article/details/gsqyltnqs.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.zdbjq.cn/Article/details/grxnambqq.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fehbvm.com/Article/details/gasebemvr.sHtML

[U51] PHP：数组解构
来源：http://read.share.hesvh.cn/Article/details/gxuggwcfy.sHtML

[$a, $b] = $arr;
来源：http://wap.zdbjq.cn/Article/details/gvehyhnqe.sHtML

[U52] PHP：箭头函数
来源：http://baike.zdbjq.cn/Article/details/glziaxtlw.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.hesvh.cn/Article/details/gburpfdvo.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.hesvh.cn/Article/details/gwyqcuotd.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.zdbjq.cn/Article/details/grddpprfj.sHtML

[U54] PHP：空安全调用
来源：http://baike.zdbjq.cn/Article/details/gwnwtqwbk.sHtML

$obj?->method()
来源：http://read.share.hesvh.cn/Article/details/gskeyuvnj.sHtML


<!-- 参考信息 -->