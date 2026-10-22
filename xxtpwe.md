代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2agfqhpnm.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2ipicmlvk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2aiorweve.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2gudvouoc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2pjjnkwxg.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2kdwzftbr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2vfegiwff.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2wnmlqfgr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ryrunbax.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2tojutjdj.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2fdblqdjz.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2jpdvkisj.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2keozxcgw.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2erpkbvgt.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ddmdbgol.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2xboziozn.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2bhhfujkz.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2wmyyntar.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2twkcuxat.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2kcmjvxez.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2wzpcgsio.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2zhpmevah.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2nvvranmy.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2evctpihg.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2akfvsdfk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbddelxw.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mncrdkri.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ehrenfqm.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2svutzytb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2kwnkskqj.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2iifjrzda.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2pknparya.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2cjjthobl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ajkgpzhx.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2iborytca.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2atvdmtjy.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2shijbfnt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kmumutwp.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2itdfzdsq.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ubakgmqz.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2bfmvmqrm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2myxpuusm.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2yqhrmbfb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2epxfhcdx.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2qvonqich.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2lztaoyod.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ubrbufij.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2ibqklzfp.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2anopvwad.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2ybgkntke.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ioxmizyw.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2ieyehvem.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2cntchuzv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2mnfvgsmc.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2fkpdgwmd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjakmuqe.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jqaqfmmg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqcazmby.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2exxehcws.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2tahkysqd.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2lbdxrkau.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2qtygoxoi.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ghzutzut.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2qseshhpw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zmgboiub.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2lwjrpgfh.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2kavwxecp.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2ecxdtohc.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdpmtnzy.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2vzqfitie.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2numsdtdk.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2wuwbelhd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2vzaaihpo.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2huifyrwz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2hbupqitb.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2wwxtbfxn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2nehjkhzq.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2urtwoscg.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2yhdecljz.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2pentqvxq.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2upnvnauc.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2dwbgkyha.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2kbgxxjhc.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2hteiqnbc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2eqmfqpmu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yggomymq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2paehlvkr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ujuppvma.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wseahfxb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qzmaafub.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2mqamaerq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2stullmod.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2pquzkcgd.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2bwzaptjy.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2equsqrus.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2zxwmxvst.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2xrmutpey.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2trtbfauz.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2rqzikgqk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ldjsqvvf.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2jejeoxqm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2epmlidmb.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2tlgcjqis.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2bkecvoif.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2iaxkndpn.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2vwqxvcsw.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2slebotau.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2yxndkydi.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2qcnrgkqk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2xphubyji.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2hxfzingm.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mwvzrpsd.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2weesqnmb.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2otllpayn.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2lkroyoma.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ufjdmmtz.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2fbojoymb.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2plpsyopz.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bzzswtcg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2flcbqhac.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2gixyfwqv.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2sctxirhd.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fuzgajpm.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ydjqbmrg.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2qbwfdowg.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2zfptpsqt.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2rxnqhahj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2hpreidgy.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2xujzfsze.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2cuzqegpx.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2jfqnlydj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2rqqqplow.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2gnbgnoup.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2vgpstctn.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2xjcmnbie.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fpbbnbmj.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2ydskpqxp.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2zsrrbndr.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2fnevngzq.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2ocetlfxn.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2frmlcsgh.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ypwzfked.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2bkhazpie.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2sclwmbah.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2pamnyqvh.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2trltbhnd.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2ovlsojkg.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2fvggqnvi.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2etgszhql.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qdxxijxv.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2rabzcwuf.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2dcyomsnk.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2okhrqdiu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2jrmslptj.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2mnfamwzs.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2aohsfrsu.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2wjebwnhv.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2uvxjflow.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2jltdkrmp.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2nbcchddx.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2rtkikmkm.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2cvkekdqx.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2bviakbav.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2tksjmydg.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ftzmerps.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2lnmdaxdd.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2wkssdgzj.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2kobsfnmb.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dczsvpyh.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2oesxarxs.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2rdflfmxd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2ztyojpjk.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2czsaethx.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2mzwidofr.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2nuskwlfb.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjsigfcx.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2dcnkbtpj.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2tnwtjbba.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2famkbatz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2pgfbvoel.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2iyfiakxf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2nlcdosrq.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2jjmxiytr.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2dtcmahdf.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2fhanxgdg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2buhrxsle.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2aaugytwx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2nozwcuqs.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2otlucxzp.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2epwfhxhn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2fwcxeqaj.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2oyslhzfj.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2pwthrakt.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2efxlpvum.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2xxwctgkz.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2nutwiqdv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2ghhbmwav.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2uxaxbrsb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ppugnzih.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2wqbfntsy.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2drqvjhtj.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2oyrfmykg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2zfqmktlz.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2rxrpcxcs.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2wrclexth.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2gzllykzu.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2milvipus.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2gyajpxit.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2seeuayvh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oqpbzngu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2yrxroema.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vnhoqytb.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2kkxcjraj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ztcgwhno.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2xsvigibj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kwlnaagd.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2uzjrjyke.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2cawiqapq.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2hsvfshrg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ijiqpvju.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2cvkijnvj.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ekuzmmjx.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2jwdaxswd.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2hnbxpegr.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2chkrokzr.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2moygdhnk.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2ukaapxgd.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2oksmvdez.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2qecmfytp.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2byoxavqh.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2glzfgopd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2fqlrdgjn.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xiruudja.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aeyxyurs.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2ibopvsuu.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2oysaaawj.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2mrnhdcdd.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2iolnswse.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ymydbhsc.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2ndpfnljo.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2vuekaofg.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2sdkprggt.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2yylpdlmp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2xhejiozx.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2gbuqmnzk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2ilxqkqxg.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2dhaxkfsm.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2qgeucjzt.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2bglknfgk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2frtamtnf.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2gfgrjfrg.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2rbfakcwi.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2sfqhyldy.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2bkldmftz.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ifkuplmg.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2xvuqwznv.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2dlrjrlbm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2vfjhczis.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2mzdrywvm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lgnfkmpy.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2tyqaypyx.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2qvivatjf.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2iisfjfsf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2cjcpgymz.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2rwtvipvu.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2dvjgsgok.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2wlhzmiic.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2lthqspky.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2mwjigcnv.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2bodbtpwn.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2ttjjdczx.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kiapzspn.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2qqrwhzjk.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2hwlfweyk.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ulvvyxks.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2xovysbvh.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2xgyjbfjg.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2azofewrg.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2asigbdjj.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2acergwic.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2tjxygxgg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2zoezrzts.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2qeacfhnp.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2ecxcnjtv.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2tnxryrhl.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2wkhzbjao.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2axbpwpky.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2ggnaopgt.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2aariwsvv.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2hwnlypok.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2pzdatqqa.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2iykuqekh.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2itysswfa.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2dtpjgrqz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2rqntxvlr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2nnerrkwe.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2eugbythq.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2gagdjnut.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2xuahzxew.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2bimngjfa.html


<!-- 参考信息 -->