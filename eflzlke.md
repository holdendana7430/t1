代发 wailian999

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gmvvxslwy.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gwtgdyqbl.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/gpjvyaxio.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gkfcqpurl.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/ggtndrfdc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/gnldhnvcv.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gkszzvgxg.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.zdbjq.cn/Article/details/gnhxwouzy.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/gqwgxwjbx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/ggsskzvco.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/grtvqxobp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/gjwdsdnym.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gqgyfooow.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/glynsuqot.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gfwjllcpa.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gxlehactt.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/gygbwjprv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/gzyzxjows.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/gwtehsweb.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/guxnetxno.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/guzsodjei.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/grmzhicck.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gicpaihjg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gdqbucyrt.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gwizvgcct.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/gxhpzrniy.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/gxfsdqyqk.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/ghpgurgiv.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gjxqvdcfw.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gykjjvtlr.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/ghrgbmvdq.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/gpbekuytz.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/gssjnhhck.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gmeyoafvs.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gmhpqavol.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/gxamskfiq.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/ghposxnad.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/gtdqtsohl.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gtaomcuwv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/geqjccpcw.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/ggsyjvyjt.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gbviuvkji.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/gavnaoxfc.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/geyzvbqxr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gaketsdqe.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/glpspyexu.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/gbkteylzo.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gaderocir.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/grihnbiuc.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/gmldskvse.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/gdagviwzp.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gllnqpkdt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/gkbajbqje.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gnpuvpccn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/gdglewxug.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gdmgiolqx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/gplnciviw.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/geobzcekv.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/gkybtyqpr.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/gzgeovzad.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gnafpfbse.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/gfzgxntgd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gqmvwwnvv.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/gwakcbvzw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/ghjabsuav.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxatrfgmp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/geqznymbt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkjdhvggu.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gjrbbpcls.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/glgkpwisb.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gbvtnxdql.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gfhsdoeen.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gafczsfym.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gbcgwtznw.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/ginvosxgh.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/gnfwxdaum.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gcjhzcstj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/ghnxwpcku.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gtvlepkvr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gpybfkzli.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gzywwbxkq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/ghoykdqqs.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/gckgzukzw.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/gayejtvjd.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.hesvh.cn/Article/details/gftfgzebq.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gbbyoicpk.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gcqjwjier.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/gsdjosmbq.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gkrdrhlsn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gbtdxtjmn.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/gehvemdmw.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gpovvumig.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/greyapavp.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjhqxmxhc.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/gmbibfaoj.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/gaqbnxgjg.sHtML

[T15] Kotlin：接口
来源：http://wap.hesvh.cn/Article/details/gixffzifn.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gqogxjsdd.sHtML

[T16] Swift：Hello World
来源：http://mobile.hesvh.cn/Article/details/gybdyfaef.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/geqrhzxta.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gogdjdplv.sHtML

var a = 1;  let b = 2
来源：http://blog.zdbjq.cn/Article/details/gubkrufkw.sHtML

[T18] Swift：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gvtbbnuhl.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gblcltidp.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/glouyjvgn.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gnkpgflji.sHtML

[T20] Swift：数组操作
来源：http://baike.zdbjq.cn/Article/details/ggtyyvpjl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gsksdqrqp.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/gnrnmgkwd.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/gngynghsz.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/ggeoclchr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gelyxpcfk.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/gyttgezhv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fehbvm.com/Article/details/gaywcyght.sHtML

[T24] Swift：闭包
来源：http://www.share.hesvh.cn/Article/details/gkjlhdhwe.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/ghuqcjdnm.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/gbjbxdona.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/gltsgqfzy.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/gilqxrdbi.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/guldfvjij.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gqzcpwtgj.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gfrjyopxv.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/gzxrhwvqo.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/ghcwgdmzp.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/gpnkswtqs.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/gegjskwja.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/gycmobuvt.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gjqnytckn.sHtML

[T31] Lua：Hello World
来源：http://www.share.hesvh.cn/Article/details/glbhwoefw.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gmiszjflz.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gmbadllew.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/gheakhvok.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/gxfsbzkqp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gtmlwsphq.sHtML

[T34] Lua：遍历表
来源：http://mobile.hesvh.cn/Article/details/gykttqulh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.hesvh.cn/Article/details/gjupvhexs.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gxppiayzy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.hesvh.cn/Article/details/gkidjtfzk.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/gstclupef.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/gicexmzte.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/grmkmxwvr.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/glgfsmwzb.sHtML

[T38] Lua：条件
来源：http://3g.hesvh.cn/Article/details/gdgdltqhw.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/ghvemkdub.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gbvuoqpwf.sHtML

string.find(s, "%d+")
来源：http://blog.hesvh.cn/Article/details/gpoowhjuc.sHtML

[T40] Lua：元表
来源：http://www.m.share.hesvh.cn/Article/details/ghyoitxpm.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.hesvh.cn/Article/details/gophxdtvt.sHtML

[T41] Perl：Hello World
来源：http://read.share.zdbjq.cn/Article/details/glynikhar.sHtML

print "Hello\n";
来源：http://mobile.zdbjq.cn/Article/details/gjqewatkd.sHtML

[T42] Perl：变量类型
来源：http://mobile.hesvh.cn/Article/details/guulijjvx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/gdkfqicdg.sHtML

[T43] Perl：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gjyfkhiyz.sHtML

"值: $a"
来源：http://read.share.hesvh.cn/Article/details/gklijlcdd.sHtML

[T44] Perl：条件
来源：http://3g.hesvh.cn/Article/details/givnurppy.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/gwahlljgu.sHtML

[T45] Perl：数组遍历
来源：http://wap.fehbvm.com/Article/details/gbetwgrsq.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fehbvm.com/Article/details/gbxneancn.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/gymzffhzm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.hesvh.cn/Article/details/gvwxzznau.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/giydzahae.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/gpyelbxzz.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/gmzpcmepl.sHtML

$s =~ s/old/new/g;
来源：http://www.share.hesvh.cn/Article/details/gofllbnlt.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/gmtflwqfx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gdxxgsmna.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/glcjhdcna.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.zdbjq.cn/Article/details/giykgvhvc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gohgplwrg.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/gnfagzgdj.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gvnpungtk.sHtML

[T52] Scala：变量
来源：http://mobile.hesvh.cn/Article/details/gwajggdbk.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gkchymrlw.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gvchextep.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gvcaythge.sHtML

[T54] Scala：集合映射
来源：http://baike.hesvh.cn/Article/details/gmtvrewtn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gwrjgdlgn.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gbgyfaztd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.zdbjq.cn/Article/details/ggomzomao.sHtML

[T56] Scala：样例类
来源：http://blog.fehbvm.com/Article/details/gbbgynkkl.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fehbvm.com/Article/details/gloopcsyb.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gsipyuafh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gzodibarv.sHtML

[T58] Scala：函数定义
来源：http://www.share.hesvh.cn/Article/details/gvpwhctur.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.hesvh.cn/Article/details/gavvcrswt.sHtML

[T59] Scala：循环
来源：http://www.share.hesvh.cn/Article/details/gylfsggky.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gxhmeprrc.sHtML

[T60] Scala：折叠
来源：http://mobile.zdbjq.cn/Article/details/gwgiwftlx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fehbvm.com/Article/details/gftofrfcf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnmbiqljq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gwyiptdxu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/garupvdbe.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gmzofqxhf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/gyoorjqvm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/gzdtsdyco.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.zdbjq.cn/Article/details/gsntlkagd.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fehbvm.com/Article/details/gnizyihmw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/ginlurwnt.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/gqjcnvmki.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/gkukpkxms.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.zdbjq.cn/Article/details/gtsxyskns.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gfzwgibjk.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.hesvh.cn/Article/details/gfgsghknb.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/gewyilwxj.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/genaigtny.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fehbvm.com/Article/details/ghysqsiwa.sHtML

[U08] Py：展平二维列表
来源：http://m.share.zdbjq.cn/Article/details/gmeavepie.sHtML

[y for x in nested for y in x]
来源：http://www.share.zdbjq.cn/Article/details/gnkbedcyy.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.hesvh.cn/Article/details/gprfuwguk.sHtML

max(d, key=d.get)
来源：http://www.m.share.zdbjq.cn/Article/details/ggafiuzrj.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.hesvh.cn/Article/details/gzmamzqxo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fehbvm.com/Article/details/gzswozchj.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fehbvm.com/Article/details/gmcaizmkl.sHtML

(x * 2 for x in arr)
来源：http://wap.zdbjq.cn/Article/details/gvlhtrbho.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fehbvm.com/Article/details/geototlue.sHtML

Counter(arr).most_common(3)
来源：http://3g.zdbjq.cn/Article/details/gyizvvcla.sHtML

[U13] Py：固定长度队列
来源：http://m.share.hesvh.cn/Article/details/gxzlituxy.sHtML

deque(maxlen=10)
来源：http://www.m.share.hesvh.cn/Article/details/gwwsnjkah.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/gqbdrsxgf.sHtML

defaultdict(list)
来源：http://3g.zdbjq.cn/Article/details/gdhnvtyvf.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/grelaydgv.sHtML

t = time.perf_counter()
来源：http://mobile.hesvh.cn/Article/details/geyurghiq.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.zdbjq.cn/Article/details/ggiohkdli.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.zdbjq.cn/Article/details/gcfnrapsq.sHtML

[U17] Py：初始化日志
来源：http://blog.fehbvm.com/Article/details/gvtrupgbj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.zdbjq.cn/Article/details/glplknvcl.sHtML

[U18] Py：预编译正则
来源：http://www.share.fehbvm.com/Article/details/gpthfbebs.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gyjsoqaka.sHtML

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/gfhhjyeya.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fehbvm.com/Article/details/gpcprtvam.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.hesvh.cn/Article/details/grfdfuufx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/gzhgprsfn.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/gugeawsmj.sHtML

@contextlib.contextmanager
来源：http://3g.fehbvm.com/Article/details/geuvvbisv.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fehbvm.com/Article/details/gjbkrmvad.sHtML

list(zip(*m))
来源：http://wap.hesvh.cn/Article/details/gulvictyr.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fehbvm.com/Article/details/guuvfiork.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/gymkuqscz.sHtML

[U24] Py：路径操作
来源：http://blog.zdbjq.cn/Article/details/gpjowyssv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gszbdfklv.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fehbvm.com/Article/details/gylrvkcpd.sHtML

csv.DictReader(f)
来源：http://baike.fehbvm.com/Article/details/ggfocvryg.sHtML

[U26] Py：并发下载
来源：http://wap.zdbjq.cn/Article/details/gilfiyznd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.hesvh.cn/Article/details/gocrtmlff.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/gbsndddex.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.zdbjq.cn/Article/details/gabvwpexj.sHtML

[U28] Py：类型别名
来源：http://3g.fehbvm.com/Article/details/gtebsmsrw.sHtML

UserId = int
来源：http://mobile.hesvh.cn/Article/details/gidltehlv.sHtML

[U29] Py：属性校验
来源：http://www.m.share.zdbjq.cn/Article/details/ghecihgmq.sHtML

@property 与 @x.setter 配合
来源：http://www.share.zdbjq.cn/Article/details/gglfpybrt.sHtML

[U30] Py：数据类
来源：http://mobile.fehbvm.com/Article/details/ghiikuemh.sHtML

@dataclass(slots=True)
来源：http://baike.zdbjq.cn/Article/details/gundbxjgw.sHtML

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/gwvzsilrh.sHtML

python -m pytest -q
来源：http://www.m.share.fehbvm.com/Article/details/gousxusbl.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fehbvm.com/Article/details/gexbapeqa.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fehbvm.com/Article/details/gudasjjie.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fehbvm.com/Article/details/gvgsroqmr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.zdbjq.cn/Article/details/gxxnmcgxk.sHtML

[U34] Py：判断编码
来源：http://3g.fehbvm.com/Article/details/goivujqgr.sHtML

chardet.detect(raw)
来源：http://mobile.zdbjq.cn/Article/details/gofikbugc.sHtML

[U35] Py：发送邮件
来源：http://www.blog.zdbjq.cn/Article/details/gwlwhyakx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.hesvh.cn/Article/details/gsdhpjkgv.sHtML

[U36] Py：定时任务
来源：http://baike.zdbjq.cn/Article/details/gxxwrhqpk.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.hesvh.cn/Article/details/gakkyvzch.sHtML

[U37] Py：读写 Excel
来源：http://m.share.zdbjq.cn/Article/details/grmsvennv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.hesvh.cn/Article/details/ghcnavodo.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/ggfxqyswi.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.hesvh.cn/Article/details/grdidfndt.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.zdbjq.cn/Article/details/gfsnbvlay.sHtML

sys.stdout.isatty()
来源：http://m.share.zdbjq.cn/Article/details/gfsoldcwr.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fehbvm.com/Article/details/gnaovpdrw.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gpfsbxwqw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fehbvm.com/Article/details/gemzfiexb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fehbvm.com/Article/details/goqhdhflf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.zdbjq.cn/Article/details/gtmwldkey.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.hesvh.cn/Article/details/gktqejlux.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.zdbjq.cn/Article/details/gcsgatkrx.sHtML

namespace App\Http;
来源：http://www.blog.zdbjq.cn/Article/details/galneebdp.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.zdbjq.cn/Article/details/ghvwrbqlx.sHtML

declare(strict_types=1);
来源：http://3g.fehbvm.com/Article/details/gsahbvvbu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.zdbjq.cn/Article/details/gwztjdgfd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gzwgpcdhn.sHtML

[U46] PHP：可空类型
来源：http://m.share.fehbvm.com/Article/details/gcpdzkwdv.sHtML

?string $name = null
来源：http://blog.zdbjq.cn/Article/details/gedfggccx.sHtML

[U47] PHP：联合类型
来源：http://read.share.fehbvm.com/Article/details/gyngdzokz.sHtML

int|string $id
来源：http://baike.hesvh.cn/Article/details/gclyauijd.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.hesvh.cn/Article/details/gbfkqriua.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/gpcbumvdi.sHtML

[U49] PHP：只读属性
来源：http://m.share.fehbvm.com/Article/details/grbucqqti.sHtML

public readonly string $name
来源：http://www.blog.hesvh.cn/Article/details/gknnotjce.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.hesvh.cn/Article/details/ghlnvxizv.sHtML

public function __construct(private int $id) {}
来源：http://m.share.hesvh.cn/Article/details/gcebjsyct.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.zdbjq.cn/Article/details/gzjijaulv.sHtML

[$a, $b] = $arr;
来源：http://www.share.hesvh.cn/Article/details/gllfturop.sHtML

[U52] PHP：箭头函数
来源：http://wap.fehbvm.com/Article/details/gvktavjly.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.zdbjq.cn/Article/details/ghgrzemxu.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fehbvm.com/Article/details/guqunqrhx.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.hesvh.cn/Article/details/gmxvrawif.sHtML

[U54] PHP：空安全调用
来源：http://wap.zdbjq.cn/Article/details/goyjddnbn.sHtML

$obj?->method()
来源：http://www.share.zdbjq.cn/Article/details/ghyzqlwhk.sHtML


<!-- 参考信息 -->