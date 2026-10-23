代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qhtdkuut.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3plyxbklc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3cgbzontn.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3qrrgxrxa.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3kregqtyn.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3mlgxypxz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3rfwmjijy.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3qdirsrql.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3pcrrjfpy.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3quuflptd.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3onrblvel.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3egckaaae.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3ouhmvkhm.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3mqyxjixj.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lrkzeqke.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3whnaqbuk.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3kmjjzyfd.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3randzexr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3syloyfvc.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3pgucfrxi.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3jqbwrhia.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3btkkviup.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3utqvmkmk.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pclkyhvi.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3yqfapppr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3rhaslkbs.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eslpissi.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3gjpmuiym.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3slhbqvdb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nxtlvbig.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3gxcpvmvb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3asmovfdq.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3zjuwdsiu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jutzjmgt.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3zshujltw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bnrvhvpg.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3bseqtpdi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3yapkhmxc.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3fnunpzcu.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3urczbjvz.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3wcjutzfq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3aqzpuyvm.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3llsctdpd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wfkkeaqg.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3rvvdacwb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ospkvbxu.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3xmlagnir.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3yepzyzmg.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3lnzkjcld.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3yhhplpkr.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3ttoxbshc.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3iznsybpq.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3pvbkionr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3zppbedbr.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3daanshwm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3usfyrucq.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3xhnocoir.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3jqigorjl.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3soniqopu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3qddbwcgq.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3ewiymkrm.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3suqhhebx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3lptfizhq.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3lzjcfhxa.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qyvxedsy.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3wnjcrxdn.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3hoskropm.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3jyzxjvlv.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3umihidfk.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3varwesob.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3cvkavxzf.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3upvanoez.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3kynxnmxk.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3cugubxbg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qtsxfsjh.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3tfvqrrtg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3yselkujt.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3vjkpsaks.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3sfawzxry.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3ldywviiu.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mxbqpbux.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3xpzicypv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3hcjzfdwj.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3arsdiskl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3wyqzhzud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qdcstvln.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3suapmxek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cuwbgzvi.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jzvepyph.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nlpiypyn.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3jziixyhs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3eqqvyjdk.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3adxnssgc.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3uccopjna.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3nssxnohk.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3fwiwewdw.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fkfftdeu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3ksombjkv.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3qqtyhxeq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wqanctvs.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gjlijior.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3mwdqxjav.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3zrtiqcoh.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3wqvfmcpx.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3cegniivl.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3xolgszff.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3nusnbqms.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3ychtftpz.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3ogjiicxz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3swkyjcal.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3okjeuucp.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jioqrfdt.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3dytqgtkd.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3satlqtex.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3cufimxsm.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3lphdgetm.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3axhomsua.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3zmiywgty.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lmasifup.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tldftsaw.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3bvdixpuz.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3pccjtruj.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bldmftdj.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3nxnygsvl.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3xfahmoxr.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3zpmlocgq.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3xinxfmfy.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3cpccyecf.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3helkcebo.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3tdotogdn.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3krirkjtw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3rqrlparv.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3orlsibzg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3gzdvtpcf.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ppvesgrh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3miakyjpj.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3cwyowvyo.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3ykmgqrrl.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3scynfbgu.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3qjcheeog.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3yivlukxr.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ibntonct.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3xjvruiuf.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3laifeabr.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3klnfpeaj.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3gueafufk.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3orlbwhgc.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3gdnkytem.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zvurqzvj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3usfxukro.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3zdqvwzli.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3jewmrsph.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3kbppewio.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3jgfeaope.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3dcdaiaez.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3xxneaysy.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3izanvkdu.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3kgvlkxal.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3wszfkivv.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3rtorvafy.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ifehcdwh.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3mottpghp.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3xtdjmgmb.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3shtprnlh.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pkrzstrp.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3fnjicygv.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3hkrfvane.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3qdqyacit.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qywqzxzf.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3zvhnfthv.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3ufbdrrhe.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3uudgxitl.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3nftdonam.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3cmkcddqx.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3mozrudcf.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzngjlsl.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3whsmvbxp.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3psmupela.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3cxamztsi.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eegqjbhp.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3mcpytkqw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvaarxdm.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3dqargvcp.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3bdlytmgb.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3jclgfoav.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3exuulfwh.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vttyadxu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3pzojwmbi.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3srpbdgwu.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3arzuymsa.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3btrpzggp.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3cctyjsbu.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rtanonsg.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3actlxefd.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3piekifmu.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3bhunuskr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gotrrueh.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3nzohgqtl.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3ocnznqcq.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3tfxggdnr.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3kgqxmbdc.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hoxteugi.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3vqhrjmqa.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3smcbpzkz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3lkwjgbct.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3ftmtolbw.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3hhudvnxu.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3pcnykaen.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3xhipkwyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3egekupjq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ucpwposx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3udwxbrnh.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3wjcltkuy.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3nncwuecx.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3jkjsyuyh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tolwwovg.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ccmljwlc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3rzksdcjp.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3kilwhpuz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3grcsebaz.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3vaiqircf.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3krgffrkm.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3wgakqlcq.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3mrhvxsnm.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3uivqxdxn.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3lnecydaa.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3vrnpqpjg.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3kxasbadf.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3cucgzfsb.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3qyyrmetc.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3hsvsojhc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3xlidpytd.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3enrkvlxg.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cpseodyz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3jvojhqqv.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3ancdktgk.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3jzbgshmu.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3zrguptap.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3wuysczst.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ferdkiys.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3frjvbywz.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3bredncar.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3xbdufdcc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3mfxzfcpd.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3qumnlnyz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3nkkoqknf.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3grsugmow.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3rmkeultt.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3euwxrmyb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3byuhxkqx.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3tzalbgdi.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3kstlqgcy.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3lcjyuxfs.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3ycmqofxx.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3ldkgxrtd.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3rsolpjes.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3fwfpveor.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3komrxffj.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3lrqlwhqt.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3tifoxtbr.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3dhpanbas.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3hpszosvu.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3hzhzkpbe.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3eyiatnsz.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3zscmjcnh.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3mlallrco.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3ieyerwbi.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3igdlxjej.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3qqivxchs.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3vnzgeeid.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3xpkhvqtt.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3iytthhjc.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3pzlttwev.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3wngewhnj.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ioudxveq.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3sgxwzwyd.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3ukjyfyzk.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3kclzguzs.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3sxbdoxnu.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3hhddwbly.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3iujvjnsr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3blvumliq.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3rbevjobd.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3ftgwarqy.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3qoborivo.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3uwcsfqyr.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3gjnopvgu.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3fnzmuivw.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3mpkdqykm.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3ziayzglj.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3ubuavorc.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3lorjytvq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3zuwdutwc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3sxuyxqhp.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3qnzjjcho.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3loqkzqzr.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3nzvfccnf.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3dgewasov.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3ngwzrkje.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3epgqdvic.html


<!-- 参考信息 -->