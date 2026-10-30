代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gloqtmfme.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/ghcoctjna.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gzvnhwkff.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/grbjdrmhg.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gmgssrmoa.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/gqsrfpzjv.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gnutguyvc.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/gljdkiuvu.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/gbjizkplk.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/grqmgtmhr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gpaxefyyq.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gofxbvqyg.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gdbouffji.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gwjlpvbkt.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gcaaxvrbh.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/gbechykdf.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/gndvoyhdc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/gcvvimyys.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gedlafabq.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/ggzjrcnsc.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/gdgzpavlr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/gaatsajeg.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/gdwbkkjtq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/gaskbtate.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/ghhxfcneq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gaajfvztu.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/gblnafbvj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gxyglggtf.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/gfzmupqlt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/grqnurcgp.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/gwwgeutag.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gyeisdqmx.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/gocdlulgo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gxertozns.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fehbvm.com/Article/details/gnbxgfcdk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gjuxsbxho.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gxmogbntf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gwsgxxods.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/grctvoesr.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/gvrvgzukw.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/gzkwrhwma.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/gphmyjcrw.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gsztvubvp.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/gxkpbomrr.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/gntsalmtn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gfjdjjyje.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gyhiosxlr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/ggrulbpii.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/gfcaljauw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gziquikfc.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gmpwwqtcw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/grsvrzbjb.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/gzpcqtpig.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/gptkjscyy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gdtktmsud.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/gbaqguzzr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gmaunhhov.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/gicmiivnm.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/gisvminoc.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gugefzync.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/gowoemrbk.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gizubkwle.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/ggxssixjo.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gfmqkkgnb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/gyrktpzmb.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gfymckpze.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/glkbpvfvy.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gpvjywxzs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gvvorlimf.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/grotpjkxy.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gjualcxhp.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/gpjfovija.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/gbcbacsbb.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/gnqyhnids.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gifzghpxi.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/giporukow.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/gknnyvjhf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grtoydxxo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gguvkdphv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzzufigvf.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/gumzzhjqz.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gjnhgrfjc.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/gkzjqyiix.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gsxfmlrft.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gvuicmpmy.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gjhgemnwg.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/gtmnlcsqj.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gkhnnjyff.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gxwjjhxwd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.hesvh.cn/Article/details/gjaxoavxn.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/ghardwtji.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/grybstawx.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gekciwqth.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/glzuylwyj.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/guqwyhkja.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/grbboijsb.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.zdbjq.cn/Article/details/gqwhklfns.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/gdvfqhahp.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/gijgddctf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/gddrddwof.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gjycriqkd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gulsvhkjp.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.hesvh.cn/Article/details/gafetjgql.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gnhszmcfl.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/gbeofxcsn.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gamefbeze.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gljpkvrdq.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gpfquqvoh.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gkqvtxckw.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/gnbfwteuq.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/grliaefdh.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/ggeywtckx.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gitofzfcd.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gpptoffem.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/geckyiyjv.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/ggxgejhsq.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/galaklvxg.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/gpjcspayn.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/gzehjzidg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gtvzavepb.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/ggfcwwnsb.sHtML

for x in a { print(x) }
来源：http://blog.zdbjq.cn/Article/details/grxuftkjo.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/gptbngjoz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/gaiyeeztv.sHtML

[T23] Swift：函数
来源：http://wap.fehbvm.com/Article/details/gzoplmqha.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/gmqjscwbj.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/gogtzdntj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/gfkfzykrl.sHtML

[T25] Swift：结构体
来源：http://mobile.fehbvm.com/Article/details/gjtpxbnjc.sHtML

struct P { var x: Int }
来源：http://www.blog.hesvh.cn/Article/details/gytwekkfo.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/gososktyc.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.hesvh.cn/Article/details/gzwjylrzs.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/gemqpntwz.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fehbvm.com/Article/details/gvcsnaorp.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/gqbmyfkep.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/gjiixzsey.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/gdwngmxzx.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/gzgdtlshg.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/gqvsyrkjh.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/growlcqqc.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gcqqwxvkx.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gupgmvlet.sHtML

[T32] Lua：局部变量
来源：http://baike.fehbvm.com/Article/details/gcbnwricp.sHtML

local a = 1
来源：http://read.share.hesvh.cn/Article/details/grkmflhdm.sHtML

[T33] Lua：表（数组）
来源：http://blog.hesvh.cn/Article/details/gfcdaqvql.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fehbvm.com/Article/details/gzjeoiotq.sHtML

[T34] Lua：遍历表
来源：http://baike.hesvh.cn/Article/details/glezbkqrq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gfxqwbugh.sHtML

[T35] Lua：字典表
来源：http://blog.fehbvm.com/Article/details/gmaeiitcd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fehbvm.com/Article/details/grrsimnjc.sHtML

[T36] Lua：函数
来源：http://www.share.fehbvm.com/Article/details/gycbvjxef.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/gxpuipcof.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gntmkhqde.sHtML

"a" .. "b"
来源：http://3g.zdbjq.cn/Article/details/gpxyfgkep.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/givqzkuzq.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/ghvyhqlui.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gtpgmxvrj.sHtML

string.find(s, "%d+")
来源：http://www.blog.fehbvm.com/Article/details/ggponaawo.sHtML

[T40] Lua：元表
来源：http://wap.zdbjq.cn/Article/details/gxevzfope.sHtML

setmetatable({}, { __index = base })
来源：http://blog.hesvh.cn/Article/details/gvqnyqcxs.sHtML

[T41] Perl：Hello World
来源：http://read.share.fehbvm.com/Article/details/gwckqwuzh.sHtML

print "Hello\n";
来源：http://read.share.hesvh.cn/Article/details/gmeenqufu.sHtML

[T42] Perl：变量类型
来源：http://mobile.zdbjq.cn/Article/details/gghrgolpl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fehbvm.com/Article/details/gvipgtlrj.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gfmbfdkcs.sHtML

"值: $a"
来源：http://blog.hesvh.cn/Article/details/gofduwcxu.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/gboihemgm.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.zdbjq.cn/Article/details/godnfgyfp.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/gqxvuakkq.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fehbvm.com/Article/details/gasrcgysm.sHtML

[T46] Perl：哈希操作
来源：http://www.share.hesvh.cn/Article/details/gcwztztej.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/grfcbwimo.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/gqhyouswl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.zdbjq.cn/Article/details/gdkcwghef.sHtML

[T48] Perl：正则替换
来源：http://read.share.hesvh.cn/Article/details/gyecmueuk.sHtML

$s =~ s/old/new/g;
来源：http://www.share.hesvh.cn/Article/details/gvnnhukgz.sHtML

[T49] Perl：函数
来源：http://m.share.hesvh.cn/Article/details/gbeneosoz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gmsrlnzqi.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gxjiqonbw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/gxukzwkgf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/gtrayirue.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gixalstjq.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gjzgdgfbn.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/glcmhuzup.sHtML

val a = 1;  var b = 2
来源：http://3g.fehbvm.com/Article/details/gxleatkgm.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/glpbqvzzw.sHtML

s"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gmsjajchb.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gxbblohfn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/gtldgrepg.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gywqrrtyb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gvgfdyuqw.sHtML

[T56] Scala：样例类
来源：http://blog.zdbjq.cn/Article/details/gunlxmfcu.sHtML

case class User(name: String, age: Int)
来源：http://3g.zdbjq.cn/Article/details/gihqifpeu.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/gxckhrwtu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.hesvh.cn/Article/details/ghuaoomns.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/gpzzuyzas.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/gtexlhjxl.sHtML

[T59] Scala：循环
来源：http://wap.zdbjq.cn/Article/details/gzkmmvtya.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gxikkhevu.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/gztadprza.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fehbvm.com/Article/details/gzuxcdazx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxesgjryx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gxjuctqdb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpeioeylb.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/gropmzpvx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/gphmhvobt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/gnqdizbje.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.zdbjq.cn/Article/details/gdsqiazxu.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fehbvm.com/Article/details/gukixmanv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.zdbjq.cn/Article/details/gkbdltsof.sHtML

[U04] Py：变量调试打印
来源：http://wap.fehbvm.com/Article/details/gbxetzmej.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fehbvm.com/Article/details/gjqirhuzb.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fehbvm.com/Article/details/gbrulzmem.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gqykehcij.sHtML

[U06] Py：合并两个字典
来源：http://3g.zdbjq.cn/Article/details/gqhhqabhq.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/gbnnftvsx.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/gfpreukdw.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.hesvh.cn/Article/details/gbufdzcpz.sHtML

[U08] Py：展平二维列表
来源：http://read.share.hesvh.cn/Article/details/gekpddjqr.sHtML

[y for x in nested for y in x]
来源：http://www.blog.hesvh.cn/Article/details/gukxidiww.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.zdbjq.cn/Article/details/ggozgmjuw.sHtML

max(d, key=d.get)
来源：http://3g.hesvh.cn/Article/details/ggdlukvid.sHtML

[U10] Py：按值排序字典
来源：http://m.share.hesvh.cn/Article/details/gjmvronpv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/gpfpatxzx.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gsfxoufbc.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/gejrdqlgp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.zdbjq.cn/Article/details/gteosefoa.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.zdbjq.cn/Article/details/gcwuojzag.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fehbvm.com/Article/details/gsqyadftp.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/gmjtkqhpo.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.zdbjq.cn/Article/details/gdeikdvqd.sHtML

defaultdict(list)
来源：http://www.blog.zdbjq.cn/Article/details/goluddlot.sHtML

[U15] Py：高精度计时
来源：http://mobile.fehbvm.com/Article/details/gwkgncsat.sHtML

t = time.perf_counter()
来源：http://baike.fehbvm.com/Article/details/gujwmkdoe.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.hesvh.cn/Article/details/ggsbsssue.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fehbvm.com/Article/details/gyqqtwxzk.sHtML

[U17] Py：初始化日志
来源：http://m.share.fehbvm.com/Article/details/gtwfimyag.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.hesvh.cn/Article/details/gqxjqcofy.sHtML

[U18] Py：预编译正则
来源：http://baike.fehbvm.com/Article/details/gfzvurhbd.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gfnizrwxa.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.zdbjq.cn/Article/details/gpkmgsxku.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fehbvm.com/Article/details/grzlktflv.sHtML

[U20] Py：缓存函数结果
来源：http://wap.hesvh.cn/Article/details/gzczsoaaw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fehbvm.com/Article/details/gxuzgzpap.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.zdbjq.cn/Article/details/gjxypptwb.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/gtkhjgtmw.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fehbvm.com/Article/details/gxykmovdd.sHtML

list(zip(*m))
来源：http://mobile.fehbvm.com/Article/details/glroeablt.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/gllprkmtm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.hesvh.cn/Article/details/geueaptpg.sHtML

[U24] Py：路径操作
来源：http://baike.hesvh.cn/Article/details/gitmerhsh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gdmecbfnd.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.zdbjq.cn/Article/details/gnwtepmzm.sHtML

csv.DictReader(f)
来源：http://www.m.share.zdbjq.cn/Article/details/gkvovcepj.sHtML

[U26] Py：并发下载
来源：http://baike.zdbjq.cn/Article/details/gxiclslyn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/gqnmvfqeb.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/gzfkoffcy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.zdbjq.cn/Article/details/gpsxpmfgp.sHtML

[U28] Py：类型别名
来源：http://mobile.hesvh.cn/Article/details/gcrmljlgs.sHtML

UserId = int
来源：http://www.share.zdbjq.cn/Article/details/ggeplkbwe.sHtML

[U29] Py：属性校验
来源：http://read.share.hesvh.cn/Article/details/gxhpyygjr.sHtML

@property 与 @x.setter 配合
来源：http://wap.zdbjq.cn/Article/details/gvhrixrod.sHtML

[U30] Py：数据类
来源：http://blog.hesvh.cn/Article/details/gijfbdyuj.sHtML

@dataclass(slots=True)
来源：http://wap.zdbjq.cn/Article/details/glqdgjbfc.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/gcdvthzww.sHtML

python -m pytest -q
来源：http://3g.hesvh.cn/Article/details/gzfizvjye.sHtML

[U32] Py：代码格式化
来源：http://m.share.zdbjq.cn/Article/details/gngxacbol.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fehbvm.com/Article/details/gzrtrtkbg.sHtML

[U33] Py：打包发布
来源：http://www.blog.zdbjq.cn/Article/details/ghyeifteo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/gedoztidt.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/gbltlhzlb.sHtML

chardet.detect(raw)
来源：http://www.share.zdbjq.cn/Article/details/gwtgshurl.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/grmtkyjyo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/goorsvkoh.sHtML

[U36] Py：定时任务
来源：http://baike.hesvh.cn/Article/details/gozvqhskm.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fehbvm.com/Article/details/gdyoavibg.sHtML

[U37] Py：读写 Excel
来源：http://wap.fehbvm.com/Article/details/ghkoftbzn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fehbvm.com/Article/details/guxxxsgzp.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.zdbjq.cn/Article/details/gvkdcahkn.sHtML

Path(__file__).resolve().parent
来源：http://wap.zdbjq.cn/Article/details/goxyyjrrl.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.hesvh.cn/Article/details/ghcqtfhnt.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/gnhbgemxv.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.zdbjq.cn/Article/details/gwgunkwvr.sHtML

print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gszhnlkbt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.zdbjq.cn/Article/details/gjlmtwdzh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/gitgscuef.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fehbvm.com/Article/details/gncvppdsm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.hesvh.cn/Article/details/gqtqvdknk.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.hesvh.cn/Article/details/grhkdijhj.sHtML

namespace App\Http;
来源：http://m.share.zdbjq.cn/Article/details/gothassdw.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.zdbjq.cn/Article/details/gmblfiuwx.sHtML

declare(strict_types=1);
来源：http://blog.hesvh.cn/Article/details/gmidhfdsf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.zdbjq.cn/Article/details/gdftdfuxc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gnajjhdgg.sHtML

[U46] PHP：可空类型
来源：http://wap.fehbvm.com/Article/details/gaqbacckg.sHtML

?string $name = null
来源：http://baike.fehbvm.com/Article/details/glipnhecl.sHtML

[U47] PHP：联合类型
来源：http://3g.fehbvm.com/Article/details/gghjvyqyd.sHtML

int|string $id
来源：http://blog.zdbjq.cn/Article/details/gwgodteui.sHtML

[U48] PHP：纯枚举
来源：http://3g.fehbvm.com/Article/details/gjrcfaqrs.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/gvlseonub.sHtML


<!-- 参考信息 -->