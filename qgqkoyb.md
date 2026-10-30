代发 wailian999

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/gzifhfcwz.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gqdrypqzx.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gvrjkndtk.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/gofwvzdaj.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gyxgwtmrz.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gbdbsqkkd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gsklbyobh.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gztqrlwvt.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gurahetpt.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/gzrqsuick.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gucwtdqgo.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gowhifbwd.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/ggsniruxe.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fehbvm.com/Article/details/glrahoggi.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/glciyliym.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gdzifuhob.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gqsvqqlbe.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/glxskisfy.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gjdtxfdjo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gcfwzetho.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gdoreyakd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gybnmbeik.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/gtsjvqurc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gshdhcrty.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/givmdldyp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gyonzgwnd.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/gyyxvfbjk.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gfefbtgqc.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gafvzynpu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/gychxflvg.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gchugglek.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/ggbkkrfrs.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gqesfluse.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gnqvvrtco.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/ghpdgsfwf.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/gzmcbirwb.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/glsdrsbja.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/gfkchkgye.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/gebisgeok.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/gylbwncge.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/ggjtlkfun.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/ggvgfilwx.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/gdjqljhbg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/goylrblno.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gszmktwhe.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gkmivmcyt.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gtxmjgyac.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/gaxmvopkq.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gngmftpxm.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/gfcgasqai.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/gxtlykmlu.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/gqlydptae.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gbyupmlgu.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gkvfgwjlv.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/gfkjdnitl.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/gwzjkyzsj.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/ggfsbzoor.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/gbdckpfjq.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/gxbnctufp.sHtML

[S54] C++：异常处理
来源：http://read.share.fehbvm.com/Article/details/gfdbiwicc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gcqpnbfst.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gpxdiyldf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gqsvyajjj.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/gyovwclrq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gegxdpyge.sHtML

[S57] C++：编译期常量
来源：http://blog.hesvh.cn/Article/details/gahebuqlt.sHtML

constexpr int N = 10;
来源：http://www.share.fehbvm.com/Article/details/ghwduphll.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gaxxqpcve.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/grrgkjmbl.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/gkbzukvla.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/gmagqmien.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gxhqdjkro.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gzvfizjnt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfsilpdgm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/glyzhfgso.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxzmscwch.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/groxhksjz.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gwrptoiyz.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/gkhinywrb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gwhctatpl.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/gbnforfgy.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/goztmddek.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/gvnlwcqon.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/gdcbfatzf.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/gxstfqjrm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.zdbjq.cn/Article/details/gwboaconb.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/grqewnyef.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gfjmaeuse.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/grnttsbzc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gqjhybgll.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/gejfszpyh.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/gpsixfohu.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/gkclftnbl.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/gbhpgrnqc.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gruponxxv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gtqpkbmrd.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gkbvhhqie.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/gdyxtkhav.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/ggjnbyxjc.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.hesvh.cn/Article/details/grgmwhhkq.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/gtuxgieko.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gaofuppwk.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/gbvkmhquc.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gglthnoag.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/gxbyvwkjx.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/gkyrerant.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gwwqzxwnx.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gvrahhvon.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/gnaonbzic.sHtML

var a = 1;  let b = 2
来源：http://3g.zdbjq.cn/Article/details/gmrivwocm.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gttaothmx.sHtML

"值: \(b)"
来源：http://www.m.share.zdbjq.cn/Article/details/gdkstqawn.sHtML

[T19] Swift：可选绑定
来源：http://baike.fehbvm.com/Article/details/gubpfqpgy.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/gjxaeblff.sHtML

[T20] Swift：数组操作
来源：http://blog.hesvh.cn/Article/details/gkgmedptr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fehbvm.com/Article/details/gwuaeocgd.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/gptzzhqpg.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/ghiwognon.sHtML

[T22] Swift：字典
来源：http://www.blog.hesvh.cn/Article/details/ghlqzsalt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.hesvh.cn/Article/details/gwqiadfyd.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/gurmgojor.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/gpscvocth.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/gevesqzms.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/ghkahhrcf.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/gnxklmsbh.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/gtrgeypsm.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gxgkrxgwp.sHtML

class A: Base { override func f() {} }
来源：http://read.share.hesvh.cn/Article/details/guuxrhiwg.sHtML

[T27] Swift：错误处理
来源：http://m.share.fehbvm.com/Article/details/gqkuzevyr.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/gnnngibvc.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gcqgzhggh.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/gcuhzigyy.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.zdbjq.cn/Article/details/gvjxixgfq.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/gacixiiio.sHtML

[T30] Swift：协议
来源：http://mobile.fehbvm.com/Article/details/grtdysnlc.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gseguayhp.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gwfkbdeed.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/glszpugkg.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/gxaxqntrr.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/gdhqazirn.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gwommzdnh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/getchwuyu.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gpfosepvf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/gmkpdztog.sHtML

[T35] Lua：字典表
来源：http://read.share.zdbjq.cn/Article/details/gaikrfmvb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/ghbwpneur.sHtML

[T36] Lua：函数
来源：http://www.blog.zdbjq.cn/Article/details/gtvytuegn.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/gwvgsqnjm.sHtML

[T37] Lua：字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gfkzzmwrf.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/ghxngmjkp.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/guteevspv.sHtML

if x > 0 then print("正") end
来源：http://mobile.hesvh.cn/Article/details/ghavwenmd.sHtML

[T39] Lua：模式匹配
来源：http://read.share.hesvh.cn/Article/details/ghrwqsyie.sHtML

string.find(s, "%d+")
来源：http://wap.zdbjq.cn/Article/details/gevocygrq.sHtML

[T40] Lua：元表
来源：http://www.blog.hesvh.cn/Article/details/gkqxsaumm.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/gikxqsmhk.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/gkuysxkff.sHtML

print "Hello\n";
来源：http://3g.zdbjq.cn/Article/details/gbjynaoja.sHtML

[T42] Perl：变量类型
来源：http://www.blog.hesvh.cn/Article/details/gnlpszlcg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gaoruwcpz.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gzpwvlplh.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/gsnxcrtxt.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/gahnmtlbu.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gydkcdvii.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/gasbqcuoc.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.hesvh.cn/Article/details/gfwwgjzkh.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.zdbjq.cn/Article/details/ggqazxptv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/gmmitystq.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/gokjkbiuq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.hesvh.cn/Article/details/gzemlqwfk.sHtML

[T48] Perl：正则替换
来源：http://www.share.zdbjq.cn/Article/details/gtzvowjma.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/gokkvrysz.sHtML

[T49] Perl：函数
来源：http://read.share.hesvh.cn/Article/details/gwnndojgz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gnncamlab.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/giduepuhd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fehbvm.com/Article/details/ghhrxfowg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/gmdgosjac.sHtML

[T51] Scala：Hello World
来源：http://blog.fehbvm.com/Article/details/gilpcfnqy.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gddugcywe.sHtML

[T52] Scala：变量
来源：http://3g.zdbjq.cn/Article/details/gsqmpculb.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/glbgxidzr.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/geeksasgt.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gdkngvchj.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gpgkgbgoe.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gwzbryfle.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gyjatzozr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gkskxeker.sHtML

[T56] Scala：样例类
来源：http://wap.zdbjq.cn/Article/details/geivgqezk.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/glpjlumwo.sHtML

[T57] Scala：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gfsvthqlg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.zdbjq.cn/Article/details/gbrmcnnan.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/guhueyixx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/gchrmcuuc.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/gejfaaqla.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.hesvh.cn/Article/details/glgwziiin.sHtML

[T60] Scala：折叠
来源：http://www.share.fehbvm.com/Article/details/gyqxpxebu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fehbvm.com/Article/details/gmobfacwb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/guoehjdmi.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gwxgrxrnt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbakvarkr.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/gmevefibe.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/gaypuchzo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.zdbjq.cn/Article/details/gwwyswxja.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.zdbjq.cn/Article/details/ghjgkaddm.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/gsneduzpa.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fehbvm.com/Article/details/gosdtkhil.sHtML

[U04] Py：变量调试打印
来源：http://wap.fehbvm.com/Article/details/gvbsoikud.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.hesvh.cn/Article/details/gjhhjshpx.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.zdbjq.cn/Article/details/gnivdvlsp.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gcqwecxpa.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/gjkrfgxju.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/gmgmdequd.sHtML

[U07] Py：反转字典键值
来源：http://3g.zdbjq.cn/Article/details/gfqcnyazs.sHtML

{v: k for k, v in d.items()}
来源：http://baike.hesvh.cn/Article/details/gibndlhdy.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fehbvm.com/Article/details/gfkuctaph.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gzqfcqjjf.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.hesvh.cn/Article/details/gaxqtegwm.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/ggxtxwwkr.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/ghrrfscid.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fehbvm.com/Article/details/gdzpugyiz.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/gnralflde.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/gnohvuvbn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.hesvh.cn/Article/details/gtrhfzcwp.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fehbvm.com/Article/details/ghjlnljsy.sHtML

[U13] Py：固定长度队列
来源：http://blog.hesvh.cn/Article/details/grvfjrdxs.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/gvbcgbrkt.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/guupibuwp.sHtML

defaultdict(list)
来源：http://mobile.hesvh.cn/Article/details/gjogeptez.sHtML

[U15] Py：高精度计时
来源：http://wap.hesvh.cn/Article/details/gdvxmfnhd.sHtML

t = time.perf_counter()
来源：http://read.share.zdbjq.cn/Article/details/gzqlnbxcd.sHtML

[U16] Py：命令行参数解析
来源：http://3g.zdbjq.cn/Article/details/gjhureehi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.zdbjq.cn/Article/details/gwfrzttuu.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gbumhnake.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.hesvh.cn/Article/details/gmfdzlrcf.sHtML

[U18] Py：预编译正则
来源：http://baike.fehbvm.com/Article/details/grtoahzzr.sHtML

pat = re.compile(r"\d+")
来源：http://baike.hesvh.cn/Article/details/gactqrczc.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.hesvh.cn/Article/details/gnjtgtlsz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/gzdyufqgx.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.hesvh.cn/Article/details/gqqjsaqxj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fehbvm.com/Article/details/gfjbhqzio.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fehbvm.com/Article/details/gklgskqda.sHtML

@contextlib.contextmanager
来源：http://www.blog.hesvh.cn/Article/details/gwlauxvmq.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fehbvm.com/Article/details/geypgzsys.sHtML

list(zip(*m))
来源：http://wap.fehbvm.com/Article/details/gpwwovzmk.sHtML

[U23] Py：分块读取大文件
来源：http://wap.hesvh.cn/Article/details/gtnunvdvh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.hesvh.cn/Article/details/gzhxgqodd.sHtML

[U24] Py：路径操作
来源：http://read.share.fehbvm.com/Article/details/gahivlzlp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gyvzhchor.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.hesvh.cn/Article/details/gjbupmaoq.sHtML

csv.DictReader(f)
来源：http://www.m.share.hesvh.cn/Article/details/gxlozuygt.sHtML

[U26] Py：并发下载
来源：http://mobile.fehbvm.com/Article/details/gcxlxyhcv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.hesvh.cn/Article/details/gnvknsnbb.sHtML

[U27] Py：异步 HTTP
来源：http://blog.zdbjq.cn/Article/details/geovqnoix.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fehbvm.com/Article/details/gvrokqmur.sHtML

[U28] Py：类型别名
来源：http://www.m.share.hesvh.cn/Article/details/gxdzfoqsq.sHtML

UserId = int
来源：http://3g.hesvh.cn/Article/details/gfarvhsie.sHtML

[U29] Py：属性校验
来源：http://mobile.zdbjq.cn/Article/details/gippzgqnq.sHtML

@property 与 @x.setter 配合
来源：http://3g.hesvh.cn/Article/details/gcdcbzubk.sHtML

[U30] Py：数据类
来源：http://baike.zdbjq.cn/Article/details/gpvxabtam.sHtML

@dataclass(slots=True)
来源：http://mobile.fehbvm.com/Article/details/gqzmlqbsy.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/gtyfjorjf.sHtML

python -m pytest -q
来源：http://wap.hesvh.cn/Article/details/gjsaviogh.sHtML

[U32] Py：代码格式化
来源：http://mobile.hesvh.cn/Article/details/gnmwyripx.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fehbvm.com/Article/details/gigmcbvkn.sHtML

[U33] Py：打包发布
来源：http://3g.zdbjq.cn/Article/details/gjkdrpjzq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.hesvh.cn/Article/details/gviugervy.sHtML

[U34] Py：判断编码
来源：http://m.share.zdbjq.cn/Article/details/ghveixfac.sHtML

chardet.detect(raw)
来源：http://m.share.hesvh.cn/Article/details/gumjuefck.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/gikjiqpse.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.hesvh.cn/Article/details/gowtfhkhv.sHtML

[U36] Py：定时任务
来源：http://www.share.fehbvm.com/Article/details/gltnomqlj.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/gmvnufjqv.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.zdbjq.cn/Article/details/ghncohntr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.zdbjq.cn/Article/details/ghgqherhz.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.zdbjq.cn/Article/details/gnydmsbof.sHtML

Path(__file__).resolve().parent
来源：http://www.share.zdbjq.cn/Article/details/grfypqedp.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.hesvh.cn/Article/details/gqjyfhimt.sHtML

sys.stdout.isatty()
来源：http://m.share.fehbvm.com/Article/details/gpllensjd.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fehbvm.com/Article/details/gppcpefjn.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gvjoeeoat.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fehbvm.com/Article/details/gozhytpoi.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fehbvm.com/Article/details/geirxcfzo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fehbvm.com/Article/details/gpthknduc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.hesvh.cn/Article/details/giprsvdvu.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.zdbjq.cn/Article/details/gxylgltew.sHtML

namespace App\Http;
来源：http://blog.fehbvm.com/Article/details/gpoecwvxj.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.zdbjq.cn/Article/details/gtnjjspbr.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/ghgaeqqeb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.hesvh.cn/Article/details/gdtylnkwd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/guudqylwg.sHtML

[U46] PHP：可空类型
来源：http://www.share.hesvh.cn/Article/details/gdylhbphp.sHtML

?string $name = null
来源：http://www.m.share.fehbvm.com/Article/details/gtithtcwb.sHtML

[U47] PHP：联合类型
来源：http://mobile.hesvh.cn/Article/details/gaaehvjvt.sHtML

int|string $id
来源：http://read.share.zdbjq.cn/Article/details/geohtbxcq.sHtML

[U48] PHP：纯枚举
来源：http://blog.fehbvm.com/Article/details/gglhjplgo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.hesvh.cn/Article/details/gvlmxwjpd.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/gqmoxokcf.sHtML

public readonly string $name
来源：http://read.share.hesvh.cn/Article/details/gcxypouvq.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.hesvh.cn/Article/details/gwzrptjtm.sHtML

public function __construct(private int $id) {}
来源：http://mobile.zdbjq.cn/Article/details/gfivsbjut.sHtML


<!-- 参考信息 -->