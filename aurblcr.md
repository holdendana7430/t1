代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gytdjsvlq.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/ghiehohdb.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/gvskdnbgb.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gaxszgvjv.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/geziytvhr.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/gaaycobak.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gaxupswjt.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gtoifzert.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/gdahnxcjm.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/ggzxegsiq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fehbvm.com/Article/details/gjtgqvirp.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/glmcldeif.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gpwgfaooj.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gwjxohdfz.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gatybbqhx.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/geqelason.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gqozgdiac.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gzywshydq.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gywsmfjeb.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/gbvklkont.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/gckiwiray.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/geamamlrp.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gojkmxyoh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/gewejxgxj.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/ggipnqmeu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gpmynbowf.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/gpaxzgyly.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/ghpgbnupn.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gwjfahazz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gdrqbypbb.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/goipzueyc.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/gykruedhh.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/grykvikrn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gviazfuvk.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/grhjwfbuy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/grqnfqfvr.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/gxvsvxxeq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/gssxxsfjq.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gpxdajvty.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/gopwpiacn.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/glvqkmcci.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fehbvm.com/Article/details/glfbvtlki.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gtjvuzonp.sHtML

void inc(int &x) { ++x; }
来源：http://baike.hesvh.cn/Article/details/gdnroncss.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gxocffbgy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gykrhjrws.sHtML

[S46] C++：函数模板
来源：http://www.share.fehbvm.com/Article/details/gdolctflg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/gisfeaqmh.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gxldxcxzr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gafshytya.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gmeijghup.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/gbgtscdou.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/ghlefkffk.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gxpvwnedt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gqwystvox.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/ggrabffga.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gzedkcyqd.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/gpozmcqff.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gbjxdjkxx.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gsuxhdyrm.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gcdfqhnis.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gryfwksjt.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gqharnyco.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/grlpxhonv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/grtxhsfvz.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/godjpegkv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.hesvh.cn/Article/details/gidgnsvbq.sHtML

[S56] C++：optional
来源：http://www.m.share.fehbvm.com/Article/details/gbijsyisq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/gguvlusbu.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gwbzzgddf.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/ghriwzioj.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/gtnbavjph.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/grechstuc.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/gxtaliyyo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/gfpellinv.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gzvpvjtea.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/gpnrrzgii.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghrzybgzx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gtyjjdfrt.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtiefwxnu.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/gwsmjalgj.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gdzkoikfl.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/gwitrirlv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.hesvh.cn/Article/details/gwgfmgety.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/gkoljbqxp.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gwtqfbrfm.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/gntovunkd.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gsuuvcbsl.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/guncigcdg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gyzclfich.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gysxbcafr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fehbvm.com/Article/details/gskcfpjqi.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gtreolbjn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gzzbvkyvg.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gcbfyuowf.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/grzvldjto.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/gnofurdfd.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/gvggqfdps.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/gbocajiqd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/gstynlpse.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gocvjksss.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gsrupvdgv.sHtML

[T12] Kotlin：解构声明
来源：http://baike.zdbjq.cn/Article/details/gznaihbvm.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gaferkrrr.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/ggolxsnpq.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/gqfopxncq.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gfiiwrgym.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/guzqlmrsc.sHtML

[T15] Kotlin：接口
来源：http://3g.fehbvm.com/Article/details/grensjlzm.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/gynrahtvk.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/grxprykif.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gvwrxhsrt.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/ggkkmtwng.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/goylcrczw.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gtkjtotht.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/gydnxtion.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fehbvm.com/Article/details/gjvmkresf.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fehbvm.com/Article/details/gtlpvhdrd.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/gbepnbobz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/ghbjkrtcq.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/gwlxhhxef.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/ggguyybtt.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/glqdpkene.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/gwfkxigxj.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gnkpqglie.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gfwcyggat.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/gmcfpcwub.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gbxpuowbp.sHtML

[T25] Swift：结构体
来源：http://mobile.zdbjq.cn/Article/details/gcuaxxqnd.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gmftfdrgx.sHtML

[T26] Swift：类与重写
来源：http://blog.zdbjq.cn/Article/details/gqxolyuzy.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.hesvh.cn/Article/details/grbhvqvcy.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/gxqqyhjzv.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/gzgeqwxzi.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gxaxppzxb.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/giewlhila.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/gtpznrkqv.sHtML

guard let x = opt else { return }
来源：http://3g.fehbvm.com/Article/details/gvfaaxznb.sHtML

[T30] Swift：协议
来源：http://3g.fehbvm.com/Article/details/gsqrvywxr.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/ganudriav.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/ghyhqkapt.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/ghdnloute.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/gschxeahv.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/gkpqdjejy.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/giabcvklq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/gnvyozhky.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/gbxuzlklf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.hesvh.cn/Article/details/gzibgmwvb.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/gyhmxpwzw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/gymxqddvm.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/ggjpnffrc.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/gztnzhpny.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gluuviute.sHtML

"a" .. "b"
来源：http://www.blog.zdbjq.cn/Article/details/gpkecaonp.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/gtxrrssdp.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/gvbzgwkzn.sHtML

[T39] Lua：模式匹配
来源：http://3g.fehbvm.com/Article/details/ghcjqqxhw.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/gzwrrqemb.sHtML

[T40] Lua：元表
来源：http://wap.zdbjq.cn/Article/details/gqcicfjnj.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fehbvm.com/Article/details/ggcklgnfs.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/gzyiugzip.sHtML

print "Hello\n";
来源：http://baike.fehbvm.com/Article/details/gwvjorlih.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gztncatrr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fehbvm.com/Article/details/gcpywtqjk.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gxlxmcmuf.sHtML

"值: $a"
来源：http://www.blog.fehbvm.com/Article/details/grospgfwc.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/ghtshixfq.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.hesvh.cn/Article/details/gliwiyfrs.sHtML

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/gmnuvuqir.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gurefrqtq.sHtML

[T46] Perl：哈希操作
来源：http://blog.zdbjq.cn/Article/details/gnvslaxpg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/ggudgrnqg.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/gwsppczwa.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/ggzatpidx.sHtML

[T48] Perl：正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gbbemqbgn.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/gresharcl.sHtML

[T49] Perl：函数
来源：http://3g.zdbjq.cn/Article/details/glcizqbun.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gcirizppg.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gmhjljjyp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fehbvm.com/Article/details/gtrwffkeh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/gwmgccuzl.sHtML

[T51] Scala：Hello World
来源：http://wap.zdbjq.cn/Article/details/gujkokqpv.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gfrngewdm.sHtML

[T52] Scala：变量
来源：http://mobile.hesvh.cn/Article/details/gsqqtfqaf.sHtML

val a = 1;  var b = 2
来源：http://wap.fehbvm.com/Article/details/gxmbiibqh.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gxlqckmwh.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gooprnihi.sHtML

[T54] Scala：集合映射
来源：http://baike.zdbjq.cn/Article/details/ghydzaqax.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/grhkzpgcv.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gvugdjagc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fehbvm.com/Article/details/gazwzkved.sHtML

[T56] Scala：样例类
来源：http://baike.hesvh.cn/Article/details/gcmgbbiiv.sHtML

case class User(name: String, age: Int)
来源：http://read.share.hesvh.cn/Article/details/ghgascexy.sHtML

[T57] Scala：模式匹配
来源：http://wap.hesvh.cn/Article/details/gczsexofv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/gaclrndkp.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/ghmgnkbhe.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.zdbjq.cn/Article/details/gosyguxtd.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/gwaytcjqd.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gxrnccogl.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/gmwajrgwu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fehbvm.com/Article/details/gwdpwtmnt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkwfrditn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gvthjzkdj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdnlsgfqq.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fehbvm.com/Article/details/gsusmogdf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.zdbjq.cn/Article/details/gpvahzqzz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.hesvh.cn/Article/details/gyigbxtif.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/gpugpbjbb.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/gvjlbehhr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/gsimhppxl.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gkjnthvqs.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.zdbjq.cn/Article/details/gblhiljaf.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/gaezlhrpu.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gphngbukx.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fehbvm.com/Article/details/gqvfniewr.sHtML

{**a, **b}
来源：http://mobile.zdbjq.cn/Article/details/gfakdiwcn.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fehbvm.com/Article/details/gsqlrdezh.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gpsmqbdsl.sHtML

[U08] Py：展平二维列表
来源：http://blog.zdbjq.cn/Article/details/gbzztijuz.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/gkddggvhs.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fehbvm.com/Article/details/gerjwsqps.sHtML

max(d, key=d.get)
来源：http://www.blog.fehbvm.com/Article/details/gvanodqde.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.hesvh.cn/Article/details/gxlarqpaa.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/gomvlwjex.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/ggmrjrqhs.sHtML

(x * 2 for x in arr)
来源：http://wap.fehbvm.com/Article/details/gpmghmfjo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.zdbjq.cn/Article/details/ggohylcrb.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/gvlqqjlub.sHtML

[U13] Py：固定长度队列
来源：http://baike.hesvh.cn/Article/details/gyhcetyye.sHtML

deque(maxlen=10)
来源：http://mobile.hesvh.cn/Article/details/gdutggtzk.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fehbvm.com/Article/details/gnlqbshny.sHtML

defaultdict(list)
来源：http://www.share.zdbjq.cn/Article/details/gsjkirtqj.sHtML

[U15] Py：高精度计时
来源：http://m.share.zdbjq.cn/Article/details/gicpqqnab.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/gslvscsij.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fehbvm.com/Article/details/gagobrsgu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/gywajdenp.sHtML

[U17] Py：初始化日志
来源：http://www.blog.zdbjq.cn/Article/details/gjybxwygs.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.zdbjq.cn/Article/details/ggtegwcvm.sHtML

[U18] Py：预编译正则
来源：http://m.share.zdbjq.cn/Article/details/gigieuqni.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/gzhumvdza.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/gyjrbspzc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fehbvm.com/Article/details/gqnemlghk.sHtML

[U20] Py：缓存函数结果
来源：http://baike.zdbjq.cn/Article/details/giotrziqj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.zdbjq.cn/Article/details/gfnjizaey.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/gyixmvsbm.sHtML

@contextlib.contextmanager
来源：http://www.blog.hesvh.cn/Article/details/gbterhykj.sHtML

[U22] Py：矩阵转置
来源：http://read.share.zdbjq.cn/Article/details/gshbqurzh.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/gefxqklbo.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.hesvh.cn/Article/details/gqtmntwqa.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fehbvm.com/Article/details/gtnewbarp.sHtML

[U24] Py：路径操作
来源：http://wap.fehbvm.com/Article/details/gbdlnsifw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/grwxfuhda.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/gkldsaroz.sHtML

csv.DictReader(f)
来源：http://3g.zdbjq.cn/Article/details/gfrjfdorn.sHtML

[U26] Py：并发下载
来源：http://m.share.fehbvm.com/Article/details/grvzccmwz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fehbvm.com/Article/details/ghfwbryxt.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fehbvm.com/Article/details/gqzdshiyn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.zdbjq.cn/Article/details/gflsyahdp.sHtML

[U28] Py：类型别名
来源：http://mobile.zdbjq.cn/Article/details/gximlbilf.sHtML

UserId = int
来源：http://m.share.fehbvm.com/Article/details/gtelsmjfc.sHtML

[U29] Py：属性校验
来源：http://www.blog.zdbjq.cn/Article/details/gbjwfunbh.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fehbvm.com/Article/details/gzwunjbao.sHtML

[U30] Py：数据类
来源：http://www.share.fehbvm.com/Article/details/gawhlzxzh.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/gulxeabkh.sHtML

[U31] Py：单测
来源：http://www.blog.hesvh.cn/Article/details/gclduedqf.sHtML

python -m pytest -q
来源：http://mobile.zdbjq.cn/Article/details/gzbwpycvc.sHtML

[U32] Py：代码格式化
来源：http://3g.fehbvm.com/Article/details/gcgtpvxkl.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fehbvm.com/Article/details/gguklvpxr.sHtML

[U33] Py：打包发布
来源：http://m.share.fehbvm.com/Article/details/ghdsevhuf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/gealfcxql.sHtML

[U34] Py：判断编码
来源：http://www.share.fehbvm.com/Article/details/gexsafoll.sHtML

chardet.detect(raw)
来源：http://read.share.fehbvm.com/Article/details/gkezotiwg.sHtML

[U35] Py：发送邮件
来源：http://3g.hesvh.cn/Article/details/gtihgawjx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/gtjqpbpwf.sHtML

[U36] Py：定时任务
来源：http://m.share.zdbjq.cn/Article/details/gbyvpncro.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fehbvm.com/Article/details/gmnkflnph.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.hesvh.cn/Article/details/geshalwkx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fehbvm.com/Article/details/giytlwrun.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fehbvm.com/Article/details/gdygqdljh.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.zdbjq.cn/Article/details/gvdztlecs.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.zdbjq.cn/Article/details/gevgswpkm.sHtML

sys.stdout.isatty()
来源：http://www.blog.fehbvm.com/Article/details/gcabqmyjt.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.zdbjq.cn/Article/details/gdyagcwwy.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/glpbjfexc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.hesvh.cn/Article/details/gjiriyamm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.hesvh.cn/Article/details/gdopeqgpk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fehbvm.com/Article/details/gxlmjctuy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.hesvh.cn/Article/details/gsnhtgswh.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.zdbjq.cn/Article/details/gdyvdomkm.sHtML

namespace App\Http;
来源：http://www.share.zdbjq.cn/Article/details/gtfvdnrtv.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/giyoyhlwb.sHtML

declare(strict_types=1);
来源：http://3g.hesvh.cn/Article/details/gybpgwksd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/gujjvmeso.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gnsxsehqw.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.hesvh.cn/Article/details/gizxoqotx.sHtML

?string $name = null
来源：http://mobile.hesvh.cn/Article/details/geqgegyuu.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.hesvh.cn/Article/details/gpfgpppgm.sHtML

int|string $id
来源：http://3g.fehbvm.com/Article/details/grvyeiqzw.sHtML

[U48] PHP：纯枚举
来源：http://read.share.zdbjq.cn/Article/details/gjsbmtppl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fehbvm.com/Article/details/gxwkttyzo.sHtML


<!-- 参考信息 -->