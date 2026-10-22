代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2ibkvrivr.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2hxuewptf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2nvmhyalt.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2zblkzrms.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ozorrped.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2auhoftwj.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2gihqoujr.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2zzyaclxd.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2scuisnec.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2qmpuxskc.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ehnuhjvf.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2pzhzcsqw.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2omisesbj.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2jlxouukk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2nahfiela.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2umrvmieg.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2bhzawzky.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2sfpbawdd.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2xfcussks.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vsuqtuzz.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2yklzuqlo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2uspxjzao.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2sbtcnyoj.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2hoigcztv.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2mzukwkei.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ykrdvitf.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ghhrdjwv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpzmwdsg.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2qfthbyzo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mjeuavhp.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ltkupjnk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tmwdodpe.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2ogkaviri.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2prfcctqy.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2zqsvgwda.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2dyrqbkae.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2bapyzhsg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2hsutxgoe.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2usxqxsii.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dmisrvmc.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2egoaoasi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2aqjwymwk.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2sctfkwjk.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2wbvfdbjp.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2qfyjcswg.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2wyfzmsgu.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2tudhdnbm.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2gwigwihi.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ejxuhemh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2fhdsruht.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2yqpdlorj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2aqyxlcie.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2xjowegcb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2vwheuuow.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ltfyliie.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2nrxuxnhc.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2stwgpawu.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2nkccygoi.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2fntezstl.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2nmmywwpd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bcomeotl.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2qcbtfuhy.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2sbeppajs.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2xomxywrf.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2olwtxqmc.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2wftptynl.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2rahbwwts.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2xmbykkir.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2geejmvwc.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2gnlxsjlw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fpcuqecb.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2lmaaivwm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ipeyjide.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2anvritts.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2azdlzubb.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2hjgijrxh.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2hejttbsh.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2yulkorix.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2qvlsonit.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2qlaqummw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2irjszdgp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cgoygbkn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ncfafkfh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2snsakjew.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hdowpqii.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rhgcgrzu.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2driilzrg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2aslhsufn.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ppbzhdoi.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2voevibxl.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2czrfqyeh.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2nyenvixj.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2zgmjviph.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2pqqrnxpk.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2clqhlxrk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2dvlrtskd.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2flgmiifk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2vsavcxyc.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2yqkrzdpe.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2bufppkwk.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2vnsyorco.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2tfgbxmbf.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2qoyqyrht.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2kvijokhl.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2ttgqnqrt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2xzaktmfl.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2xdgufowj.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gpayjdrr.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2xihfduzl.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fznegjth.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2njudpfri.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vdzpmayl.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2nlglhptj.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2xpelhllq.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ngwpqlow.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2yobndziz.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2bzgwlccf.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hltaolwf.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jmxqexec.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2moujyqio.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2onozsdwx.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2ohqrxffw.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2tilfxvno.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2wzxihczn.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2znivhttx.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2rnbhfeou.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2xectvnhx.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2dzwsulqr.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2upljhflt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2ouubhody.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2wpoufaoz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2tigmkthl.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2gwdynucu.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2ptpmanan.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ykxolyvu.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2aqrpseji.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2ttyuvmzl.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2hrzbhkom.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2fopdzlnl.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2ddyyzonu.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2kfslgpqq.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2uupxzzfl.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2grovufvy.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2ipmqsuod.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lvqsnwsu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gvpskfvd.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2fvfqbgga.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2mcgqoztg.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2qzezduet.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2rzwjutui.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2podkmgtz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2vtfdgozt.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2jykenqqh.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2dtpwhsfx.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2zgiuolkn.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2ehiwumsj.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2npqsdhzt.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2udrbepqd.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2fqhmjwsq.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2lcbasboe.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rbmucugv.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2bzcdgsty.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2xnqbwcro.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2jorqnnfg.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2outfdxvc.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2uqgiepar.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ldorufoa.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2sfactkdp.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ajttjxuu.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2dhbcyafl.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2cqxcfenk.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozhbqyvj.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gqzipbyd.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2honjtwxp.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2deipcnrf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylobopoz.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2xowsdxhs.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2cuereetn.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2nvsqxlaz.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2aawabwly.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2cbohkjbj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgykvprh.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xnkemipg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2ppmsnngv.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2wvtclele.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2oyntgarf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2miojbdvk.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2xpwcuapm.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2lupnppgg.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2yofjmzhw.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2dkdqflus.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ewntjpzj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xwamdgea.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2aefwugks.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2exxjgfbg.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2cmilhojd.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2eqplmpkc.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2smokckzg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2szzxojbj.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2aerszcra.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2kzesqiic.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2jrlvlaeo.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2aqmlmjof.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2jqsrkjzf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2rlgtllri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fianhegg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fqmmulol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cwmyprci.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2glapmkwi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2tgdbkiqy.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ziomgjcg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2wtefqngf.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2fqjkszcz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2pznpukfr.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2blfhyehg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2nafjdbcf.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2dnhhnbtm.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2bqaixxvw.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2aslxarqm.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2mfssefae.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2mxtoauiu.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2ofelgdsk.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2nbnjthba.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2peuozqye.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2spxqlaya.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2mpvglsmb.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2ioaxxutz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2xctvsdkk.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2hlaycubt.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2qoyfpsbz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2lnayyexs.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pxtltith.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2zwjspzxj.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2wrhgbpol.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2sibfpzbv.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2yrpqwtbg.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2uyjhmyrd.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2jbzxgret.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2awofhjpt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2cnybqgqs.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2btjvtfyu.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2udscemjl.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2ohylmedf.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2tabjhlmh.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2istmhtru.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2iqebdcyc.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2htchtpwy.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2zusktlie.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2vaqhiojk.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2sngpldps.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2kjmqieeo.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2ofmrivps.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2evgxkkja.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2uvlvwhhr.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2esnnobgw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ggzormgz.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2bhnyggap.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2mxneqmbx.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2xeobzfxe.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2lvuexqiz.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2kmmsixom.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2juvhelhc.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2jgidliml.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2eupramut.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2haoapkne.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2rcrsfjme.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2dagqtwce.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wyfdvqgf.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2jpmhgonp.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2qxadszzp.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2czcqaycf.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2zycfemwe.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2bpvezgpv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2abeahfns.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2nptmmjgp.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2lputzpal.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2kiwmqviw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2optfyjae.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2abizqwda.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2xafnqqao.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2bjauhdpb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2iksewqsb.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2ipnhccbh.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2uoonxcub.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2nafhtddx.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2htvqumrk.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2fsuluvdt.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2rfaesbmn.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2dbmwhpmu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2ihzhplxd.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2zbwzhekx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2nadposeh.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ueufxpde.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2hmfferkj.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2znlcfass.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2qhzlawjj.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2izmcfrpd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vasdfbiy.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2dperdpnr.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2qnsltcrr.html


<!-- 参考信息 -->