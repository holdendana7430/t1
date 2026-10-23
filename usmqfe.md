代发 wailian999

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kzoqkzzi.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3sxvmkwmo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3uxgodgkl.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3uodyyayc.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3sbtmqrpa.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3tixnelqp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3dnimnklr.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3aiovjngq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ingbywil.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3zsicsuwr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3ereuusqf.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3kupfefzn.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3iklsqxzq.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3qiaosnrv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3dxysliyv.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3zcyxzqqu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3vhaqtfos.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3ygmhvecl.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3yajomdnj.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3qxsazjpa.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3ihzxwdyh.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3uwfqzxho.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wxynybvb.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3prudazig.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3hpyakwcp.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3vdcxbqpq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3reuqzmdk.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3yvkmtfsn.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3fsvaflnv.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3xlhifemu.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3ufwobajz.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3isdhctxk.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3acpkymdd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctogtxek.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3betkwslc.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3xeeikhch.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3uxkolzyb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3ctnctmtc.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3izptmmue.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ypfjwxiw.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3kgspcnmz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vrrcwlne.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3bwyjkrdg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3evwbjlkx.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3ptndeilq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3qbdnkexn.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3ljkwvrhk.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3tzshpxdp.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3pctotxnc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3cgbmecse.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3ncxhbzea.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zikridvq.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3tywbealz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3psrqfcpx.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3bmcrwhqx.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3imwiamql.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3nqkamtwn.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3rkmwgtfq.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3bkvqpiyz.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3wkxlzzfi.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3hhuomxqu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3uiaotkxw.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3qzeuagjm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3puqfcijc.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kvmkvkhi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3lwwjowfw.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ldlpkhyp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3atzpyima.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3chtzekay.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3szkkwtyq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ocgolezw.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3jtgnhoor.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bfgpkbij.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ewctazjb.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3pfulmesl.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3newuizws.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3vvccvzfb.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3jkomcyfd.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3cleomrqu.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3rbczulcp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3doindqhu.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3hljgseti.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3giajyzgi.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3zsugalrr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwwdhqqc.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3hdufwsaj.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3jrzuqcrk.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3lszjnnnk.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uujqzobu.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3shhxulzm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3fuitcvvo.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3rukabypz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3akibztjt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ehqlevmn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3bogiqarx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lzfmvvuy.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3leltoedc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3uhaoydph.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3cotbnycl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3pqjryxfn.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3dhncyhsv.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3nvbhbbnt.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3meuzoami.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3bivjdvla.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3ttrwncse.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3qzgmnlni.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3xycazrel.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3iaokffpc.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lszxrsjv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3mwukpxou.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3mcfdzlca.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ziotuocn.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3chgkpjsq.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3rqjuwcsk.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3zekawdmv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3dotjqoob.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3vjhkqjoj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3oisxjyvc.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3zpttrfbv.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tmblkpzh.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3vdzswuvf.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3owdeqyon.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3mjrlwxax.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3zcphybio.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3draypebk.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3jkfrupya.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zuoztxpe.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ebmevxnf.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3mrvvgbts.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3etzrixrg.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3afmphecd.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ibepmcvk.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3padggbxy.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3ixqnuzog.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3enesinfi.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3qajhkgdl.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3crptftek.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3emyexuxe.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3swxspnly.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3rwjlsffx.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3lyjkriiz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3slxfqcfp.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3rlszkkjb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jfjdmpei.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3zbpnypkr.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3nobqswgm.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3oyjbupdp.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3rivgxtwf.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3qideqliv.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3kzvmihau.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ickjbaff.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3yybifgif.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3yfieumxx.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3rxmkqshx.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3pamayooh.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3xbxfvsjh.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xxuxyfyg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pzupfzkj.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3lgpsmobv.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3wfqbdpxx.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3bjeqbkto.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3yvnibsxp.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3eoblknid.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3pkrktygb.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3xgkkuyfj.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nypxdhoy.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3tntqskry.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3pjteafvt.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3kovsagko.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3lddnqcyv.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3zijifzwi.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3fsishbvd.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jfspxxod.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3inrbvicv.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3cgkvecss.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3jgocihhk.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zzmhxoop.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3vyhbejmk.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3cmwwwjvk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3wzajriux.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wjcwwusk.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3hothmvuw.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3ajjxuprc.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3dccveibw.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3vtpghmjk.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrvpwqtm.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3vwyjmdup.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aakffuql.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3sjgbpxdx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3ecxovnlb.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3kvuduxaf.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3cvnlejmw.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3qduewzja.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wiidqfnz.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jxzecqfl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3dcosykrk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3exayunlp.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3udjypanv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cbbpqhuz.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3wheystce.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3boycuvks.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jtqojhjf.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3fajofemj.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3olcktmgr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3solxdtkd.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rtmtgaej.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3yqtprllg.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3azxkbxgr.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3oblaetme.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xbqchzcr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3vetigpdj.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3tbxhdgzv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3kuteedrn.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3dytyyvdd.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3wixelwwp.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3jycsfznp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3akroacck.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yteuybmh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3dmloeaqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jtpkgbgv.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3vqivmtqh.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3qeiyuymu.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ycozxfbk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3gqenalis.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3obmfvmen.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3tbmounqf.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3pqknimnz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3vivkxbvj.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3wbhdszvk.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lrygnbzf.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3ttzslrpv.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3xvzxkobb.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3qfuvqdmz.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3zfksybao.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3vpghsrpn.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3ipaofgwr.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3jgotnksp.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3pckejabk.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3rscxmeev.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3wpruorkr.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gsblwsgi.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3qfyikkzb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3ssntlslq.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3mjsfckvz.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3ysldcrsi.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3tdasokww.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3zegpzybx.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3rkyoovpv.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3ytwdkrvd.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3ukxcwluk.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3hladwmoi.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3chmjfzqn.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3igbtmmpq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3xixmwbyd.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3shkiqhco.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3xltawxzj.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3eubperpr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3smhgwczc.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3pzpcnftv.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3mtmpnvmz.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3sihqlybs.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3iokioiho.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3rlkzmakp.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3tenpyock.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3erflzlpm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3zlewoyip.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3jgxfqyhh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3dzjglymp.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3wfijssce.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3nhcfpddc.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3vtsidhms.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3fdrtonbt.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3sodzrcuh.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3zmskrfkk.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3ppfgiiad.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3yzqtwbsn.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3aarucwvr.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3dxttcmhx.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3upulwmwr.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jllwmaqo.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3bglpsaon.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3rmcobgom.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3allgjmxo.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3muczqsve.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3wqthaaoa.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3nvqblgnu.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3iqzmzhla.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3nepbiapn.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3fywacxne.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3cvfyazho.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3hedgakpu.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3ulubehab.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3polrmnxj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3xkaipqle.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3ftiyywfl.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3edtdumaq.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3kzmwuyfn.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3kfombycq.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3xhhgomib.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3joufpnfj.html


<!-- 参考信息 -->