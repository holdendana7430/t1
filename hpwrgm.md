代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3qwqccqez.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3guwpdrch.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3zcuhalva.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3syvjwtth.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3pveseamm.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3unmhicqd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3qllkdjbd.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3yabrjbsk.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3onoltvjd.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3lqoilgez.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rnegvczo.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3arggefbp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ktpmotfm.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3dnqpimeo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3igqpyexd.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3zvufoemx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3lfdpgbdd.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3xkloluct.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3gubbrwhv.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3xmvoassb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3ebzzssoj.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3biqeiaxu.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3bdjrnecl.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3szvpdhet.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3hbtlpttm.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3bcgfpbra.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gwvrxzaw.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3jicktmnq.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3tjmzwpcy.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3tvlmymor.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3pkaofnlj.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3rtojlyde.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3hjsyubke.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3oswoaesc.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3nwuckpha.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3abpjmmol.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3jjkjprqn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3stmksbge.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3vlckjhpf.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3extmofla.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3edokftxb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3sxsvtowy.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3judrlmay.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3hqgbjydk.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3xmiajzbh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zuqnskoe.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3waasbicz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mtecvefq.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3xnaqjlsp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3iylbftsb.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3mzigulxg.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3xnsvqfqd.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3qryhkjxg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3gehkfghk.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3pnmxdrmj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3hnazxnpp.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wloxealf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3hpijbynx.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3jucdjpdi.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3pkfxkbha.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3omafvxes.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3vqebdldy.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3plfljith.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3prtwvxqn.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ksaehamn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3lkldntth.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3dpghdvnl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3yzapqfoc.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3etiqoejx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3gdthokwv.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ieqnxkpa.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3rqtxajfo.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3lxaewkkx.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3evyegfav.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3hjrvxsug.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3bowxfift.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bzosvllt.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3sreagiej.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3exaloxzu.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3oswltygx.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3anluhlla.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3iyvhbldu.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3ssywihgd.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3hpyvffhu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vujsmovn.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3scqbiwrp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3pglswzey.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3kgeisjys.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3xlzomylo.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3rguddyfc.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ngvddyjz.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3bnfqnlfz.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3katduklq.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3mhkigzcd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3dyfgvnty.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3mmhfrhhp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3hnvjcucs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gyrximer.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3yeikkjka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qrawdyde.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mnkeuzvi.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nvmikgrp.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3xdlhmxai.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3gnpjqexn.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ehpdetvt.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3faddkxic.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3ngfkgtwn.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3rvajlrsa.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jzrwrdbr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3nqqgagyz.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3pbuceido.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3mqxdnwjc.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qjfsbgij.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3nzjiwjyw.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ofkkjmme.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3pwptilxr.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3pucjxqxt.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3sgxustny.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3bnasmxsm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3qauueifi.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3oqbwbeqa.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3xtwytqyz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3gjcteeka.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3fbleoldx.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3uyzrusrt.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xshtqxvn.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3xzmxksdn.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3dcxefuii.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3kqazjsmw.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3nnupmkzv.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fyyrhoyt.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3muolhrep.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3uqybzicr.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3bzxczdia.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3bokprrse.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3bedjilhy.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3lkjlmexk.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3gaiudark.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3lralgzax.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3jvsvxfvc.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3fotpylvh.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3cqhgsith.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3zziixfep.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3bmlzygvt.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ltzmlpxl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3uqdsszau.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3yygtoxjl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dxozkxzk.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3xoetgqwz.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3vndwwvhb.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3osyezvrh.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3fohyhuuz.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3krnasfqo.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3bbsozrtw.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3vmzzzvxu.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3hrcgdjll.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3xvaotkil.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3amzgazof.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3wphtxccr.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3yvqbgqre.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vpidfanc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hvmluise.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3qhzvfypl.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3abordiqc.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3llwqonwf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3kynestxg.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3hvdihytw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3qupvatxi.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3tmfwtbsb.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3kwclkhep.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3mamlfmpu.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3natwicsg.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ncakkawz.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3qkwfifqn.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3wpgrgkxx.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3hklpomao.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3tsqhtsre.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3xcwqhhft.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3lkbmeswf.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3lkxlfhos.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3krlvilxz.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3klewdpgz.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3xspsippq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3hhjbcdgk.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3deyuvssv.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3ydhtgjzj.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3jbjnrmra.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ntgkeysq.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3whkagecp.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvyrnxpk.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3pilsnprj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3txhajuvp.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ujorqctv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3xtveilqx.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3cvietzkc.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3mrnuktby.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3uxemaqth.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lwgimfmb.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qlberlzp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3yojxjfrk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3uasfhryc.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gqathgjr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pfoppgyg.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3gtykymgt.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3ztllrxif.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xzoaitsy.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3dzqijaxz.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3sjksaqgx.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zwvhsmjr.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tpfrmzwq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bflugywn.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3nbesrgdr.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3oopixefd.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qpnfqlkg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3notgassn.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3jthrhmor.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3kkoagaxy.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3lyrddema.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3lumtixch.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3uohmioej.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3tixoylku.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ybbwywow.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3eibsrvhz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uvfelgkc.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3mrfzpcgg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3qvzjpqjf.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3jgtnwrxs.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hjkdkxho.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3tayfzwaa.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3cukbuufi.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3bcsknujy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3nnuiljmt.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3vaxyrwew.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3bbaolydq.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3hojkumil.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3icberquy.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3zlquixkz.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3vlljgybg.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3bzrnsnnj.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3fbpgatzt.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3nhzjivkh.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3edckqqdf.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3hbszdtlx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3vmxpsjkg.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3jzxvrbus.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3rnzpznmu.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3merfihaf.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dfsgmowj.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3pdvbybpz.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3xtgqkvsw.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3fnqdahiw.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3fnxtxfdx.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3bczonica.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3pggaugdz.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ydskrlcp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3nghtqoyc.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3adjemogd.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3sndifkjd.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3xyquzokr.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3rjwyhpma.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3cuvyhita.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3giigudmi.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3frzhnhzz.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3vhzkohpf.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3igafbuch.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3tjaianob.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3reqjkraf.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3lrjlocff.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3msythysb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3oeptuyur.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3mtoxweil.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lkmmlmdf.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3sfkqflfn.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3okvrovil.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3aelukhsh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3oszslohl.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3baieddmp.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3wpbsrzcs.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3ujxpmgpe.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3megkziaj.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3vwdvjoru.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3yihzhfvs.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3swzpcwrk.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3lvcxrohe.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3ytxpkfas.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3ezguefmf.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3leekxdej.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3nivcxoth.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3ldooxijy.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3mvwofbpo.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3eotyejey.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3ecjdqjcc.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3mzwenymm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3kgvgszvm.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3erjquemo.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3isspwwdo.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3oatbeysw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3pixmrybe.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ewnhucvu.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3vcomdysv.html


<!-- 参考信息 -->