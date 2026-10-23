代发 wailian999

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3yhqsaoup.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3sqpwaenm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3lsdqmasc.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3tuvpzqdq.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3uqbzmvmy.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3yonsdloc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3uxzlbnwy.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3mzaracgj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3uglznuyx.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3rzolnlhb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3zzjrlbdu.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3cvmvnqgp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3mzhrusus.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3aenqtwsp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3qlghcbqo.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3stplqcbg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3rwoswsss.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3qxlnohaa.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3gbiqliho.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ibvgmzgl.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3qjzlbtce.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3owrrjjoo.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3iynibexw.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3odbxokbw.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ipeowzaj.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3yykkzyok.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3xwmqadau.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3bwdxjuoe.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3pzeugfox.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3pmmstsqc.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3vrktthqo.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ohzsumiv.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3svskjguz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3amvbtbvq.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3cnolqenx.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3gfntjegb.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3dokxxvqf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jxurlhec.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3xfrteixq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3eyydynpn.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ggcwfqua.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wqdzmmhy.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3zipenvby.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3oraebzmn.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3rulsnebq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3xgzsntad.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3tecgixuy.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3arvctuxf.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3cprcvzqx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3rfxedbdp.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3pftebyly.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ayaydwwp.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3nbgkuzlw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3rmebvofb.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3jalrewwo.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3ogylcnyv.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3jxjintxh.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3xvvxjels.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3xphkriun.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctiqhxea.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3bzwaouie.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3cfacmkot.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3blpcyxzs.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3udhaqnma.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rbztttfr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqhovxmk.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3utdoejcu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3lzqsoise.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3afojpljy.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3lcbqpuhs.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3zxijolgl.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3mhsnagau.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wqauteow.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3snccqetx.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3jutooruz.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3zeoisdpy.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3tnuhqdxr.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3mnjnwgfr.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3hsuhvwor.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3ximiwdql.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ebfzhroh.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3nnxrjsdb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3tmajyceh.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3snsoqlyo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3nmvugrnd.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3fdskueez.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3phwefgfk.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3esqaimht.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zcbogjrw.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ulvsuncb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3blhvrgsa.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3zoacpbuw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3tbkumxmj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sloklzgz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3jsusrycd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ekzwaifw.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3phgirors.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3cxvszsrz.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3nbagxyup.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3lvtgppwl.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3ddhortlc.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3qeurleno.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3hreydsks.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3czehjyit.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3fgjjxngw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3zzuwojcr.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3jnnrtacr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dwvlxaay.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3xjnpwnek.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3mvmemjiw.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3xrfuileg.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3mgjijowo.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3dyqxxdhx.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3xnvlbcih.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3axlgpnez.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3ugazfymt.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3cmmsjiia.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3lksssqmt.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3pudkkmsu.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3esesrfij.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3qzurywao.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rpsmothp.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3cmkdhkcx.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3fsadliaz.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3bozbomgu.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3aftsphgy.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ftitiqcl.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mwcgpjvh.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3segrsnad.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3qunyfely.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3pwpxxbrl.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3exfekngi.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3wbtbrhfw.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3ytdvagvy.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3kxgxwrtt.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3lhibtpoa.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vagdklgl.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3jhrkkwcq.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3izrcubqb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mduwwesp.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3bhcdvdam.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ynmmmfms.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3nnfhzlhe.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ofnglatr.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3fdsumdcf.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3advtiupr.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3jaitcxnw.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3lbbxvtcp.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3zoaixrmq.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3ztwklfss.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nuqmhjda.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3xjausxpk.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3fmauvaao.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3zbgmippb.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3smuxqgcp.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3tismwjfy.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xxbyutki.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jbmmutvo.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ihmfevuf.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3djfelnet.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3howdsoqi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3knbhrfjs.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3nbldvffd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3cnynykud.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3ajqksjqj.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3syugknnt.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3elowtasu.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3lvmtgwzs.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ipopcsns.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3exvcsmmr.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3vxlxpxle.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3pppulesa.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ksmavdal.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3etxjalhq.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3fxphcrxu.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3fxfmurzd.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rqqdkiru.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3mwzzakck.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3iybkqffh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3akceogqu.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3pqbkrrsc.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3rllchzxp.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3eoifvmyf.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tyquolap.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3wcmtlbfs.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzjaylvx.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3sarpiyuz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3immfgeid.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3idqbzbmm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjgktgse.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3yahskgdb.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3lpakefev.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3smipnlii.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixlsipzo.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3formxjqc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3vdlqcndp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpcjyhxu.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ablmilfp.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wajuqlvx.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3nkluwqey.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nrteqhsx.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tneqkbca.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ieugjgkw.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3hoctwddh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pwdniswl.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xnmmelwi.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3khtpjdfu.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3xlkqdbel.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3wfdnarrf.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tlhmrlsz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3tjhaskbd.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3npubzebs.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3nexvmzqr.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3sfcfogpq.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3kenhpwps.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3pvqkmtei.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3siktuhtd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hkuigxzr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3prfdebzc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wuiajldn.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3otsmonsp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3djduxmmx.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3ihwyenlg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3gulrswos.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3srkrflfa.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3rthebuvh.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3zgfhoggj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3irkupzjh.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3iwcwqbte.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3pszoozof.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3aktladiw.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3srivypls.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3lqpzldep.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3wslnmajr.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3nyrdmuog.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3rgvkufww.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3vyhmkxhd.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3ildruwgd.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3vhwnhdfj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3gkzjsnar.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fbntctyl.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3fibkbbqm.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3kzxvlooo.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gqmrfhkn.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3qqddjlxi.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3jgyzpseq.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3hptphmbi.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3twkbeudp.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3wutommlz.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3hrvgvagx.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3tlvqdddg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3bycuryfh.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3asqxhpux.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3djyyyqgt.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3fqqzxojy.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3yacxeorl.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3kkaurvle.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3gjglvpxt.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3gliefbkr.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3bcbzfqmb.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3qgfnnkph.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3mqtmeyyl.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3zjdvadmu.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3prfjcxkn.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3sxjpjwfy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3qslcnagd.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3hzitxohn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uiyyfhwc.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3sxtjbygl.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3skwsdsca.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3mfdrgnkq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3dvpwgucm.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3fobqtkte.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3krkipcbv.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3fgqntyyz.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3frebosmn.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3xakijlkr.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3epelcbnl.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3lewvhmbq.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wadwvxll.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3yhopwzdt.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3yarxvkoc.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gndtgjyo.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3aiykuiyi.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3jbmwwtjb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3wmdufmni.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3mblerdcw.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3xxasexkq.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3onvsibvv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3nbqptink.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3bwyejqpo.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3usortgdq.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3fgondxzj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3lxxavhlt.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3chfbfxxl.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3exxlejfn.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3uhvauyss.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3qokkltth.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3sglkfynp.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3gqlzjjfm.html


<!-- 参考信息 -->