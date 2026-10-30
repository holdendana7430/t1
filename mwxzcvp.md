代发 wailian999

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/gkuwpxmky.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/gbxwwmfrp.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gqhzwxcby.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gchbabgal.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gibfnhglc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/glbgxmhrj.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/gjpkogtug.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gfvreqaos.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/gpgnfussm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gjzqjnmqi.sHtML

[S36] C++：unordered_map
来源：http://wap.fehbvm.com/Article/details/ghwbwuwni.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gxsffupbm.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gnyynvdoy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gtdazyrbu.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gzgeujnbh.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gifnsaswa.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/gysqtnlgm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gnqfjhosw.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/gzuwfqpho.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gxicieqgd.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/gyhqlnatx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/gtxzhguil.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gkhawouem.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/guhbsxazz.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/ggscfmkpj.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/gwzngvglq.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gryghyvlb.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/ggagdtptb.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gniutjpwt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gqtefvuqb.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/gktamrbwd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/gdorpbxpc.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/ggnuzbflx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gtgszdseq.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gjyxvktxb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/gkfgbyrcr.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/gpekqggwa.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/gesliixrv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/grjykwknr.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/gsjqmiufh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gghhgrtal.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/gedzznkam.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gnfqdvqhm.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/giaqtiqtr.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gnenkpqkt.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/gokucyxco.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/gikwblxte.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/gxzkvrnab.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gfmncfdhq.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gvmlxwobq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/gwpcexyup.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/gahydtlgr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gcidwsayq.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/gthihmqtb.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gazadzuqc.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gqeatfeih.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/guacmzwmi.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/gifcdqvto.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/gdzeizmip.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/goplmmrjq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gsmhdovyx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwqztejse.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gnvpebbby.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gszeaocce.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/gatzkmlyj.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gcohergrn.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/gixtvpfxe.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/gnaquatnd.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/gbapsuugs.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gajvpxrds.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/grozvofap.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gjwajtwmh.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/ggpfnuzgn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/geltppifr.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gdfdqoozk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gunzqgcew.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gkrlgdbnn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gmegjthmj.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gwnpesypx.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/glgnimtaf.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/guachjlwz.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/gveauaczg.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/gjohdmwwf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fehbvm.com/Article/details/gqrjjamtm.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gddysyrly.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gsrfeqxyt.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gfwvfgvpd.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gdardhomz.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gjzxbqnmt.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/govenmhfr.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gxlndwdfl.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/gzixjaxem.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/glhlqenaf.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.hesvh.cn/Article/details/gtfkqzjqm.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gdxqvepzy.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gkjftuzdj.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/gwxryfsra.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/ghxvxcfnz.sHtML

[T18] Swift：字符串插值
来源：http://blog.fehbvm.com/Article/details/ggkjbprfd.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gwdgovdot.sHtML

[T19] Swift：可选绑定
来源：http://read.share.hesvh.cn/Article/details/gccjbgurs.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/gtwhquadu.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/gxjoekqqj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/gbqadlisn.sHtML

[T21] Swift：遍历
来源：http://mobile.zdbjq.cn/Article/details/gorjqqlel.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/gceunibjy.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gkmuqhvul.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/ggcxlklha.sHtML

[T23] Swift：函数
来源：http://wap.fehbvm.com/Article/details/gyooikoez.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gjzmzeusu.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gezopharo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gdxgkbtig.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/gjndhuovy.sHtML

struct P { var x: Int }
来源：http://www.m.share.hesvh.cn/Article/details/gwcgynavj.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/gocxvfwhn.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/goddhijut.sHtML

[T27] Swift：错误处理
来源：http://www.blog.hesvh.cn/Article/details/ggttvcucw.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fehbvm.com/Article/details/ggtkgsksr.sHtML

[T28] Swift：枚举
来源：http://www.m.share.hesvh.cn/Article/details/ggcrhsyyl.sHtML

enum Color { case red, green }
来源：http://m.share.hesvh.cn/Article/details/gbdxcdxxs.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fehbvm.com/Article/details/gyuverxiz.sHtML

guard let x = opt else { return }
来源：http://baike.hesvh.cn/Article/details/gxznwtbbj.sHtML

[T30] Swift：协议
来源：http://www.share.zdbjq.cn/Article/details/giaipeacu.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gxxqihkap.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gukydqbqi.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/ghzvcdusb.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/grzeelxyc.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/gnrxwfbyo.sHtML

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/guvnbwpug.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/gcsdrlrol.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/gezgglcju.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/gzrbmbaym.sHtML

[T35] Lua：字典表
来源：http://blog.fehbvm.com/Article/details/gehlrwzhz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gsgomlbof.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/gdiddyast.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/gztdafqck.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gyutuoczj.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/gpurfqlbb.sHtML

[T38] Lua：条件
来源：http://m.share.hesvh.cn/Article/details/gjmiothec.sHtML

if x > 0 then print("正") end
来源：http://www.share.hesvh.cn/Article/details/gsnzwfrhj.sHtML

[T39] Lua：模式匹配
来源：http://3g.hesvh.cn/Article/details/gqlefhlvk.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gsxzxsemg.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/grioiarjs.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/gsfctbuou.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/glqbdpcwf.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/grcaghjhl.sHtML

[T42] Perl：变量类型
来源：http://m.share.hesvh.cn/Article/details/gjgtjorsy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fehbvm.com/Article/details/gnnzqyskg.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/gypyejftb.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/gnxzljomk.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/gamkcxysz.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.zdbjq.cn/Article/details/gaeggmzyp.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/gmorowyio.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/gahlrnpkq.sHtML

[T46] Perl：哈希操作
来源：http://read.share.zdbjq.cn/Article/details/greurvryl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/gdonkpzvu.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.hesvh.cn/Article/details/gvftckazd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fehbvm.com/Article/details/geanvbrhn.sHtML

[T48] Perl：正则替换
来源：http://read.share.fehbvm.com/Article/details/gpuhnupnk.sHtML

$s =~ s/old/new/g;
来源：http://3g.zdbjq.cn/Article/details/gatgjpnks.sHtML

[T49] Perl：函数
来源：http://www.share.zdbjq.cn/Article/details/ggxgnqbor.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gezfhrjdi.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gnksnobfh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/geytmpszv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/gomnytjqa.sHtML

[T51] Scala：Hello World
来源：http://baike.hesvh.cn/Article/details/gfstporcm.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gnsxelpzv.sHtML

[T52] Scala：变量
来源：http://wap.fehbvm.com/Article/details/gdycxiqyh.sHtML

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/gnxydahqx.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gtuuxylev.sHtML

s"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gagjvtwhk.sHtML

[T54] Scala：集合映射
来源：http://m.share.fehbvm.com/Article/details/gurfxxenb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/glmvzmabf.sHtML

[T55] Scala：集合过滤
来源：http://3g.fehbvm.com/Article/details/gtcilcvyo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fehbvm.com/Article/details/gddvafxxm.sHtML

[T56] Scala：样例类
来源：http://wap.fehbvm.com/Article/details/gjnumjixr.sHtML

case class User(name: String, age: Int)
来源：http://baike.hesvh.cn/Article/details/giofmezzo.sHtML

[T57] Scala：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gqukegkjk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.zdbjq.cn/Article/details/gqeexkixc.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/gthbseqme.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fehbvm.com/Article/details/gfbnlysdm.sHtML

[T59] Scala：循环
来源：http://baike.zdbjq.cn/Article/details/gdbukqfnm.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/glyypiofz.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/gvfuslmum.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/gatlirsgy.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gaikfcqne.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/geqedjadp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gncolfmkx.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gsvzmtlys.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/gsbsrgdvz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.hesvh.cn/Article/details/gfxiiljmn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.hesvh.cn/Article/details/gfdpmbeje.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.hesvh.cn/Article/details/glzfhfqhd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.zdbjq.cn/Article/details/gaqcnxgbq.sHtML

[U04] Py：变量调试打印
来源：http://m.share.hesvh.cn/Article/details/gihqipktc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fehbvm.com/Article/details/grfpuunjt.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.hesvh.cn/Article/details/gxzmqwhvd.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gqhopavjq.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/gupnbraaz.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/gjohbmrrx.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fehbvm.com/Article/details/gycryetrl.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.zdbjq.cn/Article/details/gbjcapolu.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/gldfyhvtk.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/giobydclq.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.zdbjq.cn/Article/details/guyituxgt.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gbqbqymua.sHtML

[U10] Py：按值排序字典
来源：http://3g.fehbvm.com/Article/details/gjmqckwqc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/gmwqieogb.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/gdrmscrkz.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/gctkqgrsu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/gtexiiylx.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/ghdorutzq.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fehbvm.com/Article/details/gpvdxkjwd.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/gvisdbqij.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.hesvh.cn/Article/details/gpshmjedg.sHtML

defaultdict(list)
来源：http://m.share.zdbjq.cn/Article/details/gfugoxvfu.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/gjzymdurb.sHtML

t = time.perf_counter()
来源：http://m.share.fehbvm.com/Article/details/gppcgzyrf.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/ghzcolucc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/gwilgwyac.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/gssjxnkfm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.zdbjq.cn/Article/details/gzakpiswd.sHtML

[U18] Py：预编译正则
来源：http://baike.zdbjq.cn/Article/details/gkehyqtar.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/gazzofpuf.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.hesvh.cn/Article/details/gmgzxooyq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.hesvh.cn/Article/details/gfdhcylme.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fehbvm.com/Article/details/gchqygyzu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.zdbjq.cn/Article/details/gylerimib.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.zdbjq.cn/Article/details/gkvteawrt.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/gewespicw.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fehbvm.com/Article/details/ghastnhmx.sHtML

list(zip(*m))
来源：http://mobile.zdbjq.cn/Article/details/gofsdslom.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fehbvm.com/Article/details/gvngbkrlx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fehbvm.com/Article/details/gztqtqbjw.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/gkbjdmfqq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gnawifomd.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fehbvm.com/Article/details/gdvyhzfob.sHtML

csv.DictReader(f)
来源：http://3g.zdbjq.cn/Article/details/gmxptfvaf.sHtML

[U26] Py：并发下载
来源：http://wap.hesvh.cn/Article/details/gnmyrauhh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fehbvm.com/Article/details/gimovisvj.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fehbvm.com/Article/details/gunjwyxto.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fehbvm.com/Article/details/gdsdkwufv.sHtML

[U28] Py：类型别名
来源：http://3g.fehbvm.com/Article/details/gxjnyvyxz.sHtML

UserId = int
来源：http://mobile.hesvh.cn/Article/details/gqjkzkqjz.sHtML

[U29] Py：属性校验
来源：http://wap.hesvh.cn/Article/details/gykwogfbo.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/gmugntdpz.sHtML

[U30] Py：数据类
来源：http://www.share.hesvh.cn/Article/details/gfmvayrhg.sHtML

@dataclass(slots=True)
来源：http://baike.fehbvm.com/Article/details/gauucrbxi.sHtML

[U31] Py：单测
来源：http://wap.zdbjq.cn/Article/details/ggddqsnmy.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/gnyfdfluw.sHtML

[U32] Py：代码格式化
来源：http://mobile.hesvh.cn/Article/details/gtuqgofqa.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/gmtanxrqk.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/gatzatxnc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/gkzzplqxa.sHtML

[U34] Py：判断编码
来源：http://read.share.fehbvm.com/Article/details/gjphcvpgq.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/gbahaefib.sHtML

[U35] Py：发送邮件
来源：http://baike.zdbjq.cn/Article/details/gntpzqgex.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/gczxqbtps.sHtML

[U36] Py：定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gklfjldrp.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fehbvm.com/Article/details/gomhtbpkr.sHtML

[U37] Py：读写 Excel
来源：http://3g.fehbvm.com/Article/details/gyynrgzil.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.hesvh.cn/Article/details/ggsoghsxm.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.hesvh.cn/Article/details/gpmqalmkt.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.zdbjq.cn/Article/details/gexwlkdho.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.zdbjq.cn/Article/details/gqalfaqfn.sHtML

sys.stdout.isatty()
来源：http://wap.zdbjq.cn/Article/details/gwedqdnzb.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/gkgovkipp.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gwyfjigga.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fehbvm.com/Article/details/gxmpshqbb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/gurlezwpy.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.hesvh.cn/Article/details/gxbvrydjm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/ggwrgmdgx.sHtML

[U43] PHP：声明命名空间
来源：http://baike.hesvh.cn/Article/details/gvqtamzcx.sHtML

namespace App\Http;
来源：http://baike.fehbvm.com/Article/details/gwpugmggl.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.zdbjq.cn/Article/details/goisxumxq.sHtML

declare(strict_types=1);
来源：http://www.blog.fehbvm.com/Article/details/gzugsmexf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.zdbjq.cn/Article/details/gwhnrojwg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/getmksvyc.sHtML

[U46] PHP：可空类型
来源：http://read.share.zdbjq.cn/Article/details/gxcuglvgb.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/gfhdklywr.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/gofvhoxxd.sHtML

int|string $id
来源：http://baike.zdbjq.cn/Article/details/ghazccrhj.sHtML

[U48] PHP：纯枚举
来源：http://mobile.hesvh.cn/Article/details/gbgjllyvu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.zdbjq.cn/Article/details/gzkjewlqf.sHtML

[U49] PHP：只读属性
来源：http://wap.hesvh.cn/Article/details/gmnchcenb.sHtML

public readonly string $name
来源：http://blog.fehbvm.com/Article/details/gplphqprt.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.zdbjq.cn/Article/details/gfvvaqjun.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.hesvh.cn/Article/details/gfgthinis.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/gpvmqbmid.sHtML

[$a, $b] = $arr;
来源：http://blog.hesvh.cn/Article/details/gwdbzmhcr.sHtML

[U52] PHP：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gicbndaxo.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/ghurvruek.sHtML

[U53] PHP：空合并运算符
来源：http://blog.hesvh.cn/Article/details/gcuzgzdve.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.zdbjq.cn/Article/details/gsccxhlaa.sHtML

[U54] PHP：空安全调用
来源：http://blog.fehbvm.com/Article/details/guvcenfzf.sHtML

$obj?->method()
来源：http://wap.fehbvm.com/Article/details/gqghtccji.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/gkvvyjtuk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.hesvh.cn/Article/details/glypnusol.sHtML

[U56] PHP：命名参数
来源：http://blog.hesvh.cn/Article/details/gdqoupcch.sHtML

f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gojztbovo.sHtML


<!-- 参考信息 -->