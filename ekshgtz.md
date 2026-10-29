代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/grhzqotaz.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gmjfcqsaf.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gqychkpto.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/gzpuoqlkw.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/gfaslsqfk.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gjdhetkqg.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gtnfahndr.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gkfrcgzcy.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/gktltdlay.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/gtwjymxzt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/giegekmfp.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/gqmqusmyn.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gjdjjdtcl.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/ggjzrsymu.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/gluzbzvfn.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gfzknkszb.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/gnvzjfgke.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/gyeubnhqt.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/gtabsstph.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.zdbjq.cn/Article/details/gkldlflea.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/gueoxhefy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gqhbwkufd.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gdiqthmam.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gqzainrrr.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gamjieyib.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gdhinsyzh.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gigxrfwka.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gnloeogif.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gxlssulqi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/gchigrtbt.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/gqohlsdjv.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/gvqjqzobm.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/gjiiyfgyf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/goupvzerr.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/gmbcndngm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/grgrugfqv.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gapwtcljr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/gdisaoiqi.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/ggmrsmxyw.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/gbmrgfnfu.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gmyxelytn.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/ggswpnrkm.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gjxwhiujy.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gtaqedjbo.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/glizbotrm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gxuymxpsg.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gizyasgta.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/ggvejoegg.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/gdlqbaaqg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/giwlkcmnc.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gburklzoa.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gvsbitpiq.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/gxtritthk.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gdgwipdsg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gblabbpvq.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/gjjfqrfph.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/ghdohdusq.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gxeaqggqd.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gtncaidto.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/gpgypjzlr.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/gvqnaetdg.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gygrrklpz.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.zdbjq.cn/Article/details/genjgkoav.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/gawvwwttl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/gpwzkahxm.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/ghrcnarls.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gbtnfynts.sHtML

[S56] C++：optional
来源：http://www.share.fehbvm.com/Article/details/gfrsedlez.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/ghqhkfwbm.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/gpwflcvaw.sHtML

constexpr int N = 10;
来源：http://www.share.fehbvm.com/Article/details/gljmgpyvn.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/gjdaxvkda.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gmxleesip.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/gxaqxenzh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gtudstzuu.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gewhiavmy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gpflssgae.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvnjyvqfb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gurrozhsi.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glstifcis.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gfgckdlag.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/girdvyxgg.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gzbhyeidv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/gxleixpap.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gjfkaimgf.sHtML

"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gjsiyvshi.sHtML

[T04] Kotlin：空安全
来源：http://mobile.zdbjq.cn/Article/details/gyqkynylt.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gzilcimhe.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/gcordxrun.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fehbvm.com/Article/details/ghwzqefnd.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fehbvm.com/Article/details/geyidlsqs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gxwjexhqa.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gbwzijsej.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/glypoxwki.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gwaltmidm.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/gsbwtsqjy.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/ghttiiajt.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/gkymqtqao.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gdmzewziq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/guwqnzrlo.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gdkvichlv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/gpzvxjrjw.sHtML

[T12] Kotlin：解构声明
来源：http://blog.zdbjq.cn/Article/details/gtuwuwlzo.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fehbvm.com/Article/details/gwumggjji.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/gutbbndte.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/grlvwgdal.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/gdymxdxdp.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gjxygbjap.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/gzbrapqsy.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/gpazfunqs.sHtML

[T16] Swift：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gcfgczyom.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gzoutjeuj.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/gdtlhjpso.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gxvksjeox.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gkqemyauw.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/glqeyojnc.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/gyheguslw.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gvclfwkzl.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/girktvnof.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.hesvh.cn/Article/details/gfcupgpxu.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/gvtzdtjof.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gvhczboey.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/gnekwxhlf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gplmktaac.sHtML

[T23] Swift：函数
来源：http://www.blog.hesvh.cn/Article/details/gfxmbmgoa.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/gytcoffzz.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/ggysaooay.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gifiqqrhx.sHtML

[T25] Swift：结构体
来源：http://blog.fehbvm.com/Article/details/gdzbrgfyk.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/gnrnvjyns.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/gxpnbfqmk.sHtML

class A: Base { override func f() {} }
来源：http://www.share.hesvh.cn/Article/details/gsimgecej.sHtML

[T27] Swift：错误处理
来源：http://wap.hesvh.cn/Article/details/gzqmztjxd.sHtML

do { try f() } catch { print(error) }
来源：http://baike.zdbjq.cn/Article/details/gevjpzfyz.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gxwvpnmol.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/gpppwhjeh.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/gpdfrosdw.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/ggiatzbdq.sHtML

[T30] Swift：协议
来源：http://m.share.fehbvm.com/Article/details/gbpizodfn.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fehbvm.com/Article/details/gjaehctqz.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gkmxnhirl.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gwugerhlj.sHtML

[T32] Lua：局部变量
来源：http://blog.zdbjq.cn/Article/details/ghdnywawt.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/ghjqagjjv.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/ggdqtfkwt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fehbvm.com/Article/details/gavmutobx.sHtML

[T34] Lua：遍历表
来源：http://wap.hesvh.cn/Article/details/gnwamipbg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.hesvh.cn/Article/details/gscgzcukf.sHtML

[T35] Lua：字典表
来源：http://m.share.zdbjq.cn/Article/details/grvqthaxz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.zdbjq.cn/Article/details/grxygmyba.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/gyshavqmx.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/graytkyzl.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gfqjvvhke.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/glmjbviik.sHtML

[T38] Lua：条件
来源：http://read.share.fehbvm.com/Article/details/goksmhemj.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/gcwqjynpb.sHtML

[T39] Lua：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gfrqysipp.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/gxtzvixgq.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/gdafiymdm.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/gxpeasvrg.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/gyasrwshh.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/grshfzpjq.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gcaqcsknd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/gltaohecn.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/ggipqdtbg.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/gmcvwtfzx.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/gkklxnxli.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/gnqppyyaj.sHtML

[T45] Perl：数组遍历
来源：http://www.share.zdbjq.cn/Article/details/gosfhgrnm.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/gxjdtectx.sHtML

[T46] Perl：哈希操作
来源：http://www.share.hesvh.cn/Article/details/goiegetmj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/gypsqldmh.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/gccihgrdb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.hesvh.cn/Article/details/gilepdeel.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/gqacfjnaq.sHtML

$s =~ s/old/new/g;
来源：http://blog.fehbvm.com/Article/details/gmpucwjke.sHtML

[T49] Perl：函数
来源：http://read.share.hesvh.cn/Article/details/gsenmtguk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gxsszojkb.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gkgtykseg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fehbvm.com/Article/details/gieptbfoq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/gztunwopp.sHtML

[T51] Scala：Hello World
来源：http://blog.fehbvm.com/Article/details/gqpsxxeyp.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/grdxspjyk.sHtML

[T52] Scala：变量
来源：http://read.share.zdbjq.cn/Article/details/gcytspgzx.sHtML

val a = 1;  var b = 2
来源：http://mobile.hesvh.cn/Article/details/gytwhbnvl.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gtuhihlmp.sHtML

s"值: $b"
来源：http://wap.fehbvm.com/Article/details/gqhuaflmb.sHtML

[T54] Scala：集合映射
来源：http://read.share.fehbvm.com/Article/details/gczdurnfs.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.zdbjq.cn/Article/details/gokuxmsel.sHtML

[T55] Scala：集合过滤
来源：http://blog.hesvh.cn/Article/details/grwvvsmls.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.zdbjq.cn/Article/details/gdrgtlsml.sHtML

[T56] Scala：样例类
来源：http://mobile.hesvh.cn/Article/details/gozxmvmqf.sHtML

case class User(name: String, age: Int)
来源：http://baike.zdbjq.cn/Article/details/gjapuzitu.sHtML

[T57] Scala：模式匹配
来源：http://wap.hesvh.cn/Article/details/gbtjjubcm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/gmiqlsijq.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/gpmbfkgeb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/gxhxokixm.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/gljygwlpz.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gumvarcth.sHtML

[T60] Scala：折叠
来源：http://blog.hesvh.cn/Article/details/gfmntibqm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fehbvm.com/Article/details/gsrhrfati.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnglhjrzn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gatpscxkh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gklcmfesd.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/gmmzjszfp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/gdpmewwpm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.hesvh.cn/Article/details/gwmyjutkf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/ganrjkujf.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fehbvm.com/Article/details/gaxerfcgg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fehbvm.com/Article/details/gymvbcrpn.sHtML

[U04] Py：变量调试打印
来源：http://m.share.zdbjq.cn/Article/details/gtgcrpwzy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fehbvm.com/Article/details/ggfjtofmk.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.zdbjq.cn/Article/details/glhqgljgu.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gvedxrnbj.sHtML

[U06] Py：合并两个字典
来源：http://baike.zdbjq.cn/Article/details/gzljzgvrp.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/gxvfwhfzw.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/gfmadyyds.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.zdbjq.cn/Article/details/guacmakac.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fehbvm.com/Article/details/guprejmfm.sHtML

[y for x in nested for y in x]
来源：http://read.share.hesvh.cn/Article/details/glhyfibah.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fehbvm.com/Article/details/gnwolirbu.sHtML

max(d, key=d.get)
来源：http://www.share.zdbjq.cn/Article/details/gqgkpkaqx.sHtML

[U10] Py：按值排序字典
来源：http://baike.fehbvm.com/Article/details/gazdgqrgs.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/gmbkzogcm.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fehbvm.com/Article/details/gmuojarib.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/gkmlnkvcl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/gzfuwwtrp.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fehbvm.com/Article/details/gkjgibugu.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/gwpxprpht.sHtML

deque(maxlen=10)
来源：http://wap.fehbvm.com/Article/details/gcwvexhwg.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fehbvm.com/Article/details/gaocjbywx.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/gchquuwbw.sHtML

[U15] Py：高精度计时
来源：http://read.share.hesvh.cn/Article/details/getealvrp.sHtML

t = time.perf_counter()
来源：http://mobile.hesvh.cn/Article/details/gvjfzjfdf.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.zdbjq.cn/Article/details/gksetsuyq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.hesvh.cn/Article/details/gtqxaelvx.sHtML

[U17] Py：初始化日志
来源：http://baike.zdbjq.cn/Article/details/gyxukmsjv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.zdbjq.cn/Article/details/gzsjfbpxr.sHtML

[U18] Py：预编译正则
来源：http://mobile.fehbvm.com/Article/details/gqscbdqay.sHtML

pat = re.compile(r"\d+")
来源：http://baike.hesvh.cn/Article/details/gnxgvlaiw.sHtML

[U19] Py：正则替换带回调
来源：http://blog.zdbjq.cn/Article/details/ggtazdqqf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fehbvm.com/Article/details/gczmkndoj.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fehbvm.com/Article/details/gutgnqxrt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fehbvm.com/Article/details/gljzxsivo.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fehbvm.com/Article/details/gxruypwph.sHtML

@contextlib.contextmanager
来源：http://blog.zdbjq.cn/Article/details/gmxzkbqbg.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/gzcuqmuky.sHtML

list(zip(*m))
来源：http://www.share.zdbjq.cn/Article/details/gacrqktpv.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/gylbgcame.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fehbvm.com/Article/details/gyhurvlzb.sHtML

[U24] Py：路径操作
来源：http://read.share.fehbvm.com/Article/details/gzixcpbao.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gqfskanqy.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.hesvh.cn/Article/details/gbsmwhwhj.sHtML

csv.DictReader(f)
来源：http://wap.fehbvm.com/Article/details/gmsqfacsw.sHtML

[U26] Py：并发下载
来源：http://m.share.hesvh.cn/Article/details/gqijyrwfw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.zdbjq.cn/Article/details/ghakvujfx.sHtML

[U27] Py：异步 HTTP
来源：http://baike.zdbjq.cn/Article/details/gvpyiqqew.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fehbvm.com/Article/details/gobqxlmzo.sHtML

[U28] Py：类型别名
来源：http://www.share.hesvh.cn/Article/details/giupxyfro.sHtML

UserId = int
来源：http://baike.fehbvm.com/Article/details/gyjdvqeco.sHtML

[U29] Py：属性校验
来源：http://mobile.fehbvm.com/Article/details/gheibglgu.sHtML

@property 与 @x.setter 配合
来源：http://wap.hesvh.cn/Article/details/gyaeeeavk.sHtML

[U30] Py：数据类
来源：http://mobile.fehbvm.com/Article/details/ghswvxbhf.sHtML

@dataclass(slots=True)
来源：http://baike.zdbjq.cn/Article/details/gaskompwp.sHtML

[U31] Py：单测
来源：http://www.blog.hesvh.cn/Article/details/grgtrnhgd.sHtML

python -m pytest -q
来源：http://mobile.hesvh.cn/Article/details/gaeukuwwd.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.hesvh.cn/Article/details/gjjenevpo.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fehbvm.com/Article/details/ghgtklrei.sHtML

[U33] Py：打包发布
来源：http://read.share.fehbvm.com/Article/details/gwshqjqca.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.zdbjq.cn/Article/details/gcrtxhryv.sHtML

[U34] Py：判断编码
来源：http://3g.hesvh.cn/Article/details/gpmcopejy.sHtML

chardet.detect(raw)
来源：http://baike.hesvh.cn/Article/details/gjqmntctx.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fehbvm.com/Article/details/gcxpwjgrh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.hesvh.cn/Article/details/gvmjgonzh.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gechnxgzf.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.hesvh.cn/Article/details/gcknxzhzw.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/gjlxnkahp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.zdbjq.cn/Article/details/gynefyujj.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.zdbjq.cn/Article/details/gvvwtwqzk.sHtML

Path(__file__).resolve().parent
来源：http://read.share.zdbjq.cn/Article/details/gxcvupvgh.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fehbvm.com/Article/details/glyjzwkrw.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/gezncprln.sHtML

[U40] Py：打印到标准错误
来源：http://baike.hesvh.cn/Article/details/gggioxwcf.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gzyjrnuil.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fehbvm.com/Article/details/gjxdvhlwm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gsmamgalh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.zdbjq.cn/Article/details/gzsbtzecl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.zdbjq.cn/Article/details/gsdasoyoq.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fehbvm.com/Article/details/gvmtygmlk.sHtML

namespace App\Http;
来源：http://www.share.fehbvm.com/Article/details/ghghrrxvd.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fehbvm.com/Article/details/gtecgfwdr.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/gtilmvpxe.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.zdbjq.cn/Article/details/gokwbcpdt.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gmygeunxt.sHtML

[U46] PHP：可空类型
来源：http://mobile.hesvh.cn/Article/details/gusduhfje.sHtML

?string $name = null
来源：http://www.blog.fehbvm.com/Article/details/ghejxixzx.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/gtpumippt.sHtML

int|string $id
来源：http://baike.zdbjq.cn/Article/details/gzyzqsdjv.sHtML

[U48] PHP：纯枚举
来源：http://3g.fehbvm.com/Article/details/gwnqunalm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fehbvm.com/Article/details/gtotlocaw.sHtML


<!-- 参考信息 -->