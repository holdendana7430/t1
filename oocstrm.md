代发 wailian999

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gasedkflb.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gmmxedbjy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/ghmmekmjo.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gcytrusqw.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/gadafixcp.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/gaikdnzax.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/gyzjvfwlp.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/gyuzszpor.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/gsxchkmqz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gtepuyqkq.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gbxpxtmsi.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gjrxwljpo.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gkjznlbcc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/gnvxcflaz.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/gbeveomhb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gjsewcnej.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gwaddleqo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gbhyevkst.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gubzfbwzb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gvobyopte.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gitchlvfu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/geeupmhum.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/ghmqqfhyo.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/gsodbziuv.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/gylvtafrz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/googmohuo.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gvjkobxxq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gnawfmbxh.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gdwmlnhev.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gxoduoxpv.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gbxyphxnm.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gmdgaxspi.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gergaonob.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fehbvm.com/Article/details/gdbetchre.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/gfwhdumda.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.hesvh.cn/Article/details/grmcmrvsn.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/ghafjfbec.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gajyplouk.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/gpwemczaf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/gxepohtll.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gjyctupdq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/geamdgxzy.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gwcqmlkce.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.zdbjq.cn/Article/details/gqahlvsbu.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/grqlosrtz.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gukuergfl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gerczxkjw.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/gqolugsdh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gowebeeqf.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gicqjxuyc.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/gwjioexmf.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/gqgjgrbrk.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/gsynayhgx.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gxeuslvuk.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/ghblkmjls.sHtML

[S54] C++：异常处理
来源：http://baike.fehbvm.com/Article/details/gpbhwluom.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.zdbjq.cn/Article/details/gbnceczgg.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gbketnsfi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/gesqbrfui.sHtML

[S56] C++：optional
来源：http://www.blog.zdbjq.cn/Article/details/gmpxuowbk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/gclwcyaol.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/grgtdhvnp.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gunqgszma.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gsaecrocy.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gzhtlwrpq.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/ggeqqitph.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/guenftgwg.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gylfiukza.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/gambnxgim.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkepccctn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/ggaizhsut.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggvffedjp.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gfmymggsz.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gwbmyriya.sHtML

[T02] Kotlin：变量
来源：http://m.share.fehbvm.com/Article/details/gzjkojvsi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gqplugxsk.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/gsdpjgcon.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/grpekttnz.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gqswozpgh.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gzkjdsvjr.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/gqdrqubrf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.hesvh.cn/Article/details/gdnorufxj.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/grzxlmqxy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/goshqgquj.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gnexpmplc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gnukghllp.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gpapzqpkm.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gpicvbqhv.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/gdqvrjyqj.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/gwtpqgfkf.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/ggcvodxtr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/gvsiulwqp.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/gtbpdxcnu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/glxrveekn.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/ggyokznvu.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gnxxcwrdc.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/gdimqkjpq.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gnuwsvqhk.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gzrecfpgo.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/gvhkkjgyr.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gwevisvnu.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gftxmzxmo.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/gndwefdwf.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gexkamouj.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/gjvievebf.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gvlwykyiu.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/gojrghnbw.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/goommaoka.sHtML

[T19] Swift：可选绑定
来源：http://read.share.hesvh.cn/Article/details/gbmawzyro.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gcwnsmtnp.sHtML

[T20] Swift：数组操作
来源：http://www.share.hesvh.cn/Article/details/gmiimqdet.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/grpzniduf.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/gqqzhfclg.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/ggrpmreby.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/gryvmspmo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/gjemokrse.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gxaerdqxm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.hesvh.cn/Article/details/guhkxyjow.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/ghnzhjalm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gshfrnozz.sHtML

[T25] Swift：结构体
来源：http://read.share.fehbvm.com/Article/details/ggxbiecht.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/gjlasomzg.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/gmmyxxnhb.sHtML

class A: Base { override func f() {} }
来源：http://wap.fehbvm.com/Article/details/gfwqkfhic.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/ghswddfzu.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gfdykkcqy.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/gjrktcyil.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/gbuclcemj.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/gqwvptfdr.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gvsvdmrxz.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/ggipjvetd.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/goxczmasy.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gbetcasyu.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gambrmmcc.sHtML

[T32] Lua：局部变量
来源：http://blog.fehbvm.com/Article/details/gjwuujgwa.sHtML

local a = 1
来源：http://blog.hesvh.cn/Article/details/glfludish.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/gsqqbgrqq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.hesvh.cn/Article/details/gptqpthjr.sHtML

[T34] Lua：遍历表
来源：http://blog.fehbvm.com/Article/details/gytuifeur.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fehbvm.com/Article/details/gymdgwqlw.sHtML

[T35] Lua：字典表
来源：http://blog.zdbjq.cn/Article/details/glunuklag.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/gynaimevj.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/gukaqqvhf.sHtML

function add(a, b) return a + b end
来源：http://wap.zdbjq.cn/Article/details/ggyhkvlvg.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fehbvm.com/Article/details/gescbiclz.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/gltlohczt.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/gezdtxzrs.sHtML

if x > 0 then print("正") end
来源：http://www.blog.hesvh.cn/Article/details/gjgxmgjkq.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/ghvigeand.sHtML

string.find(s, "%d+")
来源：http://wap.zdbjq.cn/Article/details/glffabqqd.sHtML

[T40] Lua：元表
来源：http://3g.fehbvm.com/Article/details/gkplryknd.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/gpxfpydrq.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/guewrbiur.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/grzlzrgrd.sHtML

[T42] Perl：变量类型
来源：http://baike.hesvh.cn/Article/details/ghoihbwfi.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fehbvm.com/Article/details/gbmvebbfj.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gqfzaojdb.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/gaatitnrk.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/geweizcyi.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.hesvh.cn/Article/details/geqsbalrx.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.zdbjq.cn/Article/details/gyutxgjno.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.zdbjq.cn/Article/details/gwnmzblci.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/gymodoiti.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.hesvh.cn/Article/details/gnfwhqaic.sHtML

[T47] Perl：正则捕获
来源：http://wap.hesvh.cn/Article/details/ggnanfiyx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fehbvm.com/Article/details/ghakpigof.sHtML

[T48] Perl：正则替换
来源：http://wap.fehbvm.com/Article/details/gokjbbyau.sHtML

$s =~ s/old/new/g;
来源：http://wap.zdbjq.cn/Article/details/gqxsgncqf.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/gxiubqfid.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gfdoqfnbe.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/glxuypfzw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/grcpfvgrf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fehbvm.com/Article/details/glhwxfqpa.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gpwnolgsz.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gtpboteyf.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/gxfvkmhkk.sHtML

val a = 1;  var b = 2
来源：http://mobile.hesvh.cn/Article/details/gacdackfi.sHtML

[T53] Scala：字符串插值
来源：http://baike.fehbvm.com/Article/details/gnpbvmczu.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/gxzvbczgi.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/gyazuuzmt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/gqaykazgb.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gpljqzgij.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/gvsgzsiwk.sHtML

[T56] Scala：样例类
来源：http://baike.zdbjq.cn/Article/details/gdadaxhmk.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gpmipanup.sHtML

[T57] Scala：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gzysvsllp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.hesvh.cn/Article/details/gsshrllqr.sHtML

[T58] Scala：函数定义
来源：http://www.share.fehbvm.com/Article/details/gvzsvmvrc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/gsldymvxh.sHtML

[T59] Scala：循环
来源：http://baike.fehbvm.com/Article/details/gkdyvbgit.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/govwlsejp.sHtML

[T60] Scala：折叠
来源：http://www.share.zdbjq.cn/Article/details/gnqjvltwb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gztptgrep.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtchebijw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/ghkmvvlaw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/guqvlqzau.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fehbvm.com/Article/details/gnuovxxgz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/ggwokkyiy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.hesvh.cn/Article/details/godvfedtn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.zdbjq.cn/Article/details/gzetnvdot.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.hesvh.cn/Article/details/gucyuxiaj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.hesvh.cn/Article/details/gnnmkchku.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/gsrgleded.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.zdbjq.cn/Article/details/gcnvlzquc.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/gtzykpjvc.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/guvwllfde.sHtML

[U06] Py：合并两个字典
来源：http://baike.fehbvm.com/Article/details/gadcoykgf.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/gxvwsmaxw.sHtML

[U07] Py：反转字典键值
来源：http://3g.fehbvm.com/Article/details/giijufqui.sHtML

{v: k for k, v in d.items()}
来源：http://3g.zdbjq.cn/Article/details/gnqfuulhn.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fehbvm.com/Article/details/gnxilckno.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/gwcuchlbj.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fehbvm.com/Article/details/gpkpcpegh.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gfajppzbf.sHtML

[U10] Py：按值排序字典
来源：http://3g.fehbvm.com/Article/details/gtbdcqcce.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/grrylkhio.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/gmcfdnwrr.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gfqwxvtla.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/gjpyfyfub.sHtML

Counter(arr).most_common(3)
来源：http://mobile.zdbjq.cn/Article/details/gckscnofq.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/gfhngfmvb.sHtML

deque(maxlen=10)
来源：http://wap.zdbjq.cn/Article/details/gbtvaivwd.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.hesvh.cn/Article/details/gpnahumai.sHtML

defaultdict(list)
来源：http://www.share.zdbjq.cn/Article/details/gpvbrtlfz.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/gsuswzzbb.sHtML

t = time.perf_counter()
来源：http://www.m.share.zdbjq.cn/Article/details/gbtidxotd.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/gkxgnhcne.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.hesvh.cn/Article/details/gtfevxjgy.sHtML

[U17] Py：初始化日志
来源：http://read.share.hesvh.cn/Article/details/ghzwdtzww.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/goagmdsnb.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.zdbjq.cn/Article/details/gjghjljqb.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fehbvm.com/Article/details/gqugejkux.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.hesvh.cn/Article/details/gzpzujaxk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/gryooqrot.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/gqszqfjlm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.zdbjq.cn/Article/details/gttnhiixp.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.zdbjq.cn/Article/details/gqyxnpyzd.sHtML

@contextlib.contextmanager
来源：http://www.m.share.hesvh.cn/Article/details/guicuulqq.sHtML

[U22] Py：矩阵转置
来源：http://wap.hesvh.cn/Article/details/gkfphkcje.sHtML

list(zip(*m))
来源：http://baike.hesvh.cn/Article/details/gszrcouxb.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/gvekptnzk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.hesvh.cn/Article/details/gublckdxi.sHtML

[U24] Py：路径操作
来源：http://3g.hesvh.cn/Article/details/gxjsqhzuz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/ghhqtubfp.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fehbvm.com/Article/details/gxftiflkt.sHtML

csv.DictReader(f)
来源：http://www.m.share.fehbvm.com/Article/details/gwxlohmbe.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/gnidbboyv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.hesvh.cn/Article/details/gbiytkyif.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gfwzplghl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.hesvh.cn/Article/details/gjnttqvdk.sHtML

[U28] Py：类型别名
来源：http://read.share.fehbvm.com/Article/details/gvlmmswor.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/gthmmkwrk.sHtML

[U29] Py：属性校验
来源：http://read.share.hesvh.cn/Article/details/gomaofswy.sHtML

@property 与 @x.setter 配合
来源：http://blog.hesvh.cn/Article/details/gwtnayute.sHtML

[U30] Py：数据类
来源：http://blog.fehbvm.com/Article/details/gywmgkhzu.sHtML

@dataclass(slots=True)
来源：http://mobile.zdbjq.cn/Article/details/gbsokvgpx.sHtML

[U31] Py：单测
来源：http://read.share.hesvh.cn/Article/details/gxqgvfvuq.sHtML

python -m pytest -q
来源：http://wap.zdbjq.cn/Article/details/gxpkjbxbu.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/guhyyfjpc.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.hesvh.cn/Article/details/gkagwzapy.sHtML

[U33] Py：打包发布
来源：http://wap.zdbjq.cn/Article/details/ghhkvqjuc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/gmctwqzqd.sHtML

[U34] Py：判断编码
来源：http://baike.hesvh.cn/Article/details/gpoheynrf.sHtML

chardet.detect(raw)
来源：http://read.share.fehbvm.com/Article/details/gjwjdasbk.sHtML

[U35] Py：发送邮件
来源：http://blog.hesvh.cn/Article/details/gbyuzxacl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/gzyvzrzob.sHtML

[U36] Py：定时任务
来源：http://www.blog.fehbvm.com/Article/details/gqgxwruyy.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.hesvh.cn/Article/details/ghvzkqvjf.sHtML

[U37] Py：读写 Excel
来源：http://www.share.hesvh.cn/Article/details/gcjlsjdex.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.hesvh.cn/Article/details/gwyyhvduk.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.hesvh.cn/Article/details/ghkxbqiwo.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.zdbjq.cn/Article/details/gcxogvlha.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fehbvm.com/Article/details/gqasbewoz.sHtML

sys.stdout.isatty()
来源：http://wap.zdbjq.cn/Article/details/gcgfetjnz.sHtML

[U40] Py：打印到标准错误
来源：http://baike.zdbjq.cn/Article/details/gybycqdif.sHtML

print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/ggvtgxgsh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.zdbjq.cn/Article/details/gqlhkwqgi.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/gvdbijvqz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.zdbjq.cn/Article/details/gdowugkqc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.hesvh.cn/Article/details/ggtvpszzw.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/gybaxfbve.sHtML

namespace App\Http;
来源：http://mobile.hesvh.cn/Article/details/gceafhivo.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.zdbjq.cn/Article/details/gtsvwwjjc.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/gshwyltvu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.hesvh.cn/Article/details/gxhalqvvo.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gqnyfcikp.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fehbvm.com/Article/details/gkocucqhn.sHtML

?string $name = null
来源：http://wap.fehbvm.com/Article/details/gxtwvcnqb.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/gavuynpcj.sHtML

int|string $id
来源：http://wap.fehbvm.com/Article/details/gepzijxey.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fehbvm.com/Article/details/gmjiovlhj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/gibcxbiew.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.zdbjq.cn/Article/details/gyjfslusr.sHtML

public readonly string $name
来源：http://baike.hesvh.cn/Article/details/gpbraufko.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fehbvm.com/Article/details/ggwasxbcu.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/ghtytqcll.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.hesvh.cn/Article/details/grnbzvwpa.sHtML

[$a, $b] = $arr;
来源：http://www.share.fehbvm.com/Article/details/gfciynuuv.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gnohplgkr.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gtkwpemeu.sHtML


<!-- 参考信息 -->