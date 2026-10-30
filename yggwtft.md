代发 wailian999

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/gjjxbznda.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gxjwnjgsr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/ggruwdzha.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gqagehatx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/garftchpw.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gmhxcpdsx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gsudcqogi.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gnvxugrxv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/guqvhhrqt.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/gwvwqlczb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gpluqnkfc.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/gwefenjyx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/gkxiptnae.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/gaxxnvksd.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/ghgxksxuy.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/gxxtxolcp.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gaaiwaaog.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/gewniqtyy.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/ghrupujue.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gyxjfyxin.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gialodsev.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/ghwfbjdgm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gdzybrbdz.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/gxddbvfhl.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/ghifmqjwz.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gpgznsqnn.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gduvkueyb.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/gmctpubcu.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/gwqzwjzkl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gakjtfcqv.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/ghpqfaskt.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/glpragqgk.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gbsujiclr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/gsyxvrucn.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gghjgmivx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gtunjmcfy.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/ghhegvghr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/goedqvpgc.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/gmssjnide.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/glzeyqdup.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gpztttwbg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gdezaxkyv.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gkgzckuvz.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gmnkzezmb.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/ghfluziml.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/grxxelisl.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gkfsrafhi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gazljfjzv.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/givkmkjqu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gnpfnhrmb.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gqsxajtmg.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gaqjsiqkc.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/gqocjvceb.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/gbsezmrkm.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gissaxwue.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/gkiernxou.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/geveavmnq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/gviceejff.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/gxszxhwit.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/gxgukymps.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gvvjfmhsi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fehbvm.com/Article/details/gvqexgjfp.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gtkljlogh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gxujqruhd.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/gwbrkkokp.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gfftqixat.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/gptkifbhh.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/gawhshbfw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gjyhjdqkt.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gigiwewhz.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/gvkvzetxu.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/gopmrfgnh.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gegjsecge.sHtML

[S53] C++：移动语义
来源：http://3g.hesvh.cn/Article/details/gatfvximy.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gsdkvtmsr.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gvjowjots.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/gmgunfxmb.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gxsxtcmgc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/gfdmlgjxn.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/gaswhgqxb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gjtizclxt.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/gxmpierkj.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/gsdhepeay.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gaxjtoqsj.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.zdbjq.cn/Article/details/gwuszxafv.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gvncjidek.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gynouaquo.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/gtvlmnmyn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gugqykynf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gacadpjbd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gqvhzikru.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnniyvzal.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gavxwzjiu.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gdxnivlzy.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gtxzeqezd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gwljyshvw.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/ghamcvzlz.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/grmjbzoyb.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/gpnsgmgxm.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gxenomvpj.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/gjsmnokch.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/gfvmuqunm.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gwwssvrip.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/gwtqhqctb.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/grviotryd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gorqfsaxf.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/gxbznggjy.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/gajnpsgvg.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.zdbjq.cn/Article/details/gtggvovmo.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/gtiojqctn.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gthgozlqz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gfuyzmkln.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/gdroyjrbv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/guyjockkw.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/guccthjme.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gdbtcucyp.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/gezskhcqg.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/glhwaxcxf.sHtML

[T14] Kotlin：循环
来源：http://read.share.fehbvm.com/Article/details/gwkinzawa.sHtML

for (i in 1..10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gbhaoueip.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gtxerklsw.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/gimkrtrit.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/goqmjodxx.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gdotqxoqu.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/ggowcwwfo.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/giakfnhun.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/giktxvvvf.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gonjzhjhw.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/glqbyvynn.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/gsvywegcf.sHtML

[T20] Swift：数组操作
来源：http://www.blog.hesvh.cn/Article/details/gmhpmgsjj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/gkrmssfxw.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/ggedcswsa.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/gckdnsrem.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/gutrgmlmm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/gfrqsjrug.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gwcuewrpp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/gunktlsll.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/gaqlwfarp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/gymyitztx.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/gqpolijss.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gtbisxdog.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gddbidgyg.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/gqahegafe.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/gnehnxumq.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.zdbjq.cn/Article/details/gduyfppne.sHtML

[T28] Swift：枚举
来源：http://3g.zdbjq.cn/Article/details/gpswoyici.sHtML

enum Color { case red, green }
来源：http://www.blog.zdbjq.cn/Article/details/gmgtmmorn.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.hesvh.cn/Article/details/gkggzemau.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gyykdeuft.sHtML

[T30] Swift：协议
来源：http://www.m.share.zdbjq.cn/Article/details/glkftsqug.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/gmcnlolvs.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gwqwddcqn.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gitkfelkp.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/ghwwsdlhl.sHtML

local a = 1
来源：http://read.share.hesvh.cn/Article/details/gvnagpuhu.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/ggmrpuzfs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/gofwvwfev.sHtML

[T34] Lua：遍历表
来源：http://www.blog.zdbjq.cn/Article/details/gflslcqst.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/gpkgvmcuj.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/gsavzfoau.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/gjwpjwvvc.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/gyrgxperg.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/gtqewuwkb.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gbewueljr.sHtML

"a" .. "b"
来源：http://m.share.hesvh.cn/Article/details/gercczzsm.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/gzaiiqikx.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/gslzijbin.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gwiicfuvs.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/gnceziaeu.sHtML

[T40] Lua：元表
来源：http://www.blog.hesvh.cn/Article/details/gfcwjlneg.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/gczizkqss.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/gpznbtmzq.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/gtjbbiafg.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gfsazssrz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.hesvh.cn/Article/details/gvbwdxqxq.sHtML

[T43] Perl：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gjokwugkv.sHtML

"值: $a"
来源：http://read.share.fehbvm.com/Article/details/gncmofntk.sHtML

[T44] Perl：条件
来源：http://3g.fehbvm.com/Article/details/gmvxanptu.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.hesvh.cn/Article/details/gxpidugzt.sHtML

[T45] Perl：数组遍历
来源：http://read.share.hesvh.cn/Article/details/glvitemvr.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.zdbjq.cn/Article/details/gamcnqlmm.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/gdhxleopx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/ghehbckdi.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/gvnntdqpz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/gwjzcrrtr.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/gxgknmavu.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/gvfupiwzz.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gxmuuxlkx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gijadekig.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gmslhkoof.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/gyguzgpme.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.hesvh.cn/Article/details/ggndpbvpw.sHtML

[T51] Scala：Hello World
来源：http://blog.zdbjq.cn/Article/details/gdobojjux.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gwtttgdid.sHtML

[T52] Scala：变量
来源：http://baike.hesvh.cn/Article/details/gzktzwsio.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/ggkasbien.sHtML

[T53] Scala：字符串插值
来源：http://baike.hesvh.cn/Article/details/gmafvblqw.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/grfydntwz.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gtaktqpny.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.hesvh.cn/Article/details/gmtqcarvp.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gwvamslrv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fehbvm.com/Article/details/gnihfqmrw.sHtML

[T56] Scala：样例类
来源：http://mobile.hesvh.cn/Article/details/gjreyhgey.sHtML

case class User(name: String, age: Int)
来源：http://baike.hesvh.cn/Article/details/gceiunuap.sHtML

[T57] Scala：模式匹配
来源：http://blog.fehbvm.com/Article/details/gnfssfmfw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.hesvh.cn/Article/details/gaxpebyrj.sHtML

[T58] Scala：函数定义
来源：http://read.share.fehbvm.com/Article/details/gcgrufdlz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/gjcehnnen.sHtML

[T59] Scala：循环
来源：http://read.share.fehbvm.com/Article/details/ghgfkgawd.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/giagaiezp.sHtML

[T60] Scala：折叠
来源：http://m.share.fehbvm.com/Article/details/gbpbacjea.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fehbvm.com/Article/details/gypykymrt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbkkrbvqi.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gnljovlnn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghfzsndtd.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/gynphtssu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/ghgxaeicl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/gbjlablnz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.zdbjq.cn/Article/details/gowmcpvbq.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.hesvh.cn/Article/details/ghrpkwfgs.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fehbvm.com/Article/details/gxjgxwzep.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gpjvujxdw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.zdbjq.cn/Article/details/gkjlsngfc.sHtML

[U05] Py：列表去重且保序
来源：http://baike.zdbjq.cn/Article/details/gzizzjxiv.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gqkgcmgsg.sHtML

[U06] Py：合并两个字典
来源：http://m.share.hesvh.cn/Article/details/gagrgodlf.sHtML

{**a, **b}
来源：http://baike.hesvh.cn/Article/details/gsojarnzm.sHtML

[U07] Py：反转字典键值
来源：http://wap.zdbjq.cn/Article/details/gwbunaioe.sHtML

{v: k for k, v in d.items()}
来源：http://3g.zdbjq.cn/Article/details/gwnljazuk.sHtML

[U08] Py：展平二维列表
来源：http://read.share.hesvh.cn/Article/details/gicqmhtrk.sHtML

[y for x in nested for y in x]
来源：http://www.share.zdbjq.cn/Article/details/gncjamkrd.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/gngzhugfc.sHtML

max(d, key=d.get)
来源：http://read.share.fehbvm.com/Article/details/ggzauwtmu.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/glmivaswg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fehbvm.com/Article/details/gdtgatcnm.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fehbvm.com/Article/details/gosptkqob.sHtML

(x * 2 for x in arr)
来源：http://blog.hesvh.cn/Article/details/gvlvrispw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/gemaiauje.sHtML

Counter(arr).most_common(3)
来源：http://www.share.zdbjq.cn/Article/details/gkkdurjps.sHtML

[U13] Py：固定长度队列
来源：http://www.share.zdbjq.cn/Article/details/gpxeuyggx.sHtML

deque(maxlen=10)
来源：http://baike.zdbjq.cn/Article/details/ghqihyhaj.sHtML

[U14] Py：分组收集到列表
来源：http://blog.hesvh.cn/Article/details/gjavaesqj.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/gntchtnlt.sHtML

[U15] Py：高精度计时
来源：http://baike.hesvh.cn/Article/details/gbnlryzas.sHtML

t = time.perf_counter()
来源：http://www.blog.fehbvm.com/Article/details/gfflkplae.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.zdbjq.cn/Article/details/gdkphtron.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.hesvh.cn/Article/details/glqqmntob.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gqwhflnfr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/gfwchkbph.sHtML

[U18] Py：预编译正则
来源：http://m.share.zdbjq.cn/Article/details/gkldujezz.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gtbyulart.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/gkauxmmit.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.hesvh.cn/Article/details/gmlxpmxyd.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/galjhjysp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.zdbjq.cn/Article/details/gmgrbcbuv.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fehbvm.com/Article/details/gyqksjqip.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/gjbhbusjc.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.hesvh.cn/Article/details/goqolsmst.sHtML

list(zip(*m))
来源：http://blog.fehbvm.com/Article/details/gfdiepkwl.sHtML

[U23] Py：分块读取大文件
来源：http://wap.hesvh.cn/Article/details/gqvrmhnbn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/gqquczbne.sHtML

[U24] Py：路径操作
来源：http://mobile.fehbvm.com/Article/details/gwmrrtabj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gjymxsvcr.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.zdbjq.cn/Article/details/gfkqgspoq.sHtML

csv.DictReader(f)
来源：http://www.share.zdbjq.cn/Article/details/grfywwppc.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/ggyrxrfar.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/ggouqszao.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fehbvm.com/Article/details/gvgmmkpai.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.hesvh.cn/Article/details/gvmqktbgf.sHtML

[U28] Py：类型别名
来源：http://blog.fehbvm.com/Article/details/ghjlbtidh.sHtML

UserId = int
来源：http://www.share.zdbjq.cn/Article/details/gzbizbgms.sHtML

[U29] Py：属性校验
来源：http://baike.hesvh.cn/Article/details/gkhvwcilc.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/gadcsglwo.sHtML

[U30] Py：数据类
来源：http://mobile.zdbjq.cn/Article/details/gteozwkeu.sHtML

@dataclass(slots=True)
来源：http://blog.fehbvm.com/Article/details/gtgenzyej.sHtML

[U31] Py：单测
来源：http://wap.hesvh.cn/Article/details/gqeyoyrzg.sHtML

python -m pytest -q
来源：http://www.m.share.hesvh.cn/Article/details/gsspmkyve.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/grgxopfpa.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.hesvh.cn/Article/details/gkkjobxmu.sHtML

[U33] Py：打包发布
来源：http://read.share.fehbvm.com/Article/details/gizeoagzs.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.hesvh.cn/Article/details/gowwgayis.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fehbvm.com/Article/details/gzehixjal.sHtML

chardet.detect(raw)
来源：http://wap.hesvh.cn/Article/details/ggqaglfgu.sHtML

[U35] Py：发送邮件
来源：http://baike.fehbvm.com/Article/details/gslndhdfc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.hesvh.cn/Article/details/grakzrzjh.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/goappnjdo.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/gflcyhrov.sHtML

[U37] Py：读写 Excel
来源：http://read.share.hesvh.cn/Article/details/gxqwbskwe.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gylnuwnjb.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.hesvh.cn/Article/details/gbbznfmat.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/gfxfnaasj.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.hesvh.cn/Article/details/gdjskxkqo.sHtML

sys.stdout.isatty()
来源：http://read.share.zdbjq.cn/Article/details/gilggywdj.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/gpaoidtti.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gkziriirn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/gjajuntiq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.hesvh.cn/Article/details/gechzcnyj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.hesvh.cn/Article/details/gaothsllv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.hesvh.cn/Article/details/gyvtstous.sHtML


<!-- 参考信息 -->