代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gkocsqcam.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/gwejghcxk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gasjgewpp.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gcwopziap.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/gynrzwtyj.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gjcisrpvb.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gjrlxeumv.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gdjrcnozx.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/gjetafznm.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gbhycrwih.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/ggozgkivz.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/ggybxlrag.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gfheasfns.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gzoezipgz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gcdyjigda.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gadiyorrl.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gxdvpthcy.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gjavpwlum.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/glrsnjwms.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gjxlnlnub.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/gcmxpywiw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gretohfwz.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/ghkohvpsp.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gbiyptzdh.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/gnxmrknqj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/gzjwsafop.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/glkwinvoc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/geewabzbv.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gibuahgsj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/grkdsuyvo.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/genpzxuut.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/ghnxkkjyy.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/gxcjuvpnv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/geifhuvzi.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/gsumdtqhz.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/gblhkxyvy.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/gddrvmnfp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gjeboopoz.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gaqmxfdfd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/gxahjaqax.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/gjyqarxqm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gmnrvdbrt.sHtML

[S42] C++：继承与虚函数
来源：http://blog.zdbjq.cn/Article/details/grrlowafs.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/griibyzjm.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gfolockkx.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/gsojlgnpx.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gyzcuxalp.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/ggpnmdesg.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/gjkhusqui.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gwtnzylhx.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/gsdixfqwf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gymqjwxbq.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/galztteiu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/gpdqoansw.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gbdpznrsq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gldynlzsv.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/guvlzitzk.sHtML

[S49] C++：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gwwxuqqlt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gxnewemej.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/gchutfnlz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/guvcrkdcm.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/grtnogler.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gvvwinbng.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/goclgppeu.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/gvjituqew.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/gdurjepeu.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/ghzojebpy.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/gngvkxggf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/gpiuhydsq.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/glcnbdnxk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.hesvh.cn/Article/details/ggxlfqnah.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/grergzrrh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gmgzynooh.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/gtptzlaom.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/gevifyphy.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/grhbiizfk.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.hesvh.cn/Article/details/giyvpbkgo.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/gvqkbcwtn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/gvqizyroj.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/gbnnnmwql.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gldiijkog.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grqcaiuyi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/goknlqafa.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxijguwth.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/gjnwlilke.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gxvdsvbkh.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gyuyywmqm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gyxmyaqwr.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/gjqzergoa.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/gvbyvennp.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/gjylqiwrq.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/gmfqgghab.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/gfzacabiu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/gtsdaytsp.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/gfzyzkaoh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/gigehuvkf.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/gdnopwfwa.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/gjplifhxh.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/gxivuozfe.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gzppzzzow.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/ggsnzalpp.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/gvlifcwek.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/gqvccmanq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/gdapweurg.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gjighsbpd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fehbvm.com/Article/details/ghhhoawtg.sHtML

[T12] Kotlin：解构声明
来源：http://3g.zdbjq.cn/Article/details/gxfyflmwc.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gzluazlhd.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/gxusljwsd.sHtML

val m = mapOf("a" to 1)
来源：http://baike.hesvh.cn/Article/details/gkqccdbhi.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gkxbboqeu.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/gacpzqesw.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/ggndwlzrs.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gordhnqqm.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gpxficavo.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/ggsgrphsf.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gkxjzvdwo.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/gunhzzaqj.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/grcrdfxgi.sHtML

"值: \(b)"
来源：http://baike.hesvh.cn/Article/details/gubjgzrjx.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gzojchuer.sHtML

if let n = opt { print(n) }
来源：http://m.share.fehbvm.com/Article/details/gszwhbgfl.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/gtwlqyvvj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/ghxwpyqjr.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gcqvwjdoi.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/gnykqtvnq.sHtML

[T22] Swift：字典
来源：http://baike.fehbvm.com/Article/details/ggnqqolfx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gyvsgmxcx.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/gpqaljvwc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/grzwbrsbv.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/gyjceigfp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/ghonvrppu.sHtML

[T25] Swift：结构体
来源：http://baike.fehbvm.com/Article/details/gdnuyocsx.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gjecslotv.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/gzqpufujq.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/gbsguowtd.sHtML

[T27] Swift：错误处理
来源：http://baike.zdbjq.cn/Article/details/gvetwftho.sHtML

do { try f() } catch { print(error) }
来源：http://3g.zdbjq.cn/Article/details/ggwqvxvjp.sHtML

[T28] Swift：枚举
来源：http://3g.zdbjq.cn/Article/details/gdperzksg.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/ggpkdvcyz.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/ghtzorynm.sHtML

guard let x = opt else { return }
来源：http://baike.hesvh.cn/Article/details/ghegrzvmq.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/gfflrbnjn.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/gtvmkyshn.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gvsrejqkh.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/ghjwgefug.sHtML

[T32] Lua：局部变量
来源：http://blog.hesvh.cn/Article/details/gsomoixwr.sHtML

local a = 1
来源：http://3g.hesvh.cn/Article/details/gulrsqsqa.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/gsezlnwig.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fehbvm.com/Article/details/glmjqimgk.sHtML

[T34] Lua：遍历表
来源：http://www.blog.zdbjq.cn/Article/details/ggoirheeh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gklwdutfb.sHtML

[T35] Lua：字典表
来源：http://3g.fehbvm.com/Article/details/gkcgktgdz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/gakqbyilg.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/glpcmrhul.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fehbvm.com/Article/details/gzcugghrc.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.hesvh.cn/Article/details/grxxhddxv.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/gynyngqqg.sHtML

[T38] Lua：条件
来源：http://3g.zdbjq.cn/Article/details/grncnzluv.sHtML

if x > 0 then print("正") end
来源：http://m.share.zdbjq.cn/Article/details/ghtffjfrn.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gzewflzfg.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/gckrmgdql.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/ggowjakvt.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/gstfpejbo.sHtML

[T41] Perl：Hello World
来源：http://baike.fehbvm.com/Article/details/grzidkeuo.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/goywaxppy.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gzatwxztt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fehbvm.com/Article/details/gklxtiygi.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gzxyzblgz.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/guzfywfjz.sHtML

[T44] Perl：条件
来源：http://www.blog.hesvh.cn/Article/details/gvxdgqmcz.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/gtaywcnjc.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/gjpjtdsmc.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/godqfbevk.sHtML

[T46] Perl：哈希操作
来源：http://wap.zdbjq.cn/Article/details/gonbwithb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.zdbjq.cn/Article/details/gcjggjnka.sHtML

[T47] Perl：正则捕获
来源：http://blog.fehbvm.com/Article/details/gmvqlesjg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/gxdozwtbz.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/gwdmdndto.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gasowljid.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/gurapoeaf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gjcvrtqlh.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gfxoqmyqn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/grbcuwgln.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.zdbjq.cn/Article/details/gmzcfnfix.sHtML

[T51] Scala：Hello World
来源：http://wap.hesvh.cn/Article/details/goepsirna.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gjxxmqdge.sHtML

[T52] Scala：变量
来源：http://www.share.fehbvm.com/Article/details/ghdlzcjut.sHtML

val a = 1;  var b = 2
来源：http://mobile.hesvh.cn/Article/details/gmipxotdw.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gycfcrkpk.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/gyzqsourg.sHtML

[T54] Scala：集合映射
来源：http://www.share.hesvh.cn/Article/details/ghetbeppt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fehbvm.com/Article/details/gdsxmbkmc.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gemstwtgi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/gnqnwrloo.sHtML

[T56] Scala：样例类
来源：http://mobile.hesvh.cn/Article/details/gzpdyaxss.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/gikrexjwp.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gpmcnhneh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gkpegoizs.sHtML

[T58] Scala：函数定义
来源：http://www.share.fehbvm.com/Article/details/gvkwepimr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.zdbjq.cn/Article/details/gbystrhjn.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/gsqoymuad.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gdcowpatw.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/gybbkuyux.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.hesvh.cn/Article/details/gmiukqdxt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpluebirt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/gtygtxrty.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grwxdioho.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.zdbjq.cn/Article/details/gqhnrekdz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gcmamqafb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/gowzhjdus.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.hesvh.cn/Article/details/gxfdwnayv.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/gisyxekej.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.zdbjq.cn/Article/details/gnovggrbe.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/gjhzudxxr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.hesvh.cn/Article/details/gqqucdhzj.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fehbvm.com/Article/details/grdjrzwgj.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gihoygwfg.sHtML

[U06] Py：合并两个字典
来源：http://baike.hesvh.cn/Article/details/ghthecyvr.sHtML

{**a, **b}
来源：http://m.share.zdbjq.cn/Article/details/gorkzvvnm.sHtML

[U07] Py：反转字典键值
来源：http://3g.zdbjq.cn/Article/details/ghmvewozl.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fehbvm.com/Article/details/gugkiguqe.sHtML

[U08] Py：展平二维列表
来源：http://mobile.hesvh.cn/Article/details/gdmphpdbq.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/grqsbcaaf.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fehbvm.com/Article/details/gcwpeueyi.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/ggalxeaye.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/gdkjcdygx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.hesvh.cn/Article/details/gaiijrnmd.sHtML

[U11] Py：生成器表达式
来源：http://baike.fehbvm.com/Article/details/giiujmgnv.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/grkbltswe.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fehbvm.com/Article/details/gijaniptw.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/gtqbymngi.sHtML

[U13] Py：固定长度队列
来源：http://read.share.hesvh.cn/Article/details/grigqgqwy.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/gsfhfzccj.sHtML

[U14] Py：分组收集到列表
来源：http://blog.zdbjq.cn/Article/details/gmikajrmv.sHtML

defaultdict(list)
来源：http://www.blog.fehbvm.com/Article/details/grkqyqocy.sHtML

[U15] Py：高精度计时
来源：http://mobile.fehbvm.com/Article/details/gtpndlbtf.sHtML

t = time.perf_counter()
来源：http://www.m.share.fehbvm.com/Article/details/ggnhloatp.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fehbvm.com/Article/details/gsdpcprdn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fehbvm.com/Article/details/gfuditdxn.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fehbvm.com/Article/details/gaeedzpok.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fehbvm.com/Article/details/gkugdpuqk.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/givvlvbkf.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fehbvm.com/Article/details/gwzdyugmn.sHtML

[U19] Py：正则替换带回调
来源：http://baike.zdbjq.cn/Article/details/ggwsetvqi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.hesvh.cn/Article/details/gxylysatx.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.zdbjq.cn/Article/details/guoxeyhke.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.hesvh.cn/Article/details/ggzpjshdy.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.hesvh.cn/Article/details/gkuztsexw.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/ggujvglhb.sHtML

[U22] Py：矩阵转置
来源：http://blog.zdbjq.cn/Article/details/gvjqvxmur.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/gtyfbqrxi.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.zdbjq.cn/Article/details/ghtfzqjul.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/gahawmbwq.sHtML

[U24] Py：路径操作
来源：http://m.share.zdbjq.cn/Article/details/ghncvdzbd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/guaukbvry.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fehbvm.com/Article/details/geuopgdxu.sHtML

csv.DictReader(f)
来源：http://blog.hesvh.cn/Article/details/gplpmnfjq.sHtML

[U26] Py：并发下载
来源：http://www.blog.fehbvm.com/Article/details/giugwacir.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/gnyejmybs.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.zdbjq.cn/Article/details/gbywexgba.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fehbvm.com/Article/details/gqsqgaavf.sHtML

[U28] Py：类型别名
来源：http://www.blog.zdbjq.cn/Article/details/gbjsdvgei.sHtML

UserId = int
来源：http://mobile.fehbvm.com/Article/details/gsqpnnkoh.sHtML

[U29] Py：属性校验
来源：http://m.share.hesvh.cn/Article/details/ggciltmdp.sHtML

@property 与 @x.setter 配合
来源：http://read.share.hesvh.cn/Article/details/gqajapzse.sHtML

[U30] Py：数据类
来源：http://3g.fehbvm.com/Article/details/gxahdazpk.sHtML

@dataclass(slots=True)
来源：http://m.share.zdbjq.cn/Article/details/gbqfxegac.sHtML

[U31] Py：单测
来源：http://baike.fehbvm.com/Article/details/gbvsnxmfm.sHtML

python -m pytest -q
来源：http://www.blog.hesvh.cn/Article/details/gqcqdbrmo.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.hesvh.cn/Article/details/gktuoccqp.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/gxrqiimgr.sHtML

[U33] Py：打包发布
来源：http://baike.zdbjq.cn/Article/details/gnwrwvanx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.zdbjq.cn/Article/details/gxefmhqqp.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/gxpwuqjxg.sHtML

chardet.detect(raw)
来源：http://baike.hesvh.cn/Article/details/gtmxzzrdb.sHtML

[U35] Py：发送邮件
来源：http://wap.fehbvm.com/Article/details/gwaqurygk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/gwkezbxdm.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/gddxifppb.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fehbvm.com/Article/details/gzzpiqmff.sHtML

[U37] Py：读写 Excel
来源：http://wap.hesvh.cn/Article/details/gkwxsvvag.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gkoaynlpr.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fehbvm.com/Article/details/gmrelpdwy.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/gbzymwppl.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.hesvh.cn/Article/details/gjmqekulw.sHtML

sys.stdout.isatty()
来源：http://wap.hesvh.cn/Article/details/gdlukpggx.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.zdbjq.cn/Article/details/guxzsqczs.sHtML

print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gubjeenbn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fehbvm.com/Article/details/gywjnrxwp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.zdbjq.cn/Article/details/gnpkkgfiz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/gnbpbonvv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.hesvh.cn/Article/details/gtwlmnzzv.sHtML

[U43] PHP：声明命名空间
来源：http://baike.hesvh.cn/Article/details/gzrhhqnms.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/gpnsogvhe.sHtML

[U44] PHP：开启严格类型
来源：http://wap.hesvh.cn/Article/details/gdsiemluw.sHtML

declare(strict_types=1);
来源：http://read.share.fehbvm.com/Article/details/giyigyikq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.hesvh.cn/Article/details/gfcwbrjle.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gbjqqfkqn.sHtML

[U46] PHP：可空类型
来源：http://m.share.zdbjq.cn/Article/details/gdpnexyii.sHtML

?string $name = null
来源：http://www.share.hesvh.cn/Article/details/glnfssnml.sHtML


<!-- 参考信息 -->