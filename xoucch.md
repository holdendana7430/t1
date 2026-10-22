代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2babwndqk.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2fgaienib.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2ossavrlm.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2rgtgkxed.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ikgnlvph.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2ktabikwd.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2teuopbqc.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2bbzmtryn.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2htejhcwf.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2lcuyqhcb.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dpufblax.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2xjwetvau.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2jfyjihak.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2cwzrepaw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2kfaoltwf.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2ghyldnfg.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2lpvdbnql.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2rbmtkgxj.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2fymejmso.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kncfecvy.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2rrhxgjop.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvrqnnlk.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xkktocoz.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2tuyputov.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2hhvcgubo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vycqwiuj.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2haquyraf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vixcigdt.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2usltxyry.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fcwdgjmu.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ajjroknx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ioagbnlq.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2msmmxsel.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2igoybdsy.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2yiargenk.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2fuiysjie.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ilzcrdtp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2peodlqmi.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2btkcgwhu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2tmdaktag.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ecsppkgc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2dyoycqil.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2dddgsxia.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2rsmxtofp.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2ehwfaris.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2mtfbixps.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2epqttrik.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddmjqjid.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2jexmshfc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2brolsztc.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2sancoqyc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tohmglwu.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tpyshxfq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcvcyhiq.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mxufofaf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2eqdwprlo.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2lravsssq.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2dnnpgamh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2faxbkgsm.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2zubmbxxt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rjkbbjnu.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2eqrgrleh.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2kczzrttv.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2rdyzxsjf.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdxcyzsu.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2zatljdot.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2sdnmbzfi.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2obwesagg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2zhkfsvuz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2raeogfyp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2vusnlqck.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2xcuevjth.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2mlbdlctz.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2kjtgnclm.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2kdrtlraq.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2nvricuoe.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2tdpzmspm.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2cozujlzi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2crhnibbu.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2akyzbbmf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2stthtxgc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2usxlaata.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2amnxcnjr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gsrlqdjp.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pbovsxxu.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2anzwqfcr.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2lpuyxkpv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2jcnhzgfp.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2agsdtymu.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2clucisle.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2cjglnpkt.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2kswlhhzk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2voglhrve.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2frccnlfq.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2txiiqjgh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vgqwheed.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2eqccyqcy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2euxegrvh.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2usrumxkl.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2qnszcdmi.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2lyfnvppg.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2kvvopcpu.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2wzqjcpwq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2hsqaxvvk.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2wpkkznmr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2jazonjai.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2fskpratl.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jqnmfher.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2gbaoofjp.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qxyntrbh.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2eacnycco.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2lqwhoqhp.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2jrosbruk.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2dwvpvwhi.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xdprbzfq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cvelpyuv.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2fmhmzoku.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2ibeqfwes.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hmwgvicy.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2nhkklbik.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2dcxrwelz.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2vnkgjqjt.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2habiabbi.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2oustanua.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rvtjtkdb.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2uumbhcds.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2qravxjgx.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2jzkirvaj.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2vpfndinj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2gqpkobqv.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2xvqxigrf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vbyhklih.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2vucxfgdp.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2opviklmb.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2dusyxdoq.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2chkptbvi.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2aolyrnmy.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2ozkmqbzo.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2taesyvhb.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2nraxtfbv.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2usxsclbo.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2sfcrryna.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2mxxcqexi.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2zwjmuwbk.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cnrujtbu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2excthzeq.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ulsniujp.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2yztwzjgr.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2aqlxurnh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2josofydg.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2hrbuewki.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2ktwyqqsf.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2tcfdbvnn.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ooezdrrt.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2fdscabpd.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2visvcceu.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2yfsxiyym.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2pbdbajkr.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2mlkkhail.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2ufxumxgz.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bjzbmcav.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2twvtksbl.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2sknbtufy.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2cbrmlhry.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hyiwypdg.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ppxpebww.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2rtqynwoz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2aqapqvzc.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gluchgra.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2obozpkav.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2qgqrlnjf.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxdmcjbj.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vutgidys.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2yzqywkxc.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2iaxiwlbe.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfeecxzw.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2wqnuaosr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwmtzldo.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2krqkarvj.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2mofzsstg.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2wogradtd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jfjjvuja.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xgojkitu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2ilmfpfcg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2nackgbst.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jcjncwhe.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kwhecrpv.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2psfkuehq.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jwortxmh.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ngahnpxn.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2qtlczrbr.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2dukdpzkl.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2envparpi.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2aedkcctq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jbxkabvz.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2zudtsimt.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2bejvvzux.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2vwpllyzo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2pgjyrwtt.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2nbzxjrbi.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2dpckhwnm.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2fgkplder.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2cavbgoyl.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2sixsgjkl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2lrhttjjs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wtkqgdvq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xftssabz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xwmuzkwr.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2rzpheiat.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2wyacztjr.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2fnbrwdrp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2pczucqri.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2hbdewrsw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2comgsqun.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2biufxzha.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2pvnhwfji.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ecewcyig.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cqummylw.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2swdtglpy.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2heahzyoj.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2yclmbtoa.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2ibhgvcnq.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2ybtonoyp.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2nihpvuka.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2fjeukgfa.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2mzhlfuhb.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2twbtzhwp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2hxsiuoek.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wtdmnwnt.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qrebboni.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2xoyyhvde.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2woltnlix.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2ikhvqpsd.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2oblpuhux.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2wmuclcla.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2nufbaxsz.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2pljylufu.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2gobullfa.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2jnvdkywa.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2thnmtxwf.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2wvddqaet.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2moafamlg.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2wvmjmdca.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2qkclpvvj.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2lwguhypz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2woegikaq.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2tvrtezoo.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2cemhjukg.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2lmmhuxrq.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2cwbnkowg.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2xndrksqx.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2icndqcfg.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2vsuzwlat.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2llzyybxa.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2opztuuzn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2kdsnwvvc.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2obpahtyx.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2iopbtmuy.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2bpdgyhrp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2lwkblgak.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2nhuaomsd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2ftemsgxm.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2vvjncnze.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2dczvrljz.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2wsnkvzff.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2fyjjeqsn.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2eipapudp.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2uqvxwkhj.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2brvmeejl.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2vbpkojub.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2pnshqncc.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2acodjbzq.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2znoxvmvi.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2tvixlwrv.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2fvwpcdaa.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2lxjoybvz.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2pbpenfgj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2gpxcufuw.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ingkmsfk.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2httjbzdv.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2dvvextwb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2xtbfupav.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2nbjqxdnz.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2zwhtudly.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2asyoravc.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2vedncgzw.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2vwpppwnk.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2kikydsuy.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2hrpxckiy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2dnydifpo.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2abkcvozf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2oxmmakzz.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2qoacaxps.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2gowqsqqq.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2axwlsmbl.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2mpvdjjru.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ozftnofq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sknxtpow.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2seethkjr.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2yfyevdbu.html


<!-- 参考信息 -->