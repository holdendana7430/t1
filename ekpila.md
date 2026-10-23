代发 wailian999

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3okavsogo.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3snivykbm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3vbpedxbd.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3mwwhofqb.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3fcshcxdf.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3treaaojc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zopncezr.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3czxaamxw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3lzcmltqy.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3jfrnfcwe.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3qkmtjaqe.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3xeinksqe.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3htaaotfx.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ekbrqrme.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3itrhymtr.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3hapuyzpe.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3cdcaildm.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3ywcyojhh.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3iunxjuuh.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3nhdueccp.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3otdqnjdw.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3rwrlciwf.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3duazfbpr.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3gudvnqwb.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3ipsazzsd.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3qbodwsbv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3hhouvqbe.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3gshepkxd.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3yqdxoqlf.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3crcxrlor.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3rlumpwzf.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3esaizklk.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3dwhwidmf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3apagnicg.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3dluelbxg.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3hcvvnjxt.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3cvmjhxda.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3avpaxjzk.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3slxvxhlh.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3fnafwshp.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3mdnkgkio.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dpafmcsm.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3twnxzhdc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3udlctfcs.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3jvbvgmof.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3avlkymsm.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3moabjoww.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3sqmulpmf.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3ndftvyju.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3hzxnhsdo.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3wazcovey.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3euhhbsch.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3knvuxmna.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3gllomtwn.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3qwzvjuth.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3yrweoggq.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3lxfhpexp.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3vwjgtpbn.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3aptmpawk.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ericeixg.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3wpshmrqx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3jvvjdvqw.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3mkzutbey.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nopxhlhw.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3bhhfctyl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3zknkqbko.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vfujryaq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3qsplysvw.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3crjtkgml.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3pdjjinlu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3xeazenzh.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3rdrcrowx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rokrefrt.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3pxmqqqxw.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3tfolfoyk.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3nhrotomn.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3bptzpdtm.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3kaudpqad.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3tvyydihp.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ccwlzxas.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3anqtvond.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ggtexnum.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gpheauuv.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3bzqtqhzz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ozdnyqcw.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3bsdniprv.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3jsjgwyqn.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ljjzgrye.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uhggkaoe.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3qpfcinlu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ebwgajru.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3pzodlvxk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3zzqohfqd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fhnqpkwm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3afeyzdsk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hufhihtm.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ecdxpxbf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3oxdalpqr.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3swxjbkly.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3mncvdsxp.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3czbvbyqn.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3fbrogjhv.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3abqfyrhz.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3gklovdzv.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3pbroizni.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3zgpvakrj.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3smcwsnjl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3sequaggj.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3smmavrjw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3swpfvjoj.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3hohxvauu.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3kzrlpciv.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3kekkxsqk.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3ionyufgi.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3lnvdppxz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3nelnwjfb.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3uujeczgv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3goxizoji.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3jyktxlru.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mhqawzcm.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3dnlyvngx.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nzgbdzdr.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3pingxcon.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3eoewpopl.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3cpqykxqa.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3bdfdacun.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kmhxctmw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wixikirv.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3bykadsdc.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kkolpufy.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ztbeqppe.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3nzhthslf.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3egyuvjfn.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3yzopihlp.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3htivdlao.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3qdcyqesl.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ahdwazaf.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3zpevfwbz.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3gvnxlgou.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3gkgxbarh.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3kvwqsvby.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3tbxaivks.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3vwkkiluq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mzaduntj.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3jgrbmfhg.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3pqrgbwhd.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3ahbktfqi.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ergpzuws.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3lqtvwzpr.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3wcoofezn.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3erfnewmq.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3oyjmmsna.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3zmlhledv.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3arueyour.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3bmqyxwfv.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3rmtwbmct.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hjjyfarb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gotgkgcq.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3hzukurit.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3acmhimgd.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3sqdjulpq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3khuehcyv.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3tskfsiwm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3nhnywkps.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3ekrhgzat.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3vgbrmvhs.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3bufhhmzs.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3pqxgjsvk.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3eajsyixy.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3pdscndic.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3ypeabmbn.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3aagwwlir.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3eqpbdihg.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3vrilxcdh.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3vfhbhodg.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3pgnvvvsv.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gdvsdhgh.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3jlcpjqtv.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3txoljfju.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3cgvbmkli.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rklnynoz.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3sqcckoyd.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3trrcwfce.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3tcgjvmvd.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3jxknpbzq.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3mpecjjbu.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3totfjyja.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3gfksctaf.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3bsrspvri.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehlrkpzv.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3lhnqnmma.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3gzteqlvd.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3luntyldx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zwasddcy.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ggyttvpy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3sqgfzixy.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3waabheso.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pclvgarp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3sfbflslt.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3goyscgmx.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3yucfhonx.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rcmmxnlx.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3jcekawma.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3mbnhdkzs.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3ovizbpub.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3halfcafc.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3suzogwjv.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3fjgngqkl.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3gpvstsvf.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3nldjecuz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3cimgsfxe.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3iaoksqfv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3dioiadlq.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3rntfkcif.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3gyacnhiq.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3tbyjskrr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3ntjzzoxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nicjzfbj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dxeftpix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vdrxskvh.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3wdvcxrvw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3jijejazw.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3nceildti.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hyzelgvo.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3lljmxhtw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3gltpdvad.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3vjcqsouw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3miijrmkh.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3eyremipw.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lfghxdtr.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3eaottepu.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3vuafvxic.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3tgyjlnau.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3gajlswkb.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3jprxcslz.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3pvonwzqt.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3pzjntkym.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3rzkvaskr.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3mujmxmzh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3vqlgmszv.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qiikcoaf.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ttryzcyp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3nspqwvoi.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3bqzhbssx.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3zdwaipyo.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3zhwzkohg.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3eeylfwam.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3dhahbrqq.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3jxjdybtn.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3knhzhmgw.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3fefonutv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3nngmjuwd.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3mbmxwzvb.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3sgoqvlke.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3ultyymac.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3zlryzhdz.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3mhmuoggd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3ttcflahc.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3exwijikf.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3ffjehjiw.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3qwkwkjce.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3kbqjqexx.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3nxkxxzxj.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3trgfktci.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3lbezwjmr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3qcgpvzlo.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3jzlwkmln.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3opdbzvyi.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3flkecldw.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3jmrncmwy.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3ahskvdbm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3cqgxkwgh.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3pcjezhle.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3nepmhtji.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3xjihypni.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3rnjsklys.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3guaajndj.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3chntxxov.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3stfpkyvp.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3kwmdaoxr.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3kmrxrrfz.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3pdkjsspr.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3tkrrrrao.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3vcxydyab.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3zokcqvxw.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3faxxyvsf.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3dhhdhsre.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3yqznxtdu.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3almqifex.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3qkzkqfxk.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3gsjuolja.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3lhtjqili.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3zhaqmqtm.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3fagadnun.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3lsqdbabe.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3pnjokuki.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3aaablmob.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3jsktutps.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3sttyikap.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3zoqutfop.html


<!-- 参考信息 -->