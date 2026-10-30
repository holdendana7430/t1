代发 wailian999

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gylpnmdlq.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/goustqofw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gtylqahaf.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gvougbkfp.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gpxnuogtc.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gmpqyndqf.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gdoergqst.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/gasewqntq.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/gniouvqmd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/gixznzmud.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gmzkvklay.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/giocjokfi.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/gaqltwywl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gzdkeslju.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/gwybqmwuk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/gwgrskeen.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gwqouaqgu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gyymcaupn.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gkfemgade.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/glhhpdgby.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/gxgwmaetp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/ghxcymksc.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/gciapoetu.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/ganqevvar.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/ggbfcokpj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gwwaxkfqj.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gykofsdbw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/guzkrhege.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/gvzbewkgo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/gkpmzcrpu.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/gekrwaqsu.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/gsryztnjq.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/getjbeuug.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gporwuuzx.sHtML

[S44] C++：引用传参
来源：http://wap.fehbvm.com/Article/details/gxbrngvut.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/gmupgouiu.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/ghwicjglw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gbowzaawa.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gexdyvktz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/glfpmvorg.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gjbxxlzxr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gexljapfi.sHtML

[S48] C++：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gmdumalqv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gftdycvvs.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/gvuxmhtfv.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/gcfmztkuy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gqteljzcu.sHtML

[S50] C++：格式化数字
来源：http://blog.zdbjq.cn/Article/details/gydjyeiza.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gtiipywsz.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/ghvqodcos.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/ghmhvrmvq.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/gwitaqovo.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/ghziqaswj.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/gkbslirgs.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gvxdqoixg.sHtML

[S54] C++：异常处理
来源：http://baike.fehbvm.com/Article/details/gbtvhgehl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/goajgooit.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gqmpnfbrw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gyctlinkr.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/gfrwnaygj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fehbvm.com/Article/details/guwridgzk.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/gbpuncgwy.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/grtuhdzqw.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/gxaivmkzk.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/guqqfvgyq.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/gnjfzuooe.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/gcdkaiikn.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fehbvm.com/Article/details/gazcvyeuk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/gtzkjqnjt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glecyxqjz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gfgtuqzvw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcvwoxwct.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gekcimqal.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gcuplhoel.sHtML

[T02] Kotlin：变量
来源：http://blog.hesvh.cn/Article/details/gfktchanz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gbwlxudzq.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/gacknbmuj.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gtjnmaqgs.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/gbsveykwi.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gfkuumdqu.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/gyuhwpwlt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gvgjqedrq.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gzvuuxuda.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/gygyhicen.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gcdfpumyn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gilgakjeh.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/grcrktvxi.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gmpqwqsrg.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gibbjxeyq.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.zdbjq.cn/Article/details/gqkfbrvty.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gbhucqexz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gldxfcule.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/gxmpqjzxp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/glwzxiats.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/gzioinqun.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gkviiauov.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/gajvyoref.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gdjawdrnc.sHtML

[T14] Kotlin：循环
来源：http://blog.hesvh.cn/Article/details/gzsplgczd.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gzrqzfczy.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/ghmqiljuu.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gcmcghntu.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gniihctdl.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gmkvtogps.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/glguccwsx.sHtML

var a = 1;  let b = 2
来源：http://mobile.zdbjq.cn/Article/details/gqmefpmch.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/gobauywxn.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/gjhwmdpbe.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/gvrcglfgq.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/gffbfbjgo.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/gaskpyavf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.hesvh.cn/Article/details/ghiurwaip.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/gaufusvog.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/gmcoroudo.sHtML

[T22] Swift：字典
来源：http://blog.fehbvm.com/Article/details/gsxlyuzjb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/gtyqrbpmf.sHtML

[T23] Swift：函数
来源：http://blog.fehbvm.com/Article/details/gcbgwxkfn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/gdgrrqiqj.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/gbctyknru.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gcvnhossp.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/gkerchabw.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/geioujndn.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/gzqorrzia.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/gisbvbcrv.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/grgshtxxo.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/gzitskxwi.sHtML

[T28] Swift：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gthajhbxp.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/ghnatbhwj.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/gpknckyba.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fehbvm.com/Article/details/gywesmpyk.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/gtbpubrsz.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.zdbjq.cn/Article/details/gakerkxnx.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gkisxbuxd.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/ggmewjdmp.sHtML

[T32] Lua：局部变量
来源：http://wap.fehbvm.com/Article/details/gcwxjkqnt.sHtML

local a = 1
来源：http://www.m.share.hesvh.cn/Article/details/goaxkqfrk.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fehbvm.com/Article/details/glqbhsqoz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/gvppkshls.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/ggtukuepv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.zdbjq.cn/Article/details/guvujyejz.sHtML

[T35] Lua：字典表
来源：http://wap.hesvh.cn/Article/details/ghmmdmhct.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.hesvh.cn/Article/details/ghzevbblt.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/gvvcfkpsy.sHtML

function add(a, b) return a + b end
来源：http://read.share.fehbvm.com/Article/details/giszqmqcw.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gnluyqwij.sHtML

"a" .. "b"
来源：http://wap.fehbvm.com/Article/details/govpruunl.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/gfuprmgsa.sHtML

if x > 0 then print("正") end
来源：http://www.share.hesvh.cn/Article/details/gklnjyjwt.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gimwgktye.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/gcrdektrg.sHtML

[T40] Lua：元表
来源：http://baike.hesvh.cn/Article/details/gcfsrwaih.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/gkaythicp.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/gcrfbdakl.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/gltftkvyy.sHtML

[T42] Perl：变量类型
来源：http://m.share.fehbvm.com/Article/details/gfftwhlfj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.zdbjq.cn/Article/details/goujyjndj.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gaqkuaaow.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/gurmtcsyj.sHtML

[T44] Perl：条件
来源：http://www.share.fehbvm.com/Article/details/glhalambd.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/gigbjtkml.sHtML

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/ggyspwqef.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.zdbjq.cn/Article/details/gpmytmrot.sHtML

[T46] Perl：哈希操作
来源：http://wap.zdbjq.cn/Article/details/gpztcfink.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gacaquvuk.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.hesvh.cn/Article/details/gzdxuzqlz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.zdbjq.cn/Article/details/gsvqhkkwa.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/gtsgsnlot.sHtML

$s =~ s/old/new/g;
来源：http://www.share.zdbjq.cn/Article/details/gcddlwlel.sHtML

[T49] Perl：函数
来源：http://mobile.hesvh.cn/Article/details/gapvaplnm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gstxwoqgz.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gcvcpqicv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fehbvm.com/Article/details/grjkuuvrg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fehbvm.com/Article/details/gufwqdzwn.sHtML

[T51] Scala：Hello World
来源：http://baike.hesvh.cn/Article/details/gjuehvcqz.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gioufzbfo.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/gqpoqyrcd.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/gchjgojmp.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/ghbzkpyim.sHtML

s"值: $b"
来源：http://m.share.hesvh.cn/Article/details/guyhngwbp.sHtML

[T54] Scala：集合映射
来源：http://m.share.hesvh.cn/Article/details/gqoqesjfc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/grepwqlkl.sHtML

[T55] Scala：集合过滤
来源：http://3g.fehbvm.com/Article/details/gfdptjzjw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fehbvm.com/Article/details/gpvvyrgqu.sHtML

[T56] Scala：样例类
来源：http://baike.hesvh.cn/Article/details/gkfeismpz.sHtML

case class User(name: String, age: Int)
来源：http://www.share.hesvh.cn/Article/details/gfvbvbyvh.sHtML

[T57] Scala：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gbdkozvol.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fehbvm.com/Article/details/glmaqifww.sHtML

[T58] Scala：函数定义
来源：http://read.share.zdbjq.cn/Article/details/gasnprohj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.zdbjq.cn/Article/details/gesmgipfo.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/gijmduxky.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/gonjoactf.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/ggwypojea.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fehbvm.com/Article/details/gkokoesvi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/garjjaubf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/goenowtee.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqfvweigt.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.zdbjq.cn/Article/details/gfqlukenf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.zdbjq.cn/Article/details/ggmmuarjk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.hesvh.cn/Article/details/gmystrecs.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fehbvm.com/Article/details/gviwligqe.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fehbvm.com/Article/details/guaxqncgu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fehbvm.com/Article/details/gwxtsariz.sHtML

[U04] Py：变量调试打印
来源：http://www.share.hesvh.cn/Article/details/gcilrzzgm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/gsyozwfja.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/gjgvxszot.sHtML

list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gfdlkcxsp.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/ggbhglrsz.sHtML

{**a, **b}
来源：http://3g.fehbvm.com/Article/details/gvyoxknzx.sHtML

[U07] Py：反转字典键值
来源：http://www.share.hesvh.cn/Article/details/gbgkmjymh.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/gfykpnyzn.sHtML

[U08] Py：展平二维列表
来源：http://m.share.zdbjq.cn/Article/details/glsqoyddo.sHtML

[y for x in nested for y in x]
来源：http://www.share.zdbjq.cn/Article/details/gdekmpwmq.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fehbvm.com/Article/details/gedcxzmfb.sHtML

max(d, key=d.get)
来源：http://3g.hesvh.cn/Article/details/glgvtycxk.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/gfjwwiixj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/geftjdkfr.sHtML

[U11] Py：生成器表达式
来源：http://www.share.hesvh.cn/Article/details/gpelzkqho.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/gdnmhrtsv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fehbvm.com/Article/details/grmdyidsj.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fehbvm.com/Article/details/gzanyzufn.sHtML

[U13] Py：固定长度队列
来源：http://3g.zdbjq.cn/Article/details/gngpleina.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/gknsluddo.sHtML

[U14] Py：分组收集到列表
来源：http://baike.zdbjq.cn/Article/details/gfbgbcfno.sHtML

defaultdict(list)
来源：http://blog.zdbjq.cn/Article/details/gdqarnxga.sHtML

[U15] Py：高精度计时
来源：http://read.share.zdbjq.cn/Article/details/gtzuwernf.sHtML

t = time.perf_counter()
来源：http://mobile.zdbjq.cn/Article/details/gntafdilw.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.zdbjq.cn/Article/details/gnukgtxkx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/gudslkddo.sHtML

[U17] Py：初始化日志
来源：http://3g.zdbjq.cn/Article/details/gohyydbjw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/gmnudkkui.sHtML

[U18] Py：预编译正则
来源：http://read.share.zdbjq.cn/Article/details/gsjesnmsi.sHtML

pat = re.compile(r"\d+")
来源：http://wap.zdbjq.cn/Article/details/geusqcota.sHtML

[U19] Py：正则替换带回调
来源：http://wap.zdbjq.cn/Article/details/gslggcxne.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fehbvm.com/Article/details/gtnnjcgfr.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.hesvh.cn/Article/details/gpnolzlek.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.hesvh.cn/Article/details/gaofgubkk.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fehbvm.com/Article/details/gaveeykaa.sHtML

@contextlib.contextmanager
来源：http://read.share.hesvh.cn/Article/details/gockpnycd.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.hesvh.cn/Article/details/gtpjsfhsw.sHtML

list(zip(*m))
来源：http://baike.hesvh.cn/Article/details/gxxfiwexj.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.hesvh.cn/Article/details/gnioqbqpi.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.zdbjq.cn/Article/details/glikfmvez.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/gttjvoppe.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gencnriul.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fehbvm.com/Article/details/gcxcrowfl.sHtML

csv.DictReader(f)
来源：http://3g.hesvh.cn/Article/details/gppfdtugx.sHtML

[U26] Py：并发下载
来源：http://3g.hesvh.cn/Article/details/glcoyjaak.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.hesvh.cn/Article/details/gtjvdhebu.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.zdbjq.cn/Article/details/gfudmnsus.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.hesvh.cn/Article/details/gkpeyesiw.sHtML

[U28] Py：类型别名
来源：http://www.share.hesvh.cn/Article/details/ggwcfpqgq.sHtML

UserId = int
来源：http://blog.zdbjq.cn/Article/details/gbvwpifvh.sHtML

[U29] Py：属性校验
来源：http://3g.fehbvm.com/Article/details/gvhjuzrws.sHtML

@property 与 @x.setter 配合
来源：http://www.share.zdbjq.cn/Article/details/gjwflsefb.sHtML

[U30] Py：数据类
来源：http://3g.zdbjq.cn/Article/details/gzxemevqo.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fehbvm.com/Article/details/gfwnaskmt.sHtML

[U31] Py：单测
来源：http://read.share.hesvh.cn/Article/details/gfnavyedo.sHtML

python -m pytest -q
来源：http://www.share.hesvh.cn/Article/details/gburyogqg.sHtML

[U32] Py：代码格式化
来源：http://www.blog.zdbjq.cn/Article/details/gmzlwwmei.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fehbvm.com/Article/details/gdrijheqb.sHtML

[U33] Py：打包发布
来源：http://wap.hesvh.cn/Article/details/gcazlrrek.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.zdbjq.cn/Article/details/gszabfjkl.sHtML

[U34] Py：判断编码
来源：http://www.blog.fehbvm.com/Article/details/gksojhkfl.sHtML

chardet.detect(raw)
来源：http://www.m.share.fehbvm.com/Article/details/gmopjcnun.sHtML

[U35] Py：发送邮件
来源：http://m.share.hesvh.cn/Article/details/gyxhaazxi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/gzczlolxr.sHtML

[U36] Py：定时任务
来源：http://read.share.zdbjq.cn/Article/details/gbwdtzcth.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.hesvh.cn/Article/details/gsagjjrtd.sHtML

[U37] Py：读写 Excel
来源：http://blog.zdbjq.cn/Article/details/gudweopkh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fehbvm.com/Article/details/gxyfjdvsu.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.hesvh.cn/Article/details/gvqitpqff.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fehbvm.com/Article/details/gyxqkkpsj.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.hesvh.cn/Article/details/gcxepojak.sHtML

sys.stdout.isatty()
来源：http://wap.zdbjq.cn/Article/details/ggulujlhy.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/ghomzfhls.sHtML

print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gioywdfwo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.zdbjq.cn/Article/details/gukjcewlx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fehbvm.com/Article/details/gelfrmlym.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fehbvm.com/Article/details/gordkqdcq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fehbvm.com/Article/details/gxyknvpaz.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.zdbjq.cn/Article/details/grxirnxmw.sHtML

namespace App\Http;
来源：http://read.share.hesvh.cn/Article/details/givjblubi.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.zdbjq.cn/Article/details/gwzrtitsh.sHtML

declare(strict_types=1);
来源：http://3g.hesvh.cn/Article/details/gggaxhupy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.zdbjq.cn/Article/details/gjhncwczk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gptggaddl.sHtML

[U46] PHP：可空类型
来源：http://wap.zdbjq.cn/Article/details/gxnpiviez.sHtML

?string $name = null
来源：http://www.share.fehbvm.com/Article/details/gdxsgvisx.sHtML

[U47] PHP：联合类型
来源：http://m.share.fehbvm.com/Article/details/gocaayave.sHtML

int|string $id
来源：http://3g.zdbjq.cn/Article/details/gqvbgtpqb.sHtML

[U48] PHP：纯枚举
来源：http://3g.hesvh.cn/Article/details/gnsftruqt.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fehbvm.com/Article/details/gkrgrjjzl.sHtML

[U49] PHP：只读属性
来源：http://blog.zdbjq.cn/Article/details/gzkrryezs.sHtML

public readonly string $name
来源：http://blog.fehbvm.com/Article/details/glhagvuok.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fehbvm.com/Article/details/gvkmmvmyf.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.zdbjq.cn/Article/details/gopbsbakl.sHtML

[U51] PHP：数组解构
来源：http://read.share.zdbjq.cn/Article/details/givoapcvp.sHtML

[$a, $b] = $arr;
来源：http://mobile.hesvh.cn/Article/details/gsiykcuig.sHtML

[U52] PHP：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gpdcnlgur.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fehbvm.com/Article/details/gckewzzpk.sHtML


<!-- 参考信息 -->