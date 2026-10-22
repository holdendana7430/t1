代发 wailian999

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2jlbwuuip.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cdtuhwmv.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2nmsdpobx.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2xnqliamb.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2dsvdaraj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2wmtccrvt.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2uirgrogi.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2fkxoejlh.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2biqfesnh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lqaecvyh.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2hqmsxprn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2idgeilqq.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2lwnqvxhy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2dpyboodm.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2xeluviqx.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2pdsahiyy.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2yojgxhps.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2cupifgmk.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2avzjadbw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2lthkkttp.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2rrzgcfcl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2spogbdee.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ryulmvii.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2svwdtqwj.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2empitfmg.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ymxfznsc.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2vtaedeys.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwuqbkap.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2sskcipmk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2lfrhrmuk.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2dapqxblw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tyrrgvgv.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2zwcdlexj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqbgsanz.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qfvhcvos.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2orkecgkh.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2llkdmcld.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2yoquncxz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2burfrfbo.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2yvdsccsq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ojwbgyzc.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2nxjdnodd.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ciovhvuf.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2jcatfkqi.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2gpehrxap.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2sqdchllk.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2bfaypesp.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2vvjgenqt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2istjkyah.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qxhqyimz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2pxpmxxpp.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2efhevkqz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2wheqdmdr.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2alvcltti.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2exkndnbm.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2lsxggasy.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2yjgrqvcf.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2qpmllenq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2wmqqyaup.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2uyhcaszh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2udeiqqgn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ukdhydjn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2mcdcjejc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ipzjdrpj.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fxpxotkf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2yqduxhpu.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2vinphmkv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2pfduwlze.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2hvivcwfk.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ttkqxvzp.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2hldgcggy.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2kztpwqmo.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2hyibuklb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2dbcyyecn.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2jgmhyhpj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jczxiamo.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2nyfvbiht.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2vuqylibz.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2gyxqbboq.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2vskxvclt.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2wahaccqz.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2opaizmzm.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2bnmyxoot.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2uhyfrkhi.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2foydidrl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2pwlipjws.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2wlwwsmsb.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fazuhasr.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ikyqdhjg.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rlevwqnz.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2gmbvyzbk.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2drkhqovv.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2enlybohu.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2ypkphhbr.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2druplled.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2nfgccfsi.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2ijqxnxib.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2uajechoa.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fqvwcgtp.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2mslthdho.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2nthwxvwc.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2spzsjubg.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2zgrvrwov.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2lvawwasa.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lmqfyulg.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2uyhmjruw.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2noqwxzkw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ipgjdvvq.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qmvrjozv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2icpwrbfe.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2errtlmoi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wzxjztnm.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2fevbmhmv.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2xtdtzucc.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2tvgxrmqq.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2lcfatclz.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2fwpvlkok.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ueyzhaku.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2qjjoobri.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2vbqfahys.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2igpismad.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2ixajemcm.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2pfqrayae.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2qdjtxqff.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qdjhudzz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2usqrhxtk.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2isyhiffg.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2svjvwilp.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2nmrolvde.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2jqlnivzc.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2sowllutz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2yhakgjfw.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2jpaqhhun.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2giyyugmi.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2netsgqmn.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2qanarrwk.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2qjacrhsn.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2crcqczci.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2xxlltrke.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2jygolsre.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2bvjqrepf.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2wtrmysvy.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2logpvkeo.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2juyacuhj.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ceugzcyy.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2dbqtenhw.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2adskpvvx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2aaejjxdi.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kbathwtb.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2srmsnepv.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2duphhumy.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymepzvim.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tymaesdx.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rwhffvlt.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2guwyaogn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2zjvaechz.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2khcflvzn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gylgauku.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2kgfteccd.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2flqqmtcx.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2fpftadlr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwdlbxgo.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2txwoajau.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2ejbwkyas.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2oetqkxld.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hofttrox.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2diyyhagy.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2twskihwn.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2avkywziq.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vnhxjrhk.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2huapuysw.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2zyrqwudv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kizojoer.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gftiposp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2naqonqlr.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2uqrstlfm.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2vgkffsdd.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zrktuxpz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ryhcrdmt.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2bekzotuf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2wnqtlfrt.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2sgzxngkq.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ipghbdvf.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2jihsabeh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2tfwkxbea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nauzvnkl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2paypklho.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lkeysfwu.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2oeygygxd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2jajbuybc.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ikxribnb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2hvoabkab.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2flzayirg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2olsbhxac.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2rcyrmnrq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ilfaabge.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2lrbkvgat.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2abvqevsd.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2couszlpl.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2nwveanzi.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2uxnmiuez.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2xrauecqe.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2upijzjym.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2hgrouote.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ujhlivcp.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2pybdozob.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2nohxztsa.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2mfrjoxkb.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2rfkyuwov.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2fiuynufi.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2fzafooau.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zgsfaxpd.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2jdlmsfnt.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2ngwdnove.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2wezlfbmf.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2kktiersk.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2zrrtgjhi.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2xrmrxxxi.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2qpgcsncu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2vohvjxlr.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2fnhlmssd.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2jqwtbsyx.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2qubrgzlo.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2psutvzmz.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2crpwvuoe.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2anonrkvw.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2tqtdwsyn.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2bzekswib.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2oexyytwx.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2yvwmiisg.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2cpmqphmj.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2dbywaxhx.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2qelxfjax.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2ynulonqo.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2qcrhagoa.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mahdyids.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2nivclhqq.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2wqzwglea.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2hzlrxzzg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2jxqhluws.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2hyatdcby.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2pjkyuhbh.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2hjnbifoj.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2qgunsgcs.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2nuyuycfw.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2ejgdxoiv.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2igbzrose.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2odrclpnj.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2dgwdbgkx.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2znkuqbrn.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2prdisxfd.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2iqdcbimc.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2erfpisqs.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2uhmynpwl.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2jsdossxr.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2qjqyppfp.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2qjqlbkes.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2ndtdlnpr.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ipgmiymg.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2xcmbkqlq.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2psdfnjig.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2foiqmaza.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2swgszlas.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2gchnofqf.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2kihafzrv.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2uveyswgj.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ucxofswp.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2npbrvgoa.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2dfohygfp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2gfatsihs.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2wmizqnkd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2hbrssrnn.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2ckxaojec.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2ghrnpkpw.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2yapchctv.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2lwjpqmmy.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2utibmfqc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghenbekb.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2swqzgsln.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2dkaqzkfo.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2kpypkglw.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2oajnayjl.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2plcapzii.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2xlfcwrqj.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2gboaydzi.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2cgvykilx.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2omlaizxl.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iuqhntpr.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2urfwlsxv.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2hyonikfj.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2sqhbzvlu.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2gytluymf.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2noianphm.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2jyrlbltz.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2boplelhd.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2izdyruoe.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2msxakdyk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2kqjryuhh.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2jaxmkmxl.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2plkulyjo.html


<!-- 参考信息 -->