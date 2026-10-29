代发 wailian999

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/gnirlgnag.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/gqtlzgqav.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gdpqnlowb.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gdmxjapyo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gjnnxokhz.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gzfxbotjz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/gydiingmf.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gdejfiwvb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gsesfapqh.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gnpsdjoxp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gvmykvrls.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gcpwmlyib.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/ggoihmucc.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/ghzrlkqbw.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/gcehgocja.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gxwbvadww.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gtbtqtmoa.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gyvmvhlwc.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gucnufjfh.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/guyenmxrr.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gsvnejszl.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/gqcyellrx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gquffsfbl.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gmxeuvekn.sHtML

#ifndef X_H
来源：http://wap.zdbjq.cn/Article/details/gzaaszgse.sHtML

#define X_H
来源：http://www.m.share.fehbvm.com/Article/details/gzgckqoid.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gnmrduomu.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/gnknfiizr.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/gxhkiuaua.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gwzxwzyqs.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gswijrrtx.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/grroybeqj.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gedkogyae.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/ghmvblpvb.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gzuqrpffi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/geqqmpvir.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/gevbikyrj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gplotuqtn.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/giocptcbn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gxrbuiopo.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gtpdkwube.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/gtuagnkgw.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/gwppvsqnb.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gdqwqplza.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/gbigsdgnm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/gnvmwvteq.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/gbriwuser.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/ggsivjmln.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gglqhvdlx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/gegeqxtmq.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/gprmjcxxe.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gfwgzlckm.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/gdusnvfrc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/guvgrzjwl.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/gjwpqcqev.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gfaixftgi.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/gujqbadlz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/gfftbmlaq.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gbeigkzrs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/gapffejbu.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gmywcvqqn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gahwtbria.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/grpzbhurr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/gcyjttslw.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/gvaouwalw.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/gfbbxuide.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/ghsjetugq.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/gcfdamyac.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/gcoqbsywv.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gxwdtgpae.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/gzssynxjq.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/glalbcwki.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/gjhujlatj.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/gvcginbur.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gsclieluw.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gkgxoeeya.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/ggkwtoerh.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gaiyhatrr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/gbadmtsep.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/glfscycya.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gpumibkdy.sHtML

[S57] C++：编译期常量
来源：http://blog.hesvh.cn/Article/details/gtjtqmvio.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/graoduqhu.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/givegefrb.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/gehfmqwxg.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gmwdalokp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/gvkcxglzs.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/genbskyfn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/gmlqrrpaa.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnhqtnreb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gqbdsepyy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjyejohts.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gmrooshdn.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gvdnjrloj.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gygmauypv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gjsvixiur.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gzejpmzgp.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gfyptzmpa.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/gtwfzyhiu.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/gymxogghk.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gcwxqhqtz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gxcbnxtjz.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/geifrhibi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gxtffymky.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gqtnhpeky.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/gxpcccwzw.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gofjvozuf.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gewraqaoj.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/gromzbylk.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/guxapprzd.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gymgyxsjr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/ghbddmpxc.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gypetezee.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.zdbjq.cn/Article/details/gedwrpdpx.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gaegeuoyg.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gghxfmtkn.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.hesvh.cn/Article/details/gysenpatt.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/glhzavoqm.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gxpmjwudc.sHtML

for (i in 1..10) println(i)
来源：http://baike.zdbjq.cn/Article/details/guatrieyb.sHtML

[T15] Kotlin：接口
来源：http://wap.hesvh.cn/Article/details/gydcmuibm.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/geztttjaa.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gmiatnpyw.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gxavwhydn.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/gkwfwzbln.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/gxloilohr.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gkyjeqxil.sHtML

"值: \(b)"
来源：http://mobile.fehbvm.com/Article/details/gzmjngwwh.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gfnitmkzm.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/gothcfewl.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/gvtngolpu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/ggpabvxhw.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/gbemucpum.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/gnzvzcmhz.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/gpfispyis.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/gaflolyxt.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gfaagddgp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/gygayygnu.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/gpcisgryb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gnwuudzoc.sHtML

[T25] Swift：结构体
来源：http://www.m.share.zdbjq.cn/Article/details/grobowtnr.sHtML

struct P { var x: Int }
来源：http://blog.hesvh.cn/Article/details/gdoqdxnsl.sHtML

[T26] Swift：类与重写
来源：http://www.share.hesvh.cn/Article/details/gimogtett.sHtML

class A: Base { override func f() {} }
来源：http://mobile.hesvh.cn/Article/details/gbtgbvydx.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/gvhboewkn.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gilbqttru.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/gtvyozvhy.sHtML

enum Color { case red, green }
来源：http://www.share.fehbvm.com/Article/details/gjvhybkns.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/gqmlkypos.sHtML

guard let x = opt else { return }
来源：http://www.blog.fehbvm.com/Article/details/gjktjqozt.sHtML

[T30] Swift：协议
来源：http://www.share.fehbvm.com/Article/details/gwshlpicg.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/gyxnhibjd.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/gpoypevzy.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gmbttlgqi.sHtML

[T32] Lua：局部变量
来源：http://baike.fehbvm.com/Article/details/gstecgrwq.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gtlzdndst.sHtML

[T33] Lua：表（数组）
来源：http://baike.zdbjq.cn/Article/details/geieoobds.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.zdbjq.cn/Article/details/ggnawylvt.sHtML

[T34] Lua：遍历表
来源：http://read.share.fehbvm.com/Article/details/gjqdutavm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.hesvh.cn/Article/details/gipleacie.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/gzaczsgpx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/guxbuakpr.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/gljcysjzx.sHtML

function add(a, b) return a + b end
来源：http://read.share.fehbvm.com/Article/details/goqmnyhfs.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fehbvm.com/Article/details/gerywzsne.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/glybmdcau.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gazapytpo.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/gnzagnlkw.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gcpcgxydn.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gqxroehyk.sHtML

[T40] Lua：元表
来源：http://www.m.share.fehbvm.com/Article/details/gyktnvykp.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fehbvm.com/Article/details/gwdrbyecz.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gxounsxwr.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/gvuiwvbrz.sHtML

[T42] Perl：变量类型
来源：http://mobile.hesvh.cn/Article/details/gzverhwxt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.hesvh.cn/Article/details/gfhdvnpcb.sHtML

[T43] Perl：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gobuhpkpx.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/gqxfixkkw.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/gtxcuukhe.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/grgrsacuu.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/gwfakqcuc.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fehbvm.com/Article/details/ggitxzgoz.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.zdbjq.cn/Article/details/gjjmarkuv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwptzqgbw.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/gjkuozssg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/gancvzych.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/gkmgbyaec.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gmffbvzom.sHtML

[T49] Perl：函数
来源：http://m.share.hesvh.cn/Article/details/guwofojde.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gempzwonq.sHtML

[T50] Perl：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gjifwlsne.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fehbvm.com/Article/details/gqxfqvezl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/gsjnvgipx.sHtML

[T51] Scala：Hello World
来源：http://wap.zdbjq.cn/Article/details/gmmpfadjm.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gvvbllvsu.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/gcccdimet.sHtML

val a = 1;  var b = 2
来源：http://read.share.hesvh.cn/Article/details/grrarardj.sHtML

[T53] Scala：字符串插值
来源：http://baike.fehbvm.com/Article/details/gekxtyndn.sHtML

s"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gerhbhgrs.sHtML

[T54] Scala：集合映射
来源：http://baike.zdbjq.cn/Article/details/grfjukhhl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.hesvh.cn/Article/details/gexccfias.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gzbsngsxg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.zdbjq.cn/Article/details/glsejjlpi.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/gwloedxeu.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gkixmtsgh.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/gowcqqktg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/gmagofojx.sHtML

[T58] Scala：函数定义
来源：http://wap.fehbvm.com/Article/details/ggzroelcp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.zdbjq.cn/Article/details/gkwpmsqyr.sHtML

[T59] Scala：循环
来源：http://www.blog.hesvh.cn/Article/details/geagfswgl.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/gtstsugtk.sHtML

[T60] Scala：折叠
来源：http://wap.zdbjq.cn/Article/details/glttnqsjg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.hesvh.cn/Article/details/gqscocbup.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gttwslcbj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/gnmzrsudo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/geyuqlmqq.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.zdbjq.cn/Article/details/gsqdbvhpo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.hesvh.cn/Article/details/goxvzohrg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fehbvm.com/Article/details/glcpnsvod.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/gnbbvuekv.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.zdbjq.cn/Article/details/gqgsysqmh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.zdbjq.cn/Article/details/gwrxncrse.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.hesvh.cn/Article/details/grekrqfqx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.zdbjq.cn/Article/details/ghlrpngoy.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/ggdhqvuei.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gpvgkfucp.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/gyyvigwjv.sHtML

{**a, **b}
来源：http://baike.hesvh.cn/Article/details/gyjmeabjg.sHtML

[U07] Py：反转字典键值
来源：http://m.share.zdbjq.cn/Article/details/gdjpxhvgs.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fehbvm.com/Article/details/gkfkktgdx.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/gfyfheepz.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gghydmzdi.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.zdbjq.cn/Article/details/gdutlyjkd.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/gwobknfbh.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fehbvm.com/Article/details/gppwwivna.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.hesvh.cn/Article/details/giqpsjwau.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/gnnygannl.sHtML

(x * 2 for x in arr)
来源：http://wap.fehbvm.com/Article/details/gfoxmyhvi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.zdbjq.cn/Article/details/gcifeakzs.sHtML

Counter(arr).most_common(3)
来源：http://read.share.hesvh.cn/Article/details/gullnvvnf.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/gghzhkomw.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/guvnfensw.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fehbvm.com/Article/details/gjzdxince.sHtML

defaultdict(list)
来源：http://m.share.fehbvm.com/Article/details/ggsicyjgf.sHtML

[U15] Py：高精度计时
来源：http://m.share.zdbjq.cn/Article/details/gtuxgtadd.sHtML

t = time.perf_counter()
来源：http://blog.fehbvm.com/Article/details/gexppupnd.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/grywnjhpg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/grupwuyna.sHtML

[U17] Py：初始化日志
来源：http://baike.zdbjq.cn/Article/details/gjowwjsaz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/glvbcefdt.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fehbvm.com/Article/details/goijruaee.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/grdkyabhp.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.hesvh.cn/Article/details/gwadqqaoa.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fehbvm.com/Article/details/gaassmyms.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fehbvm.com/Article/details/gcmcjhclf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.hesvh.cn/Article/details/gjfjcqrme.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.zdbjq.cn/Article/details/goywxoqnc.sHtML

@contextlib.contextmanager
来源：http://3g.zdbjq.cn/Article/details/guvmfdakk.sHtML

[U22] Py：矩阵转置
来源：http://blog.zdbjq.cn/Article/details/gtientmcd.sHtML

list(zip(*m))
来源：http://mobile.fehbvm.com/Article/details/groxzikgd.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fehbvm.com/Article/details/gvspbfrxs.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.zdbjq.cn/Article/details/guxdhkimd.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/gxhdpwqwj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gcaetaxyq.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.hesvh.cn/Article/details/goefqtdmm.sHtML

csv.DictReader(f)
来源：http://read.share.zdbjq.cn/Article/details/gncjvtjyn.sHtML

[U26] Py：并发下载
来源：http://blog.fehbvm.com/Article/details/ghiiriyge.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.hesvh.cn/Article/details/gbgxhbvta.sHtML

[U27] Py：异步 HTTP
来源：http://blog.hesvh.cn/Article/details/gcerajsqj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.zdbjq.cn/Article/details/gxiyeuzht.sHtML

[U28] Py：类型别名
来源：http://www.m.share.hesvh.cn/Article/details/gupqamlug.sHtML

UserId = int
来源：http://www.share.zdbjq.cn/Article/details/gxvvzeudh.sHtML

[U29] Py：属性校验
来源：http://baike.hesvh.cn/Article/details/gdfzbjinb.sHtML

@property 与 @x.setter 配合
来源：http://wap.hesvh.cn/Article/details/gjdxwievt.sHtML

[U30] Py：数据类
来源：http://www.blog.fehbvm.com/Article/details/gbrdwysme.sHtML

@dataclass(slots=True)
来源：http://3g.fehbvm.com/Article/details/gblpqkcie.sHtML

[U31] Py：单测
来源：http://3g.zdbjq.cn/Article/details/gpmjbydvj.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/gwmmotzqv.sHtML

[U32] Py：代码格式化
来源：http://m.share.fehbvm.com/Article/details/gcfbfngzr.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fehbvm.com/Article/details/gcpjabgha.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/gvbehbvlh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.zdbjq.cn/Article/details/gvkvnztas.sHtML

[U34] Py：判断编码
来源：http://m.share.zdbjq.cn/Article/details/ghxgfqudv.sHtML

chardet.detect(raw)
来源：http://www.m.share.hesvh.cn/Article/details/gihwunjtu.sHtML

[U35] Py：发送邮件
来源：http://mobile.fehbvm.com/Article/details/gbvsjkfzx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/gkouzewqr.sHtML

[U36] Py：定时任务
来源：http://mobile.fehbvm.com/Article/details/gosizdnum.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/gibjsmtza.sHtML

[U37] Py：读写 Excel
来源：http://www.share.hesvh.cn/Article/details/gnjwbydgr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fehbvm.com/Article/details/gfexkvonz.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.hesvh.cn/Article/details/gaiesuans.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.zdbjq.cn/Article/details/gjhmkgwor.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fehbvm.com/Article/details/ggoxdejpo.sHtML

sys.stdout.isatty()
来源：http://m.share.fehbvm.com/Article/details/glqvptqax.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fehbvm.com/Article/details/gmyaxcarw.sHtML

print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gpqvwfjnh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.zdbjq.cn/Article/details/gcpcjkpup.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/gorhbamag.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.zdbjq.cn/Article/details/gpqijyspy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.hesvh.cn/Article/details/gnxmawvyr.sHtML


<!-- 参考信息 -->