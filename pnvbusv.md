代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/getxqxioo.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/gxqcsjipk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gcpbkjinf.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gqspkbtmo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/gfosfhfil.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gqzvxhyqa.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/gfuhpvulv.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/gwoklrwhn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/ggrrsrddv.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/gxcrascja.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gpqgmnxna.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gjvupmroc.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gvducmydj.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/gnlkkydad.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/grsltiwqi.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gxrizafaj.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/gltxldzlo.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/gmzhclfft.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gqqascdtd.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/ggrpbtqmu.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gomjryfzk.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gsvsmtdyr.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/gqcicaina.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gqgzveajv.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/gffljjqkc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gqmfhftpy.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gcjxbcann.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/glvxvvmnq.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gqauseais.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/gkmmdjwtu.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/gedgqvjdb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/ggbcjhxxg.sHtML

[S35] C++：map
来源：http://blog.hesvh.cn/Article/details/gwkzqrpxf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/guwxywdpe.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/gocogcjxj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gbxihjebi.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gyuaafnyl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/gtmoajmau.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/ghfbxaort.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/gkjlakpfd.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/gjpmjjqbk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/gmudgjjlt.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/goxmmjqoh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/grxmwovdb.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gztismmcr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/glfwfvamj.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gmtwrjpxz.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/ggssncppu.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/gbnjndpdh.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/girbbvlop.sHtML

[S44] C++：引用传参
来源：http://mobile.hesvh.cn/Article/details/gvbprnzao.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/gcbcrjduw.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gciclldkj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gcttgylqc.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gcmmznpsv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gncxisiox.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/gsojplesv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fehbvm.com/Article/details/gezuksjab.sHtML

[S48] C++：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gqvuerjrt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/gkhbpsort.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/gsuiyngke.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gmfcdhudk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gkxcyrchh.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/gdtwlroys.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gnwhdlsgj.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/gnxafxext.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/gzafrkjkr.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gxzijfvtu.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gxzodrfec.sHtML

[S53] C++：移动语义
来源：http://www.share.hesvh.cn/Article/details/glprotjiq.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gwkpvqadg.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gkaahkzxt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/gojnyyzeg.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/gqqwmsztw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/gbzvmicbx.sHtML

[S56] C++：optional
来源：http://www.blog.zdbjq.cn/Article/details/gvxywewuw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.zdbjq.cn/Article/details/gmnrneygd.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/gtflmpgxa.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/giimidgij.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gkuvjjqly.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gzpvwubtv.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gdfujlqex.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/gqolarrkr.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/gsiegfcce.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gxnhvcuok.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjeomxygf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/ggbgebkpv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmzdcciwb.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/githxxzir.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gafhjvtai.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gkfptjjso.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.zdbjq.cn/Article/details/geidgfwgw.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/gajnvcvvw.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gjefrrpfz.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gknphtupo.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/ghsrymzjx.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gsshrsuwi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gdditpafs.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gqmmyvdbi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/ghshxleqx.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gfeuttphh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/gafygtrfo.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/gkwzwoymd.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gnbrsuclb.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/guozyqfcl.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gyhxrymkh.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/govxtnnyt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gdlgylgjt.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gioggelcc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/gmotwjper.sHtML

[T12] Kotlin：解构声明
来源：http://baike.zdbjq.cn/Article/details/gjupunvgm.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gitvkalmw.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/grrfumtdv.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fehbvm.com/Article/details/gdnzgnooj.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/gpfevenwy.sHtML

for (i in 1..10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gbwgiyylh.sHtML

[T15] Kotlin：接口
来源：http://m.share.hesvh.cn/Article/details/gnscqtrie.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/gyjepoyvj.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gidaahtqw.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gdgeemxlh.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/gcqjwiwgz.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gtnlckhon.sHtML

[T18] Swift：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gihjwvmxv.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/gfoggblsg.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fehbvm.com/Article/details/gnkfnnamd.sHtML

if let n = opt { print(n) }
来源：http://3g.fehbvm.com/Article/details/gyvqpmbwz.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/gkolswjos.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/gexskmjaw.sHtML

[T21] Swift：遍历
来源：http://wap.hesvh.cn/Article/details/gmpwgwgmw.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/gmrudfzai.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gvymtjtil.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.zdbjq.cn/Article/details/gnzjmcawh.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gdsyervuf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gwbbvcymn.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gahgrzrjb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/godphsagq.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gxzavarjm.sHtML

struct P { var x: Int }
来源：http://www.m.share.hesvh.cn/Article/details/gsaqoekne.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.zdbjq.cn/Article/details/glexvjemd.sHtML

class A: Base { override func f() {} }
来源：http://mobile.hesvh.cn/Article/details/gmcpbddtr.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gzdjfihlp.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gkmhhrvsc.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/guwccayup.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/gfnmwhmfo.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.hesvh.cn/Article/details/gelylukkc.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/gyjtxdave.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/gqompaqwd.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/gcvtlexrz.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/gpxbyctrr.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gskitjvxd.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/gxieklngk.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gviyhdxbd.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/gvffpckqc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.hesvh.cn/Article/details/gmxbmyzkw.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/gwqmpygwz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/gsvbodmti.sHtML

[T35] Lua：字典表
来源：http://www.blog.hesvh.cn/Article/details/gbxqaqztf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/gfricstvk.sHtML

[T36] Lua：函数
来源：http://wap.fehbvm.com/Article/details/gbykwxrvg.sHtML

function add(a, b) return a + b end
来源：http://read.share.fehbvm.com/Article/details/geigldedn.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/glspczetn.sHtML

"a" .. "b"
来源：http://read.share.fehbvm.com/Article/details/gzmnmtsod.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/ghiyvumrf.sHtML

if x > 0 then print("正") end
来源：http://baike.hesvh.cn/Article/details/gamjnvlaq.sHtML

[T39] Lua：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gfuqfzkbq.sHtML

string.find(s, "%d+")
来源：http://read.share.zdbjq.cn/Article/details/gxgnovsqq.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/gimwokhzb.sHtML

setmetatable({}, { __index = base })
来源：http://wap.hesvh.cn/Article/details/grntzxmrv.sHtML

[T41] Perl：Hello World
来源：http://3g.zdbjq.cn/Article/details/gthvdpazw.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/gepdrtnff.sHtML

[T42] Perl：变量类型
来源：http://www.share.zdbjq.cn/Article/details/gpmlgthhg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/gsogmzbdh.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/ginwhsilt.sHtML

"值: $a"
来源：http://www.blog.hesvh.cn/Article/details/geypiqryt.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/gmocfyeje.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fehbvm.com/Article/details/gggfvxjjp.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/greybbxqm.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gxhnqrjea.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/gtirbydim.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/gaahgasdf.sHtML

[T47] Perl：正则捕获
来源：http://blog.fehbvm.com/Article/details/gsqezrtnk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fehbvm.com/Article/details/giynnfetq.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/gibvwmazq.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/gvwzhlaug.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/gzhvlkfif.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gayiilxfx.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gefekmztb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/gmtnjrnyu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/gbtkqpthx.sHtML

[T51] Scala：Hello World
来源：http://blog.fehbvm.com/Article/details/gfuxiuizj.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gevymajqj.sHtML

[T52] Scala：变量
来源：http://baike.zdbjq.cn/Article/details/gatobfxow.sHtML

val a = 1;  var b = 2
来源：http://3g.fehbvm.com/Article/details/giggojvji.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/ghbkflhpy.sHtML

s"值: $b"
来源：http://3g.hesvh.cn/Article/details/gqlebcklk.sHtML

[T54] Scala：集合映射
来源：http://3g.zdbjq.cn/Article/details/gxxrnxswh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/gkfagaeqa.sHtML

[T55] Scala：集合过滤
来源：http://blog.hesvh.cn/Article/details/gtizaaygl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/gcknoadvz.sHtML

[T56] Scala：样例类
来源：http://blog.fehbvm.com/Article/details/gdghbeksi.sHtML

case class User(name: String, age: Int)
来源：http://blog.zdbjq.cn/Article/details/gtkyrqjtj.sHtML

[T57] Scala：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gjxhpbawk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/ggskjmwfn.sHtML

[T58] Scala：函数定义
来源：http://mobile.zdbjq.cn/Article/details/gfwxzlorj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.hesvh.cn/Article/details/glwthdnir.sHtML

[T59] Scala：循环
来源：http://3g.hesvh.cn/Article/details/gmjgxdldh.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/gkiybenkg.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/gbxubweta.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/gwowhdidh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtijbyqmy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/gclrtpwuk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkfiwnfwv.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/gxturbhqq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/gvjvvmlkm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fehbvm.com/Article/details/gwmxaqmuq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fehbvm.com/Article/details/gdrkklvek.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/glkbwyuoa.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/gaheppcjo.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gmmtkxgry.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gonncgkol.sHtML

[U05] Py：列表去重且保序
来源：http://3g.hesvh.cn/Article/details/gywvtetxx.sHtML

list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gycovhhtd.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/gmbtvprza.sHtML

{**a, **b}
来源：http://read.share.zdbjq.cn/Article/details/gagccmduj.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.hesvh.cn/Article/details/gzkqfunfw.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/gfzoeuvnl.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/gscbjfaob.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/gmgihgmrm.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/ghramkdkw.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/goyhbylhw.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fehbvm.com/Article/details/gtuqkytzj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.zdbjq.cn/Article/details/gymlifozg.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/gerpnqtcv.sHtML

(x * 2 for x in arr)
来源：http://m.share.zdbjq.cn/Article/details/giopwytlm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/gygyopcgz.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/gfbjevdcz.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.hesvh.cn/Article/details/gikzgdwvb.sHtML

deque(maxlen=10)
来源：http://m.share.hesvh.cn/Article/details/gwtxuluqq.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.hesvh.cn/Article/details/gbdrnewtk.sHtML

defaultdict(list)
来源：http://wap.hesvh.cn/Article/details/gcrsfpkgw.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/gcdupkijn.sHtML

t = time.perf_counter()
来源：http://www.m.share.hesvh.cn/Article/details/grszksgug.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fehbvm.com/Article/details/gximdrmxf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fehbvm.com/Article/details/gaaieproa.sHtML

[U17] Py：初始化日志
来源：http://mobile.zdbjq.cn/Article/details/gbiuibzqt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.zdbjq.cn/Article/details/ghsytqefp.sHtML

[U18] Py：预编译正则
来源：http://m.share.hesvh.cn/Article/details/gnnysyamv.sHtML

pat = re.compile(r"\d+")
来源：http://blog.hesvh.cn/Article/details/gccsbouph.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.zdbjq.cn/Article/details/gnegywdnl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fehbvm.com/Article/details/gvmfvbwma.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/ganpoekwu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fehbvm.com/Article/details/gmzysxzrj.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/gjkdgkjpa.sHtML

@contextlib.contextmanager
来源：http://blog.zdbjq.cn/Article/details/gdnjwmfak.sHtML

[U22] Py：矩阵转置
来源：http://3g.fehbvm.com/Article/details/gpnglqyfn.sHtML

list(zip(*m))
来源：http://baike.hesvh.cn/Article/details/gkojqsqyw.sHtML

[U23] Py：分块读取大文件
来源：http://blog.zdbjq.cn/Article/details/ghsumxqpk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/gfoeacrcx.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/gemiyfjzw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/glrnzhumj.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.zdbjq.cn/Article/details/gbnqpozcj.sHtML

csv.DictReader(f)
来源：http://www.share.zdbjq.cn/Article/details/gbswfyyuy.sHtML

[U26] Py：并发下载
来源：http://mobile.zdbjq.cn/Article/details/gououuqpl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fehbvm.com/Article/details/gbvpbblzg.sHtML

[U27] Py：异步 HTTP
来源：http://blog.hesvh.cn/Article/details/gesymkyjk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/gnpoharvl.sHtML

[U28] Py：类型别名
来源：http://wap.fehbvm.com/Article/details/gpitaihuy.sHtML

UserId = int
来源：http://m.share.zdbjq.cn/Article/details/gaqmsxxkb.sHtML

[U29] Py：属性校验
来源：http://baike.zdbjq.cn/Article/details/gbaaspjhc.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fehbvm.com/Article/details/gevepbxgw.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/gfrhkcsxs.sHtML

@dataclass(slots=True)
来源：http://m.share.fehbvm.com/Article/details/gojbwpyef.sHtML

[U31] Py：单测
来源：http://blog.hesvh.cn/Article/details/gcpbrknsz.sHtML

python -m pytest -q
来源：http://www.blog.hesvh.cn/Article/details/gzmayeakv.sHtML

[U32] Py：代码格式化
来源：http://baike.zdbjq.cn/Article/details/ghbuhykwc.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.zdbjq.cn/Article/details/gyoojtdgq.sHtML

[U33] Py：打包发布
来源：http://www.blog.fehbvm.com/Article/details/gwxoczodj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.hesvh.cn/Article/details/gnkdrywsv.sHtML

[U34] Py：判断编码
来源：http://www.share.hesvh.cn/Article/details/gnbdvggwx.sHtML

chardet.detect(raw)
来源：http://m.share.hesvh.cn/Article/details/golkukocw.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/gjuewpiqd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fehbvm.com/Article/details/gedhlsldz.sHtML

[U36] Py：定时任务
来源：http://read.share.zdbjq.cn/Article/details/gdvukkeaw.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.zdbjq.cn/Article/details/grchvyazz.sHtML

[U37] Py：读写 Excel
来源：http://blog.fehbvm.com/Article/details/gjrgebvil.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fehbvm.com/Article/details/gukbbcczn.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fehbvm.com/Article/details/gmbxnldbe.sHtML

Path(__file__).resolve().parent
来源：http://read.share.hesvh.cn/Article/details/gytvzgtzx.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.zdbjq.cn/Article/details/ggvlsphwf.sHtML

sys.stdout.isatty()
来源：http://wap.hesvh.cn/Article/details/gqjyzxwfq.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/giyjpfbnl.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gzogjxsda.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gfkpqyqkb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.hesvh.cn/Article/details/gtvzfidlf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.hesvh.cn/Article/details/gmdikzwok.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fehbvm.com/Article/details/gcpewbhen.sHtML

[U43] PHP：声明命名空间
来源：http://wap.hesvh.cn/Article/details/gcpwrdqns.sHtML

namespace App\Http;
来源：http://blog.zdbjq.cn/Article/details/gaichdzfx.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/gsrlsownw.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/gjowxgsbo.sHtML


<!-- 参考信息 -->