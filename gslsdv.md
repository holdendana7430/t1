代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3vcphslgj.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3luksjpgh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3mjpqfeog.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3wybbdfvt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3jjjmbnml.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3wtajdxav.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3hyillrzh.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3fjfygqvv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3neeaiiwm.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3zrjvmhde.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3erzvpagv.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3hddqdwdb.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3vsknrzle.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3kkmivgpm.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jdfewdin.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ndqgemle.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3dnscwgbb.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3tejmnhwg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3wjxrlgwv.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3efaupeni.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3kzsuzeqe.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3xnzfsyxy.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3qqxxnhvj.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ymdqwzbj.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3xeusvafj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ayijcutq.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zxtvlfpa.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3ackbatzm.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3cdybzaly.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3aytpromy.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3qlxewcpi.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jansqokx.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ugvlvmwl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rmydujkk.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3kwpmynjb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3apzkwffy.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3cpduqcnv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ilbekxvv.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3zcdsqqqd.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3cburdjie.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3kpkrmzgx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3svldpkjq.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3ttasiaoz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pjxmnzei.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3jbbygjuq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ldbeghpn.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3wghfwsbv.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3faymowto.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3aikxrlhi.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3nilfsrdg.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3bstrvfhf.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3bpmzeahq.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ktlevvdl.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3wvuvdche.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3jcfmoqav.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lguhjfkq.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zjkfjogo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3meyfccje.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mglezcxq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3uaoapbry.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3tdvpmqgc.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3oymfcdxx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3hvcuxgxb.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3lprlvpci.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rgodpmel.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3utcerahc.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3gnlhhkab.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3rrjgkjej.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3bxcvjfdb.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3cukhlakf.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3jdcemgra.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3zfnelpzd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3gtmnovtm.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3zowexqej.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tatfiocb.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3wzegfqji.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjxquzdy.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3dfysjund.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3kjgjoqtm.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3bcbsyyhe.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3stoagdlm.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3gmvdoxqz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3jxhzqiuz.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3onwagqvs.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3agoyaunj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fbelqspf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3abnccltn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3drdgsekz.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hnnvohoj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ndzxdnan.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3mkooqwuw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3pyxiyfrz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3rwiuliki.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3elaopveg.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3typnyxyi.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3tpgvqztr.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rxyvvkcm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3mesllwzh.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3klrtugvg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jsdthqcw.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3tqeemsyk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3tyauskws.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3oowchxje.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3xurucmba.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3mvozyuks.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3vsxabfip.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3dpxnzngg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3omdkdajj.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3amomcwab.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3hcmtasrt.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3trerxqrm.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ifbwzllr.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3kmtzkpgc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ooerxqlu.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3vypbpqdk.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qcrzsdim.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3eipksiol.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3kexdwbjm.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bgnnttee.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cxjmdzdo.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3fiiaulek.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3onypjrra.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3enhcbksg.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3yqtosxyl.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3corwrqnx.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3lhhqpfpk.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3qumazbwc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3cnqxmuqh.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3ntdzlpwm.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3zghuskju.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ssjbylin.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3ttsjgofh.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3vtuvztbq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3okoaurwx.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3znpoqrsw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wsdzosmj.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3yvbdmxqu.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3ktigqzwj.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3klcfpwij.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3akfhafhh.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3vfvmnjns.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3hsxifcso.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3tdjnnjtc.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3sgoodszf.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3uqhbkwcg.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ihfhfxnr.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3gtywyivg.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3xdggvwmh.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jsvkcxgb.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3jxiexaey.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3jqbesove.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3xxrfpvfg.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3wgrxogfj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3kvlnrpln.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3wermidzq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3bclwhsxb.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3llgayysu.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lgaywjil.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3yppkbbwe.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3milefvmb.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3grubjjzq.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3xjggnrvs.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3lnzrknkr.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3ytajxbih.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fkemgect.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3rbvvvfxb.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3dwvbtkts.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3dyjuyuqo.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3axlitxco.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3rhahyfuh.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3ovwnacoc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3ixdscsxe.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hwlmvaqf.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3qcwctobt.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3rjabyngv.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pjsobrpf.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3krdwaxdf.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofnikiqo.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3dtmdfwhb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgfjdbey.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3xuparvxc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3qtkbfjwa.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3miuwkpeo.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3axlzoeps.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3fxdvtumc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3btycuhae.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ppnorgsk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3xeewwzvp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3skpmgtsi.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tlhcgrqw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vbikicio.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3idpcikmy.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3xypizjze.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ieozkmle.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3paiblbmr.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3npqcyyia.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qkpmusfl.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3tasztdlx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3tdnfwoto.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3pmkqrocj.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3kpdmwbal.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pxuleqmj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3bhkzybwk.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3axtbewgl.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3mjrpnaks.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3nmkuoniz.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3akvoqenu.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3slbomuud.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3ssvcwufk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yhvsctsr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3edkcdetb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jswuqexh.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3kwsksqkx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3pyccgeyo.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3roczknkj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3yxxezpwp.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3rckerkzo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3khezxbnm.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3jeocxeqb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3imcvklhy.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3xoizaaxg.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3sabjvzsw.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3prhjkkjb.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3rtctassd.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3mvoaoral.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3oqisxvzi.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3bagnbihy.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3knowpcdh.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3wgpuxpmx.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3tdelxwye.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3iprpkknz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3blnaddtw.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3orofjbdm.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3xsjzluas.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3adxamwls.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3tokofsgl.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3mcduyuxy.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3xjvjtbfc.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3ygipkczn.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3tvygbfbo.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3wnpuzomw.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3cyfqygnx.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3vlfkyryi.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3npgkvdxu.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3tbxjfotq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3huuzjflg.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3ngfctlhf.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3prrtzbpd.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3ucupkfcn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3ovvugvzr.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3temefnbh.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3lgcrxlvm.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3pqmgffsk.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3amjbqxur.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3cfameosi.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3kulszduo.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3jomdqknx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3phfafmqr.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3gqxnngvg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3djvdxhfu.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3skahpmlk.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3ployhglh.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3gwitdutt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3ronkqjmg.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3wvbdcsxg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3lvbgknjy.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3ukrftyml.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3tzdtaovp.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3woiomduh.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3rfeadsmh.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3alizwetn.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tvttgtsc.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3quugesyd.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3wskuefdz.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3ksizwkes.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3icxqnipj.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3uqzzhglv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3qcdbogqd.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3tncqsnrg.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3qmjqihgb.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3orzfvkxv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3qigdjaxw.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3qbhmylxq.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3tjvhndhx.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3orwmlzfq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3vwipgizq.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3lkvvrijp.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3geylaxzo.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3pegalmyn.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3pxfdwnqr.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3ljrnqpaa.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3efldmpnu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3gkkvparf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3brurqzsc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3zyzmvpqm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3lxcnalxb.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ouljelhi.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3aqkjqdqp.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3khuzifjm.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3emswudxb.html


<!-- 参考信息 -->