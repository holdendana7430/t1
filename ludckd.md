代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2drouvphn.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2lvupxvtr.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2xoaskysw.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2yklngisz.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2ohnolvyo.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2thlgjmhy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2gkdkmvzm.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ixttqjwv.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2igbfkjfk.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2jdwfxthl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2convoppc.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2aixbncbu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2hidmocvb.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ztbrtnuq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2qhrgutnm.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2cuxzmonk.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2rkbsvbdn.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2kybimgiy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2arpzgzws.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2fxfhxmvm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2giumkvmj.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ipecpwwu.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2fgaczjlt.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2jvgkpnri.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2izurtusd.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2uxjxbyyr.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2imagpbkr.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2dprkcxaf.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ilcnhgil.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2zwmsizja.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2morxzzsx.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2ryxqaptv.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2nzjainex.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2mlywjwpo.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2gyadeljd.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yqmfglqr.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2poekezvx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2fveddgfm.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aibodwbx.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2odmsopkh.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ggpbocvx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2sasypjby.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2mpmaclft.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2utvrgkeq.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2wfmqcael.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ayzqcjwv.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2cwewtjpk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jawekjes.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2vchuszds.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rswozxem.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2tlkrktdo.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ygunhtuo.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2nwycaydt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2lhpecmnd.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2psspjwpx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jsqjptmg.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2oitkbfvy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2wjfuwunf.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2idnjjliv.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2zozezzlq.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2pqogverj.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2wlzeqcgj.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2erljmyun.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2opgfokcn.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2pvuqzpjp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2pdessgnl.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2rfcpguto.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzozptsm.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2remqkxvc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2hwsvqnxx.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qcpggopn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2fxradwej.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2tgddrmvl.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2nwcclhlm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2rnzkfaac.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2ypasgnon.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ehgxbbao.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2mwgcortt.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ybgrmuao.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2flmlhgfm.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2caaixjzp.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2hrcwgbci.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2dyrhdjgf.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2sworutps.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ssswmnhm.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2vfehowzj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2rzvgsrrn.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2hqnvlksc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2pfepmvjy.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2wpssobfj.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mjphseuk.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2muhikfjb.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kpvhiurn.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2nrchdylt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2uqvmhdbo.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ymrbvpjv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2cnmnebsd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zfmgqstp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2pirdgbgd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dsrmipdc.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ybnptnlt.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ihzncgyr.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2bxfesjkf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2owszpgez.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2wbwatpmv.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2jqwzxmqv.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2yfyfyjdu.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2bwrhpqnl.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2rsqhiecu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2egiytsbx.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2siuktbwx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mmawjnen.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2hmxszpni.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2jqvgvyjp.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2syueriak.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2hlmtlwrj.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2dvqmgkrx.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ohsudlcb.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2mlivqdwb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2rmhxidpg.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2fvevyrrz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2zajopati.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2owaullas.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gzhufyxu.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ftsxkvjf.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2iwygfqkb.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2oerkoueg.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2hphxmjfl.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2yafkbvtw.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2jjeraamz.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qyasgdoi.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ywxburul.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2qmzdipts.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2lihzaubd.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fvlzzdbr.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2gejxryoq.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2ekwkhkap.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2hbdaipsd.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2nsezndlt.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2snhrsmuy.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2fwvnpbdd.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2imkmcewk.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2shelzhrk.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2iwgetpmd.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xecwmnxv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2dexfjwfr.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ghxhzymg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qdcugnps.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2alqhnzcq.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2rylftctp.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2wgddcwkf.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2maomselw.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2utnotelf.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ehkrlwff.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lmufjgal.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2tuquqojw.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2cqebjrru.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2uunhqqfq.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2omrebvor.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2gnbdakxq.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vtbihycc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zyafuvav.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2nubyygpt.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2vbfwjkiq.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2gmbbkndj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2kejxgkeg.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2cdbnxeyx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2zseznoyk.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2akhmbnxv.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2kkskbvsr.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2pokmtimw.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2ccusnhxy.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2kqmjppcj.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2azskdpfd.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2cgmcmasm.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2oyhgfhle.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2wmqbofbm.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2lmwvjzqq.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2ciqotnhz.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2ktvhgftc.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fqwqxvng.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2tlfdqvrn.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2bjvckvte.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2rebchowh.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fnnfxocv.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ifhlmvhv.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2dpracihr.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2brpwfsio.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2xrprabla.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2gxyasnaz.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2butkqmpy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gpowztqu.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2xfrfqwpe.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2bonrfdot.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2zfbtaxaf.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2ctosxgai.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wksgogea.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdrjuyai.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kmzsjrfz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2vfbvzoeo.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2helxnbkp.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2unnnmxfj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hducstra.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2bbsvwiyv.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2nttsccye.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hqsunzfx.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2tghujhvh.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ollvpbld.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2aormzbhv.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2cqejfkez.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2btcdwleu.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2edoteggu.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2nwdzxvzz.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gztgwyow.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2pszopdva.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2pezfqlvt.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2odgxuoyk.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2vjtayuas.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2oqytpiur.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2qvrxkrxv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2oclkfavz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vklnahqx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ybdemiqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ldnyatpv.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2cwegjwtj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2zluklfnn.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2nsypjtye.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2lwgtkiwm.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2hauctleb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2bjddzkfy.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2syytudpt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2oagtpext.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2psiceynu.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2mvcawuzf.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2dncsbant.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2xwnvmvtt.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2gflklchp.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2ppkixmgh.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2cwlmwigm.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2jtcnaoww.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2esbamqjb.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2eyjfqake.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2aqcptqun.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2tjrgigur.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2bvcwfdpq.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2csverfqt.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2oymeletp.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2etsjrbxu.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2qcrtpmrt.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2rqfeycts.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2afzlljln.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2wgykoggo.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2kayrczpl.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2uigdgzcd.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2gczrajha.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2wejpiweu.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2wnyiyrsf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2liuunqqo.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2wcgnulmj.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2tbzgovna.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2ktztmndz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2xfvtqlwk.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2loqijbye.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2wnwwffnk.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2whcguggz.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2lfseoklr.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2ipiraznj.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2lczfvgmy.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2usuhanxj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2kofwsivo.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2wqoowmeb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vkitvppl.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2mvbqgmtt.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2htzpclvv.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2dgcxmpfq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2juoinnlt.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2rrpyetvc.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2naczinqe.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2sznafjiu.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2vigsmviu.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2hhwvmamv.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2cgaawlro.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2snoxxjxf.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ioqxyhsj.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2zhhmxetm.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2lygonmoy.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2iipyarht.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2bjbkkrsf.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2dpftiidy.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2gvhwoksg.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2zledoeql.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2dyilggsi.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2wxfdrhhl.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2eyohietc.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2wiaqlkhh.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2rggxaubs.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2vyjdbgly.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2idpgxmsw.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2bmekvpfi.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2wmeqoepn.html


<!-- 参考信息 -->