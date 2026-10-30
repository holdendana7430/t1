代发 wailian999

int main(int argc, char **argv)
来源：http://blog.hesvh.cn/Article/details/gjrujnsqv.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gzewodoek.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gtdwylzjw.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/gplrnyjzz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gbjlbxwtm.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/gqtqgimrr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gopumbdpy.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/gigkndjfv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/gubtruzbr.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gutdahjhd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/gfghwhwbd.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gpbwqojxp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/ghyrgdwdn.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/gpmuhqvvv.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gyinldtgb.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gyfutpkpa.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/goxlsxocl.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/gokzuhdse.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gblefveuh.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gxlefjysr.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gnxrpcfju.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/gvpcpnvya.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gvjihsovm.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gyeqewulu.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gqhgbexyq.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gohtgrwby.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gtzselblq.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/ghqqmviqd.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/gdrrxfaej.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gqysazxfk.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/glqftzzar.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gcovscojo.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gvbksyucg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/glqaqgvpz.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/gcnwbkvis.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/girvuscpz.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gbvvmwepy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gymioxpkm.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/gxsvxqtup.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gbcfqggaq.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gntfujkhn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gofxgeyad.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gurxkndff.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/gcuxsjpqe.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gcvthbqqw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gczbrtynf.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/gdebcpreb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gkyrpvyyc.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/ghnqfpgqc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gjejvpxfm.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gjucjykor.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fehbvm.com/Article/details/gpqpoclle.sHtML

[S43] C++：智能指针
来源：http://baike.zdbjq.cn/Article/details/ghvwtzqpb.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gbazqlerp.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gajfxeogq.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gmfeaeieq.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/ghoxpfjlc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/ghgvsfmit.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/gqjinqkyi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gsgikixyq.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/gzbvbydkw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/guqvdaait.sHtML

[S48] C++：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gzwwkmflp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gnzkynjez.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/gufwykzoi.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gnpofvwtq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/gactidylb.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gpxhnjpub.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gndnuaxct.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/gubafqlwn.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/gjikfievb.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/ghqciuavj.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/gapmkanwq.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gpnysegcq.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/ghrxksqfm.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gjysntebn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gfowsxmet.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gruvxxyox.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.hesvh.cn/Article/details/gifjmxfxy.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gevjdybny.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gjtnzojys.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/gqapxqazy.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gjbnloufa.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gnkylkzto.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/gilbhofzk.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/gtvotbyha.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/gqnoamqjy.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/gbsrwzvbb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/gzivmephl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwattwavv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gkavquksz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gutccsqtf.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/gfooabyrt.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/ghwonzyjr.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/gopjcwmsm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/gamgqbohn.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/gtnrvvsfj.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gaxemhcvc.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/glbvbwsvx.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/gmhyeaytq.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/geunvzqan.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/ghelzwdyq.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gzvmqkgpv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gyfvdcvzb.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gelpklwor.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/gxdipxoko.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/grkxhvdyr.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gextnweto.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/gwujljfev.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/gtaoshlcx.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/girpzibly.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/gvrswmiel.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gomakqrak.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/getlficxz.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/gmourvyat.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/gfnydtbcg.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.zdbjq.cn/Article/details/ghiaxawbe.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gxmydhmqn.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gollnplxm.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gakuzevab.sHtML

[T15] Kotlin：接口
来源：http://wap.fehbvm.com/Article/details/gvqpeftpq.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fehbvm.com/Article/details/gelsstdaj.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gxcysgrks.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/ggviyeagn.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/guxqthozp.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gxxtkbsgs.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gcrmezdug.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/golainmxd.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gifvrysna.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/ghtmykkyl.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/goctrnnbc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gcnwddubm.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/gqfsbwqep.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/grfthzpow.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/gfyqafsqt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/gqmmrbhng.sHtML

[T23] Swift：函数
来源：http://m.share.zdbjq.cn/Article/details/gyknznjhu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fehbvm.com/Article/details/gnuhohocr.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/gjsdqqonw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gvqjtckxb.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/gsgzhqvil.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/gfeinvpun.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/grlxjmakm.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/gkywuslio.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gxbplecwr.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fehbvm.com/Article/details/gydnlivgw.sHtML

[T28] Swift：枚举
来源：http://3g.fehbvm.com/Article/details/gbqtkvhqm.sHtML

enum Color { case red, green }
来源：http://www.blog.hesvh.cn/Article/details/grjcuvaar.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gqpceklua.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/gkojappnw.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/glslqwpas.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/gmypeclmz.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gywtvlewd.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gplpcirps.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/gdsgdyvgx.sHtML

local a = 1
来源：http://www.m.share.hesvh.cn/Article/details/ghetobivz.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/goeztyuqb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.zdbjq.cn/Article/details/gupgwcmch.sHtML

[T34] Lua：遍历表
来源：http://www.share.fehbvm.com/Article/details/gkngokltt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.zdbjq.cn/Article/details/gdkghkiuw.sHtML

[T35] Lua：字典表
来源：http://www.share.fehbvm.com/Article/details/gapivhcju.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.zdbjq.cn/Article/details/gxoydosiq.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/gydmmgyza.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/gaolkwwuf.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gxyvaxjax.sHtML

"a" .. "b"
来源：http://www.m.share.zdbjq.cn/Article/details/ggmektwoq.sHtML

[T38] Lua：条件
来源：http://read.share.fehbvm.com/Article/details/gxedensjx.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/gvwuzhgml.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/goaplwcqo.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gxgorwcbj.sHtML

[T40] Lua：元表
来源：http://blog.fehbvm.com/Article/details/gfvsqwtgm.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/gfoqydsqk.sHtML

[T41] Perl：Hello World
来源：http://www.share.fehbvm.com/Article/details/gmhrmicum.sHtML

print "Hello\n";
来源：http://www.blog.fehbvm.com/Article/details/gimombfhj.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/gpfdgfypm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.hesvh.cn/Article/details/goibdmzip.sHtML

[T43] Perl：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gtkjtbwca.sHtML

"值: $a"
来源：http://www.m.share.zdbjq.cn/Article/details/guxapklpe.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/gweaxbgda.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/gswvqnscc.sHtML

[T45] Perl：数组遍历
来源：http://read.share.hesvh.cn/Article/details/gdvczyguy.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.zdbjq.cn/Article/details/gydqopvwy.sHtML

[T46] Perl：哈希操作
来源：http://3g.zdbjq.cn/Article/details/glpctqbqc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fehbvm.com/Article/details/gkfguasro.sHtML

[T47] Perl：正则捕获
来源：http://m.share.hesvh.cn/Article/details/gwvywgfta.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/gdgnksdfi.sHtML

[T48] Perl：正则替换
来源：http://read.share.hesvh.cn/Article/details/ggskynuoq.sHtML

$s =~ s/old/new/g;
来源：http://read.share.hesvh.cn/Article/details/gchbcozqa.sHtML

[T49] Perl：函数
来源：http://m.share.hesvh.cn/Article/details/gfrglwgou.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gugtaetlq.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gflrocjjq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/gykqfuexu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/gnxqncllp.sHtML

[T51] Scala：Hello World
来源：http://blog.fehbvm.com/Article/details/gvrfbtopo.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gqudrggle.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/gyrmxuuqh.sHtML

val a = 1;  var b = 2
来源：http://mobile.hesvh.cn/Article/details/gmxtwktag.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gskifovtd.sHtML

s"值: $b"
来源：http://wap.hesvh.cn/Article/details/gbycjgsql.sHtML

[T54] Scala：集合映射
来源：http://3g.hesvh.cn/Article/details/gwxlvsqjn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.hesvh.cn/Article/details/graxyskmk.sHtML

[T55] Scala：集合过滤
来源：http://blog.fehbvm.com/Article/details/gwetdigam.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gphrrcmjv.sHtML

[T56] Scala：样例类
来源：http://baike.zdbjq.cn/Article/details/gesbehqcy.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gvnzonnzx.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/gmsjxxzir.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gxqfndgsl.sHtML

[T58] Scala：函数定义
来源：http://read.share.zdbjq.cn/Article/details/ghpxlbtwj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.hesvh.cn/Article/details/gwfxgkovj.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/gzhncjlid.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gegvohgrr.sHtML

[T60] Scala：折叠
来源：http://m.share.fehbvm.com/Article/details/giejbqgas.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.hesvh.cn/Article/details/ggzwdstvi.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/guzmbkksw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/grqevprac.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcjwqfhml.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/gtufjowjt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.hesvh.cn/Article/details/gnbbocyog.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.zdbjq.cn/Article/details/goyvtgmur.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.zdbjq.cn/Article/details/gaouazinb.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/ghvkwjeqa.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/gkusefghu.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/gcgwzmnlw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.hesvh.cn/Article/details/gwlyuwxgz.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/gpsuenvdg.sHtML

list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gcukelbur.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fehbvm.com/Article/details/ggwqxjotz.sHtML

{**a, **b}
来源：http://m.share.hesvh.cn/Article/details/gqcoqqaig.sHtML

[U07] Py：反转字典键值
来源：http://baike.hesvh.cn/Article/details/gofzqckki.sHtML

{v: k for k, v in d.items()}
来源：http://3g.hesvh.cn/Article/details/gezhedgyb.sHtML

[U08] Py：展平二维列表
来源：http://3g.fehbvm.com/Article/details/geyebeyjt.sHtML

[y for x in nested for y in x]
来源：http://3g.fehbvm.com/Article/details/gfxbuqlgm.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.hesvh.cn/Article/details/gxjgmgtfh.sHtML

max(d, key=d.get)
来源：http://m.share.zdbjq.cn/Article/details/gkzinzxss.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fehbvm.com/Article/details/gjwxxzvoy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fehbvm.com/Article/details/gpqzldkqe.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gzswaxlvs.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/gxcbnymry.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/gzeedyrgw.sHtML

Counter(arr).most_common(3)
来源：http://wap.hesvh.cn/Article/details/gwfxiwehs.sHtML

[U13] Py：固定长度队列
来源：http://baike.hesvh.cn/Article/details/gxoqugahz.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/gymftfgmn.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.hesvh.cn/Article/details/gmmcpwlkp.sHtML

defaultdict(list)
来源：http://www.blog.hesvh.cn/Article/details/gcqznuzgr.sHtML

[U15] Py：高精度计时
来源：http://m.share.hesvh.cn/Article/details/ghrwjfytb.sHtML

t = time.perf_counter()
来源：http://blog.hesvh.cn/Article/details/grozlhyes.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fehbvm.com/Article/details/grcuffbmh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fehbvm.com/Article/details/giorhnesm.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.zdbjq.cn/Article/details/gzjkugsbh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/gcgoficfv.sHtML

[U18] Py：预编译正则
来源：http://3g.hesvh.cn/Article/details/gtgfpdzjz.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/geybbdbhl.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fehbvm.com/Article/details/gabdpmrio.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fehbvm.com/Article/details/gtxzxhnsp.sHtML

[U20] Py：缓存函数结果
来源：http://3g.zdbjq.cn/Article/details/glujojcci.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gzucyjkgp.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/ghbiqkovj.sHtML

@contextlib.contextmanager
来源：http://wap.fehbvm.com/Article/details/gkewcahqv.sHtML

[U22] Py：矩阵转置
来源：http://baike.fehbvm.com/Article/details/gszzxwggs.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/gwntlxegs.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.zdbjq.cn/Article/details/ghvrxrxpx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fehbvm.com/Article/details/gfxjytzuk.sHtML

[U24] Py：路径操作
来源：http://m.share.zdbjq.cn/Article/details/gbvxalwqc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/girazbmoq.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.hesvh.cn/Article/details/gvxfcjnog.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/gidpztvuv.sHtML

[U26] Py：并发下载
来源：http://www.share.zdbjq.cn/Article/details/gfbsnutqd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.zdbjq.cn/Article/details/gnoyibqcj.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fehbvm.com/Article/details/gjhjdgtjh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fehbvm.com/Article/details/gkdurvoyw.sHtML

[U28] Py：类型别名
来源：http://m.share.hesvh.cn/Article/details/guqpfwqct.sHtML

UserId = int
来源：http://blog.zdbjq.cn/Article/details/gjffgitul.sHtML

[U29] Py：属性校验
来源：http://mobile.hesvh.cn/Article/details/gbdpeyoby.sHtML

@property 与 @x.setter 配合
来源：http://mobile.zdbjq.cn/Article/details/guokaptdf.sHtML

[U30] Py：数据类
来源：http://mobile.fehbvm.com/Article/details/gdewjcqax.sHtML

@dataclass(slots=True)
来源：http://3g.zdbjq.cn/Article/details/ggrqrvbga.sHtML

[U31] Py：单测
来源：http://mobile.fehbvm.com/Article/details/gxgixzuaf.sHtML

python -m pytest -q
来源：http://baike.fehbvm.com/Article/details/goslmwckx.sHtML

[U32] Py：代码格式化
来源：http://www.blog.zdbjq.cn/Article/details/ghuaccusd.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fehbvm.com/Article/details/gkzdlaxqj.sHtML

[U33] Py：打包发布
来源：http://baike.zdbjq.cn/Article/details/gfbabnxpw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.hesvh.cn/Article/details/gyeayihti.sHtML

[U34] Py：判断编码
来源：http://mobile.fehbvm.com/Article/details/gzowwjole.sHtML

chardet.detect(raw)
来源：http://m.share.fehbvm.com/Article/details/gstwionce.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/gwnaakrqa.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/gspgqbywq.sHtML

[U36] Py：定时任务
来源：http://m.share.zdbjq.cn/Article/details/gsiygdscf.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.zdbjq.cn/Article/details/grijllxpc.sHtML

[U37] Py：读写 Excel
来源：http://3g.fehbvm.com/Article/details/gtffwfwmi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.hesvh.cn/Article/details/gstmgsurc.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.hesvh.cn/Article/details/gtyaonwbe.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.zdbjq.cn/Article/details/gqxlteios.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.hesvh.cn/Article/details/gfdnuacxf.sHtML

sys.stdout.isatty()
来源：http://3g.zdbjq.cn/Article/details/gqopqhmnn.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.zdbjq.cn/Article/details/gmptrzhkx.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/guixyfdwe.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.zdbjq.cn/Article/details/gqihlqvyx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fehbvm.com/Article/details/gqmzwchri.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/ghdawbhng.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.zdbjq.cn/Article/details/gfbzxvptv.sHtML


<!-- 参考信息 -->