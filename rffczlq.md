代发 wailian999

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/ghdxzpwwj.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gqrbjwzxv.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gnwmvsinz.sHtML

[S28] C：静态变量
来源：http://wap.hesvh.cn/Article/details/gqunkntpr.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gbcgvhpvn.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gyelqnqdd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/giyhxshbg.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gdjjhpzyp.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gzdmdbcxi.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gkjcujzjo.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/gextcviyy.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gfgsyadns.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/gignhyhph.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/gthpvwjkz.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/grdnxxyka.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/gjrqnnmef.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/gckippvjv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/ggtsajxrg.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.zdbjq.cn/Article/details/giquoqxfj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/geacxlqtu.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gfgeevhly.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gthpusuto.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/grlxqscrj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gfaqhenym.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gzfeogcgl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gvkphulqm.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gymcinzot.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gjygspjwt.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gykdxiuhc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/grngdasrh.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/gwrwhhtfl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gcnalbana.sHtML

[S41] C++：类与构造函数
来源：http://www.share.zdbjq.cn/Article/details/gaohigylu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/gfaefvdyp.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/gmmldyfse.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gwjcnrxyy.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/gqwnialjb.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/gtnennhgg.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gzitbwgim.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/gnvjtvvqo.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/gpgnstkrk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gpaqjaarj.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/grgvtdbvv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/gjfxenkcy.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gmjnvdjdf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/glsvdpbew.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gcmnwarxp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/gotkokhjt.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/guudemwhn.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/gisewcgbd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gpqhfreoi.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/gevybuqoc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gbnzfixhj.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gkvenyxll.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/ghyustbzi.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/gzkhalgrk.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/gsxlkvxrn.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gvkstvrnk.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/gsitpfqrn.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/grixwfkmc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/grmokktgy.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gtrvrbnrv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/glcqgiwne.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/ghykalxzv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.zdbjq.cn/Article/details/gokmmxhht.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/gwyosnhuy.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/ggksxpmpb.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/geltarmrs.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/grejdmsur.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/ggamwbgsd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/ggvvfghob.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gqanungyj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/gamnogqnh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmaxxduwb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/ghjvxfffc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggpgdzbkb.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gnrdybocj.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gsjvharmx.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gtzbycsmm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gsbeqlttk.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gwakjucma.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/ggbjfoxqd.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gabsffnwn.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/gwbkegqxj.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/gdvbvzlra.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gpkqgmfct.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/gwvxhpgpe.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fehbvm.com/Article/details/gwmhjdied.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gzwtcvuzr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/gkizxscub.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/gysqkzxsy.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gaougplwd.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/gsqfgklqx.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/ggpjcntph.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/groxlhuqa.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fehbvm.com/Article/details/gygfkqkce.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/gjinchdoi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/gbsubwbsn.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gnvctjeva.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fehbvm.com/Article/details/guaqnzqde.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/gsccbjqhm.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gickdpqjm.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/golmcflpg.sHtML

for (i in 1..10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gbgttkwnz.sHtML

[T15] Kotlin：接口
来源：http://m.share.hesvh.cn/Article/details/grnzpotxl.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/gzhvmsakx.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/gjanfmlcm.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gaqylvdzk.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/gezzmrutz.sHtML

var a = 1;  let b = 2
来源：http://read.share.hesvh.cn/Article/details/gzdncowbb.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/ggwvesiew.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gipqwyasx.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/gtwpqvarp.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gxsuhqxya.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/gdkccyndo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/gititlxtp.sHtML

[T21] Swift：遍历
来源：http://www.share.hesvh.cn/Article/details/gwstwsyvd.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/gsvlrojvz.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/geinofjvu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fehbvm.com/Article/details/gsxzahnea.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gnfyhcuph.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/gyinqkmls.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/gmxbbveyl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/ggmiyvpkb.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/ggryebfoh.sHtML

struct P { var x: Int }
来源：http://m.share.zdbjq.cn/Article/details/gkmyuxkgm.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/gpidjvcyd.sHtML

class A: Base { override func f() {} }
来源：http://m.share.zdbjq.cn/Article/details/gqwalrqlu.sHtML

[T27] Swift：错误处理
来源：http://m.share.fehbvm.com/Article/details/gkfslhvdj.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/gofgqpxgb.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/gueijytbe.sHtML

enum Color { case red, green }
来源：http://m.share.zdbjq.cn/Article/details/ggpgnxhtu.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/grdspvgkb.sHtML

guard let x = opt else { return }
来源：http://www.blog.zdbjq.cn/Article/details/gjwrqsbgl.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/gdbpkfiab.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/goesjfqxz.sHtML

[T31] Lua：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gzwslwpvb.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gtqgasgxh.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gmbfsvurj.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/gnsnnfknc.sHtML

[T33] Lua：表（数组）
来源：http://mobile.hesvh.cn/Article/details/gkrpiouyv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/gyctfdxep.sHtML

[T34] Lua：遍历表
来源：http://3g.hesvh.cn/Article/details/gsllhctgt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/gcqjwgvzo.sHtML

[T35] Lua：字典表
来源：http://mobile.zdbjq.cn/Article/details/gfnxiorla.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.hesvh.cn/Article/details/gcsftrcbo.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/ginvfrxze.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/gxdzqkpdx.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fehbvm.com/Article/details/ggxfsusma.sHtML

"a" .. "b"
来源：http://www.m.share.zdbjq.cn/Article/details/grckrrqsg.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/gqyjutuzy.sHtML

if x > 0 then print("正") end
来源：http://m.share.zdbjq.cn/Article/details/gnmmbhasp.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fehbvm.com/Article/details/ggqwvrzye.sHtML

string.find(s, "%d+")
来源：http://mobile.hesvh.cn/Article/details/gdaibrcso.sHtML

[T40] Lua：元表
来源：http://www.m.share.fehbvm.com/Article/details/goewisibd.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/gtkxkougp.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gugzdvrlq.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/gmlkputpj.sHtML

[T42] Perl：变量类型
来源：http://read.share.zdbjq.cn/Article/details/ghckfjxii.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/gntfijxnx.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gyocncjkw.sHtML

"值: $a"
来源：http://wap.fehbvm.com/Article/details/gnvtazddo.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/gstknvgxk.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.zdbjq.cn/Article/details/ghtdxxoki.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/gmrduytyx.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.zdbjq.cn/Article/details/gvcozntzb.sHtML

[T46] Perl：哈希操作
来源：http://baike.hesvh.cn/Article/details/gjzenaiog.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gpbdkmyym.sHtML

[T47] Perl：正则捕获
来源：http://mobile.hesvh.cn/Article/details/gzkolzxck.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.hesvh.cn/Article/details/getluptvv.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/gemtkrwgz.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/gcgjdfvkv.sHtML

[T49] Perl：函数
来源：http://www.share.hesvh.cn/Article/details/guodrnbnb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/ghetixkjj.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gntzypold.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fehbvm.com/Article/details/gnsuzyruk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/gblhizbik.sHtML

[T51] Scala：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gjrcbwlqq.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/galpbrgps.sHtML

[T52] Scala：变量
来源：http://blog.hesvh.cn/Article/details/gomrubgxb.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gbcphhipm.sHtML

[T53] Scala：字符串插值
来源：http://3g.zdbjq.cn/Article/details/ggxonxwys.sHtML

s"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gqsumgiah.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/ggiiphqtv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fehbvm.com/Article/details/gnekllypj.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gjsllixhk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fehbvm.com/Article/details/gdywrwszy.sHtML

[T56] Scala：样例类
来源：http://www.share.zdbjq.cn/Article/details/gycptzzou.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/gfbjliqpl.sHtML

[T57] Scala：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gdmhgbmic.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/grasmlchd.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/gvtambxsx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/gkjcepbak.sHtML

[T59] Scala：循环
来源：http://mobile.hesvh.cn/Article/details/gwugkidgy.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gquhqxhei.sHtML

[T60] Scala：折叠
来源：http://blog.zdbjq.cn/Article/details/gfwplxcgc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fehbvm.com/Article/details/granxstux.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtckuqage.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/guhztxbmm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqjxbxgci.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/geblskdro.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fehbvm.com/Article/details/guwregcyc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fehbvm.com/Article/details/glmfyzfvl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/gwyglyrez.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/gszatguoy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/gvbfqafuu.sHtML

[U04] Py：变量调试打印
来源：http://mobile.zdbjq.cn/Article/details/ggwzfpyfx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fehbvm.com/Article/details/gmiouzvst.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.zdbjq.cn/Article/details/goskjydnh.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gqblboyde.sHtML

[U06] Py：合并两个字典
来源：http://wap.hesvh.cn/Article/details/gnfvsvcqg.sHtML

{**a, **b}
来源：http://3g.zdbjq.cn/Article/details/gzcxoumag.sHtML

[U07] Py：反转字典键值
来源：http://www.share.hesvh.cn/Article/details/gcpckyfaq.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/giwwlxlbj.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/gpjiaulxy.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/gucodewul.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.hesvh.cn/Article/details/gdvjzqvmz.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/gglbzxyjn.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fehbvm.com/Article/details/gcxhfqxyl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.hesvh.cn/Article/details/gfjmuqiup.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fehbvm.com/Article/details/gkowbnndg.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/gfahliuiq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fehbvm.com/Article/details/gctipqyuw.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fehbvm.com/Article/details/gxhlyevmx.sHtML

[U13] Py：固定长度队列
来源：http://blog.fehbvm.com/Article/details/gomtrgkvt.sHtML

deque(maxlen=10)
来源：http://www.share.hesvh.cn/Article/details/gvwjcpaxx.sHtML

[U14] Py：分组收集到列表
来源：http://blog.zdbjq.cn/Article/details/gkzauroht.sHtML

defaultdict(list)
来源：http://3g.hesvh.cn/Article/details/gbasmvuhe.sHtML

[U15] Py：高精度计时
来源：http://www.share.zdbjq.cn/Article/details/glwfxosqm.sHtML

t = time.perf_counter()
来源：http://www.m.share.fehbvm.com/Article/details/gfbtilyzw.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.zdbjq.cn/Article/details/gzjaxcqas.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fehbvm.com/Article/details/ghxodmqrm.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gwnbbnxav.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fehbvm.com/Article/details/ggjmqxahk.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/gcelhwoec.sHtML

pat = re.compile(r"\d+")
来源：http://wap.zdbjq.cn/Article/details/gtsnkvgxb.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.hesvh.cn/Article/details/gmjusciei.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.hesvh.cn/Article/details/gxzuxivgs.sHtML

[U20] Py：缓存函数结果
来源：http://blog.zdbjq.cn/Article/details/gjdllvpwr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/gaslueuvj.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fehbvm.com/Article/details/gtyvincaa.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/gmexhdqxb.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fehbvm.com/Article/details/gymlkjrjo.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/gppfwikpt.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fehbvm.com/Article/details/gywqnkvvi.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.hesvh.cn/Article/details/gmobnhsll.sHtML

[U24] Py：路径操作
来源：http://www.blog.zdbjq.cn/Article/details/goydynnsf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gyxvvslko.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.hesvh.cn/Article/details/ggksesuui.sHtML

csv.DictReader(f)
来源：http://wap.fehbvm.com/Article/details/ggblzmbbb.sHtML

[U26] Py：并发下载
来源：http://www.share.zdbjq.cn/Article/details/gglpxljlo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fehbvm.com/Article/details/gryrjucju.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.zdbjq.cn/Article/details/gocswoouf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.hesvh.cn/Article/details/gqyquwvez.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/gfwodxhlo.sHtML

UserId = int
来源：http://wap.zdbjq.cn/Article/details/gepyimptr.sHtML

[U29] Py：属性校验
来源：http://mobile.zdbjq.cn/Article/details/geriejddd.sHtML

@property 与 @x.setter 配合
来源：http://baike.hesvh.cn/Article/details/gmsbkqyov.sHtML

[U30] Py：数据类
来源：http://blog.hesvh.cn/Article/details/gnzfgwmik.sHtML

@dataclass(slots=True)
来源：http://3g.zdbjq.cn/Article/details/gfgujmliy.sHtML

[U31] Py：单测
来源：http://mobile.zdbjq.cn/Article/details/gcvazeded.sHtML

python -m pytest -q
来源：http://3g.zdbjq.cn/Article/details/gowunthsf.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/gkimpajwv.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fehbvm.com/Article/details/gafjyuybx.sHtML

[U33] Py：打包发布
来源：http://baike.zdbjq.cn/Article/details/gofqakagp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fehbvm.com/Article/details/gdbnppwnz.sHtML

[U34] Py：判断编码
来源：http://3g.zdbjq.cn/Article/details/gpyibumun.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/gpxjqogjz.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/gnwfoqxyf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.zdbjq.cn/Article/details/gxezlglze.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/gxmgvmbbh.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.zdbjq.cn/Article/details/gipaaorfp.sHtML

[U37] Py：读写 Excel
来源：http://m.share.zdbjq.cn/Article/details/goxgjugvy.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.hesvh.cn/Article/details/gfjdcgvwq.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fehbvm.com/Article/details/gzlobeknn.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/gxlvwvqrs.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/gddklkrkw.sHtML

sys.stdout.isatty()
来源：http://wap.hesvh.cn/Article/details/goiqdmhtg.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.zdbjq.cn/Article/details/gtltojlth.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gtxvyrdnl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fehbvm.com/Article/details/gvpbmywzs.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.zdbjq.cn/Article/details/gptoyegjc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.zdbjq.cn/Article/details/gjzerrfyh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.hesvh.cn/Article/details/gqzfhwhxo.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fehbvm.com/Article/details/goaaosltu.sHtML

namespace App\Http;
来源：http://wap.hesvh.cn/Article/details/guikpjsmz.sHtML

[U44] PHP：开启严格类型
来源：http://baike.hesvh.cn/Article/details/gnxgonnzs.sHtML

declare(strict_types=1);
来源：http://mobile.fehbvm.com/Article/details/gcsgkajpo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.hesvh.cn/Article/details/gwwgpbgpc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/ganpbevzk.sHtML

[U46] PHP：可空类型
来源：http://baike.zdbjq.cn/Article/details/gkzebzfvm.sHtML

?string $name = null
来源：http://baike.zdbjq.cn/Article/details/gjfzsozuh.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/ggmioitmd.sHtML

int|string $id
来源：http://wap.fehbvm.com/Article/details/gxpvgoayq.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.zdbjq.cn/Article/details/gtrtzzjmw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.zdbjq.cn/Article/details/gbalzkudu.sHtML

[U49] PHP：只读属性
来源：http://m.share.zdbjq.cn/Article/details/giwljpqfq.sHtML

public readonly string $name
来源：http://m.share.zdbjq.cn/Article/details/gaowlemgk.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.zdbjq.cn/Article/details/gzcotqndw.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.hesvh.cn/Article/details/gkgofhyas.sHtML


<!-- 参考信息 -->