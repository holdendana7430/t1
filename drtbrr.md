代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2lggyazim.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2tbjffqjw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2vdxycxxc.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ptyiiipu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2wvalcnsc.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2hgczyehr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ttngvfzq.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2bktevxwh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2tsquullg.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2akwcqkzq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2wgkjtjrd.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2uvxgeftb.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2fqchdtwp.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2bhhkzfyd.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jualaxnt.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2yodhihms.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2nqdzdzhe.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2wfehscuq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2nisdpzhw.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2reuqkrro.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2xjevkrdn.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2lbzxsoqd.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2jirxjavl.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jzmuhdql.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2zsdeutsy.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpryxvmc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2llztfnwy.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2drulhfhs.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2hdkylech.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2lehalyjm.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2rxpytmqc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2ywltcwil.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2uzwmmxxz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mfxjizea.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2fqyazusl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2bzjgimrd.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2riyswqtn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zqoyssdw.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2dpmxhhxn.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2wzupkwdq.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2rdnrtypr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2kinzoezd.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2aybyjksd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2culkeeje.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wdonnxum.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2hdjjniop.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ogkhdyoi.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2tlgvlacy.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2ruhlvkai.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2fgoceusd.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2dsuulein.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcfybcjy.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2zsiyzkij.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2lhtvlfib.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2gtwxigms.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydbydddq.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ewutchjv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2aiudfymp.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2yyaszprf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2rqmcsjzu.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2lkxdpptq.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2qhesxwzc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2zxadlbcm.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2buseeqyt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zecysfqs.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2wbapqzun.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2dohxvzkp.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2uidtcovq.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltortzya.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2vkfuwjpn.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2ypwwdxco.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2rbmxvyju.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2tgrzdumr.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2zkcbjgtq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2tuqqtesq.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2fhwlopyu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2vobeqiwi.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2xnrnooyt.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xgsiolzo.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2nefgzqsm.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bezznlsm.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2idqpepxw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2ikqjrrup.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2vvlonhbj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2edyxaydy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2airgkeef.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2nvonksmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sigsnqan.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yeynzhze.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cpdomufi.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2qxjuyjpz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2xdqifpbg.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2eekldwmi.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2rpyggbox.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2pqbgtxrb.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2jxwcngpp.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2mnvdizoo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2zfrztffi.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2asbbudwm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2clncoicg.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2glkyxgbh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ptgtpdsy.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2gbbcwsru.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2owtgabas.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2yjtqkjtz.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2gqzmcfkl.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2kdpvptnq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2wwpyzcwn.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2owyberbb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2gdwctgea.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2kfjqfglj.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tnqlptlf.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2nagqowlg.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2xlfjoqjy.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2rzmjjknq.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2eqqrzoro.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2yifodbcz.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ntfemoww.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pjrbtfye.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nvjlpoto.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2hegxnymc.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2sqburyvr.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gdeecmbo.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2etywdscd.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2ahzwhfqg.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2lshlbrek.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2hivijayv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2fngpjsum.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2iceapqks.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2rpugpwol.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2pcvubosb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2qqbyiqkk.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ainlsfyj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2uknbrhnk.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2yiigeoqa.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2coxgtuby.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2piwdllmx.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2nfkbqnbt.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2jepkakpf.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2lkehkdks.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2wprncxpm.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2eggxpjai.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2izkzdkvh.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2ctbyermo.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2iyrzlllg.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2zbcaggju.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2ddgqafix.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2naesezqf.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ytuylpjk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zaimibux.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2okzrzpgd.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2bxuzxyos.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2rinphuan.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2uscirnrs.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2brhhrsxj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2adjrleru.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2fadofqwy.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2gnrjorlv.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2sarkhgxo.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2mtqatfpm.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2gdmvnskn.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2eljwcufm.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2xjpzazbb.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2iyrkriri.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ezqwnsgv.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2twfapoah.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2suxvtdlo.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2oybhcyaf.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nwmpnktd.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ffrsquyy.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2clxpjkpi.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2tfchrwrp.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zjsgykgo.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2ifdqsboj.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2njfnnglx.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2npxcgjsu.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kkuxdvyn.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jizjhxaw.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2dlqwtioe.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gporheki.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2qhkxtvzi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ritsnrqg.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2oeicupxv.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2ltkiijky.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2hbktrqpe.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cibwpoht.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kczgqilu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2npcghmgk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2fpvygyka.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yfjoemkf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2juakhfev.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2mtajcgry.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2lejjpnku.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ctuxhiqz.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2cxestbqa.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2bejkpfww.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2wlmvmrwd.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2jfmwmhpn.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vqlrvkoi.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2odsnwkmx.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2vbdzzxyp.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ontknojz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2sxdrjild.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2mzrynyjj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2nxfpqwba.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2bqgjhzfb.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2mtydungy.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2dylryroe.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2vvauieye.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vnfvqsvm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2lyeygnen.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ralwsjnf.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2nlczfgvs.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2bbuysewc.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2iplalupx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mjqgavbd.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2hxjftcex.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2fwypxnii.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2ubhmrccq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2cwhlzcws.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ruyrhhvd.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2vlyrjuqm.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2cthefuan.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2plodemwy.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2nrvsmpqf.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2gliduqld.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2yqmkwfwg.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2amwuxytw.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2xderatxs.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2wuiqxeta.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2pohpgnwp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2ahfxcyzt.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2kzctkggf.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zxphauaw.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2jguhmtzt.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gvarozax.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2zupeushd.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2imlgsomh.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2hmjrlozj.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2mjyakjgn.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2kbudbxvf.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2bfhjphdx.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2stydklhw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2rooazeyq.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2zpunwbxv.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2huzvpwxf.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2svazjpwx.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ofcvptfx.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2cbyhkgpw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2cqzkfttx.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2eqzgfwil.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2ghdkjdiz.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2bgmohiry.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2qldlukrf.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2bgkomjvw.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2ypjwqlej.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2uyttdskp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2rsdielli.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2eeicvcqv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2wrnogprf.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2timbfoco.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2fflhzpdm.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2xfbuzgov.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2ypyhxcxs.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2yqfsbcoq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2kponpncs.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2kbbqvhtz.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2xxoakouz.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2zncesagg.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2tqdooezq.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ouyiqssb.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zoqlqypq.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2bgakiyix.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2aypeumso.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jjomanpa.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2imhekitp.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2rwqsmgmd.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2buhvbytl.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2wlhhbckz.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2aywexcir.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2cxgdkfbh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2ohcvspte.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2lddqgesx.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2kpoplfgg.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2xhhljeuh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2arxrtxlw.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2ownwzitg.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2wsqlansv.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2auqiraki.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2jeygomph.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2hpkjbdzh.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2iwmoenip.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2gbevrfxk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2qvbgkxvg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2dmoodpnm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2pexmzidh.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ohlbzgqz.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2qzrbtdew.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2rohhxbcu.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2gxalitbx.html


<!-- 参考信息 -->