代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2rjxrcqsa.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2hbgdjxbd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2vosnnkek.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2qcynzwav.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2sxalpsmf.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2rsadzsbh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2olipriqg.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2dgtwxopy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2plckefjq.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2xihzhjds.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2cnnlwuxo.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2wlfqkrkn.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2lsnadzzr.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2xgaahedu.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ygxertvr.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2rtqlapkk.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2fmpfqhzi.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2whvduhbo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2lbuewqac.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2acjomqpm.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2eeiylkno.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2kwednsas.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2guotltdi.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lwokomaz.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2ddwqivvt.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfjiszku.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bhszqiut.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2apgnnuqv.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2zuisuydq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qnaucnqm.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2qhbjbgvu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vyadajbm.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2pwqbozmx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2stzbuter.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ntaoehlu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ejkgysxe.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2bkuziomb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2jrfwmlxu.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2aafnnygx.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2qgdvfekq.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2mdgfxwqk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2fcrlxuou.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2jqbvwovc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2yzazfdth.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2bwsocyuh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2mlpuchic.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2tcanhmgu.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2ohdszunn.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2galruftb.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2przgethk.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2oxiwwxrp.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2mhtmnehq.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ppfehqea.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2slntfruz.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2juydstsu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvddidob.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2wcggysjz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2kflwfuok.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2goyvizyq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2zevwbxbl.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2wroqgnbr.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2hxuycgrr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2vhabzweo.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2vxgwcpfu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kyeevvhz.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2drjcfyto.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2iqaqgfkq.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2cwrydjkn.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2wjegelpa.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2dlqrtgnl.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2jjclpdlx.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2jkpfaoot.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2yaiqhvmh.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ckrpbbsw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2btuhhrcq.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2kanewmgq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2jlpglsva.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2giesuryc.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2oexqpfbe.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2pgecnojx.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gcxwpqsh.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2fzxbvqus.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2nunhydzw.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2smydrcqb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2inhxqyta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jhwrbdew.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ktatsqma.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wcrpahpb.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dcqmorbb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2fiibfqut.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2psznuppi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2lzaavomx.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2xqumqzzx.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2qbnfdbkc.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2scqgvibn.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2etjqndtx.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pwbbkoqc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2flptgigl.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2xmltdoon.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pcchdnjc.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2tdoaftfn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2wbruzegb.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2bbrrifty.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2swgpddlv.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2dndgexns.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2eipzufdu.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2qdhejlaq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2egtrgsnz.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2dddkaudy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2gjfmtcwn.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2htincqeu.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fltkykci.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ccqbhhfg.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ywulcqdv.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2eqpjbjvu.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2cdvxqnsv.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2kzztlzzr.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2cvypxelg.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hyqhqfee.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gpxcpnvd.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2qcxuyesh.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2watjnyux.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jjambbbi.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2grabkraw.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2ogqqxbur.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2eygopyzw.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2bcjcpznf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2kaztlboj.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2jgmnuzbv.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2dfcsihfp.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2ktpezkrd.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xzfulybs.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ksruoekf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2pfjkytwm.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2bwojuxrl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2edeyphqw.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2alitygoy.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2qqghoczv.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ajpepqpn.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2potkgoap.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2lpznzdvz.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2bjsmyeaw.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2craqqcwu.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2rmvcvshv.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2nxnlefqx.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2czjutshq.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2lxemdzsx.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2rmsbgxro.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2eqlcdflv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lvetcolz.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2dbsmfalf.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2qrixtpgb.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2usciizde.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2lbbzhvse.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2mqgdrgxr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2oxorwiwf.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2vozwclum.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2oyfddpcs.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2fkugutut.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2ksibxsui.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2yscqbkog.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2hllfsctd.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2nfulapvj.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2thtevnfy.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2evxuqnst.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2niinahfw.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2evuwijhf.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2rhdhcojt.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pdusfagv.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2asobnsfz.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2sewpborh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2pzwawgyw.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wyxaicmo.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2dwlwolxe.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2lckakync.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ubqpensg.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pduohvfb.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wpvfmdgf.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2yucmxdoj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2wvybhqne.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2dxtbhtyq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvhcuqob.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2jamujtrn.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2fmjbefwz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ujiyfbvd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ufrqcigm.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tfjarder.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2qcmlzuug.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2sndlslei.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vfvgyxpw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2amwfcojq.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2ornyvnxy.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2zruugelc.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gbgdrelg.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ahkbdhiq.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2qtotlwce.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2thdfvcnb.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zhoncrpi.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2ilkmxxbw.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2pmsedict.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ufjdpjjh.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wmznrrqb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2qaelvjkk.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2anzuoexx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2kfnpcbrg.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2wqcdlkls.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ajzzhjpi.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2lgsyqwlp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2mkkyeama.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zkafcibv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2gvbauqzb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kzuvgnwa.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2lkikmtan.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2uybugrjq.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ryyeragl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2iconwdqm.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2iesjwcko.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2buyafxov.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2vulfcpvz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2rujctjzw.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2igoaqvdx.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2jccbxsii.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2jjqbrqod.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2wavygvkk.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2zsradmcb.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2nafxewxg.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2cjijobif.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2ctsgjmvp.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2rdmimixu.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2ktompjpw.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2xrmmeahq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2welqxngr.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2wjqfejls.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pbdfghan.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2gagyacyx.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2okeefrfe.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2delivbrh.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2uaygjytn.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2wjvrnjqy.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2hlmksjxh.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2myywkpks.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2jewroejn.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2oewqazby.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2apdaykbv.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2alpaobpg.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2utbgacuj.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2lmwpvubh.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ombcygfy.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2iewxobyu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2ykrfxoxr.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2mfmkaqty.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2imaazkrm.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2wuyohcad.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2tczixdpn.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2jahlziew.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2noyczvhs.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2qesrthzg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2ijedrlcd.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2yocavasm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2asdmdcrp.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2lrnthiwl.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2garrvvkt.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2xjxhjdxq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2jxdtciip.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2npxwjsfi.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2tupircox.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2jyztpeeg.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2tmbwwciv.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2sjseyqvd.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2tkwpytxu.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2nmpobdyt.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2xmjjkblr.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2qjhocgoi.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2fcjlguod.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2steaixuu.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2mpklvyls.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2yuaqnqbl.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2peplgerd.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2euhizxxy.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2udubvcao.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2sxblzkmx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2juzuhcwz.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2mytimvmx.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2rpamlhtz.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2unypmvrs.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2mnhqjowh.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2sgvylsru.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2qmrfddar.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2fmlqmuse.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2jpkefgbk.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2oxesrlcp.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2otmrjtdj.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2wdtwmjdn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2dkvrywhc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2zukmupzz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2yzcrayzj.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2hknvfxbc.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2byjfwpuk.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2uucrtudc.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2wxzvwjaq.html


<!-- 参考信息 -->