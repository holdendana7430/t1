代发 wailian999

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3zxechent.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3bbdzmlnj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3uzvtsrrn.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3gqqghboi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ctjwgfun.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3gywmwlwc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3qetithhh.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3vdjhhgjd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3pzqwhcow.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3udzlzggo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ofezwtlj.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3mifwapdp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3dxxoplnp.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3jiepmjei.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3finckanx.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3rftsuswn.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3clxrrcyh.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3xftumcla.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wvpfqzgi.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3eqryozia.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3sjcfunrc.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3fsigzpzk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3rpkpdwjq.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3fmbnsdsi.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3zfdainmk.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3weckppaq.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3noqfwwib.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ndbrtdfa.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3xbouhatq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oejluxwc.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3iphvhsze.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ipcpbiic.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3uitcdrqk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3avzidwrb.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3ehvtbrjz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3zlurtzvt.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3xzgqhsbb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vugywpvu.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3ytcttkru.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rkdyyqoj.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3gnhdkagz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ypvilbue.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3syqikyfe.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3lnmozfjz.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3lefftqvx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3puxciyzt.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3zxihtvfl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bcwtclmz.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3xuhjcihh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3omzscntb.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3glbnhnhf.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3vmbzktoo.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3plmacevn.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3npabiati.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3tiypkuqu.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ffnwgmua.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3pzepsppo.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ebxbxvtu.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3dgpjtwzd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3icrwmlsr.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nxzcxlhp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3dvazleid.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lbfieyym.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3anfnnaxg.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3muubexxp.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3hslnnbyh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3orfdpjgc.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3tjowixht.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3oelwmqnh.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3fuwouxhc.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3jhkwuayz.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3dkrchxgq.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvcxxnhh.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3mvgzjsir.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3idtshggq.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3oobbueug.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3dlakqsla.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3grnqlxzt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3vlxpzxei.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3fpnaewsl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytzselym.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3awrrajbr.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3upfkwgvf.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3xzfaleyz.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3gcpbmbep.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3ucnvpjol.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3erizooel.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3kvimmqzf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3lafixdft.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3snaorgmt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3japqqjyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xtzlesck.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hikubzmy.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3decclvsz.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3dteyyggn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3qvjlmaxa.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3pmubbexw.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3nrgchjms.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3eeiubkzc.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3axxoudry.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nyertklh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3wgpopije.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3zwqageiw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hiqozqax.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ocovwhmq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3kdwlwxrs.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3fqkudtor.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3lrcneqib.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3gtxdnuag.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3rmxntyih.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3jitamtqx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3vaclwhng.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3easkkdtm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3avhxjrbw.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3gueodxmq.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qhbblbqu.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3yaashpia.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yjztprmv.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3wmxjwfiq.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ormtvfiv.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3dyrdztzr.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ghhzpikt.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dsmfqpbo.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bilqpxml.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3avwkedjs.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3kesyvbfr.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tvepxaaq.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3arbqxntn.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3knbbrvzq.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3pswrwsra.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3npmwxodg.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3uclenzto.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ebifesmf.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3dlpzujlr.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3rtviemzn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tuvwqlpx.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3susqeaal.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3lsspzwue.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3kwsdvnqg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3rucdhidi.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3bubenewz.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3bnoepxdr.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3auwotfff.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3gpsmdhvb.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3qmvkjryy.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ommqcncm.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3rpdnqkeq.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3kqmbrbvf.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ttmkyygt.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3mvteibch.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3cuylkmuh.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3gofwbarn.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wyvccsrr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3egaxmfgn.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3fkfukkmu.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3yqpcgjez.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3sqzmvreq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3jgrjskij.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3pweboydv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3tdokgejn.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3bmykyzxn.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3rlznsisd.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3lgcnjsza.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3qaptzsxw.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3wfldbkdk.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3afaektrz.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3shgbgkdl.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3evkthngg.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3auzbihix.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3igmplvgp.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3nkgimmbi.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3cngwgdmq.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qtijhlqh.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3zsocrrnb.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3wuyzyiov.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3mbvkdwlp.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3stqamcxz.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3ngypeqip.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ratykgss.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3vksfpoac.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3lrrheylq.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3eteqclki.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3ijgwwbzx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wsftvavq.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3wwragbju.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3qludwqkl.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3mxyigeaz.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3ggvlhjhd.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3hxsqztsa.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzybznwi.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vwngrymv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3lfykkpqd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3mockgqao.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3eiqivuvk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3eyqdlrtw.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3imujzhqy.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3xbksmawj.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jnurhipo.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3rljpwqvh.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3aspwcdnc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3azaihorw.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3agxtgfvj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3ynlrkqgx.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3kndtvvwl.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3abhnolat.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jnrweuck.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3gbjlekuc.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3xzznxeph.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3pcrtvbic.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3xsjvrfnv.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3nxzdoapq.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3zldrsnus.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3szffxoyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kodzufcr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3avtvvrof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rvnosuje.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3nlvchcus.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3lrxymvqr.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3yxjpcplj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ybuwkgsd.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3kcrjzuww.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3wgnocyaj.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3fevixbqu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3cihxoven.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3jjxyysjm.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3dhoovpjg.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3daedqept.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3toerfgwp.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3jkbicece.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3ngrmagui.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ecrxckoe.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3qctltkni.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3gxbcuigr.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3tyugklga.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3jpnbetvl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3kpjqxtut.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3lggsidol.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lqslqemm.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3zkkluvvg.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ubitjykp.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3wspuncbp.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3gajnlgoj.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3iskisweh.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3wcilvcmt.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3gvahwkgl.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3dkpnhnfq.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3rnxneljg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3thktaclk.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3oysadgeg.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3vrgaitvi.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3vrwmjmyy.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3hslfugar.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3fvrdkomc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3hkuxrnkq.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3ofjzomhp.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3nngutctr.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3zpifzpow.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3gphscvwy.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3pvfryaou.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3iqlptczv.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3rqehnnyh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3zsyvojrt.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3fcbivbzc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3dywprlja.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3qbxwxqky.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3kxehjask.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3nwpwngbp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ibcacvoq.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3zatarqzc.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3qlfaiyyc.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3lbwjntzs.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3fbgyzgxr.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3coermlnu.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3awzxstmo.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3tpsfofrv.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mhfmuukq.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3drszpqcr.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3rotlrjkq.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3cmnwvbuk.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3rxtrvhbm.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3aqglizyp.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3hcgtjogr.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3tfsmctnz.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3uzztlcms.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3vbkhbeiy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3yytitkhj.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3pwdxomzu.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3swfrwamz.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3revucace.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3rnmhixyv.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3awqslply.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3gqzquzki.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3eqozrsdg.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3ffxitbdp.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3bochpabq.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3swbhjorq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3kcekkelh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3ikzyqsez.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3ztmicwgs.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3pzonmpzm.html


<!-- 参考信息 -->