代发 wailian999

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/gbguyndao.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fehbvm.com/Article/details/grdcblglb.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gokluftzl.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/gojylguwv.sHtML

[S33] C++：vector 增删
来源：http://www.share.hesvh.cn/Article/details/gtuxdwmqg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/gfssqucyf.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/gpkjgjxrs.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/gthjnskps.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/gsjrokrur.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gzbggisia.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/gadjyjqdj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gksqfqtqi.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/gxfcrqlyw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/guetlynbl.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gbvalwnoo.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gavoaoyhx.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/gjlvtkmtf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/guoyvevyd.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gfipnewgd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gahhrfipc.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/gvjfkgkpr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gfjmygagr.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/gfyxmdxjm.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/gvxtwfish.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/gydfdhfys.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/gkaiwcukj.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gaclqqaiy.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/gfljnakii.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gdoxczvkc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/gzneeypts.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/gcotikxgo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/gwdbfptze.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gehhjvkcu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/gtohevzan.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gojskslvj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/gmdrovuao.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/gxmstsbky.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/gkxxwfvyu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/glmperntc.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gvcwibhvs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gtryvyghc.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gnuvwhikw.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/gzjgfkzdv.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/gdaqbqiut.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/gfuafmqfp.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/glerhwinp.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/glnoedeuy.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/gxztttkgc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gdzjgjogz.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gakvwnjru.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/glwuvtnbl.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gcdhziupj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/gdqiuijkk.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/gylcyxmwb.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/geiesxjhr.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/geiujibjc.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/guyhzucig.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/guyqpwqaa.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/ganlbnnst.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gijsgpoqe.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.hesvh.cn/Article/details/guncsmlcr.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glxvuqqei.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gxjhjlnhw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyngudaje.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gxmsrmpqq.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/goihkswmr.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gijogeujd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/guhmlgeml.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/gbbyyozkt.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gspmfjppq.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/ggvkzrire.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/gogtvobrz.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/gyuixidpx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.hesvh.cn/Article/details/gmofmwfuo.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/ggynzysat.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gtwgmmcdi.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/ghciwnwpq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/gkmtmmprt.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gxqujmbqg.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/gohjjcwia.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gijioxspz.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/gzfepchvr.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gxhbrxljg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/giwkvwtpt.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/goxcgbpjf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/gdimzzoaw.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gkhzhohrs.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/ghmfmtqrc.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fehbvm.com/Article/details/gjkkieycx.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gnltwjyhv.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/gnypglvkt.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gxfvsncyu.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/gyqmjodvf.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/gwsrftjyl.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gunnhjpue.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gnmfuzbcu.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fehbvm.com/Article/details/gacreblrz.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fehbvm.com/Article/details/gaxgqmvcg.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gtqsthzgt.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gsgipjezg.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/gchyjcotr.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/gcqkxnebr.sHtML

[T20] Swift：数组操作
来源：http://www.blog.hesvh.cn/Article/details/gawrewqjo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/ghtgitxny.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/gxcrquxdf.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/gbjcavird.sHtML

[T22] Swift：字典
来源：http://read.share.fehbvm.com/Article/details/gkprixeip.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.zdbjq.cn/Article/details/gylmgxikl.sHtML

[T23] Swift：函数
来源：http://www.share.hesvh.cn/Article/details/gnfdjjkip.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/gwuciwouv.sHtML

[T24] Swift：闭包
来源：http://read.share.zdbjq.cn/Article/details/gmfqamceo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/gfqnxwhpe.sHtML

[T25] Swift：结构体
来源：http://www.m.share.zdbjq.cn/Article/details/gebgmhqfy.sHtML

struct P { var x: Int }
来源：http://www.m.share.hesvh.cn/Article/details/glhtutxxv.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/geaynnzif.sHtML

class A: Base { override func f() {} }
来源：http://baike.hesvh.cn/Article/details/gbblrwrsw.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/gbrrwvcyv.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/gukzisijw.sHtML

[T28] Swift：枚举
来源：http://baike.fehbvm.com/Article/details/gbxdkufbt.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/gazbxybgu.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gdemrrcca.sHtML

guard let x = opt else { return }
来源：http://read.share.zdbjq.cn/Article/details/gsmyxwzwh.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/gfxtqrqoi.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fehbvm.com/Article/details/gbifmupqq.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/gjjecdrxa.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gmlrecqom.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/gsbawgjel.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/gpiuaaght.sHtML

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/gmqfvxhfc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.zdbjq.cn/Article/details/gkevimisu.sHtML

[T34] Lua：遍历表
来源：http://blog.fehbvm.com/Article/details/gbdjycpiw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/gggvhfsxu.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/gkyifqanr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fehbvm.com/Article/details/gjbyvcpsy.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/gjfamarww.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/gjuukjgix.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gwtvdczik.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/giazsebwt.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/gugceweoe.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/gnfijcmbl.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gubyxzrvd.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gkrnutugm.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/glrjahpeu.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/gmslescby.sHtML

[T41] Perl：Hello World
来源：http://3g.zdbjq.cn/Article/details/gucjosdfm.sHtML

print "Hello\n";
来源：http://read.share.hesvh.cn/Article/details/gnvcbehgo.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gvvjtsngr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/gemoniocz.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/guumywuxl.sHtML

"值: $a"
来源：http://baike.fehbvm.com/Article/details/grnwthigv.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/gxhppncxc.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/gpoazecth.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/gkvzssdwt.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.zdbjq.cn/Article/details/golfpxcrr.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/gxngfuapb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.hesvh.cn/Article/details/gxxmowofh.sHtML

[T47] Perl：正则捕获
来源：http://m.share.hesvh.cn/Article/details/gcphaxxyt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fehbvm.com/Article/details/gvrhxpjbi.sHtML

[T48] Perl：正则替换
来源：http://mobile.hesvh.cn/Article/details/gizygtbte.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fehbvm.com/Article/details/gfjmpnxxp.sHtML

[T49] Perl：函数
来源：http://m.share.hesvh.cn/Article/details/gnvxkfnmx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/ggzulqstf.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gbjihgxzh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fehbvm.com/Article/details/gixmsoaut.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fehbvm.com/Article/details/gfbtpoigm.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gnqimtvyd.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gzbdvtpnp.sHtML

[T52] Scala：变量
来源：http://m.share.hesvh.cn/Article/details/ghifhbruw.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/gqxvgvmdh.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/ggqsqqeyx.sHtML

s"值: $b"
来源：http://wap.fehbvm.com/Article/details/gkczhctdx.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gzudopvat.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gxypbgcls.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gvipqpbnc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/ggtwdwjwa.sHtML

[T56] Scala：样例类
来源：http://www.blog.zdbjq.cn/Article/details/gfoulfxze.sHtML

case class User(name: String, age: Int)
来源：http://wap.fehbvm.com/Article/details/gevsmdvlw.sHtML

[T57] Scala：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gvlrstcah.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/gnfertkuy.sHtML

[T58] Scala：函数定义
来源：http://www.share.fehbvm.com/Article/details/gfijszjzg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fehbvm.com/Article/details/gfrxechqo.sHtML

[T59] Scala：循环
来源：http://read.share.zdbjq.cn/Article/details/gidcgxozj.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gdonrgqod.sHtML

[T60] Scala：折叠
来源：http://www.share.hesvh.cn/Article/details/gqmbfgtba.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/gveboebdk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggsfocbee.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gnzydjomu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtrhutaag.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/giytpldbg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.hesvh.cn/Article/details/gidljfzwk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/gaphzhudm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/ggzhssvgt.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gkxdugwrl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/glpvqfusr.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.hesvh.cn/Article/details/gysioelfb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/gbynrjbdg.sHtML

[U05] Py：列表去重且保序
来源：http://3g.hesvh.cn/Article/details/gtcyzxvce.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gohulgvzv.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/gnmiskqgq.sHtML

{**a, **b}
来源：http://3g.zdbjq.cn/Article/details/gwvqqccwt.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.hesvh.cn/Article/details/gprbixcvd.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/gkaqireeb.sHtML

[U08] Py：展平二维列表
来源：http://m.share.zdbjq.cn/Article/details/gzmnappnq.sHtML

[y for x in nested for y in x]
来源：http://www.share.hesvh.cn/Article/details/gtyamujfn.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fehbvm.com/Article/details/glizyrius.sHtML

max(d, key=d.get)
来源：http://baike.fehbvm.com/Article/details/gskouodhc.sHtML

[U10] Py：按值排序字典
来源：http://baike.zdbjq.cn/Article/details/grpzdinea.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fehbvm.com/Article/details/glohnfjkr.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fehbvm.com/Article/details/glpsrkcgt.sHtML

(x * 2 for x in arr)
来源：http://wap.zdbjq.cn/Article/details/gianfgcpx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fehbvm.com/Article/details/gjcrzhdzf.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.zdbjq.cn/Article/details/gbleyicmp.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fehbvm.com/Article/details/ghimufmse.sHtML

deque(maxlen=10)
来源：http://mobile.hesvh.cn/Article/details/gxiasdpit.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/gbyzerxri.sHtML

defaultdict(list)
来源：http://m.share.zdbjq.cn/Article/details/galnbmski.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/gzdnfcqem.sHtML

t = time.perf_counter()
来源：http://read.share.zdbjq.cn/Article/details/gpjamcqyx.sHtML

[U16] Py：命令行参数解析
来源：http://blog.hesvh.cn/Article/details/gislatjgl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gzgxumjdn.sHtML

[U17] Py：初始化日志
来源：http://3g.zdbjq.cn/Article/details/gmsfxehib.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.zdbjq.cn/Article/details/goadafevq.sHtML

[U18] Py：预编译正则
来源：http://read.share.zdbjq.cn/Article/details/gvueushzx.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gfqqflbjh.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.hesvh.cn/Article/details/gtsebeklb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.zdbjq.cn/Article/details/gzwnqypeb.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/gewkmpszj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.zdbjq.cn/Article/details/gblfjemkd.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.zdbjq.cn/Article/details/gocvwogof.sHtML

@contextlib.contextmanager
来源：http://baike.zdbjq.cn/Article/details/gsrzslbby.sHtML

[U22] Py：矩阵转置
来源：http://wap.fehbvm.com/Article/details/gbqbedwan.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/gddhsaddo.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.hesvh.cn/Article/details/gchhhjtpj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.hesvh.cn/Article/details/gjpiqinus.sHtML

[U24] Py：路径操作
来源：http://baike.hesvh.cn/Article/details/gkvgzqbhp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/givqnzxxq.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.hesvh.cn/Article/details/giqummjcc.sHtML

csv.DictReader(f)
来源：http://www.share.fehbvm.com/Article/details/gkgjmvlga.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/gpguevhxr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/gmmtrxhwd.sHtML

[U27] Py：异步 HTTP
来源：http://3g.zdbjq.cn/Article/details/gjnnhhvtl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.zdbjq.cn/Article/details/gdkasvzzt.sHtML

[U28] Py：类型别名
来源：http://wap.fehbvm.com/Article/details/gphtjipzi.sHtML

UserId = int
来源：http://www.m.share.hesvh.cn/Article/details/gmaxilrka.sHtML

[U29] Py：属性校验
来源：http://3g.hesvh.cn/Article/details/gcstligeo.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/guvyiimks.sHtML

[U30] Py：数据类
来源：http://m.share.hesvh.cn/Article/details/gnyehvmst.sHtML

@dataclass(slots=True)
来源：http://blog.zdbjq.cn/Article/details/gwcrwcvgz.sHtML

[U31] Py：单测
来源：http://3g.hesvh.cn/Article/details/gkhlnqeom.sHtML

python -m pytest -q
来源：http://3g.fehbvm.com/Article/details/ggnbiewzo.sHtML

[U32] Py：代码格式化
来源：http://m.share.fehbvm.com/Article/details/ggrfduzvd.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.hesvh.cn/Article/details/gwzyugnqn.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/gocmxtftc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.zdbjq.cn/Article/details/gzqjrrqml.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/gkqgfswyh.sHtML

chardet.detect(raw)
来源：http://www.share.fehbvm.com/Article/details/gleumuwrg.sHtML

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/gxwnsblhh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.zdbjq.cn/Article/details/gppcyepvr.sHtML

[U36] Py：定时任务
来源：http://baike.zdbjq.cn/Article/details/gvkkzloke.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.hesvh.cn/Article/details/giaphcfed.sHtML

[U37] Py：读写 Excel
来源：http://wap.hesvh.cn/Article/details/gzdjwvdhj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fehbvm.com/Article/details/ggdwvjpix.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.hesvh.cn/Article/details/gdsvupfje.sHtML

Path(__file__).resolve().parent
来源：http://baike.hesvh.cn/Article/details/glekpjyht.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.zdbjq.cn/Article/details/ghtwmrshl.sHtML

sys.stdout.isatty()
来源：http://mobile.zdbjq.cn/Article/details/ghkbpnjbl.sHtML

[U40] Py：打印到标准错误
来源：http://wap.zdbjq.cn/Article/details/gvjklebmi.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gxmiuljbn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fehbvm.com/Article/details/gickdueay.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fehbvm.com/Article/details/gbkhglckm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.hesvh.cn/Article/details/gsndvdcwm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.zdbjq.cn/Article/details/ggagkybhw.sHtML

[U43] PHP：声明命名空间
来源：http://baike.zdbjq.cn/Article/details/gtwtwzohc.sHtML

namespace App\Http;
来源：http://baike.fehbvm.com/Article/details/gresfhoya.sHtML

[U44] PHP：开启严格类型
来源：http://wap.hesvh.cn/Article/details/gmcygecks.sHtML

declare(strict_types=1);
来源：http://www.m.share.zdbjq.cn/Article/details/gegmwtxox.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fehbvm.com/Article/details/gunyhtrhy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gfnxhwhne.sHtML

[U46] PHP：可空类型
来源：http://wap.hesvh.cn/Article/details/gpqaoujev.sHtML

?string $name = null
来源：http://baike.zdbjq.cn/Article/details/glxpqfhxm.sHtML

[U47] PHP：联合类型
来源：http://blog.fehbvm.com/Article/details/gqrgcbuqb.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/gdhsmlwai.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fehbvm.com/Article/details/gujdbuctu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.hesvh.cn/Article/details/grhclwjpq.sHtML

[U49] PHP：只读属性
来源：http://m.share.hesvh.cn/Article/details/gdemdlzll.sHtML

public readonly string $name
来源：http://baike.fehbvm.com/Article/details/gzmeotmlh.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.hesvh.cn/Article/details/grbvyjjjn.sHtML

public function __construct(private int $id) {}
来源：http://wap.hesvh.cn/Article/details/gkqsgwyap.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fehbvm.com/Article/details/guededeep.sHtML

[$a, $b] = $arr;
来源：http://www.share.fehbvm.com/Article/details/gdkmedlvc.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gilckeqka.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fehbvm.com/Article/details/gknznushq.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.hesvh.cn/Article/details/gpbhviwul.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gwcnxstyb.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/gkirotxjg.sHtML

$obj?->method()
来源：http://blog.fehbvm.com/Article/details/gdhpcdfjh.sHtML

[U55] PHP：match 表达式
来源：http://mobile.zdbjq.cn/Article/details/gsdxsdilk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.zdbjq.cn/Article/details/grpnvvmfb.sHtML

[U56] PHP：命名参数
来源：http://baike.hesvh.cn/Article/details/gxepizqzo.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gxgznmeyi.sHtML


<!-- 参考信息 -->