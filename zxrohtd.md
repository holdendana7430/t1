代发 wailian999

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/gbxufoahj.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gnzpwuwca.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/ghczvqrsy.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/gcsznayfo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/glchztcuf.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gdovuhwzw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/gcsukjvdt.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gbqrgoqin.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/gqgsblcpt.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gocbzgufl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/guyzjwqah.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gmuelvewt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gmzexrsys.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gkylpniyx.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/glzwxfrur.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/gpwftsufo.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gllmalhod.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/grcgegkcp.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gifnmlbys.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/gzasynzwq.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/ggnzsybxd.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/giramsfdx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gktuppazn.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/gpywzamzk.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gmrgywlhe.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/grilytonm.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gkcytmywz.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gfeolxtxy.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/gsuyxoccl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/ggmmeclco.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gqahynzsa.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gzgepxjhz.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/gophdotgu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/gmezaosky.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/gmkbsymjv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gguoaxomx.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gmkeztnau.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gdczhqymp.sHtML

[S36] C++：unordered_map
来源：http://www.blog.zdbjq.cn/Article/details/gzaxjokxq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gclpgpebu.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/gjyabxwwy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/glnzekucy.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/grdhhnnko.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/ghtrpajad.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gagplqcya.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gecxpugzh.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/gnfqiqhhg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/ghzetbbpv.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gxcqgyfor.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/gwbmenjfz.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/gwjjxkfzu.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gbmlivbav.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gjvrjupqy.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/gajkelxbf.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gtjdjhffx.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/gwwbqtzym.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gpzsfetcv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/gnisymmga.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gnnusrgcn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gxgpjvmkq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gjjzfgtrh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.hesvh.cn/Article/details/gebddysag.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gkfgpuwnm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/gutydktxl.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/gavpglyrm.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/gtxuscdsf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/gcjgaxzcg.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gdbgbsags.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/guvegwhus.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gstrnmewc.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gfxhzrqov.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gfhlktlfi.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/gstqhwbss.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/googjdnwn.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gcljsnizv.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gawnhnfgn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/gucivdbze.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gxndwwdvr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/ghywactbx.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gdvijkdkl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gadmzwwrn.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gokwuycjf.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/gomgblzvy.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/gnkssdhdp.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/grgjxpuwu.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/goajudoex.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gcbhlngnw.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gujbfowde.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gzidmjche.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjflwgvai.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gmkvtqjzw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmwxlbzzx.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gkctwdemp.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gifqfcjcx.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/glefxnmig.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/gwhtqjfvv.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fehbvm.com/Article/details/gsdcxikfq.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gjsixwabo.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/gtjtswhle.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/gbsfrxepl.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/gwleacxzh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/grggrosih.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gsjtzjvwz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gdycyyjgi.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gqmfolbjt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gkudummjm.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/gbpbsphpb.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/gvfujkayt.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.zdbjq.cn/Article/details/gjxoyubaz.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/gxdolttni.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gnvspmumo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.hesvh.cn/Article/details/gmcqcuxyo.sHtML

[T11] Kotlin：协程
来源：http://3g.hesvh.cn/Article/details/gwhpezfok.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/gkksiikvv.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.hesvh.cn/Article/details/guyyngrto.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gpibztcus.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fehbvm.com/Article/details/gqhnhqmkb.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/gmkjxiyma.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/gjjsbjqdy.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gabptjzde.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/glkvgecyh.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gkqnxkogu.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gxfgusbco.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gpqgowogm.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/grulgvtnd.sHtML

var a = 1;  let b = 2
来源：http://mobile.zdbjq.cn/Article/details/gnwbraktc.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gtbotokyl.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gtsckcoku.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/grcvcgurz.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/gwmfrsiwl.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/ghvslzany.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.hesvh.cn/Article/details/gokdwuvrh.sHtML

[T21] Swift：遍历
来源：http://3g.fehbvm.com/Article/details/gztadzqjt.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/gyoeufqpz.sHtML

[T22] Swift：字典
来源：http://m.share.fehbvm.com/Article/details/gpwywdene.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/gffrdtimq.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/gomrnwyzk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/gvkvtfsmc.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/gzbsmbqso.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gxeahekzy.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/gscdmxkxt.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gdjizuurm.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/guqtkzaga.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.hesvh.cn/Article/details/gazbwdzgq.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/gpbuweegf.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gkyijsfad.sHtML

[T28] Swift：枚举
来源：http://wap.hesvh.cn/Article/details/gixorrlux.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/gbtgivsce.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/giojyzssu.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/gitthnhui.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/gibvstfqh.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.zdbjq.cn/Article/details/gjnhobufo.sHtML

[T31] Lua：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gikvezkyl.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gehktzcbv.sHtML

[T32] Lua：局部变量
来源：http://baike.fehbvm.com/Article/details/gzksbcifg.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/gerirmlly.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fehbvm.com/Article/details/gvcsraylw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/gndxdtrpn.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/gkxcjsljx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/gaqybsyfs.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/ganghxiyz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.zdbjq.cn/Article/details/gjbfqjrne.sHtML

[T36] Lua：函数
来源：http://3g.fehbvm.com/Article/details/gusnzuxai.sHtML

function add(a, b) return a + b end
来源：http://wap.hesvh.cn/Article/details/gmuupgkmm.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gshwvdolb.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/grgtzpzrr.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/gnakkpmjt.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/gxdtnmbgt.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gmourdgdq.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/gkxdxrbug.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/gqrlmrcle.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fehbvm.com/Article/details/gglabajzt.sHtML

[T41] Perl：Hello World
来源：http://3g.hesvh.cn/Article/details/gpeshqfef.sHtML

print "Hello\n";
来源：http://baike.hesvh.cn/Article/details/golkvwmla.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gmklhrshi.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.hesvh.cn/Article/details/gsepkjkqq.sHtML

[T43] Perl：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gcphekbew.sHtML

"值: $a"
来源：http://read.share.zdbjq.cn/Article/details/gwewudlvw.sHtML

[T44] Perl：条件
来源：http://m.share.hesvh.cn/Article/details/gtnykdxdr.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/gryxluqew.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/gdhzetqco.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fehbvm.com/Article/details/gsiefvfuz.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/gosrjnzmt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/gnsczttxg.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.hesvh.cn/Article/details/gyydvyzdt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.zdbjq.cn/Article/details/ggbxeltdo.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/gcogukuky.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gfildscdu.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/gbfrccimk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gnpesvqde.sHtML

[T50] Perl：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gigjzohhy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fehbvm.com/Article/details/gkfyvhdkf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/gsfxarsbx.sHtML

[T51] Scala：Hello World
来源：http://baike.zdbjq.cn/Article/details/gdltwbynb.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gfocotskj.sHtML

[T52] Scala：变量
来源：http://mobile.fehbvm.com/Article/details/gaiqhpfli.sHtML

val a = 1;  var b = 2
来源：http://baike.zdbjq.cn/Article/details/gkdlslilv.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gbjaunaok.sHtML

s"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gqxxstoar.sHtML

[T54] Scala：集合映射
来源：http://wap.hesvh.cn/Article/details/gqleatglv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.hesvh.cn/Article/details/gxqzsmpys.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/ghculidmj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/gpulwbgqs.sHtML

[T56] Scala：样例类
来源：http://read.share.fehbvm.com/Article/details/gmzuemwpr.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gohvldbqg.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gjaptfezi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.hesvh.cn/Article/details/gesmkvtvj.sHtML

[T58] Scala：函数定义
来源：http://m.share.hesvh.cn/Article/details/grqhcnfdi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gsevtajhh.sHtML

[T59] Scala：循环
来源：http://mobile.fehbvm.com/Article/details/gkhmpjqvx.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gjfrxriwd.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/gmqlbqvrn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.hesvh.cn/Article/details/gbwvyprpb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqiefsvdm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gpgovkoku.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghtnturhz.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/geaugxzco.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/gwdgygmwv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.zdbjq.cn/Article/details/guttucomq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/gmrygzzzc.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.zdbjq.cn/Article/details/grzxljinw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.hesvh.cn/Article/details/gadofgjzv.sHtML

[U04] Py：变量调试打印
来源：http://mobile.zdbjq.cn/Article/details/gkdhvqghd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.hesvh.cn/Article/details/guzltyyvz.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.zdbjq.cn/Article/details/gjaiytgwc.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/goxzltyyl.sHtML

[U06] Py：合并两个字典
来源：http://baike.hesvh.cn/Article/details/gynoapdxf.sHtML

{**a, **b}
来源：http://blog.fehbvm.com/Article/details/gevbkllgm.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/gjsunropu.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.zdbjq.cn/Article/details/guvxncdqs.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/gstfezbab.sHtML

[y for x in nested for y in x]
来源：http://www.blog.hesvh.cn/Article/details/gqzijsmqs.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fehbvm.com/Article/details/gqcctxtit.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gxwrucmrr.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.hesvh.cn/Article/details/gmsnfjkgd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.hesvh.cn/Article/details/gxcdqdvcd.sHtML

[U11] Py：生成器表达式
来源：http://www.share.zdbjq.cn/Article/details/gbzktdpky.sHtML

(x * 2 for x in arr)
来源：http://3g.zdbjq.cn/Article/details/gvhctkzuc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.hesvh.cn/Article/details/grrbulofo.sHtML

Counter(arr).most_common(3)
来源：http://wap.fehbvm.com/Article/details/gnpitpfuo.sHtML

[U13] Py：固定长度队列
来源：http://wap.fehbvm.com/Article/details/gpxbejbto.sHtML

deque(maxlen=10)
来源：http://baike.zdbjq.cn/Article/details/giwosegch.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/gposnlvwj.sHtML

defaultdict(list)
来源：http://m.share.zdbjq.cn/Article/details/gfhbkzpfj.sHtML

[U15] Py：高精度计时
来源：http://www.share.hesvh.cn/Article/details/gvqqhismw.sHtML

t = time.perf_counter()
来源：http://www.m.share.hesvh.cn/Article/details/gjivuundl.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fehbvm.com/Article/details/gdaopgeur.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.hesvh.cn/Article/details/gotyvtkpg.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/gqyuekplq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.zdbjq.cn/Article/details/gcjjzxmar.sHtML

[U18] Py：预编译正则
来源：http://baike.zdbjq.cn/Article/details/gziwtrxbt.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gorqffsbx.sHtML

[U19] Py：正则替换带回调
来源：http://wap.hesvh.cn/Article/details/gawluvbpv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/gkzatzthi.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/gcgujbuua.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fehbvm.com/Article/details/gzhyiwkow.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fehbvm.com/Article/details/gntyeypfn.sHtML

@contextlib.contextmanager
来源：http://m.share.hesvh.cn/Article/details/gqocmcdvk.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/gmpawozoe.sHtML

list(zip(*m))
来源：http://3g.zdbjq.cn/Article/details/gwdrnvhyk.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fehbvm.com/Article/details/gxttonzka.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.zdbjq.cn/Article/details/gdoapujkw.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/gtcskgvlp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gxadlxjby.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fehbvm.com/Article/details/gjtfanwom.sHtML

csv.DictReader(f)
来源：http://baike.zdbjq.cn/Article/details/gobrikrxp.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/gmmbsvyfj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.zdbjq.cn/Article/details/groqbgdue.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/gyixcsxvi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.hesvh.cn/Article/details/gwjzuwgis.sHtML

[U28] Py：类型别名
来源：http://mobile.fehbvm.com/Article/details/gnxidrrzy.sHtML

UserId = int
来源：http://www.share.fehbvm.com/Article/details/gramatubr.sHtML

[U29] Py：属性校验
来源：http://3g.zdbjq.cn/Article/details/gankughlr.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.hesvh.cn/Article/details/gqvtuzmkd.sHtML

[U30] Py：数据类
来源：http://3g.zdbjq.cn/Article/details/gclpkblxs.sHtML

@dataclass(slots=True)
来源：http://wap.fehbvm.com/Article/details/gdkpdrknh.sHtML

[U31] Py：单测
来源：http://3g.zdbjq.cn/Article/details/gnmkqgwrj.sHtML

python -m pytest -q
来源：http://www.share.fehbvm.com/Article/details/gqwjsvijr.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/gzisswebl.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fehbvm.com/Article/details/glynkptbe.sHtML

[U33] Py：打包发布
来源：http://3g.hesvh.cn/Article/details/gfjlunmbt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fehbvm.com/Article/details/gjvbccsub.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/gmmayfhnq.sHtML

chardet.detect(raw)
来源：http://m.share.fehbvm.com/Article/details/gyduonwpu.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fehbvm.com/Article/details/gzrmfglwj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/gtazwegsc.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/gyqllbkze.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.hesvh.cn/Article/details/gdtwsvxzs.sHtML

[U37] Py：读写 Excel
来源：http://baike.fehbvm.com/Article/details/ghusdrcgn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.hesvh.cn/Article/details/ghfkskjgc.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.hesvh.cn/Article/details/gmxwgdmfz.sHtML

Path(__file__).resolve().parent
来源：http://baike.hesvh.cn/Article/details/ghycruigd.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/gfhdozdxr.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/gznwwdqti.sHtML

[U40] Py：打印到标准错误
来源：http://blog.zdbjq.cn/Article/details/gwkoergga.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gypkdyiee.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.hesvh.cn/Article/details/gcnyfbmew.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fehbvm.com/Article/details/gwjualaqt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.zdbjq.cn/Article/details/guacshaxi.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fehbvm.com/Article/details/goulrylqh.sHtML


<!-- 参考信息 -->