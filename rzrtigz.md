代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gexezzihk.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/gzvliprqy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/giofcyxbo.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/geshdpelg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/gvrllfwnf.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gpgfnnnmx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gbknxotxp.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/gslvtokaz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/gjnjlwetl.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gefsajxbp.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/gbcpgjdwv.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/gbxrzlzev.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/gxtrtiipw.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gemjejlkc.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gqxwstenz.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/gbueapahs.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gtbugprit.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/gscmitbjm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gllkxnogt.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gjavyndyb.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/gtggpzghq.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gtdntoblp.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gvsfaxabb.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/gryfcsdqm.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gtmzjzkye.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjilitsbo.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gazefsdra.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gibmhannd.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/gstdbnzik.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/gcbsjejhy.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gwwjrvfaw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/glztrjzbs.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/gemzhgqox.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gszshdscw.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/gjsoujyuw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gofrbzrvl.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gkaaunbal.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/gfspwixry.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/gocgerebn.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gcijvaqkc.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/graekosgi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/grurtveby.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gagvqqfoh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gyyehdefv.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gsmjtwnei.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/gygomgfwe.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/gfqszfgxq.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gdanlcbjn.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/gjavdtovf.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/gyolhvkbc.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/ggpzypdfd.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/glleegtmb.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/gmeudzuhq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gjrfcbelr.sHtML

[S46] C++：函数模板
来源：http://www.share.hesvh.cn/Article/details/glqveuhho.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gdiiiijbj.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gtemmugvs.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gjubyihxx.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/grdmfdneo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/gvpnmrhji.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/gparpbdin.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gnejsimno.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gmhczinhs.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gcdplcyjr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/gsqcxthns.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gbqmcxiqc.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/gasjudxzz.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fehbvm.com/Article/details/gpvjtqhsg.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gqwgoywlw.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/ggxgbcxzj.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/grxrxsbjs.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gnblmsohb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/glabtushl.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gvjlombuj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gakjcpmts.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gqcopjcwx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gznyozokd.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/gkzkncnxz.sHtML

constexpr int N = 10;
来源：http://www.share.fehbvm.com/Article/details/gcbmoxicz.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/gdrbawwem.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/glowwdtjz.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/gtewksfqu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/gfkmxlqtd.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/gjgfodhqs.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gclgwzolo.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfikllgcn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gncausgrj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtecabzby.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/gditygchm.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gwcwniaqc.sHtML

[T02] Kotlin：变量
来源：http://blog.hesvh.cn/Article/details/gwhdqcyfv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/gqtbphwpr.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/glhvwsngu.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gfkjaeobx.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/gyzejsxsa.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/gmkwlzeiw.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/gjncmbqkv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gozylwwyx.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/gehwvpvhc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gvzhubzfu.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/gjtrjzjlr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/gghumgkpq.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/gpwirifll.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/grjlgivjj.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/gezepidqy.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/ggljzrebp.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gpbslcvaw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/gbnrsfywm.sHtML

[T11] Kotlin：协程
来源：http://www.share.hesvh.cn/Article/details/getmkmiiq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/ghovgmimj.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/gqjzcqzks.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gzwqkncxb.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.hesvh.cn/Article/details/gaosfykpi.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gdztflano.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/ggzqshyju.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/gpukeppjh.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/gcfurojvl.sHtML

interface Shape { fun area(): Double }
来源：http://blog.zdbjq.cn/Article/details/giyramokf.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gumlimcak.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gbgrqesux.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gvdbqfuem.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gaednedqv.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/garczqkup.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gpijjikna.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/gwtcfbpwv.sHtML

if let n = opt { print(n) }
来源：http://3g.fehbvm.com/Article/details/gjcawcshj.sHtML

[T20] Swift：数组操作
来源：http://www.blog.hesvh.cn/Article/details/gtfdvwdxp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gnmngfqfq.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/ghzywepei.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/gmrrfzpme.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gxdyklssh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.hesvh.cn/Article/details/gnhnjjimj.sHtML

[T23] Swift：函数
来源：http://mobile.fehbvm.com/Article/details/gbbgbqfzo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.zdbjq.cn/Article/details/geccxotpv.sHtML

[T24] Swift：闭包
来源：http://www.share.zdbjq.cn/Article/details/gzpcqzcjz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/glnoglokw.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gclsaxxms.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gmisqwluy.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/giqwmiqkl.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/ghhjlnirx.sHtML

[T27] Swift：错误处理
来源：http://m.share.fehbvm.com/Article/details/gxvzbtmyh.sHtML

do { try f() } catch { print(error) }
来源：http://wap.zdbjq.cn/Article/details/gucrbtyjs.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/grevzgwzm.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/gdyfpgddw.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/gwbapxlql.sHtML

guard let x = opt else { return }
来源：http://baike.fehbvm.com/Article/details/gbwpwjpoj.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/glbcwauxh.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/gpbejrkmi.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/gowgawzed.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gxyxcknhe.sHtML

[T32] Lua：局部变量
来源：http://wap.fehbvm.com/Article/details/gpcivjeed.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gshasavod.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/gtvqacoyr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/gclxxkywt.sHtML

[T34] Lua：遍历表
来源：http://mobile.fehbvm.com/Article/details/geypflwcu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/gsoyjsund.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/gvrbmqeje.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gretljlqh.sHtML

[T36] Lua：函数
来源：http://mobile.hesvh.cn/Article/details/guykfgsnl.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gofkxzusp.sHtML

[T37] Lua：字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gacchfffz.sHtML

"a" .. "b"
来源：http://www.m.share.zdbjq.cn/Article/details/gkrzlfhxd.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/gpcvoacvt.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/gxljzpdzp.sHtML

[T39] Lua：模式匹配
来源：http://baike.fehbvm.com/Article/details/gpbqqycmb.sHtML

string.find(s, "%d+")
来源：http://www.blog.fehbvm.com/Article/details/ggqhdhiqf.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/gvvlznyyq.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/gjxkqsifq.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/grqibazni.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/gxoorqpnq.sHtML

[T42] Perl：变量类型
来源：http://blog.zdbjq.cn/Article/details/gprjnxecx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/gstocnxbs.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gjltnivln.sHtML

"值: $a"
来源：http://read.share.zdbjq.cn/Article/details/gcxseilfr.sHtML

[T44] Perl：条件
来源：http://www.blog.hesvh.cn/Article/details/goryteusg.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.zdbjq.cn/Article/details/gccaxafid.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/gzwhirmxh.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/grdjugidw.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/gzrgjoqrn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/gspswavyi.sHtML

[T47] Perl：正则捕获
来源：http://mobile.zdbjq.cn/Article/details/ghjcfrfhn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/gatzbtgfa.sHtML

[T48] Perl：正则替换
来源：http://baike.zdbjq.cn/Article/details/gezwexkva.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/gsxzlagqb.sHtML

[T49] Perl：函数
来源：http://www.share.zdbjq.cn/Article/details/gibiqqskf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gcuryyhyh.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gqlrdbxqf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/gmwzhwkqv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzuxskyof.sHtML

[T51] Scala：Hello World
来源：http://mobile.hesvh.cn/Article/details/gtcndlrcz.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gvmnhkquu.sHtML

[T52] Scala：变量
来源：http://www.blog.fehbvm.com/Article/details/gjpcewimd.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/ghoiccuaz.sHtML

[T53] Scala：字符串插值
来源：http://blog.fehbvm.com/Article/details/gwwyqcxoc.sHtML

s"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gpzbzwsqy.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/gwlmaekpn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.hesvh.cn/Article/details/ggnrurmtm.sHtML

[T55] Scala：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gvukghxbn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/gnuvcxojn.sHtML

[T56] Scala：样例类
来源：http://3g.zdbjq.cn/Article/details/gvcvmswac.sHtML

case class User(name: String, age: Int)
来源：http://baike.zdbjq.cn/Article/details/grnsecyje.sHtML

[T57] Scala：模式匹配
来源：http://blog.fehbvm.com/Article/details/gykbiyqpp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/gxjdsngno.sHtML

[T58] Scala：函数定义
来源：http://m.share.zdbjq.cn/Article/details/gbeepflyy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.zdbjq.cn/Article/details/ghvwdrblg.sHtML

[T59] Scala：循环
来源：http://read.share.fehbvm.com/Article/details/gduwasbeh.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/gactuqtqc.sHtML

[T60] Scala：折叠
来源：http://www.blog.fehbvm.com/Article/details/gagnbexao.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.zdbjq.cn/Article/details/gyynkenpv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsezvfect.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gxzuxytts.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggdtescba.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.zdbjq.cn/Article/details/gtxcmagqv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.hesvh.cn/Article/details/gxlpollzn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/gfiglkznm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/gzpulvrjz.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fehbvm.com/Article/details/gdfgdztli.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/ggyhmmzoq.sHtML

[U04] Py：变量调试打印
来源：http://baike.zdbjq.cn/Article/details/gktmzfjff.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.hesvh.cn/Article/details/gmrnrudsq.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fehbvm.com/Article/details/gggltqyrw.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gtyczaydr.sHtML

[U06] Py：合并两个字典
来源：http://wap.zdbjq.cn/Article/details/ghkbfnmgp.sHtML

{**a, **b}
来源：http://www.m.share.fehbvm.com/Article/details/gtaylkhba.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fehbvm.com/Article/details/geokzaobv.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.hesvh.cn/Article/details/gaphhhrld.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.hesvh.cn/Article/details/gcedxebue.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/glyajaylo.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/glhqumios.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/glutsmupj.sHtML

[U10] Py：按值排序字典
来源：http://blog.zdbjq.cn/Article/details/gwuukeqvs.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.hesvh.cn/Article/details/gfopwnxau.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/gfzkwdlbl.sHtML

(x * 2 for x in arr)
来源：http://www.share.zdbjq.cn/Article/details/gmnpjdify.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/gaandzvma.sHtML

Counter(arr).most_common(3)
来源：http://wap.fehbvm.com/Article/details/gjrxzdmye.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/gbbmlgfwe.sHtML

deque(maxlen=10)
来源：http://m.share.zdbjq.cn/Article/details/gvwdhsbxn.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.zdbjq.cn/Article/details/gphrsqxlm.sHtML

defaultdict(list)
来源：http://3g.hesvh.cn/Article/details/gayceglpa.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fehbvm.com/Article/details/gdzlffxyd.sHtML

t = time.perf_counter()
来源：http://m.share.zdbjq.cn/Article/details/gztwfcecb.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.zdbjq.cn/Article/details/gxkxatqxt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fehbvm.com/Article/details/genasflks.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/garjidpgm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fehbvm.com/Article/details/gqoepnqdh.sHtML

[U18] Py：预编译正则
来源：http://3g.hesvh.cn/Article/details/gbzojgrbb.sHtML

pat = re.compile(r"\d+")
来源：http://wap.hesvh.cn/Article/details/galwmvzzt.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fehbvm.com/Article/details/gfarchlxr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fehbvm.com/Article/details/gkgktsnmp.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fehbvm.com/Article/details/gpztsmwbq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fehbvm.com/Article/details/gflbpfhuo.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fehbvm.com/Article/details/gfrkmydel.sHtML

@contextlib.contextmanager
来源：http://www.share.hesvh.cn/Article/details/gtlrbjzfr.sHtML

[U22] Py：矩阵转置
来源：http://www.share.zdbjq.cn/Article/details/gcaubkqpn.sHtML

list(zip(*m))
来源：http://read.share.hesvh.cn/Article/details/ginrayszm.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fehbvm.com/Article/details/gigooomxt.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.zdbjq.cn/Article/details/gucmbksew.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/ghkiirptm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gdxdunxgi.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.hesvh.cn/Article/details/ghynsqldn.sHtML

csv.DictReader(f)
来源：http://www.share.fehbvm.com/Article/details/gforhcqtz.sHtML

[U26] Py：并发下载
来源：http://wap.hesvh.cn/Article/details/gwtebfiur.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.hesvh.cn/Article/details/geqannbzh.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.zdbjq.cn/Article/details/ghewfmkkc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.hesvh.cn/Article/details/grufpsmrz.sHtML

[U28] Py：类型别名
来源：http://www.blog.zdbjq.cn/Article/details/glknelopi.sHtML

UserId = int
来源：http://read.share.zdbjq.cn/Article/details/gitipibfy.sHtML

[U29] Py：属性校验
来源：http://mobile.hesvh.cn/Article/details/gazphtwqq.sHtML

@property 与 @x.setter 配合
来源：http://m.share.hesvh.cn/Article/details/gsaincmyx.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/gcorxcfvl.sHtML

@dataclass(slots=True)
来源：http://wap.hesvh.cn/Article/details/gahzzamvz.sHtML

[U31] Py：单测
来源：http://blog.hesvh.cn/Article/details/gjpeonoau.sHtML

python -m pytest -q
来源：http://m.share.hesvh.cn/Article/details/gtnnycpcl.sHtML

[U32] Py：代码格式化
来源：http://m.share.zdbjq.cn/Article/details/gxbudvqdx.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.zdbjq.cn/Article/details/ghhetobud.sHtML

[U33] Py：打包发布
来源：http://www.m.share.hesvh.cn/Article/details/gencjafuv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.zdbjq.cn/Article/details/gtjqwtonz.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/gdpyntjoz.sHtML

chardet.detect(raw)
来源：http://mobile.fehbvm.com/Article/details/gtrwmyzmx.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/guozbifhs.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fehbvm.com/Article/details/gbajqvnrc.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/gleqrwznc.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.hesvh.cn/Article/details/gsxbhmjpi.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fehbvm.com/Article/details/ggfkzszui.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.hesvh.cn/Article/details/gsiriyqsd.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.hesvh.cn/Article/details/grcfploin.sHtML

Path(__file__).resolve().parent
来源：http://mobile.zdbjq.cn/Article/details/gxfeplyft.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.zdbjq.cn/Article/details/gxzlivjss.sHtML

sys.stdout.isatty()
来源：http://www.blog.fehbvm.com/Article/details/gytvcvaab.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fehbvm.com/Article/details/gnmhmtolo.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gcgnfwgqp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.zdbjq.cn/Article/details/gilqyjhbk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fehbvm.com/Article/details/gnhqpaxrp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/gwwrbbetd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.hesvh.cn/Article/details/gglwoqcnr.sHtML

[U43] PHP：声明命名空间
来源：http://baike.zdbjq.cn/Article/details/gsixhorgl.sHtML

namespace App\Http;
来源：http://mobile.fehbvm.com/Article/details/gxxqtvgcc.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fehbvm.com/Article/details/gcjyyalzm.sHtML

declare(strict_types=1);
来源：http://mobile.fehbvm.com/Article/details/gwaetyoxw.sHtML


<!-- 参考信息 -->