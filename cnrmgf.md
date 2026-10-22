代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2kbrfcllu.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2oiqunqkb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2lvwgegzd.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2dpbtmwfw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2fwmztfaa.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2odhvqukg.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2vruuaeom.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2zxucappy.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2cnouposr.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2yisfpxdy.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vcxaqcux.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2krgzhynp.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2xxevetme.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2nvczdamd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2lepkzzol.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2leqlejrt.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2mbcaamtg.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2reizngpc.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ftilowni.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kceaozpi.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2jfaqakgc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghvpqsjx.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2ivrxjvbb.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2hyygkxhc.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ooprrmty.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2enbzwyjg.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2gucgcckn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2boqjwdgz.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2peubfvjm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2bsiyprds.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2lzkjdkhe.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2loullgqq.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2jorqaumx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kssrnbas.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2bqpxplbh.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2lqqwcwmf.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2wsxqnkyk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2vradcafx.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2rgtynnji.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yztalstu.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ciynrlgq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2xltwxckh.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2yhmvnpyc.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2zglqxxdv.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2utljyupn.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2xfdurtql.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2woppifle.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2jolcntqi.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2absliskl.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2hrpgskqx.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2osnfqwmd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2uvnyfngk.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2fjxhrhmi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ueojwwyr.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2sbwkmlup.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2bhgebabq.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2lirlzqge.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2bwxieysm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2enxuvpdu.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2sriyiihd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vqqjooud.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2jnejjikj.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2vvfvxqzy.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2xhdvqwqi.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2guomkkkn.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2ulctwxva.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2yogdydqu.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2vyvuxvtc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2pkbtnvfh.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2vodwdeln.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dnormfid.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2jbfknfbc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2dthkexik.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2nhqkypgw.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2olupvqyh.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2evaekrap.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2hotzcvkc.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2wgcrclok.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2vmpdbbwc.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2yajsrtyq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2zteenbcm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vrquwgaq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2qquenlws.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2glejjtli.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nkdtsupx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fmjilhtr.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2bagooylr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2uyctmynp.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2eesjzgxn.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ltsukjtb.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2yktqssfz.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2qepzpcte.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2fdiwypgt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2guwxsgmq.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ihccxqsh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2thrxgpgt.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2migolicw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2ctwlfeil.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2uunyguoe.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2qqbsfinn.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ksjzjwpi.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2zgqdyszp.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2lljctess.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ddyioksq.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2jopjfgdy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2cqzilgul.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2bmedcfxk.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bdoymouf.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2jzcbdgxb.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2euuklsov.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2wcyjigkh.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2hrfryanh.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2olxcblvm.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2hifmajub.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hnuwmwoo.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nomgpyau.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2gitzigew.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2xlchdise.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2iwmdavwb.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2hmlszcgj.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2ovxqzpxn.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2xmifajmn.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2poszyeju.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2lhgabjhj.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2blcdlxsw.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2qaczptzd.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2gbgwirdc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2dvohhghe.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2oxrhampn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2hntpryuk.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2hvxbmiqx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nsrsokkw.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2dnkcghmx.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2nxtowkaq.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2whisomnp.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2sbneirqa.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2yftirbjp.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2bhsoyfwm.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gxxqwjmy.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2guqtetdy.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2yqfggyyi.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2hvtawfjd.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2ditutfur.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2whaeeuat.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wpdrkplk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lxoesbct.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2fyvhmbnp.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2wsphshni.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2xrmwjsto.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2cbbwclkx.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2epxvdjpg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2gbcdejkp.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2eiyqaciy.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2kbvouhos.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2fhakcaif.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2zjriddin.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ngduglzj.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2zlnhvzbs.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2dkmxsatd.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2cxoswkau.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2wvzgkfav.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2qmodsxac.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ngyhvnke.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2seosynob.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nowokith.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2ntadumtj.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2wsvmkwhi.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2bvbottwb.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ntpgxmjr.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2mvyrethw.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2vduwylwu.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2awfdgnud.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2jumfocum.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxmozsyx.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2vvtgghfl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2zmpsczse.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2yuxxocmp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ggrsmytr.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2gymnzode.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2gvrcnrdu.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2hjohjudt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bvazfebh.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mcntwzay.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2nlzkopfq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2balcayic.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gqflafyn.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rllmgadq.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2mhgyqaxm.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2zqsqqddm.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kdeviufz.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2vhzmmtsw.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2sgwzprvn.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2lkpxqfsr.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jxijuglw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2mtghrhhd.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2xakppqjp.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2bkifsrha.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2vjxpklox.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2wckxpfgj.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2yzeruftl.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2jqzicnpl.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2rqdsngpi.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2dinhbqua.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2okeqcsop.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2emsjrfku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2snnkknaf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2knonumrr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xpotaokd.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2gesnuwlq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2mhssyfhb.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2thellvmc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bmkbtfqq.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2ywledzpz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2aozkkjqb.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2ftddfwkg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2uomsapej.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2mengmkum.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wrgfqglx.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2ygeqmstf.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2lmsobszw.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2wzwpkifl.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2rkomztnl.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2pmflqgye.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ryvfzwtj.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2wvwtpuxn.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2jlyrqlqz.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2yoqispsp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2aevfetvj.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2xusjwgqg.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2svvqiyrq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2faxazpcg.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2mcyrioxr.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2inkkugse.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2psstxtwo.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2heccvneo.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2bseujjyz.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2dmiqnnhj.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2ejsvhjvq.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2joohqzvc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2mgjvazru.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2kpxjquxc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2talubppw.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2hdjfcpgk.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2rrlyqbxn.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2kszykgic.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2niziyzgx.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2hdqkrqqx.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2stddlvbo.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2qiiegsai.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2smzgojct.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ihauseel.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2jpblmsot.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2igpokkkv.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2gipgvllg.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2exswcegw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2fsujmknv.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2cexpxvvf.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2wnfxarsv.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2eoigyvrg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2ipaqjcqu.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2pemylhci.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2xlspckkv.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2zsgsthnz.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2tuofqgpe.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2mbiaclvb.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2whuyotsj.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2gauacdtb.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pvsdzjxa.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2dwumjixk.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2ombqtpbj.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ecdwhvgl.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2hyhrcufl.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2jwmpjybt.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2bmhnnkkb.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2vfyhoqqc.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2leyiamjt.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2gqvgggve.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2tdzvrqsw.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2lsioyhfu.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2qqqcuwkl.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2gbetjnxt.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2yuujleql.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2zneqwyax.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2buunjrvs.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2kbtqsblo.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2juyygake.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2pbmimmfx.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2qlfxqlmv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2ytxlbnlp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2vhlebcwb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2nkjynrbi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2xiqhzjbu.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2kcwtprxn.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2eqnxjlvc.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2tuxayseo.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2zpghbsll.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2oezyaaqh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2cnxmxzkb.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2yfbjlosf.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2jhqgshwz.html


<!-- 参考信息 -->