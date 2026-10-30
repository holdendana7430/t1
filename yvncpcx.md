代发 wailian999

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/gdzteafzx.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/gjsnvjjkh.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/gszwrjehj.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/ghzqnwrbm.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/ggenazkyu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gnlykbkwx.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gfxumxjip.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/ghtpkndua.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/gjkljswla.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/gzayhagiz.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fehbvm.com/Article/details/gmzindcwd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/glxwhuytz.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gziblokfd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/glknzqdzu.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/gdtpoaeap.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gktikaabe.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gaisiutwt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gewnhehto.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gsfjchygi.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/gyfuxkmwz.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gberhvtpt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.zdbjq.cn/Article/details/ghspufwvw.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/gsmzldmbm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gmlyovtqz.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/gwfdfqvbv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/gqpomhovx.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gmwolpifu.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fehbvm.com/Article/details/gazrpdxgp.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/ghctrmvtc.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/gliyzemfz.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gykygqgzx.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/guxrbcyme.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/gjjabfpjz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/gftkypjeo.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gztlbxilh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gybymehjq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/ggqpzyufx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqfhnyjxx.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/goquwammk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/ghpezbcvg.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/giechqsew.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gnabrwtxg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/glymwqnqq.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gtgncoeku.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gnwfjacmt.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gpeoyixtp.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/gcsvmdwug.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/gjazxapjk.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/gwfwwmowt.sHtML

[S53] C++：移动语义
来源：http://www.share.hesvh.cn/Article/details/gosimetkg.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/gckkvrndy.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gmebskboz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/gymjjypao.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gzdeagbwm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gtkpnwlmz.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/gvqiunqzo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/gkyghbtwf.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/gykgqvzjc.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/gsybjmnot.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/gwicmsaao.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/gclovaxuj.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gfbynowas.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/gaswwadko.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gvqvebhve.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gqmhsxcwt.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtujcpvfi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gluvrhlxf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gccprapqp.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gqwrkvstb.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gbfqfildw.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.hesvh.cn/Article/details/ggnhzgcmf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/gvygjlbvc.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/gqjzizuyl.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/grhevfdls.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/gkupkxeig.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gfapulcth.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/ghobpcmem.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gqovwggjh.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/gquftlnuh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/gyqagvquy.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gardcgwqu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/ggvtgtjat.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/gfpkvdalg.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gwokxveyx.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/gwrpihtau.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/gfazjccok.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gglxijdvk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/gvjcaubeu.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/glycwkjac.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/ginfdkwcx.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/glmhvisqz.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gntusyjyj.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.hesvh.cn/Article/details/gfurqdbvk.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/gtrlygfsr.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gcqigsghg.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gqugljxhr.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/gqxpevaex.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/gnxdovils.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gqrlqmugx.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gfzenctfw.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gcnsfimyn.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/gnatdldnk.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/ghixcbwlv.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/gyxmcablo.sHtML

[T19] Swift：可选绑定
来源：http://3g.hesvh.cn/Article/details/ghnnyobim.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/gfwezwxhs.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/gyqybacol.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/gjibwrcca.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gjakgvrgp.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/gmtwhylvw.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/gmnkxivej.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fehbvm.com/Article/details/gwbbpchgo.sHtML

[T23] Swift：函数
来源：http://m.share.fehbvm.com/Article/details/gkzqqmuqd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fehbvm.com/Article/details/gzprrfkzm.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/gqipqdewh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gocqmkbmx.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/geslawkwv.sHtML

struct P { var x: Int }
来源：http://blog.hesvh.cn/Article/details/ggpyjspow.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/gvjiyawrs.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/gkrsxmqzb.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/glqasauyb.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/gkjeuhfqk.sHtML

[T28] Swift：枚举
来源：http://3g.fehbvm.com/Article/details/glotsssqv.sHtML

enum Color { case red, green }
来源：http://wap.hesvh.cn/Article/details/gpsoewqjb.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.hesvh.cn/Article/details/gvivohsqy.sHtML

guard let x = opt else { return }
来源：http://3g.fehbvm.com/Article/details/gcyuafkdw.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/gqhrwrpzd.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/ghhaxgosj.sHtML

[T31] Lua：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gykudjkbp.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gzesdypsc.sHtML

[T32] Lua：局部变量
来源：http://mobile.hesvh.cn/Article/details/gttzzmomc.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gipmrebvo.sHtML

[T33] Lua：表（数组）
来源：http://wap.hesvh.cn/Article/details/gxgdpjcsq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/gsxzmhkys.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gbrrzchpg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/gajqscsny.sHtML

[T35] Lua：字典表
来源：http://www.share.fehbvm.com/Article/details/gcibbtcak.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gkmdfuezd.sHtML

[T36] Lua：函数
来源：http://m.share.zdbjq.cn/Article/details/gfklxpmja.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fehbvm.com/Article/details/gwpxqpjih.sHtML

[T37] Lua：字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gyiwqxiil.sHtML

"a" .. "b"
来源：http://3g.hesvh.cn/Article/details/gqfiuvoyp.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/gzzbsromp.sHtML

if x > 0 then print("正") end
来源：http://www.share.hesvh.cn/Article/details/gyvjsejgs.sHtML

[T39] Lua：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/grkddoufg.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/ghvaczrga.sHtML

[T40] Lua：元表
来源：http://www.m.share.fehbvm.com/Article/details/glqfrixuu.sHtML

setmetatable({}, { __index = base })
来源：http://blog.hesvh.cn/Article/details/gutzcuwvw.sHtML

[T41] Perl：Hello World
来源：http://wap.zdbjq.cn/Article/details/gtbksnepc.sHtML

print "Hello\n";
来源：http://read.share.hesvh.cn/Article/details/grdfavpwh.sHtML

[T42] Perl：变量类型
来源：http://wap.hesvh.cn/Article/details/gabhedyak.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.hesvh.cn/Article/details/gvesdtvit.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gsojavykj.sHtML

"值: $a"
来源：http://www.m.share.fehbvm.com/Article/details/gwkkqezmt.sHtML

[T44] Perl：条件
来源：http://www.blog.hesvh.cn/Article/details/glzofkbbi.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fehbvm.com/Article/details/glnlpoudk.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/gkqjiargq.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/gvsswubkq.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gdvfnovwu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/gpbwluigk.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/gnurwytsr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.zdbjq.cn/Article/details/gspbppcdn.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gzaeaqvjl.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/goxdwtdox.sHtML

[T49] Perl：函数
来源：http://mobile.hesvh.cn/Article/details/ggfvloqff.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gsibbwvek.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gimwwsruz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.zdbjq.cn/Article/details/gqsavlmgl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.zdbjq.cn/Article/details/gaxairinn.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/gnxwebokr.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gdfentpgk.sHtML

[T52] Scala：变量
来源：http://read.share.zdbjq.cn/Article/details/gccxmgocw.sHtML

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/gbofxkghw.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gwxwdxthc.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/glrbcqrur.sHtML

[T54] Scala：集合映射
来源：http://blog.fehbvm.com/Article/details/gybqlkdqc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.hesvh.cn/Article/details/gguunsobu.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gwoiqsifc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fehbvm.com/Article/details/gwyocoovw.sHtML

[T56] Scala：样例类
来源：http://read.share.zdbjq.cn/Article/details/gujyghims.sHtML

case class User(name: String, age: Int)
来源：http://blog.hesvh.cn/Article/details/gmawkinjo.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gmwwhacjd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.zdbjq.cn/Article/details/gslfyjrfm.sHtML

[T58] Scala：函数定义
来源：http://read.share.fehbvm.com/Article/details/gvakhwssp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.hesvh.cn/Article/details/gwbgcuxmr.sHtML

[T59] Scala：循环
来源：http://read.share.hesvh.cn/Article/details/gqzagodrk.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gagiothoz.sHtML

[T60] Scala：折叠
来源：http://blog.fehbvm.com/Article/details/gxheowtfg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fehbvm.com/Article/details/giigikkqn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvlyxahax.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/giwufuzdp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/guhmrcfha.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.zdbjq.cn/Article/details/gvwbpteav.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/goyjklevn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/gwelllivc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/gskuuxssn.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/gkyhvfnkp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.hesvh.cn/Article/details/gvkfvipsb.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fehbvm.com/Article/details/gvvnawgxd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.hesvh.cn/Article/details/gzgucgwdv.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/gaymtlnvh.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gpktziikl.sHtML

[U06] Py：合并两个字典
来源：http://baike.zdbjq.cn/Article/details/gklwmurmq.sHtML

{**a, **b}
来源：http://www.m.share.fehbvm.com/Article/details/gbjacgapy.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/gvhpgwksg.sHtML

{v: k for k, v in d.items()}
来源：http://baike.zdbjq.cn/Article/details/gwapfkhwy.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.hesvh.cn/Article/details/gqzjtmtba.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/gohvhrcam.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fehbvm.com/Article/details/gzdpaxbhu.sHtML

max(d, key=d.get)
来源：http://baike.fehbvm.com/Article/details/gyipnspjc.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/gpnvwufij.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/ghpxidaiz.sHtML

[U11] Py：生成器表达式
来源：http://wap.fehbvm.com/Article/details/gtgopxecv.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/grzlibwvb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fehbvm.com/Article/details/gikidqjas.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/gcnkxooeh.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fehbvm.com/Article/details/goqytmprm.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/grxfcncoy.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.zdbjq.cn/Article/details/gtivaxnow.sHtML

defaultdict(list)
来源：http://3g.fehbvm.com/Article/details/gnizlvjla.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.zdbjq.cn/Article/details/gpnxhbcqc.sHtML

t = time.perf_counter()
来源：http://www.blog.fehbvm.com/Article/details/gobhfvvrr.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/gvoyifgsn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fehbvm.com/Article/details/gubdbkepa.sHtML

[U17] Py：初始化日志
来源：http://baike.hesvh.cn/Article/details/gtdraimwm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fehbvm.com/Article/details/geqndywgh.sHtML

[U18] Py：预编译正则
来源：http://m.share.fehbvm.com/Article/details/gitvvznil.sHtML

pat = re.compile(r"\d+")
来源：http://baike.hesvh.cn/Article/details/gebgqdsda.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.hesvh.cn/Article/details/goflmccgf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fehbvm.com/Article/details/gwccjarpe.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fehbvm.com/Article/details/gyquyefhh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.zdbjq.cn/Article/details/guchayqct.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.hesvh.cn/Article/details/gkzdxrhml.sHtML

@contextlib.contextmanager
来源：http://mobile.fehbvm.com/Article/details/gibovuzez.sHtML

[U22] Py：矩阵转置
来源：http://wap.hesvh.cn/Article/details/gdjmeassy.sHtML

list(zip(*m))
来源：http://blog.fehbvm.com/Article/details/gdrfkdhdb.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fehbvm.com/Article/details/gifapmrtw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.zdbjq.cn/Article/details/gvrgqpywn.sHtML

[U24] Py：路径操作
来源：http://www.share.zdbjq.cn/Article/details/gyddbehdr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gxzpxikxu.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.hesvh.cn/Article/details/ggeqykmyw.sHtML

csv.DictReader(f)
来源：http://www.share.fehbvm.com/Article/details/gsvikxekc.sHtML

[U26] Py：并发下载
来源：http://read.share.fehbvm.com/Article/details/gawxckljj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fehbvm.com/Article/details/gbpnpxypc.sHtML

[U27] Py：异步 HTTP
来源：http://baike.hesvh.cn/Article/details/gdohzodxm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/gosubmwcv.sHtML

[U28] Py：类型别名
来源：http://read.share.hesvh.cn/Article/details/glsenujkj.sHtML

UserId = int
来源：http://mobile.hesvh.cn/Article/details/gpgplzvzy.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fehbvm.com/Article/details/gccnwgcht.sHtML

@property 与 @x.setter 配合
来源：http://mobile.zdbjq.cn/Article/details/gmafgqill.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/gbglxrphg.sHtML

@dataclass(slots=True)
来源：http://www.share.zdbjq.cn/Article/details/gtozwlujg.sHtML

[U31] Py：单测
来源：http://www.blog.hesvh.cn/Article/details/gvszojoeq.sHtML

python -m pytest -q
来源：http://www.blog.zdbjq.cn/Article/details/gbtqrhukm.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/gwdeoggxy.sHtML

ruff format . && ruff check --fix .
来源：http://3g.hesvh.cn/Article/details/gtqwhydfb.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/gghzjqdtx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.hesvh.cn/Article/details/gapdrxoya.sHtML

[U34] Py：判断编码
来源：http://read.share.zdbjq.cn/Article/details/gorwqetuo.sHtML

chardet.detect(raw)
来源：http://www.blog.fehbvm.com/Article/details/gjszxttti.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/gbltcvdln.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fehbvm.com/Article/details/gatqyyqnp.sHtML

[U36] Py：定时任务
来源：http://mobile.zdbjq.cn/Article/details/gipbetavt.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.hesvh.cn/Article/details/gvovqfpjc.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.hesvh.cn/Article/details/gfafhdyfg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.zdbjq.cn/Article/details/gcpvpqqww.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fehbvm.com/Article/details/gygtunqnc.sHtML

Path(__file__).resolve().parent
来源：http://m.share.zdbjq.cn/Article/details/ghbssitbe.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/gkyhvpaqx.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/gvondmauh.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fehbvm.com/Article/details/gxfklykdv.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gaszldcky.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fehbvm.com/Article/details/gtwiqqelp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.hesvh.cn/Article/details/gyewizybn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.zdbjq.cn/Article/details/gkchkorqu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/gdakbtmgw.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gjdqslwsh.sHtML

namespace App\Http;
来源：http://wap.zdbjq.cn/Article/details/grycjfvlg.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.hesvh.cn/Article/details/gnmdpypln.sHtML

declare(strict_types=1);
来源：http://wap.hesvh.cn/Article/details/gelpatgll.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.hesvh.cn/Article/details/gcxofvcih.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gbivcrpjo.sHtML

[U46] PHP：可空类型
来源：http://www.share.hesvh.cn/Article/details/gcigxtjfw.sHtML

?string $name = null
来源：http://blog.hesvh.cn/Article/details/grhbnjywk.sHtML

[U47] PHP：联合类型
来源：http://mobile.fehbvm.com/Article/details/gpdbjvfwr.sHtML

int|string $id
来源：http://3g.hesvh.cn/Article/details/gjubdlofn.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fehbvm.com/Article/details/geprphfrv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.zdbjq.cn/Article/details/gpznurhfg.sHtML

[U49] PHP：只读属性
来源：http://wap.hesvh.cn/Article/details/gvgtesoov.sHtML

public readonly string $name
来源：http://wap.fehbvm.com/Article/details/gboqrdoti.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.hesvh.cn/Article/details/gayyhhkjc.sHtML

public function __construct(private int $id) {}
来源：http://baike.fehbvm.com/Article/details/gszrywrix.sHtML

[U51] PHP：数组解构
来源：http://mobile.zdbjq.cn/Article/details/glyhzkvsp.sHtML

[$a, $b] = $arr;
来源：http://blog.hesvh.cn/Article/details/gzpltufhr.sHtML

[U52] PHP：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gihtdfaqx.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/ghnflqtbb.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.zdbjq.cn/Article/details/galotjfsq.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fehbvm.com/Article/details/gqqolvoyf.sHtML

[U54] PHP：空安全调用
来源：http://wap.zdbjq.cn/Article/details/gqpoenvyz.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/grqmoxrjz.sHtML


<!-- 参考信息 -->