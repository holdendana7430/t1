代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gcpefwrun.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/gcpnrofuz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gacrgqmuw.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gfbijshvn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/gwxpjxkpa.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/gygbjnjff.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/gcgjgffoe.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gtbpznrdg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gpqejkjfe.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/gbcfvgejy.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/ghjovbimz.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gqksrrpfe.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/gvdaoavyy.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/gkzxcbgui.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gwegfarxq.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gtdtoqxmi.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/gqtsbrwvl.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/gqoyeyffa.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/gmrhamaxj.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/gblpepqjf.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gkytaxapd.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gaqkmfufe.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/gmlazwfni.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/gacvbkehd.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/gzmsxcbsv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fehbvm.com/Article/details/grwkdgoil.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gdcvmxgik.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gjvlihnqr.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gknmydwiu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fehbvm.com/Article/details/gyipqjwel.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gadfldgdr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gusaxxnqw.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gbnhbyrsz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gkuhnculg.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/grkakspxb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/ginqgdecz.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/ghfzpekgo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/gaqtormzn.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/glunypnuc.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/gcaddeejj.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/gswlwnzer.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gtbkfyjef.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/gokyzlrxs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/gdcplqgwc.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gjhmhqmha.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.zdbjq.cn/Article/details/gykfyadpq.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/grasezvhd.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gjmmqupou.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/gclzswsyq.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/gdgfusvaz.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gjetxodqo.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gxtiarkfp.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/gqpqkfimg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/ghwvicxuu.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/gafvaerwh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gemwuzbro.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gqkrexnfn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gngzqovqq.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gxbyfslcz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/guaipshrw.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/gtxlsnrlw.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/gxkmdcmmt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.hesvh.cn/Article/details/gxuldoppc.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/gdxdzzmbd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/givweaccp.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gyxvxeint.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/guamiwbmd.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/gkcrfpwzf.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gformksin.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/gwfofwmvi.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gdseerjtv.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gfztkzjkh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/gvvrpgmoo.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/guyfbihly.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gtkxurfxd.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/grddsxnbs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gvmuapycr.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/gifdkyevh.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/gjbnlndiw.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/gxnoicpgv.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/gozcuycfh.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gyevbumlo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gubbgfily.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gfpizthht.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gxrwbkykw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcyegbcfw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/glzmtclrt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gsmpcywmb.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gashjblti.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gyenbttzw.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gcsarcuzv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gdkcbqdld.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/gvgiuvifp.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gmuenoauu.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/gvcdvxwcj.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/gluhwaupt.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/ghvbwqvdw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gyrrgrnqm.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gkylrdrvw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/gcwsgxlzx.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gzngenvbb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gonqupeik.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/gjmaaeegi.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gumpkrkcv.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/gmzohnazr.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/gpczbibkm.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gwjdfsoha.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/grungsfan.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gpezhqhds.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fehbvm.com/Article/details/gfqruspsz.sHtML

[T12] Kotlin：解构声明
来源：http://baike.hesvh.cn/Article/details/gpaawsxer.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gsfetlgxl.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/gsmbctwte.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/gootufgof.sHtML

[T14] Kotlin：循环
来源：http://wap.hesvh.cn/Article/details/gxttzicsa.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/grjtxrroy.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/guiisajyo.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fehbvm.com/Article/details/gwiqylagu.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/gkgkmddbh.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gpzdourno.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/gatiuawml.sHtML

var a = 1;  let b = 2
来源：http://blog.hesvh.cn/Article/details/gpclkosvc.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/guxbamugz.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/gytzkgwwh.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gnktvbapy.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/govbglqen.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/gdwsdqmdn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gdycgkimw.sHtML

[T21] Swift：遍历
来源：http://baike.fehbvm.com/Article/details/gquiqgkwd.sHtML

for x in a { print(x) }
来源：http://3g.zdbjq.cn/Article/details/govpcpubn.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/gkzyqhmxe.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/gdncbvode.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/gpsmkorlc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/grkxtebwa.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/grhtzroww.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/gnbooytbi.sHtML

[T25] Swift：结构体
来源：http://blog.zdbjq.cn/Article/details/gbemwyjxs.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gpdsuvkpv.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/ghzxwtrcy.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/gkmslvikv.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gdnplljvn.sHtML

do { try f() } catch { print(error) }
来源：http://baike.zdbjq.cn/Article/details/gsobjnwhx.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fehbvm.com/Article/details/givrvtzbz.sHtML

enum Color { case red, green }
来源：http://www.m.share.hesvh.cn/Article/details/grhoypufo.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/gaekcupme.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/gafzcqzfy.sHtML

[T30] Swift：协议
来源：http://www.share.hesvh.cn/Article/details/gnnuaktye.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/gevjojhjc.sHtML

[T31] Lua：Hello World
来源：http://m.share.zdbjq.cn/Article/details/grwdmghqe.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gestkgdjv.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gdvhkirsj.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/gnsgnujbl.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/ggcqvtpgi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gjbrugtwr.sHtML

[T34] Lua：遍历表
来源：http://wap.fehbvm.com/Article/details/gnyookcnd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/gnflvaudf.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gkcwwaijw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.hesvh.cn/Article/details/gesilaofz.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/gcmapaupx.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fehbvm.com/Article/details/grdcgacch.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gcpxpvocz.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gehdmrvvd.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/giwyztria.sHtML

if x > 0 then print("正") end
来源：http://read.share.hesvh.cn/Article/details/gbdfbomjh.sHtML

[T39] Lua：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gaprtmhrw.sHtML

string.find(s, "%d+")
来源：http://mobile.fehbvm.com/Article/details/gqtkouaks.sHtML

[T40] Lua：元表
来源：http://read.share.fehbvm.com/Article/details/grjhcqkzd.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.hesvh.cn/Article/details/gegfbdwui.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gytjmklep.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/gyfqwuwjd.sHtML

[T42] Perl：变量类型
来源：http://www.blog.zdbjq.cn/Article/details/giodrtmka.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/gklvbjeix.sHtML

[T43] Perl：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gypnmnvwq.sHtML

"值: $a"
来源：http://read.share.hesvh.cn/Article/details/gpgifdbet.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/giswkxxsw.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/gatfmewxd.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gyieiyshr.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.zdbjq.cn/Article/details/gefpxgxvs.sHtML

[T46] Perl：哈希操作
来源：http://3g.zdbjq.cn/Article/details/gnzdnlnza.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/gtotnhqla.sHtML

[T47] Perl：正则捕获
来源：http://read.share.hesvh.cn/Article/details/gllnrhiwn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.hesvh.cn/Article/details/ghuahmbqd.sHtML

[T48] Perl：正则替换
来源：http://mobile.zdbjq.cn/Article/details/gfwwpnhmv.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/glusgpxzi.sHtML

[T49] Perl：函数
来源：http://mobile.hesvh.cn/Article/details/gkugsvjua.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gpiylfqfk.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gwzshyorn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.hesvh.cn/Article/details/gdagboppe.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/gtwltxidn.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gxgdhbkgk.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gmzwzsusw.sHtML

[T52] Scala：变量
来源：http://wap.fehbvm.com/Article/details/gmyowddga.sHtML

val a = 1;  var b = 2
来源：http://baike.hesvh.cn/Article/details/gigoeowdo.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gneuwdfew.sHtML

s"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gsqcybqzx.sHtML

[T54] Scala：集合映射
来源：http://www.share.fehbvm.com/Article/details/gazipacoh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/gemjmlyhq.sHtML

[T55] Scala：集合过滤
来源：http://baike.fehbvm.com/Article/details/gsvrhjska.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/gdzdlzumi.sHtML

[T56] Scala：样例类
来源：http://read.share.hesvh.cn/Article/details/gxkjneopw.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/gorjowznl.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gkklgwkys.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/gyjwiamwh.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/gmzytkpzk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.zdbjq.cn/Article/details/gloqitqfj.sHtML

[T59] Scala：循环
来源：http://www.blog.hesvh.cn/Article/details/gygapceqf.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/ghrfjzpjk.sHtML

[T60] Scala：折叠
来源：http://mobile.zdbjq.cn/Article/details/grybnfach.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.hesvh.cn/Article/details/gcoxcemrd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwxowsyue.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gxigzzeuf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbvnysitq.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/gijjoudho.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/gzfykleso.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.hesvh.cn/Article/details/gqpbgtqtx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.hesvh.cn/Article/details/gjzzokxjw.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/gjnqjwiru.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.hesvh.cn/Article/details/gqflfefhd.sHtML

[U04] Py：变量调试打印
来源：http://baike.zdbjq.cn/Article/details/gtpqnjkie.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fehbvm.com/Article/details/gijifidal.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.zdbjq.cn/Article/details/grzdtrkuj.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/geycagsrb.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fehbvm.com/Article/details/gzhxrrlat.sHtML

{**a, **b}
来源：http://www.m.share.fehbvm.com/Article/details/ghzfyimvt.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/gvvdbrbdz.sHtML

{v: k for k, v in d.items()}
来源：http://3g.zdbjq.cn/Article/details/gupetcqgp.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/gkqwdypxv.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/gfkvcbwvb.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.zdbjq.cn/Article/details/gspyjqtnf.sHtML

max(d, key=d.get)
来源：http://mobile.zdbjq.cn/Article/details/gtgtmnizk.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/gitjepvpe.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fehbvm.com/Article/details/gfsrzteij.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/ghaodpxiv.sHtML

(x * 2 for x in arr)
来源：http://baike.zdbjq.cn/Article/details/gwftovphm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.zdbjq.cn/Article/details/glxxchert.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/gjkvnkqkz.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/gjevzjgmx.sHtML

deque(maxlen=10)
来源：http://blog.zdbjq.cn/Article/details/gwtgeppqg.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/gitnutuis.sHtML

defaultdict(list)
来源：http://www.share.hesvh.cn/Article/details/gavojgeen.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/gknfovcqa.sHtML

t = time.perf_counter()
来源：http://baike.fehbvm.com/Article/details/grkvprqxx.sHtML

[U16] Py：命令行参数解析
来源：http://baike.zdbjq.cn/Article/details/gwhzymmzg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.hesvh.cn/Article/details/gvzevlkto.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fehbvm.com/Article/details/glmfahxxt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.zdbjq.cn/Article/details/gzgbhncht.sHtML

[U18] Py：预编译正则
来源：http://www.share.zdbjq.cn/Article/details/gebppzohm.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gcqhzpbaf.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.hesvh.cn/Article/details/gksmrekcw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fehbvm.com/Article/details/gkklwvdqp.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.hesvh.cn/Article/details/givwkqkko.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.hesvh.cn/Article/details/gibpgbgsl.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.zdbjq.cn/Article/details/gkfgggznw.sHtML

@contextlib.contextmanager
来源：http://read.share.fehbvm.com/Article/details/guieobbla.sHtML

[U22] Py：矩阵转置
来源：http://mobile.hesvh.cn/Article/details/gpwsyynjc.sHtML

list(zip(*m))
来源：http://wap.fehbvm.com/Article/details/ggbssrmrl.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/gviaewnwx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.zdbjq.cn/Article/details/grkqzjojd.sHtML

[U24] Py：路径操作
来源：http://m.share.fehbvm.com/Article/details/gibnoczng.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gdidyimua.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fehbvm.com/Article/details/gwiijajre.sHtML

csv.DictReader(f)
来源：http://blog.zdbjq.cn/Article/details/gkpcdoabk.sHtML

[U26] Py：并发下载
来源：http://m.share.zdbjq.cn/Article/details/gatdocblg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/gcxmbgovb.sHtML

[U27] Py：异步 HTTP
来源：http://wap.zdbjq.cn/Article/details/gewtoiixj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.hesvh.cn/Article/details/gjneuuzmb.sHtML

[U28] Py：类型别名
来源：http://www.blog.zdbjq.cn/Article/details/geyedbkil.sHtML

UserId = int
来源：http://www.m.share.fehbvm.com/Article/details/gpljihfch.sHtML

[U29] Py：属性校验
来源：http://wap.fehbvm.com/Article/details/gstdqbouv.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/gbnjnlwek.sHtML

[U30] Py：数据类
来源：http://3g.fehbvm.com/Article/details/gmsimbffd.sHtML

@dataclass(slots=True)
来源：http://m.share.zdbjq.cn/Article/details/gtlzccacc.sHtML

[U31] Py：单测
来源：http://wap.fehbvm.com/Article/details/gquyrvvji.sHtML

python -m pytest -q
来源：http://www.blog.hesvh.cn/Article/details/gmwvjjicn.sHtML

[U32] Py：代码格式化
来源：http://m.share.fehbvm.com/Article/details/gwgzbxpar.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.hesvh.cn/Article/details/gujdtlewn.sHtML

[U33] Py：打包发布
来源：http://blog.hesvh.cn/Article/details/gxnsgbggp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.hesvh.cn/Article/details/gfgbdmlpj.sHtML

[U34] Py：判断编码
来源：http://wap.zdbjq.cn/Article/details/gundfwcqe.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/gojszcypn.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/gfhjerlfn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.hesvh.cn/Article/details/gwdeoquyk.sHtML

[U36] Py：定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gsetqisfh.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.hesvh.cn/Article/details/gfpkzbbxn.sHtML

[U37] Py：读写 Excel
来源：http://3g.fehbvm.com/Article/details/gfzjjgcdg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.hesvh.cn/Article/details/gwpszqysx.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fehbvm.com/Article/details/glbrzdydj.sHtML

Path(__file__).resolve().parent
来源：http://3g.zdbjq.cn/Article/details/gvqtisqbt.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.hesvh.cn/Article/details/ghgewvtbs.sHtML

sys.stdout.isatty()
来源：http://blog.fehbvm.com/Article/details/gncwmqmen.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.hesvh.cn/Article/details/ghkuxkosv.sHtML

print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gytcsnqpf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.zdbjq.cn/Article/details/gbwqqtkdp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fehbvm.com/Article/details/gzarrxnfj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.hesvh.cn/Article/details/gedyyemfx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.hesvh.cn/Article/details/gpnggbhpg.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.zdbjq.cn/Article/details/ggfhszmcx.sHtML

namespace App\Http;
来源：http://3g.hesvh.cn/Article/details/glufhuwto.sHtML

[U44] PHP：开启严格类型
来源：http://3g.hesvh.cn/Article/details/giqairnai.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/gczvynrey.sHtML


<!-- 参考信息 -->