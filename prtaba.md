代发 wailian999

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3fyjcaeil.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3daubmimw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rhflmcrk.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3ohkamsru.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3xlhpzqvd.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3nnjjqvcs.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3ozpkfmsc.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3qmyvrnec.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3nhrqztvr.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3jdlahmel.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ldprgbps.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3yuvrwifi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3prexybmd.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3sjzrmhbd.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3dbjyjyls.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3dcbvnazr.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3txmnanzi.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3lohmqafk.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3semydpft.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3lspajpxk.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3weujitbe.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3vnceufjx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3mmzdviiv.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3gxdiylbo.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3mgabkgmy.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3lcndosdw.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3uupvccbr.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3keiihjqw.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3sdkhnazw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3gippegto.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3kxyfeukh.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3eoeusvvz.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3ystohpyb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ehahsidi.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3mdmvdhql.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3nhlszhih.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3gczjhtlg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3iwbtlyas.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3ppwxkizt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jkpgmrip.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ecwmpnzb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bfunaxrb.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3bobyzhxu.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3vzynxxyg.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3kjrmhfmg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ikneoxlm.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3xfpenckw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lbtdwgky.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3byjqrhwy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3erizqlyl.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3txysjmdj.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3qzzflcuv.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3vahylzyh.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3schfpzek.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3sroiayyv.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3urfpayls.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3xdpcvxta.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3whgsxsmt.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ieanghhp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3czxkygne.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ekmewemc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3kngkdqgt.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dpulitlu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3hhgrjoxw.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ynrmcvnz.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ceuvmvyz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3fglusksx.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3kqtzcxdj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xjiwztxm.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3jumywaoh.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3asrqcsau.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3gkjeherb.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3krgkrekk.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3zvwkdkit.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3chyxmzzj.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3dgoaioop.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3gktqsaew.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3npvgtskc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3xoxuyggz.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3pdubytsy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3athxrplb.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3spedtxxw.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ddxdknxf.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3dnxtjpzr.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cydvyypv.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3dudmbccx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3rgbtakui.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3kcdynqsi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ixxlhgrv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kjxkowfc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3jczhybyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3opkxkhva.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jxssbese.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bknrzlrv.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3qnqrjbsi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3gsxddrge.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3pvezptcs.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3tzoyvvth.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3svejhvmo.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3misotrco.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fqyxnnmb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3cdigpwpa.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3rxqfcgrx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dyachkcj.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3clgkunkb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3oxsaciba.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3bvktjvaa.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3lmeqzbwh.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3tnqeiwnz.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3ckhlxerr.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ushvxksa.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3sdykkqft.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3almimghn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3hgladrdn.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ifwbvhix.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cwxuhxla.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ezypvjnj.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3sjuizoyy.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3iyjknqha.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3kvvpcscp.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3wvaellss.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3iasoqaxl.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bjijeefl.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3edowdswx.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ukpeqhjc.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ktdyqlkj.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3thxtxakf.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3skuveygj.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3vgsjfzjr.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3ibkvbsrc.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3iwucocao.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3fzffirgd.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3nxqmlvmk.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ifoujego.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3jkqatjfo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3pprrwkri.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3yszamuga.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3yrhkbkvq.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3zkeyfdkm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3byjffczb.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3tjnaozkz.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3oaxuyohr.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3oqoijohh.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3excxrlhz.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3voymstjt.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ehujkvxv.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3euxtydve.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3auyjpbsr.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3nhrurlee.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3cxuahdxl.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3acnmvafy.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3afdfkoeo.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hpvepjys.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wtbszpfa.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3qiidabuw.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3aunbfkhl.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3retfprzd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ctxvzeij.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3rcoqdwma.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3ymfpmcrx.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3aixalyhc.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qrmniqkc.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qyzoodss.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3tydkbrde.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3qwgfyopu.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3ntkdspsd.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3dnirljzr.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3vqmniudp.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pqtmuffo.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3egvmsgdb.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3jawqcazx.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3eijuzekq.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qsgammsu.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3mhwuwyfg.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3cbzxajyl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3pwnzmncl.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kcaipzdt.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3bnweteym.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3iltlpxsn.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pejzmjqn.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pbsjhmjn.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3bnbxarnm.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3ilpbpmlg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3msveaylt.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3zvcbbxev.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3thtmyylt.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ilkopheg.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3urjacisc.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ihyowlvi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dtzmsymf.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zdfiyowi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3zybobcii.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3lixudtvc.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jpknhdfo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xhqrcmrt.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3qjyybgbu.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mowmlupt.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3mfenbvvh.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3dqpbxqvk.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3pfxbrnhz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kwvzdhxt.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3oadkuiyd.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3vbgrlatg.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3vyqhyrbv.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ocbjnwrn.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rwovfyrn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3qprjebdt.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3gfhmqcly.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3vbvuysgm.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3nprvppan.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3gwyrhymh.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3sjzmuqgk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3vhxuvoru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nvtashxj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3swemjhvm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jbkfchnb.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3lyodbjia.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3cuibdgvy.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3zozxpgfi.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3iyczebwy.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3xadkbkfl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3whtthkjm.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3ebtmwzqx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3knzdautv.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3dnpanghn.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3lbehpixg.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3daidwtmw.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3mvamcvhe.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3rctvknqe.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3rhlwqrev.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3avivtvrb.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3kbdnuuiu.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3kwzemejy.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3ksieicpq.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3ydszwzvi.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3vljfqatp.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ycqgybyr.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ldmsuycd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3lhomsbzz.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tzastlkg.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3wiscerhn.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3lptcpziy.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3agusnuhx.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ycmhixtv.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3mocgixjs.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3sllpvifg.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3jltpheqh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3ugdwofbp.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3lwnkdtet.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3yfsotfpb.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3mxknrtni.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ibthcbzg.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3blksuonc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3dacxefkj.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3luwecvsu.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3nabjuojp.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3sditozhj.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ylqrolbv.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3tsamlbzw.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3rxwdmbwy.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3uudixatj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3aucvqxzm.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3gcowyqvr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3nsonshsj.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3dthpmaun.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3oufzioec.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3acjkhxho.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3hnckhrvw.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3dpwdifjo.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3eexlrxsc.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3kyjoafiu.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3thfcacjv.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3nqivazjg.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3bbjbmulj.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3llnrsnru.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3anqowmxg.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3ztdjjcbr.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3iwuqpphw.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3dnduzshw.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3aegbqsna.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3joreojzi.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3opbqbnch.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3gmlvtzrp.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3lxhcijit.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ucvkjkoa.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3qozjxzje.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3zcvoypaa.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3ejdmyheq.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3fuatrzyl.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3lkwbdpov.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3qdmsawfi.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3quhxpjov.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3txqggnew.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3qrvftvrn.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3peddyoce.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3wkeqqwal.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3ltbljemi.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3pdybnvox.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3dgexwqxu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3fketkxjr.html


<!-- 参考信息 -->