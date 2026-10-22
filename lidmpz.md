代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2nvgkmvqj.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2tnslyrvg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ztbysxls.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2erspnryh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2oezqfldq.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2zqhdsdaj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2agedtrlj.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2lqumjtnm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2upboudps.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2tcekzncc.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2satkxhxh.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2lxgqlcqm.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2wrheewgq.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2iflxtdax.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ljruoznz.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2iordsfgp.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2mhwuwlif.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2nqcyhgvx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2ntgazhfb.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2vmlnycif.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2bnocjqgw.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2qemvhvqf.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2bzmyieod.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lgxmyttk.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2jggzoozb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2oikexotz.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lirohskg.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2vrwtbijg.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2sqjpgomy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tihxvxeo.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2qqvgtifu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcljmqey.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2bxirjejg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jcnckrve.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2trjgexgu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pvfrhroc.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2usqfmzsu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jdzuicrn.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2paelzgpn.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2jhuuzzmh.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2pevbzaap.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2zdnlkhwd.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2kdnopgzs.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2cewwjrle.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2rmutwkxk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2yycaujra.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2dunewodk.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2czzubcta.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2tbvmcuxy.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2kwezuixf.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2ngvzbxlb.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2yappoypl.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2bmoczlzz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2elnwizbn.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2jrstwmvk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbqpzrwu.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2auxakxmx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxwxpaki.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nqtseccl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2yivfhqkn.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2zgyeeijx.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2xopmtnhl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2wtciyala.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2lwnxhlzm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pltbehhg.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2mxyvkiei.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2wtdnuroq.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2nemigefh.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwavckdi.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2sliakodv.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2dekrhqyz.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2kebbxxav.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2tzdxgcgz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2yoiaeygh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2uxxxtyeg.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2xgzdqlvi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2wvlujjjn.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2mfswzrvp.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2zusdfekj.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2nnqkdhwp.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2ybczkyfv.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2fnnnfqkc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2pqyuaiht.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2ulfzznye.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2xltyugze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dczszjig.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2uqlnnbnx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ndiaqegm.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rqfjvjur.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wxksnrpa.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2tqwbuwkc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2hevfbdwf.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2afrndlnb.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2gmlurhyr.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2kpjwhekm.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2azkpwyef.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2xvupfxla.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2bmcdxvbw.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2txlhsxxe.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2mufpzhhe.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2yhjmhcqq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2gpeyhitz.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2vcbggpjb.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2xrwtsfal.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2iikmlohv.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2doybxped.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2njjvbest.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2hrlafazx.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2zvwltrwz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2uzactahk.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2npwrdloz.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lugdgcmw.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2zzvsgtxz.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2oaxhipls.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2rccfdfro.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ijsuocwj.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2hrspqaje.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2tifpbeir.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lpijyrew.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gzhqwxeb.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2wqwnqkoa.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2nvdjjmxd.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gjekfdzd.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2qleeymsp.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2miuaenjv.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ucutooup.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2gypphmiy.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2bvwoxmta.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xegeqczq.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2lwmwlgjc.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2ntiglikz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2igabrgbo.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2gtnehmik.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2nowtnkyu.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2itbhfuod.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lrgadozq.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2qswfbvei.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2tgtcbcbr.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2vmefqjil.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2kixfcytx.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2limupycn.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2patmqpsh.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xhhxopnu.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2vwlajwuw.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2fuqjuhft.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2lesvnlgd.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2apavsnxy.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2kbgvihnc.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2frqzrayo.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qgjvxfuh.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2iamtakig.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2onuaxbhz.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2snwcqona.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2pybodqgk.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2cefwsziw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2tuoyhirq.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2etmhtmzs.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2solvxqka.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2oineckql.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2pxuxoicy.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2qtjsjtns.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2nwoieooq.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2veeitvfe.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2murajpjh.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2gqxbrqrw.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2scibqcnj.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2bqwxrssy.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2nvfoovng.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ejtbhhms.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2kxheavoi.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2kilomfep.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2wcsaiatw.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fheontnm.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2qxcrybov.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ysfogqwc.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ecwigrej.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qfgkzvxp.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2fexqcofl.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2qfnczerx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2pypjmbac.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2hyrdciex.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2fkpfrvyh.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2kfhdheii.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2lyoamlis.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2jmeaphrt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jbongcnh.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2tlzpkyqw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2jpnoggkr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2mnwztmlu.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iterhbhg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2pnvzehdg.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2pxibyelp.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2wmynxtrs.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2njefpgvn.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2pgfkamow.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2hxrlvrvb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2byexawrn.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2wrxjoypy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2fkeutjyo.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2pazqghyo.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2johqgorv.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mphoxqfy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2nmuneagq.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2fuibfsbx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2xojotwqt.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2xqrcjopw.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2mhtygjnu.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2mvvadtir.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2kuuoidje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rfouzriu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fzqqnurd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ewzgcczy.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2ldtpxpap.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2irzgudjk.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ljytnhem.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2ogictezc.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2cnqvlovo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2ydttpfva.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2ropxjegj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2uuhjajhm.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2irerlmyf.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xilrnccb.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2jiesviug.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2ttfwwgtb.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2kcdsaind.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2meuddoqp.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2kfhnuxhi.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2jegkzdxd.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2uoumyjiu.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2liilgtzi.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2vujhgcer.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2odicsnsp.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2quapctbs.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2xjayiymn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2maunrhkr.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fgrsiywn.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2gvfrlzhv.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2ndxueddz.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2tufbihrh.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2xycaooyo.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2xntzksbz.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2cqudtbaa.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2dmptvvrd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2xinqeaor.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2abosxqnx.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2yvjhpmxy.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2hlqnsknt.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2izgmgnpa.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2bqinvwak.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2lnhereij.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2agwiqolt.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2nbsqrnii.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2jtqcbvhd.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2vmcpnxfv.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2kxzgsljr.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2dnoxhsaf.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2yqbgjfxv.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2nvhfleli.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2rnkelsct.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tdplbafj.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2njoegydl.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2iqockkto.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2baafwsif.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2erzvsrbo.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2ndyapinv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2xxdrckas.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2audyslej.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2eskgukxd.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2pxyhlqxt.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2hknkwurp.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2ttdmoxpa.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2otheebum.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2iuxiofrs.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2hwiojodo.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2tdnxyjtf.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2gccrgykm.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2qlhtzrvl.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2oyhxijec.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2vgjbrgwj.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2cpzjmpbj.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2hkvbebzu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2fjpwprtr.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ewfjhkpt.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2dtbwhozc.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2bchdaenl.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2iutxnnfl.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2xxgoekuh.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2dhhgogbh.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2ydcfvfci.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2ukzxxbmv.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2fwygwmbv.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ckaxmyyx.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2wzebelat.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2rlxbclhr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2dazemewo.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2mltafnui.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2sxmgeelk.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2zgzczkhy.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2tvhlywcf.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2hjautfzi.html


<!-- 参考信息 -->