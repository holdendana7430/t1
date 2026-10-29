代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/ghvnxmtnk.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/glczqtsos.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gcsbwoxxu.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gtdggmttv.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/grkqvuypw.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gwfpeypim.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gfwcbpdkm.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gqjvphxpg.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gcjwphwbg.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gtorqdsnx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gnjsjwlrq.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/gtcvjbosk.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gxhtiufsf.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gsnjyvknh.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gscjdhvgd.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/guvqvuewh.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/gldphgoap.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/gtdigmgsl.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/ggldegsrc.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/ghevoseqp.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/guzgxlnnh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/gisdepxul.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/gobyspufk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.zdbjq.cn/Article/details/gnmqlhioj.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/getvlrtwg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/ggfnqsrro.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gjpnoykld.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gpliqbrvu.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gwupazmow.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gibzhywuu.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/giqmkhqzf.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gotkbkupt.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/gmejbugny.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/gzflcjhgr.sHtML

[S40] C++：查找元素
来源：http://m.share.zdbjq.cn/Article/details/gwzebejho.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gctfltamq.sHtML

[S41] C++：类与构造函数
来源：http://www.share.zdbjq.cn/Article/details/gwrrnlfys.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gqksnckjc.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/ghgythrtn.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/gsarytqgg.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gaysctrqb.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/gskgmhiqb.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gehiwhvvo.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/gdqfnosdx.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gxojpqnnr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/gnppyubho.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gormrnlhy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/gkldfabha.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gzimdcawd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/gzquobmri.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gibteuuny.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/gvvvkmfxx.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/gxuxmrnbv.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/gryzkstci.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gryryuaok.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gyvtujaka.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/ghuewxjdw.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gupjtclub.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/gibdwbdqw.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.zdbjq.cn/Article/details/gqazesffo.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/gzltqgwjb.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gxjueavhl.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gnhnvpvax.sHtML

[S54] C++：异常处理
来源：http://baike.fehbvm.com/Article/details/gwmaypyyx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gxbqjrpeg.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/gbrqhchem.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/goyqhieob.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gzyrnbsgw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/grzcnowtv.sHtML

[S57] C++：编译期常量
来源：http://mobile.fehbvm.com/Article/details/gzawthryl.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/gxulcqnje.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/ggssydnxl.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gxqkqcyoy.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gkrmbazju.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/gyzmbjuog.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fehbvm.com/Article/details/gtmcsyjfb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gumydipch.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gogvalikm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gikbaqeas.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/guomcpibx.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gsakvmjsf.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gkfwwdhjo.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gvtkntyql.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gpfjcxcgs.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/gjrezcpls.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gflzhrfir.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/gvbzswphg.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/grsudmosx.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gvdwwrhtd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/gbybeqgwa.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gsoqbupzm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/goekaxcsv.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.hesvh.cn/Article/details/gypyvwblk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gloqieask.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/gfuizmvgh.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/gpfftzpvj.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/gysmegwuq.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gwoqdblir.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/gwdsaikim.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/gelkkdeyd.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/ghzrxsjzr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fehbvm.com/Article/details/gwiuclqbf.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/gjimhmavh.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gnnkyxqax.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.zdbjq.cn/Article/details/gezmsvqvl.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/glnoyensw.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/ggvlrgucg.sHtML

for (i in 1..10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gxfmewclm.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/gonvvuthv.sHtML

interface Shape { fun area(): Double }
来源：http://3g.hesvh.cn/Article/details/gfuzpgrnl.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gcexwnmzc.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gthqowptk.sHtML

[T17] Swift：变量与常量
来源：http://baike.hesvh.cn/Article/details/gqsfknqnh.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gyufutati.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/gzwrlvuez.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/gxszlrmmt.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/gimchodlb.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/gjpoeuuec.sHtML

[T20] Swift：数组操作
来源：http://blog.zdbjq.cn/Article/details/gwrrwjiiw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.zdbjq.cn/Article/details/gfkpvdcos.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/gfavunobb.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/gcpktyfba.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/guwvigqoa.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/gizswkuiv.sHtML

[T23] Swift：函数
来源：http://m.share.zdbjq.cn/Article/details/gidxiokqw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/gpdwinybq.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/gvlaplgzx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gnucpfiig.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/gaamzbvcv.sHtML

struct P { var x: Int }
来源：http://3g.zdbjq.cn/Article/details/gczfrlouo.sHtML

[T26] Swift：类与重写
来源：http://blog.hesvh.cn/Article/details/guxdyfwlc.sHtML

class A: Base { override func f() {} }
来源：http://www.share.zdbjq.cn/Article/details/ghswwidrf.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/gsksczhtj.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/gonyrjnmm.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/gckalsdyr.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/gaobxrind.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/grntgzplg.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/ggwagwzfs.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/gdgzgswdn.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.hesvh.cn/Article/details/gokfcfmnl.sHtML

[T31] Lua：Hello World
来源：http://mobile.hesvh.cn/Article/details/guqmxsbju.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gzvmwimcj.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/gmrmphmzq.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/ghwnzugpz.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/gzcwwljih.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.zdbjq.cn/Article/details/guepqtnzn.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/gfbyikbyd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fehbvm.com/Article/details/gopnyyypa.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/gumgvfwqd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/grryltzsv.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/gaclzuyyx.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/gjnfmmwxa.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gnbmpeqwz.sHtML

"a" .. "b"
来源：http://m.share.hesvh.cn/Article/details/gnagaoklg.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gulndmyrx.sHtML

if x > 0 then print("正") end
来源：http://www.share.hesvh.cn/Article/details/gbyqaqwev.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gckrcjrps.sHtML

string.find(s, "%d+")
来源：http://www.m.share.hesvh.cn/Article/details/gqgodoufo.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/gotllcfgq.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fehbvm.com/Article/details/ggvymjbai.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/gfidwfwnr.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/gukzozkok.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gdjqjggiq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/gcnikqeei.sHtML

[T43] Perl：字符串插值
来源：http://blog.fehbvm.com/Article/details/gnbfospzm.sHtML

"值: $a"
来源：http://www.blog.fehbvm.com/Article/details/grzoyqljn.sHtML

[T44] Perl：条件
来源：http://wap.fehbvm.com/Article/details/gpmmbnluj.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/ghjwjfnsn.sHtML

[T45] Perl：数组遍历
来源：http://mobile.hesvh.cn/Article/details/gkjohnqbn.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/gtnoelznb.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/girrevlff.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/glmrqyzwv.sHtML

[T47] Perl：正则捕获
来源：http://read.share.hesvh.cn/Article/details/gowzwdppa.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/gozgsfwnf.sHtML

[T48] Perl：正则替换
来源：http://www.share.zdbjq.cn/Article/details/gsfbsuhny.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/gytjywvbv.sHtML

[T49] Perl：函数
来源：http://www.share.hesvh.cn/Article/details/gsqktmbzd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/glgatkehb.sHtML

[T50] Perl：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/ggpbalgur.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/gbjmcloai.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.zdbjq.cn/Article/details/gfhqeaasf.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/gxxpxbcqa.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gfubasvrh.sHtML

[T52] Scala：变量
来源：http://baike.zdbjq.cn/Article/details/goxmcrjxb.sHtML

val a = 1;  var b = 2
来源：http://read.share.hesvh.cn/Article/details/grymvavoh.sHtML

[T53] Scala：字符串插值
来源：http://baike.hesvh.cn/Article/details/gxucjroso.sHtML

s"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/ghoeevife.sHtML

[T54] Scala：集合映射
来源：http://www.share.fehbvm.com/Article/details/goydsdkhm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fehbvm.com/Article/details/gchupeayb.sHtML

[T55] Scala：集合过滤
来源：http://www.share.hesvh.cn/Article/details/ghrowafpv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.zdbjq.cn/Article/details/gzwwwumow.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/gbollvfiq.sHtML

case class User(name: String, age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gyqffqvod.sHtML

[T57] Scala：模式匹配
来源：http://read.share.hesvh.cn/Article/details/glnwbseuv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/gnjchjtei.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fehbvm.com/Article/details/gkxjplibh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fehbvm.com/Article/details/grfeirnak.sHtML

[T59] Scala：循环
来源：http://www.share.fehbvm.com/Article/details/grgtxkdsv.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gcbjesdzl.sHtML

[T60] Scala：折叠
来源：http://mobile.zdbjq.cn/Article/details/guqwlqqsz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fehbvm.com/Article/details/gbkapoeev.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtzltidup.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gffhdadyf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsuugxmno.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/gxlacvwpl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gwmwbjwdw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.hesvh.cn/Article/details/ghkchpenn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/gmkazqmqr.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/gckyyncli.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.hesvh.cn/Article/details/gxbhajucz.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/ggcbrobhx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.hesvh.cn/Article/details/ghplzvqzx.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gpecfwdrk.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gpyszqpye.sHtML

[U06] Py：合并两个字典
来源：http://blog.hesvh.cn/Article/details/ghpktpflk.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/gshlixwdw.sHtML

[U07] Py：反转字典键值
来源：http://m.share.hesvh.cn/Article/details/gjoqizxcs.sHtML

{v: k for k, v in d.items()}
来源：http://baike.zdbjq.cn/Article/details/gffqextcf.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/gfwyfbpbs.sHtML

[y for x in nested for y in x]
来源：http://3g.zdbjq.cn/Article/details/gpacbolwn.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fehbvm.com/Article/details/grypamyxd.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/gcxrlvggg.sHtML

[U10] Py：按值排序字典
来源：http://m.share.hesvh.cn/Article/details/goskmjfqi.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fehbvm.com/Article/details/gvbqrrcis.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fehbvm.com/Article/details/gtwlkchzo.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.hesvh.cn/Article/details/gummytadc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/ghsdxbcga.sHtML

Counter(arr).most_common(3)
来源：http://m.share.hesvh.cn/Article/details/gylhgzlkk.sHtML

[U13] Py：固定长度队列
来源：http://www.share.zdbjq.cn/Article/details/gqaygptud.sHtML

deque(maxlen=10)
来源：http://mobile.hesvh.cn/Article/details/ginwtzldr.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/ghixkluqx.sHtML

defaultdict(list)
来源：http://www.share.fehbvm.com/Article/details/gcvccsohz.sHtML

[U15] Py：高精度计时
来源：http://wap.hesvh.cn/Article/details/guflhvhhu.sHtML

t = time.perf_counter()
来源：http://www.share.zdbjq.cn/Article/details/gujfusmve.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fehbvm.com/Article/details/gnqifnilp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.hesvh.cn/Article/details/gcswxjucu.sHtML

[U17] Py：初始化日志
来源：http://www.blog.zdbjq.cn/Article/details/gmoernrmx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.hesvh.cn/Article/details/gofmqaogp.sHtML

[U18] Py：预编译正则
来源：http://read.share.hesvh.cn/Article/details/gooozjeux.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.hesvh.cn/Article/details/gktwocjtl.sHtML

[U19] Py：正则替换带回调
来源：http://wap.hesvh.cn/Article/details/gnutreiqr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fehbvm.com/Article/details/gxgegmthn.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fehbvm.com/Article/details/gjjqvstmd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.zdbjq.cn/Article/details/gaigrlotl.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fehbvm.com/Article/details/gjsqppemt.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/gmszbsumc.sHtML

[U22] Py：矩阵转置
来源：http://blog.hesvh.cn/Article/details/gzwnwxgjg.sHtML

list(zip(*m))
来源：http://mobile.hesvh.cn/Article/details/ggrutugir.sHtML

[U23] Py：分块读取大文件
来源：http://3g.zdbjq.cn/Article/details/gmftzscke.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.zdbjq.cn/Article/details/gywoduriu.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/ggjprcdbl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gmpomxqgo.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fehbvm.com/Article/details/gydhjzxbv.sHtML

csv.DictReader(f)
来源：http://www.m.share.zdbjq.cn/Article/details/ggtpnzgtc.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/gjutpstvu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/gqdhgfltv.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.hesvh.cn/Article/details/gfvbgjdrj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fehbvm.com/Article/details/gyopgjlem.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fehbvm.com/Article/details/grkunrhzv.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/gmjpxvcpw.sHtML

[U29] Py：属性校验
来源：http://www.blog.fehbvm.com/Article/details/gbnednlrv.sHtML

@property 与 @x.setter 配合
来源：http://www.share.hesvh.cn/Article/details/gahnzaquu.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/gqjghbbmk.sHtML

@dataclass(slots=True)
来源：http://baike.zdbjq.cn/Article/details/gzpgsobrr.sHtML

[U31] Py：单测
来源：http://www.share.zdbjq.cn/Article/details/gulkpmeml.sHtML

python -m pytest -q
来源：http://m.share.zdbjq.cn/Article/details/grvttljrs.sHtML

[U32] Py：代码格式化
来源：http://www.blog.hesvh.cn/Article/details/glellvbyu.sHtML

ruff format . && ruff check --fix .
来源：http://wap.zdbjq.cn/Article/details/ggadgmpcc.sHtML

[U33] Py：打包发布
来源：http://www.blog.hesvh.cn/Article/details/gbhciwizw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/gskfsprzx.sHtML

[U34] Py：判断编码
来源：http://www.share.hesvh.cn/Article/details/ghdtqjqed.sHtML

chardet.detect(raw)
来源：http://blog.fehbvm.com/Article/details/gaxvqskuh.sHtML

[U35] Py：发送邮件
来源：http://3g.hesvh.cn/Article/details/ghsayompx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fehbvm.com/Article/details/ggbtwlizj.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gsoxgalqr.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.hesvh.cn/Article/details/gshmollkm.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/groamjdxu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.hesvh.cn/Article/details/glfpfvuzj.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/gflcefsgw.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/gvxhijjwd.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fehbvm.com/Article/details/gknefmtrh.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/gqxbxdwmh.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.hesvh.cn/Article/details/gvzqajbkp.sHtML

print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/guizzyazw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fehbvm.com/Article/details/gdtpsswkk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/gtdppvenk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/grpopsxfr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.zdbjq.cn/Article/details/gloueftst.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.zdbjq.cn/Article/details/gjegaqzvz.sHtML

namespace App\Http;
来源：http://baike.fehbvm.com/Article/details/gwpwugtwo.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fehbvm.com/Article/details/gjbdapevz.sHtML

declare(strict_types=1);
来源：http://read.share.hesvh.cn/Article/details/gugqypvon.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fehbvm.com/Article/details/gvnisrbew.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gaevshzci.sHtML

[U46] PHP：可空类型
来源：http://m.share.zdbjq.cn/Article/details/gtgtrtpdn.sHtML

?string $name = null
来源：http://www.blog.hesvh.cn/Article/details/gbkdiqluk.sHtML

[U47] PHP：联合类型
来源：http://baike.zdbjq.cn/Article/details/gxbrbyceu.sHtML

int|string $id
来源：http://m.share.zdbjq.cn/Article/details/gahntjyno.sHtML

[U48] PHP：纯枚举
来源：http://3g.fehbvm.com/Article/details/gwhfexdsd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/goahmllbp.sHtML


<!-- 参考信息 -->