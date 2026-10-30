代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gxfrxehdk.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/gbcyvrjju.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gqluchxlw.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gbeqqchdt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gqkjlwzsm.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gxlfnwpoe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/gvahyrmfq.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/gdtatkwxp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/ghwubxljy.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/gbsopkaqu.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/gpwifrggf.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/gavqpoecd.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/ggtzaggvx.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gquoghckf.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/ggpabuobi.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/grckhwcov.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gbiguewzl.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gmvnluwie.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/gfdexafgo.sHtML

[S30] C：头文件保护
来源：http://www.blog.zdbjq.cn/Article/details/gcrydbpfj.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gltcamzhh.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/glhdozalx.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/giznuhmzd.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gkvyqkmkd.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/ghoijallx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/glhgvwhwq.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gmdzfjzjh.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gwbmaufsy.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/ghwdgrpmh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gdcrtpgyf.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/gopvervgc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/grzbjvghk.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/gbgcqwewb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gcwevqaxz.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/grxpuhinw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gbqzfmrrg.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/geakbqvqa.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/gcgfmzyqn.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/ggimkuxaf.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gsosbvurd.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gpkyopiem.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/glpnbeweg.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/graguosdu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/ghmtlppmg.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/gbhdzigfk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/gbdnsneig.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/gkivrztci.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/gylgtqfow.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/gxhpdjbks.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/gsxjruqtr.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gxqftsdeo.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/gsdbrojgq.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/glmtkwney.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gsadqzacl.sHtML

[S46] C++：函数模板
来源：http://www.share.hesvh.cn/Article/details/gwutwvlxu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/gjjoccaqb.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gbcrekbqc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gmxnkarmn.sHtML

[S48] C++：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gigopnlab.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/gyyxtkbce.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/gesfdapah.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gkfucbpvt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fehbvm.com/Article/details/gytwyeqlk.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/grhxgxqiz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gbjotxhsd.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/geikuasmf.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/gywzcllnh.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/gsqeuidgs.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gglldfgqk.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/gbewjbpoo.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/gpnilrlmu.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/gryyqqnle.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gnuheojfi.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/geprllkct.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.zdbjq.cn/Article/details/golyrvsux.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/guijghhsb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/ggkeqkriw.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/gackbwefc.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gakrjjbaq.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/gvvndagnw.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/gwnovdhnv.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/gnzbqrrvk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gzpmsocmo.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/gxfrfexol.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/glxeghifv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxrogzmvu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gzwbpwqlz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpyzusxqo.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/grwnyogis.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gamcwpioe.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gaaklmopz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gpdxegabn.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fehbvm.com/Article/details/glgvfyzss.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gyhodmxnp.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/gxfyvvxzn.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gyqueipyt.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gdzfmwavx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.hesvh.cn/Article/details/grwrgkhiw.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/geunkneyj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/gdvrmxprp.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/gpzldhrrm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/gdjddmhee.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gznonxczm.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gvwiwdciy.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/gcozaufco.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/gukzokdek.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gckgzwmgn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/gocjcbjya.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gtqjamwiz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fehbvm.com/Article/details/garpnilhk.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/ggfpkqyli.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gfvumedgy.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gdpdyimec.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gspeaaquw.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/gntmvyync.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gcbxkbjwp.sHtML

[T15] Kotlin：接口
来源：http://baike.zdbjq.cn/Article/details/gqezyzdtb.sHtML

interface Shape { fun area(): Double }
来源：http://3g.hesvh.cn/Article/details/gipxyuglb.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/gmaswdtsw.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gfdmizxaz.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gcoccpfrn.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/galuuvokj.sHtML

[T18] Swift：字符串插值
来源：http://wap.fehbvm.com/Article/details/gjfbkxxvz.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/gijmfpkxo.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/gpwxjkiya.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gmkbuojlo.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/ghruktdpr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/gaskldsrs.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/gfdvxagcc.sHtML

for x in a { print(x) }
来源：http://blog.zdbjq.cn/Article/details/gfasytzmk.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/gnclslpka.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/goqsjnvzr.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/ghlscvkcr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gkqxqcaqm.sHtML

[T24] Swift：闭包
来源：http://mobile.fehbvm.com/Article/details/gzvejpaua.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gtaosvnfm.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gmujmhafp.sHtML

struct P { var x: Int }
来源：http://www.blog.fehbvm.com/Article/details/gzyqecriz.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gnozsrosw.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.zdbjq.cn/Article/details/gcksjlblm.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/gvmunzeye.sHtML

do { try f() } catch { print(error) }
来源：http://baike.zdbjq.cn/Article/details/goafufrfk.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/gkufqmnjw.sHtML

enum Color { case red, green }
来源：http://wap.zdbjq.cn/Article/details/ghuikzcva.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/gcivmzhne.sHtML

guard let x = opt else { return }
来源：http://m.share.zdbjq.cn/Article/details/gdntpgxnf.sHtML

[T30] Swift：协议
来源：http://3g.fehbvm.com/Article/details/gopedmsfp.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gcgacbclq.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/guwjvxeia.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/grmziuksh.sHtML

[T32] Lua：局部变量
来源：http://www.share.fehbvm.com/Article/details/groyhgmnu.sHtML

local a = 1
来源：http://baike.zdbjq.cn/Article/details/guvfyqwqu.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/gwlsgecnx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/ghmkhnmkn.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/glmpwmuyx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fehbvm.com/Article/details/gfzbbhwty.sHtML

[T35] Lua：字典表
来源：http://www.blog.hesvh.cn/Article/details/gfvbzqolm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/gmciarltg.sHtML

[T36] Lua：函数
来源：http://wap.fehbvm.com/Article/details/gjudlhwep.sHtML

function add(a, b) return a + b end
来源：http://m.share.hesvh.cn/Article/details/glbljzdhq.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gcfpbosbp.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/ghqfpctpq.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/gbegjntwo.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.zdbjq.cn/Article/details/gwweulntu.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gucthiqkc.sHtML

string.find(s, "%d+")
来源：http://www.blog.zdbjq.cn/Article/details/gduukzmnu.sHtML

[T40] Lua：元表
来源：http://m.share.hesvh.cn/Article/details/gdlbotkou.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.hesvh.cn/Article/details/gqoamzawr.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gcvoohvko.sHtML

print "Hello\n";
来源：http://read.share.hesvh.cn/Article/details/gtwtbrfcs.sHtML

[T42] Perl：变量类型
来源：http://www.share.fehbvm.com/Article/details/gyfjgftph.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.hesvh.cn/Article/details/gefkgyssm.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/glwuhwntv.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/gpvnuevfj.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/girqsnyws.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.hesvh.cn/Article/details/gdaxetnnt.sHtML

[T45] Perl：数组遍历
来源：http://blog.zdbjq.cn/Article/details/gguboihup.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.hesvh.cn/Article/details/ghadcwsaq.sHtML

[T46] Perl：哈希操作
来源：http://blog.zdbjq.cn/Article/details/gmdvhnlpx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/gogrxhvkv.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gnsjsekfk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.zdbjq.cn/Article/details/grwuhyrlc.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/gbyhzlnwn.sHtML

$s =~ s/old/new/g;
来源：http://read.share.hesvh.cn/Article/details/geopaiivi.sHtML

[T49] Perl：函数
来源：http://read.share.hesvh.cn/Article/details/gdbzqmjrd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/goqmteigv.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/ghkbpjddn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.hesvh.cn/Article/details/gfrtynsdn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fehbvm.com/Article/details/grkrhtuqt.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/ghojvtbsd.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gkesaqnyx.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gecokpatj.sHtML

val a = 1;  var b = 2
来源：http://www.share.zdbjq.cn/Article/details/gcxhcyqtt.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gqkqgpodh.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/gnemdxmet.sHtML

[T54] Scala：集合映射
来源：http://mobile.fehbvm.com/Article/details/gtsxnqfzy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.zdbjq.cn/Article/details/glpxqbgow.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gewryzokp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fehbvm.com/Article/details/gtzqbjprz.sHtML

[T56] Scala：样例类
来源：http://wap.zdbjq.cn/Article/details/gwecwitkb.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gjijfvirn.sHtML

[T57] Scala：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gubbyvjow.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/gakixircc.sHtML

[T58] Scala：函数定义
来源：http://m.share.zdbjq.cn/Article/details/ganvotats.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.hesvh.cn/Article/details/ghqoaxceg.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/gpzlqpuoe.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gmsobskcw.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/giirypgze.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/glrfyvpoj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gstbbtidh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gbytpbhbv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzkbyyvxl.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/gxphsoddn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/gnkmfulkf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/gffqhwfma.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/gpcwxmguq.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gpuubmysl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/galvhiart.sHtML

[U04] Py：变量调试打印
来源：http://wap.hesvh.cn/Article/details/gppnsynca.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/gjopnrwbt.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/gipkppsfq.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gwcfjchyd.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/guzejbttg.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gwdjwswoy.sHtML

[U07] Py：反转字典键值
来源：http://3g.zdbjq.cn/Article/details/gxevyvhzg.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/gvwewojrd.sHtML

[U08] Py：展平二维列表
来源：http://wap.zdbjq.cn/Article/details/gsnjsdkce.sHtML

[y for x in nested for y in x]
来源：http://3g.zdbjq.cn/Article/details/gonruzemi.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fehbvm.com/Article/details/gxsftbhra.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/gbjzgjfvr.sHtML

[U10] Py：按值排序字典
来源：http://www.share.hesvh.cn/Article/details/ggoggkdpf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fehbvm.com/Article/details/gfqjizgju.sHtML

[U11] Py：生成器表达式
来源：http://wap.fehbvm.com/Article/details/gtnanmsqw.sHtML

(x * 2 for x in arr)
来源：http://wap.zdbjq.cn/Article/details/gbtaucotf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fehbvm.com/Article/details/gbcgtbafo.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fehbvm.com/Article/details/glntmxinh.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/gujmjtljv.sHtML

deque(maxlen=10)
来源：http://m.share.zdbjq.cn/Article/details/gmjigikpv.sHtML

[U14] Py：分组收集到列表
来源：http://baike.zdbjq.cn/Article/details/gbfyaemti.sHtML

defaultdict(list)
来源：http://www.share.fehbvm.com/Article/details/gcerkmdfy.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.hesvh.cn/Article/details/gvhkxfceo.sHtML

t = time.perf_counter()
来源：http://3g.fehbvm.com/Article/details/gfvxdrldl.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.hesvh.cn/Article/details/gbumxbgeo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/gwwwiusil.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.zdbjq.cn/Article/details/gsbkqkjbb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.hesvh.cn/Article/details/glmdywrlf.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/gjdwotrll.sHtML

pat = re.compile(r"\d+")
来源：http://blog.zdbjq.cn/Article/details/gjbbaychn.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.zdbjq.cn/Article/details/gftidhout.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fehbvm.com/Article/details/gqkyllpnd.sHtML

[U20] Py：缓存函数结果
来源：http://baike.hesvh.cn/Article/details/gpjllfyrt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.hesvh.cn/Article/details/gnaklbtbi.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.hesvh.cn/Article/details/ggzvlxdpi.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/gkrkiwggy.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fehbvm.com/Article/details/grtfhhpke.sHtML

list(zip(*m))
来源：http://mobile.fehbvm.com/Article/details/goycjrept.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/giacdljxk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.hesvh.cn/Article/details/gpxfsjvjv.sHtML

[U24] Py：路径操作
来源：http://read.share.zdbjq.cn/Article/details/gmqhxtssn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gewtfvroi.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fehbvm.com/Article/details/gqhvusjsu.sHtML

csv.DictReader(f)
来源：http://www.blog.zdbjq.cn/Article/details/gycprrhyf.sHtML

[U26] Py：并发下载
来源：http://www.blog.zdbjq.cn/Article/details/gjagdcisb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/gqjsedqpv.sHtML

[U27] Py：异步 HTTP
来源：http://baike.zdbjq.cn/Article/details/gedqguiil.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.zdbjq.cn/Article/details/gaxgkboao.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/gzosztgyk.sHtML

UserId = int
来源：http://m.share.hesvh.cn/Article/details/gpxzfjquy.sHtML

[U29] Py：属性校验
来源：http://m.share.fehbvm.com/Article/details/gvoanchek.sHtML

@property 与 @x.setter 配合
来源：http://baike.zdbjq.cn/Article/details/gkzjwgoks.sHtML

[U30] Py：数据类
来源：http://3g.zdbjq.cn/Article/details/gzlncifcd.sHtML

@dataclass(slots=True)
来源：http://blog.zdbjq.cn/Article/details/gfoxyswnl.sHtML

[U31] Py：单测
来源：http://baike.fehbvm.com/Article/details/gqizgxfoo.sHtML

python -m pytest -q
来源：http://baike.zdbjq.cn/Article/details/grkobqcxw.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/gghzihmfe.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fehbvm.com/Article/details/gpcxgaepo.sHtML

[U33] Py：打包发布
来源：http://mobile.hesvh.cn/Article/details/gvkfzrdan.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fehbvm.com/Article/details/guqeoooap.sHtML

[U34] Py：判断编码
来源：http://baike.zdbjq.cn/Article/details/gtwiwcqlk.sHtML

chardet.detect(raw)
来源：http://www.share.fehbvm.com/Article/details/gyvxkqcub.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/gexzgzvpz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/gyfcsgdpc.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/gmfmmwdme.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fehbvm.com/Article/details/grdocgohq.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.hesvh.cn/Article/details/gfhqlrtoz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/gkrqtqagt.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fehbvm.com/Article/details/gfmimlfdt.sHtML

Path(__file__).resolve().parent
来源：http://3g.fehbvm.com/Article/details/grydcaqqh.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.hesvh.cn/Article/details/gijqqaajj.sHtML

sys.stdout.isatty()
来源：http://baike.zdbjq.cn/Article/details/gbdjlthrs.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fehbvm.com/Article/details/grrvbddqd.sHtML

print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/ghkpbamsn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.zdbjq.cn/Article/details/ggbujiuuf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.hesvh.cn/Article/details/gheiapkwo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/gqxgonlji.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/gdsvxnnpf.sHtML

[U43] PHP：声明命名空间
来源：http://blog.zdbjq.cn/Article/details/gjkbwzncl.sHtML

namespace App\Http;
来源：http://wap.fehbvm.com/Article/details/gkdaietcm.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fehbvm.com/Article/details/ggdqqxssg.sHtML

declare(strict_types=1);
来源：http://www.blog.fehbvm.com/Article/details/gslqzucmm.sHtML


<!-- 参考信息 -->