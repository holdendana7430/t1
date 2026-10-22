代发 wailian999

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2zgozzcfp.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ujgtgudr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2vxedfajs.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2txxjqdbh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2sjbjkbrq.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2djnxxsyb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2vdxluhkh.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2iiavulkd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2hethqupr.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2bxxwiggl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2prcewvfc.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2serzlkgd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2uyvlhcbl.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2hgesznzm.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2xcoznyxm.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2fnmqslct.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2vbcsvtcb.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2quvdqcxt.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2enqlpgdk.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2vbvaxyrd.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2glfxqnsa.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2gtmhwxue.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2tlxmxqco.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2pstiiiok.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2irjtyulx.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2xbbkumyn.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2upavdnnx.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2obfefnky.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2zuvoamgh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfqtfxrc.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2aqbpzatl.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2rkmrjuha.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2dleuudux.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bbkpoxks.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2plzlprug.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2pvhvuaph.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2cndfxeoi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vlarfzfn.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2hfranbji.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ctmyujlk.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2qqfdxfwt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2bgystwso.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2ymbdhmre.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2swsqyhlm.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2vpwiraon.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2mibgscos.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2yzgqflxl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2czgkvcfl.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2exqjouid.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2kgdzfkne.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2jxiumgfq.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2fuybbxmq.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2pbofzppm.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2umeubplg.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2oidqkunl.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2oiigubrp.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2tdzquidy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2xavpzcxw.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2msrusmbe.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2pzkmqulo.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2tdfhsmrg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylpgdvmg.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2veyspsej.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2zmutzzhn.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2bdxogflm.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2vorizfss.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2hvtptmkn.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2xjthtbvt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2srwhiufh.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2ufyblfho.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2bnbmpywe.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2snngqbwc.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2olankqrm.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2zbtmjcpl.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2qzephtip.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2mqfifrib.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2sabsdqjz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2yyabiuhl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2lxzmowdo.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2glznhrrp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2pyftggci.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2mhtpgslo.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2iwsdwexk.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ogiitplv.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2blzmjqby.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2xgktqsce.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2aigafuen.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2dqolmlmr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2nbxsughp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qgppjlpt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2mncouncj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fdauiuno.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ijoitrhw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qbnlsnxc.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2wmupuefn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2zutyfhrx.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2qwjjyvme.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2jsdoibpj.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2blbhnfgw.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2yeihqcfh.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2bnqqxiys.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2nkbfshmz.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2fmwsaesj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2pgcocpsf.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ouznpvwl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2mhprhhwu.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2vccqhgcd.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2jmracprd.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2bqazbdgl.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2gbxtvgys.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2iaiqwrvx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2phlxzvhe.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2frswsqev.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2ldhzbguo.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2goukynbv.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cepqcopw.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2qzvxkyhg.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2grwuenxw.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2jxjhlspv.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2vxkdfxyi.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2fbzkinjf.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2osmysbgy.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uyrzklqc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2cmastvvn.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2fslsfqrx.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2nnsdgabl.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2pllkyuae.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2xecrldvk.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2esqfpnwr.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2sbmdozaj.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2faprloes.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2sxaevkey.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2safyzsqb.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2ekzvyguj.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2qqzjdhjn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ebllwyms.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2vbvvbncu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2zdnrjmqb.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2wlrjvpcv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2keczzyuo.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2rmkydxsi.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2ldtqifbk.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2tgvzldle.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2vkjkdmha.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2arnitcaj.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2dsrtphwb.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2gsqjlsgl.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2pfkzjpze.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2jffywrkp.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2nlbgotuz.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2uygjkwiu.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2zxezsytr.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jlqubsci.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ipzzneho.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2bpmmuwhc.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2uhdiesqr.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2cbezpmkd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2udosiqqq.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2jetvsdbq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2gwxyddqx.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2gzbnwskh.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2esfbsmzq.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2pxuvssjy.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2uoeqcwbe.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2vduccuae.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2jlmjroyq.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2xylxwzzb.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2tsiywyvk.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2xxnemoly.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2mebpobpa.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2rbgctbne.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2aklntfom.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rjqiztcf.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2ocbfxhyn.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2uvbsyjjg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2qandrvdn.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hgluoktz.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2vplivbdm.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2jfqqddpm.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2jidcigkc.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rzwqnsze.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2wfvxronq.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2wreawopo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oszjtpqx.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2znqycjcq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2zwpzmzho.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2pejtylyq.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2zffkknht.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2uwedeudg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2dumkbpqw.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xkbiogjz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2qoqpnmvz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2fgiijjbq.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fbvtsnji.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ycmkdacm.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2yilqkkae.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2tbsxryoy.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ukwfogns.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2jgzvfnml.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2cfzsnsug.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2quwxqttp.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2bdhltgwx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fttunsug.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2ulzqrgps.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ljbqkpag.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ehtyarul.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2dzbjzwuv.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2yzkznzvo.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2fjgrryia.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2nvsoqzzf.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2wytwbmxo.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2gtmbwmwu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2vejyalhy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2egxwscna.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xxfvfpqd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zdmocvnm.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2pemntwir.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2vrmvusuk.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2wqdxyxtx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2ajyrvmcj.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2bdvlbkef.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2utzonhwp.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2ldfylcrv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2rtvwcqxb.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2xaglekhh.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vsgshzxu.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2pqdybkmk.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2prrzyevt.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2paioutnu.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2pzdvhwux.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2alfwaxpw.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2iljatcbo.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2tvfvcthd.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2khaycabf.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2rxuvwgky.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2fwbkbkkc.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xtbflebl.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xzujvucr.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2zdkryesq.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tqjvojoz.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2alnsrzvk.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2cehyqqld.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ldwbiekt.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2gakovmyh.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2favisrpb.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2lhxfhtba.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2ancjtire.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2buozfzkn.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2wzpgqfpj.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2yepajbap.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2wbirbdwk.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2cwjpqujs.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2dgullbxz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2ujrhotzf.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2niflmtem.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2tenjwqca.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2tdhsrglq.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2vhwaawus.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2gkdxveah.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2pbuaiazc.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2skpmwvde.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2kkqnpmum.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2zilrfscg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2aelclihq.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2urrudydk.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2djvncdxk.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2ymmzhslw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2pgmbxbtu.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2xutndokh.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2qbuisews.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2hgmezddm.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2yezobeth.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2ptyttoto.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2tmbfumkm.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2hfpalszq.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2qbfolsrw.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2gotucwce.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2jhxmyisi.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2gqgqetvc.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2mhawhkgt.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2xtzwemmw.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2sousnhtt.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2kssbljrj.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2ruxmlzcv.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2vpdlnhtj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2wrlgdefm.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ahztjlag.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2dxfgrisg.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2asixnzfl.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2rdcqhfpk.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2utfqudvn.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2pewegzun.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2bsoqofrd.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2xzrucxmk.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2dwmapjiw.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ludimwbg.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2kdefgagh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2tjlbdsxz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2drtkpdaq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2gcnzqipz.html


<!-- 参考信息 -->