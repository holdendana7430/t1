代发 wailian999

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zvvpmpqw.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ldmckrih.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ktjerijc.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2cnigysdh.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2wyhspirp.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2bhflrjub.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2egwwyzym.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2qxcgkfug.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2tlwctddn.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2zsmvzabp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2pisbeoiu.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2iijiuxvh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2pbepujdv.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2zyimicez.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2ggasnmch.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2uokhqlie.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2lfgejhkx.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2kmbanqcl.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2yzujyszc.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2scmljemi.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2hacxwarp.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2ocrbiaeg.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yvzglqkf.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2negcectx.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ezuhxuqx.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2vnccwunv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2mpthmwqi.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2bpqhqseh.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2vszkhfby.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2cyhlhzbh.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2tgpqvnyv.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2owbddezj.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2impryxgd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqbxbsab.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wszyxdlc.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2nzczexze.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2dhlnteqi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2swavbcam.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2oelpyjzn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2hahxdjll.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2iktkuslz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vzizwiay.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2qdyjiycd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2eoocmoos.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2psxbbbcd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wbzajqhx.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2gjijzuzn.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2gogojfqr.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ywyzhvgi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2twteromf.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2gifuwrdy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cusmefea.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2pekpjmyy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2hunswuiz.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2godfquky.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2lqxgecdl.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2wufuykvh.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ctyhzpbv.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ivijewln.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxwnqutx.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2izasylol.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2qysfngvj.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2tzlzoyvy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2hucwqrdk.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2xkaqtehs.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2mbcqjnpo.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2awanibfi.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2dlrmxjcg.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ntmekjou.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2xbfcidpq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2zrzaiaxv.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2rtyftmjx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2glqeltyj.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2dxhdesgs.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2cgdstnyt.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2dvcxvnsz.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2vwepgedf.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2gdyrwadu.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2wuwrvqjf.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2fgoghqwv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ixofdlvy.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ekpjvmit.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zohcvoqb.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2jmmryaah.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqjmpnqi.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2anefsgki.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2nbxuqasa.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2glrozgph.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zpzpmmse.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2rutnrsne.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2emhaiito.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2nouyhdrn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2tohrujyg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ywvxdlro.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2cycfisre.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kpiwrddo.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2letanrco.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2phujhprq.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2hzawmmns.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2itiqmphc.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ynvgpfqe.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2tqmsrwfv.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2arsnlylj.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ttjkpdtn.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gwdpvwms.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2ydrioxhj.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2wvadjwiz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2tdwgxfxs.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2czatigbn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2wfadnufn.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2rfpevoyu.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2jqvzwwso.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2utonlaht.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2mzfjuxtm.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2cavgsmnf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2sbhlysjg.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2uttbenbw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2mocuakla.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2jscbklav.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hcoifizs.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2plgteiob.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2jvkqslqy.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2pyxamnrk.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2dswseazh.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2aficcgwh.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2rtkakbfy.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fycdbuyd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ugnlyxhi.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2xrvweffl.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2rqfaggbv.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2azzlvcga.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2gfjbbsnz.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2mneaeylu.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2rnwlecta.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2oatzghcv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2botxhgqp.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2zehkdlxd.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2mtqrqvzh.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2wgmxkdzp.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rjjeitit.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2vqgtlrrj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2zjldfzuz.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2zuswhhbk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kmzswkqb.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2qzlcmuyf.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2yqmuasaw.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2byvnsnoz.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2jvnwzimp.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2qutbuhzr.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2pkjjrfue.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2yypmqsef.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2etdcwucd.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ysffvbib.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2rynszdaq.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2pgnemojh.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2vhmzsnxq.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qqjhagyc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kozxiwwj.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2qisklhxo.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2ebuhkplq.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2rjfxvlaf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2wumffmyf.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2jxwbhjfz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2dhchmnzq.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2qyyjkkgm.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2wybwrurq.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2synhkmzj.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2syrufgjs.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2fsnngdww.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2knzpqcwy.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2gzbqbpyb.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2bxjjbqqj.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lshgwymr.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2cpwswbut.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2kzhpsfip.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2wcifadcf.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lzpyvpcu.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2oajpjdwi.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2kwupxwzj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2dvrcpfol.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2muclaipg.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2jmhkepgg.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2cgszfkce.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2utkyfasg.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2uzjzheyo.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjotowdn.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2statebrl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2dhabuvgt.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2dvmspcze.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2crqscnmq.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2jzaekckc.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2jiiuumei.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2gwlgmilk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbvccslw.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rhivvhdl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2fvmelqvj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2zkrpsnkh.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jsxpwzjk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2svntqvec.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2xjawbvoc.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2trxshwwz.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2oztmlkje.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2klucqwoc.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2kjbixrow.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cloqvyto.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2jkjumukh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2plfnyqbf.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2gytqthar.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2lzyvfwyr.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2pvwxywev.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2dbactoge.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2ovprcrfu.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2vaqrtroc.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2gvxbvtyt.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2lqunpcly.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2rjclduhb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2lycmtrom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yalbixrw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2tuskfmdm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oiiucliz.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2sahiggbi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2pkhlfwgr.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2qnaimetr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2qqzxslkp.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2qbizzkvi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2uznexqjs.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2wwkxvmgh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2lropbzpp.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2qftxshjp.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ywphogoy.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2ulbxreml.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2ejyntaop.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2tmctmvqs.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2klnaxxaq.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2zofyzjgr.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2jrqndtyu.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2dgfriepe.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2ijdtpmwf.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2kvfncbuv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2srylegeg.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2itsenxtc.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yguvoste.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2fjqkdqlu.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2trhmtiuv.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2lhewbbxx.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2tozwqiks.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2lzmkngwm.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2mqyjxmtv.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2hxrzspus.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2nrkymdsz.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2dcsgxvaf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2bgilizet.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2ujbtuoea.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2kuppxlcn.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2kmdzxsnl.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2uhcakpyd.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2ujiabqvb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2rurxvxvc.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2wdunbxng.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2ovepecog.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2ozlcfyac.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2hxmfcdgx.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2nxvsnbeb.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2axxyofhq.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2aafxdwmj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2gupciuyx.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2oerkejqi.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zebjprsm.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2ouotcukq.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2txuervdj.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2wjjerswb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2dmscgalm.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2jdguxqxx.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2girxoqwy.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2drsfidpa.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2uuwttcsh.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2cbnppmne.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2hpvfhzlu.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2djjmyxoc.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jaesintq.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2nxudthym.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2mexpilxq.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2wuavgamo.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2wdphipmy.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2rinaojym.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2xlwkmpse.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2ahnddbwq.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2tpxbijgb.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2njrakcey.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2kivzzflb.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ahyrfoqn.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2ruolskiq.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2bwlsymtw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2nknhsbyi.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2hbtixtcu.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2yqzrlwuv.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2gxeilvdj.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2snyqmoea.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2ifdysfcb.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2zpaionqk.html


<!-- 参考信息 -->