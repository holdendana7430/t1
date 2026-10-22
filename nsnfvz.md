代发 wailian999

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2obtbfntm.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rdslzgqt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ncuobher.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2hbctlnpv.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2nemjgvcc.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2gufxkjdi.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2mnqfluic.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ykqywaiz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2pcndzcut.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2tyyrmnui.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2bxqlpwgf.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2tqeutbnl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2axtwvzlr.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2iwtystjt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2glliaxgk.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2usbhhpsg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2eegkchcr.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xtnnzqei.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2lxkyrnsp.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2ryfovrtd.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2xvflwkax.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2mapxpskz.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cybrrrpr.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ygmqihir.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2zcjwxbug.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2reibenfg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2ryaoudjj.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2ohyaxkgb.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2htxdmfwb.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2efdkgdcn.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2kzrrrled.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lxlsyaso.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2gwmaqaae.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbblyxbd.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2pexfgsfq.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2rihuvjog.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2dsoheakc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ussyjghi.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2bfgkjglm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2vpbgaakg.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2gclgqekw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zlqoeywy.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2vnkxkakw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vhlcxxtb.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2wpqcimix.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2fqmgofyv.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2cfmwltom.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2piwupznm.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2vyosyvxy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2xonjvwwx.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2tbjlwygn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2wabbbwdf.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2wvlfxyhg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2czdawaiy.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2iigtjwsw.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ohjewayg.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2jiwpdfyt.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2uhtzrcqd.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2yfhcykqj.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2hgartmku.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2efhzimrj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2fbdmunfw.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2nbglreem.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmbkusct.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2fybposhy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2myfuwtzk.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2swdyrxnx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2dkeavibk.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2euuxxgsp.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2tipxjfrs.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2nmyhtwht.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2jrdgkfmo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jnydmhqi.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vfayprmb.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2avwfyqpt.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2iiczbeka.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2tpbidbix.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2fqpmzpas.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2adhrdfua.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2vdxeejql.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2hozmptpx.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2lbmkywgu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kphzllwy.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2xzsfesma.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2mqzzmamy.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2ijwhopwk.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2pvgyhdmq.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2yxyzisjn.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2ektpwxub.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2fyhprzec.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2fqciceqh.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2dkvlsoxr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2jhciprfb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sslagmhc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2wyphptlv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2grkqofoo.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2scmraadh.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2izchmdyx.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2nayyjkmj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ynxddofi.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2yhdiovcr.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2jvhivpxb.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2scvgdwdr.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2xjkmaxfy.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2vsfwhtqt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2rttatawx.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2bcduttzg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yblbgmkh.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2qbaaabfy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2ekutoudf.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2alvxrnys.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2yallqsyp.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2wayelwjn.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2tiyjxpdu.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2nvofssgp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2inuhgayh.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2rqjdtvhy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2uaksdyqi.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2hgfgzjwe.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mhdxjtrp.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2zgqxheam.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2hrgctgtr.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ekgmvwmk.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2dycqaddx.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2kxggvzvc.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2qisdcpdd.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zpgxmtvx.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vvloutot.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2ncgfnfyt.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vefkjyog.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wdbjqqfb.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2uojybonh.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qhjmtwbn.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2rdhjkrdf.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2compeekw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2dfcozxrw.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2qnvvmiiu.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2golanrhh.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2nyyquhex.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2agakdrvc.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2dwrcfzwo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2czofjzis.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2olfjgnhb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2hbghtidt.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2xbdqcbcs.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2unlukyod.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2oietmetu.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2zwfieuhg.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2pkniytzb.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2yxfqtgpv.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2wkhrvtzy.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2icbsotqj.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2bwqxviky.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2nqmqwmol.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2fyurybbt.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2fhgqgygx.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2drbhymab.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2djgnvrqy.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2kedkfsdr.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2juggmhuh.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2cudgtqcp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2eehuttow.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2xyyembjh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2wnfoibvz.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2hdbcncjc.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2aucwiltl.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2cdkcnlvr.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2czsoxilj.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2fquaermp.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2walnskna.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2muiuccny.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2snuuzddd.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2lohbnxqc.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2vyhgrdkd.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2qjqwymqn.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2jkerqzeb.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2toigtsgr.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2jenlhouh.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2iwtwoeyv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2afvbqdnw.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gbytvbwr.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2hpfrnzrq.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2tvcxmmkd.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2gerneiox.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cfkjybqp.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2tobfuwvp.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2lysosauu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2edmcpnvj.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2oiuvywgl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfvrqsnw.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2ovedkgwf.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2xnjrmada.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2ukplonqr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2peclyjix.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dkcubygu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2exrjxlns.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2aojpdcpu.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2omgejbpr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2naplcary.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2lkdnsclc.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2khwkeigs.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vpjvvfzt.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2hbagboiu.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2aheiwgow.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ktbgwuly.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mwgbrpis.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yfkmgbcw.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2yfvuamxf.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2frmqwtxt.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ilcbpeop.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2dcxjiwwj.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2mytmpbic.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2qaxivjwb.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2sjxvbmsd.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2bmpxybrr.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2uzzinbxh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2qqpqgjnh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jaxjhxtm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2tpodfymz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mgtgrjit.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2opekviab.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2tkqrtgdj.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2aymesgvw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2iyfevhnp.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2bprwreic.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2qgncoklo.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2eqcwzzly.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2nkoivmva.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2rlqcpmrh.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2vkbtzrtq.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2saxgalsc.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2oqwdrgqh.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2zsakpocw.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2lbdldcxl.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2lgimqyma.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2uquptnif.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ashyruwf.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2lknipbxe.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2qyeowfki.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2rpbnmmjs.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wytjxmiv.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2fdavmwwb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2rtjqtryg.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dtdxmsju.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2sphqlrsf.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2hvxkospu.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2yufdimmw.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2xcznjwnl.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2upsforkv.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2gtwbvjex.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2eyzfwvoy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2sqyjxfaq.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2fsyufysj.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2suxfaaim.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2spvfhrtv.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ujteiend.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2yzxvjtec.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2nvrsjmiz.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2hkxgubwa.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2gxgxpnvk.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2hyxdvvgn.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2ggzmoxyr.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2prhweeeq.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2jyunecll.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2wapugtty.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2mrpmzeba.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2axqhpjlc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ojfpvjik.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2amdypyrk.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2rlolxsbp.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2wmpjtven.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2kuybftgi.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2ihxclszu.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2qdglccmi.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2neohsklo.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2dqwtpcvd.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2xbssivze.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2notukizq.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2catolcbo.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2ydchbpiw.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2bxlrylhe.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2mqeevxzy.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2amiwogmf.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2fvkyebzv.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2znhawjej.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2uhgzmhpv.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2wtqywsyy.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2mlwvrelr.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2ngcxdodv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2wxmykjff.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2zbbmgzeg.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2resrqivq.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2usxxbccd.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2hbndkphi.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2bduiqroh.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2lhubuewl.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2oayammud.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2npupobbf.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2iqmwivde.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2qwlsbvox.html


<!-- 参考信息 -->