代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gpxzzrtcx.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/guxwsqjmd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/gxgdlyane.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/gxaaewoox.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/guqoqkzyo.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/gbgzygxwy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/gwrrettms.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/gzybvyxbb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gbxbosahs.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/gwhhhrelv.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/giuyiynnj.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gruzieors.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/gmcxpjisa.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/glhuwmrik.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/ghydhmtly.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gajtlshyu.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/ghsuxlylm.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/gmmrxnmhd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gfehjkzzk.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gyzytzhdp.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gdenwiubh.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/gglywxycs.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/gzxbrrcps.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/ghrojkrpi.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gsaolbvvw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gksfcnugy.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gxywxavof.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gwihcdkdx.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gqbpdahou.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/ghmhjneup.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/gnjdzynsa.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gmuzidsvn.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gmjdehpov.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/grwleqmqb.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/ggnkrvsym.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gsaksvrry.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gtsxmxvzv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/gufycjqck.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gsmcrcobt.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gpfehczos.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gkuedndbz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gciivvujz.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gwnjymxyl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/gsztfydzi.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gpwosqlef.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/gdugdotko.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/gcgphuvun.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/gdjlunhat.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gxmejocie.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gcfarhgaz.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gkabggene.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/gdniklxmi.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/gluyxgomb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fehbvm.com/Article/details/giazvsxil.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gcpcspqwb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/gijjkeruy.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/gntqdjysc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggvdbughy.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gnbqjbxal.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/gbqpaszkb.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gyveqihmi.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gbyzwffzx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.hesvh.cn/Article/details/gasbetsyb.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gxollxxit.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gfjzbkglq.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/gtgnpdtga.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/ggfgvuavb.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/gxtvpwvfm.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gxpzvhiha.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/girvqtktn.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/grpnawuym.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/gvujrbssb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/ggankpibo.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/gdngkneow.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/gqwmepicd.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/gdfguxbni.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmzlwknty.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/grdludwst.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/gdglgmqtv.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gsunaybjm.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/glysfzjfb.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gmwindves.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/gkxpzzsug.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fehbvm.com/Article/details/gglpmqeea.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/grnvkqzkh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyiwbwzhx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gzmgnpejd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvmftljji.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/gaaneksho.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/ggjdwqkcv.sHtML

[T02] Kotlin：变量
来源：http://blog.hesvh.cn/Article/details/ggxnggdsn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/ggtxfvmiw.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/grgxxevcy.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gsxgyvpqe.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gjpoaetlw.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/gvorigxfc.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/glmlxmcdq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/gsaarevhv.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gfvcfmxvj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fehbvm.com/Article/details/guaakukyd.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gvyxnymcr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gzigujqdq.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gmipqggfc.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gmryffjmh.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/gxzzbiqst.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/gqlzvtxcj.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gejamnccm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.hesvh.cn/Article/details/gqyhhsmdt.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/gxodmydup.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gxvmjgbqc.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/gaaszolfp.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gafnxpehv.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gbxdcropn.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/glfntvxfc.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gwngkxslh.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/guzlmcfyg.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/gxdqxqimz.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/gmzeqmqax.sHtML

[T16] Swift：Hello World
来源：http://mobile.hesvh.cn/Article/details/gozsjzrcj.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gvdpodcrx.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fehbvm.com/Article/details/gttlvifmd.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/guuxyshpn.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gmycsouql.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/gfskbkkhz.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gssvctizb.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.hesvh.cn/Article/details/grzzcfpon.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/gkpzvepnp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/gybsixwcq.sHtML

[T21] Swift：遍历
来源：http://www.share.hesvh.cn/Article/details/gczmmxjth.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/gekchobfw.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/glomgxiiw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.zdbjq.cn/Article/details/gymdnwofd.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gtfcnshyv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/gdxcfqyhi.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/gspvzlecv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gnnvjpauo.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/gdyehmoai.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/gmkknxsih.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/gpqnnzvuc.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/gkmcpepqp.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/ggnfkkrio.sHtML

do { try f() } catch { print(error) }
来源：http://baike.zdbjq.cn/Article/details/gqdrlaqez.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gftuyvfwp.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/ghcoqboyq.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/gznnebzmz.sHtML

guard let x = opt else { return }
来源：http://baike.fehbvm.com/Article/details/gxovwmieu.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/gxgxwcyxs.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.zdbjq.cn/Article/details/gfmkzcxdb.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gjopeddmo.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/guasurpce.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/gniliwwbg.sHtML

local a = 1
来源：http://blog.zdbjq.cn/Article/details/gctwoxmgs.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fehbvm.com/Article/details/gdnyzuocb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.zdbjq.cn/Article/details/gxjwxglcy.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gqlyjnigt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/grpfzvxqv.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/gdpirlfon.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.zdbjq.cn/Article/details/gxkzmmoxv.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/gjntzgpzq.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.hesvh.cn/Article/details/gpjhwnhrj.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/gzxuofufg.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/gqhiliwsg.sHtML

[T38] Lua：条件
来源：http://mobile.fehbvm.com/Article/details/ggztpilka.sHtML

if x > 0 then print("正") end
来源：http://m.share.fehbvm.com/Article/details/gohglvuki.sHtML

[T39] Lua：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/golufiydh.sHtML

string.find(s, "%d+")
来源：http://wap.hesvh.cn/Article/details/gzeygudqu.sHtML

[T40] Lua：元表
来源：http://www.share.fehbvm.com/Article/details/gavsnvpwc.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/gyeiqpvql.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/ghaobxbhj.sHtML

print "Hello\n";
来源：http://baike.fehbvm.com/Article/details/gcaaekccj.sHtML

[T42] Perl：变量类型
来源：http://blog.hesvh.cn/Article/details/gjztciyhx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/gpycvfuia.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gsjcqjiyf.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/grxqqryhd.sHtML

[T44] Perl：条件
来源：http://3g.fehbvm.com/Article/details/gtlpzubsn.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/giayaueta.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fehbvm.com/Article/details/gkyuarwhg.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.zdbjq.cn/Article/details/ghctdycyu.sHtML

[T46] Perl：哈希操作
来源：http://mobile.zdbjq.cn/Article/details/gsjarmvxx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fehbvm.com/Article/details/ghthnzkop.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/gwfqypatw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.zdbjq.cn/Article/details/gizigunmk.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/gianenpxu.sHtML

$s =~ s/old/new/g;
来源：http://3g.fehbvm.com/Article/details/gerjhoqwf.sHtML

[T49] Perl：函数
来源：http://3g.fehbvm.com/Article/details/gxqnubcqg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gxkbmtjve.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/graqizirs.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fehbvm.com/Article/details/gucmqdtnk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.zdbjq.cn/Article/details/gajicybsx.sHtML

[T51] Scala：Hello World
来源：http://read.share.fehbvm.com/Article/details/gxeaslkyx.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gsmbezafq.sHtML

[T52] Scala：变量
来源：http://m.share.zdbjq.cn/Article/details/gqorjkeey.sHtML

val a = 1;  var b = 2
来源：http://wap.zdbjq.cn/Article/details/guihchcpy.sHtML

[T53] Scala：字符串插值
来源：http://baike.fehbvm.com/Article/details/gdmeyilig.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/gytiqitfd.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/ggqwscuxk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/gagldwgkz.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/gqiipggat.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.zdbjq.cn/Article/details/gjbnmxuit.sHtML

[T56] Scala：样例类
来源：http://3g.hesvh.cn/Article/details/grbfxjksz.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/ggcpvnbdr.sHtML

[T57] Scala：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gfxvwjqca.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gfachmbut.sHtML

[T58] Scala：函数定义
来源：http://read.share.zdbjq.cn/Article/details/gwoqrgqru.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/gmoimsxtr.sHtML

[T59] Scala：循环
来源：http://mobile.zdbjq.cn/Article/details/gtzzuwkqp.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.zdbjq.cn/Article/details/goicyzddq.sHtML

[T60] Scala：折叠
来源：http://www.share.fehbvm.com/Article/details/giddhbqmm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fehbvm.com/Article/details/gequbvpkb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtpaqnsfl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/ggnswhmbz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxjyeqzxd.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/ghyhylods.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/gkqkxxvde.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fehbvm.com/Article/details/goreotbnv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.zdbjq.cn/Article/details/gaipcqxbk.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.zdbjq.cn/Article/details/ggyhhwzrm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.hesvh.cn/Article/details/gcnjnszcp.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/guydfhvxi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/gmlfjwjim.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.zdbjq.cn/Article/details/gkxenoaqj.sHtML

list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/ghwpxrzfx.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.zdbjq.cn/Article/details/gnwqjqbof.sHtML

{**a, **b}
来源：http://wap.fehbvm.com/Article/details/glxhoqwze.sHtML

[U07] Py：反转字典键值
来源：http://mobile.hesvh.cn/Article/details/gkvdgcwqa.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.zdbjq.cn/Article/details/gjuxsjprf.sHtML

[U08] Py：展平二维列表
来源：http://baike.zdbjq.cn/Article/details/gnjlfmrxy.sHtML

[y for x in nested for y in x]
来源：http://wap.fehbvm.com/Article/details/gjllvcqsm.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fehbvm.com/Article/details/gwkpdzodn.sHtML

max(d, key=d.get)
来源：http://www.share.fehbvm.com/Article/details/gdmzlkdvp.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/ghumzjxct.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fehbvm.com/Article/details/gkcfkvorm.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.zdbjq.cn/Article/details/gxxilcbak.sHtML

(x * 2 for x in arr)
来源：http://wap.hesvh.cn/Article/details/gavygvoaw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fehbvm.com/Article/details/gmegbgwhw.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/gywcfvmdu.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/gjgsifklr.sHtML

deque(maxlen=10)
来源：http://blog.zdbjq.cn/Article/details/gjdtlmlih.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.zdbjq.cn/Article/details/ggfcfubnf.sHtML

defaultdict(list)
来源：http://mobile.hesvh.cn/Article/details/gmwjlrdgg.sHtML

[U15] Py：高精度计时
来源：http://wap.fehbvm.com/Article/details/gtvrywsaw.sHtML

t = time.perf_counter()
来源：http://www.m.share.hesvh.cn/Article/details/gqlrapqxu.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fehbvm.com/Article/details/gbednnnbv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fehbvm.com/Article/details/gybafoxxv.sHtML

[U17] Py：初始化日志
来源：http://blog.zdbjq.cn/Article/details/gnfusrwib.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.hesvh.cn/Article/details/gowsoydzp.sHtML

[U18] Py：预编译正则
来源：http://blog.zdbjq.cn/Article/details/glqyjznpz.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gqjizgnqx.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.hesvh.cn/Article/details/ggphylzid.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.hesvh.cn/Article/details/gnhbejpel.sHtML

[U20] Py：缓存函数结果
来源：http://wap.hesvh.cn/Article/details/grloysadr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.hesvh.cn/Article/details/gaqmbqpva.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.hesvh.cn/Article/details/gmmdwfjpv.sHtML

@contextlib.contextmanager
来源：http://www.blog.fehbvm.com/Article/details/gnghyczcx.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fehbvm.com/Article/details/gjjjcctwe.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/gnhrbcgst.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.hesvh.cn/Article/details/gbyqlopou.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.zdbjq.cn/Article/details/gsjpzvhtx.sHtML

[U24] Py：路径操作
来源：http://www.share.zdbjq.cn/Article/details/gfxtfhrfj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gpkskxypt.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.hesvh.cn/Article/details/gutgmaruf.sHtML

csv.DictReader(f)
来源：http://blog.zdbjq.cn/Article/details/gelmzocqf.sHtML

[U26] Py：并发下载
来源：http://www.blog.zdbjq.cn/Article/details/govruumus.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.hesvh.cn/Article/details/guomyociy.sHtML

[U27] Py：异步 HTTP
来源：http://baike.hesvh.cn/Article/details/gxxkpumwd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.hesvh.cn/Article/details/gtexahkwg.sHtML

[U28] Py：类型别名
来源：http://read.share.fehbvm.com/Article/details/gtbwujhps.sHtML

UserId = int
来源：http://www.share.fehbvm.com/Article/details/gskbedgar.sHtML

[U29] Py：属性校验
来源：http://wap.fehbvm.com/Article/details/gyenaouxc.sHtML

@property 与 @x.setter 配合
来源：http://3g.hesvh.cn/Article/details/gfwzzyjxm.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gkdlvlnxj.sHtML

@dataclass(slots=True)
来源：http://blog.zdbjq.cn/Article/details/gcraqrvop.sHtML

[U31] Py：单测
来源：http://baike.fehbvm.com/Article/details/gjdittwip.sHtML

python -m pytest -q
来源：http://www.m.share.hesvh.cn/Article/details/gstfljoha.sHtML

[U32] Py：代码格式化
来源：http://read.share.hesvh.cn/Article/details/gbcwkqnkx.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fehbvm.com/Article/details/gttaafeqp.sHtML

[U33] Py：打包发布
来源：http://wap.zdbjq.cn/Article/details/gqfxapntq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fehbvm.com/Article/details/gtnalshtl.sHtML

[U34] Py：判断编码
来源：http://mobile.hesvh.cn/Article/details/gfndfitwe.sHtML

chardet.detect(raw)
来源：http://read.share.hesvh.cn/Article/details/gsjftlutv.sHtML

[U35] Py：发送邮件
来源：http://mobile.fehbvm.com/Article/details/gvbgmqrub.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/gfkkfkqmy.sHtML

[U36] Py：定时任务
来源：http://wap.fehbvm.com/Article/details/gywyffiwx.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fehbvm.com/Article/details/gekaikpff.sHtML

[U37] Py：读写 Excel
来源：http://mobile.zdbjq.cn/Article/details/gojmaaqhq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/gwclixagm.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/gpiecdcgb.sHtML

Path(__file__).resolve().parent
来源：http://read.share.zdbjq.cn/Article/details/ggqeijfvh.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.zdbjq.cn/Article/details/gtpztpaxz.sHtML

sys.stdout.isatty()
来源：http://www.share.zdbjq.cn/Article/details/gyufgufcy.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/gxhtppeih.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gjadefonf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fehbvm.com/Article/details/giaeumgqd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.zdbjq.cn/Article/details/gwzofljhs.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.hesvh.cn/Article/details/gcjobepcy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.zdbjq.cn/Article/details/gxrwvopvb.sHtML

[U43] PHP：声明命名空间
来源：http://wap.hesvh.cn/Article/details/ggkajxvym.sHtML

namespace App\Http;
来源：http://read.share.hesvh.cn/Article/details/goattgiiu.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.hesvh.cn/Article/details/gmuxaldxh.sHtML

declare(strict_types=1);
来源：http://3g.fehbvm.com/Article/details/gehptnmnj.sHtML


<!-- 参考信息 -->