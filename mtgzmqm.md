代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gcxlmtbnf.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitfrqgyn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjoykotiz.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gnnxykolp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gdrqfujzu.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gdpxwjwvv.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/ggaxuyged.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gifhjrzkw.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gtauvshbi.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusvhgdkr.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gmyuewfrl.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhjaflbi.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjchjcwpx.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gmdaljdxe.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggimrzmie.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gvrwslfhq.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gddclfraa.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpbgzajz.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gxeftiqqo.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gojwmapbp.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gttfrqddw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/guuyypluf.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyoftoaa.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/guijrmbvb.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gcdkvgkmq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/grjzaxzne.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxhqtzho.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmubgcryu.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpoarcpq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvuryiyd.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/ghywitaym.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/grutrxeau.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gzxftderz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqsotcum.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxuonaoq.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcgfoicd.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gtthpesvy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrkvlgtm.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gbykfdkpu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gtddifjeq.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtdhghtx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gjxdntrzy.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyqvcyjh.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxlmdopx.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/glgworoyg.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gtapueccw.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/ghtassaqw.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gftpautnv.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gephivhqu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsixvleq.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gqirffkkl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqpyzcap.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gmvprorlg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmheazqfw.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvrlelyr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gehygnecb.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gltonobno.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/geuenyyro.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gugprrtpf.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/guvsgkhkg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafnfaoow.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gnufvofdi.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gplpmuogw.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvxsloxm.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghukflndj.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhrsptcb.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gdwixdanr.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gqoownrox.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gxvcsgspe.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjgjttub.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrsxagxf.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfqgpgqr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdavgdmbh.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdiccirx.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/guofgiibt.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdrlzxzt.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcvqqbdd.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gwboxqtsu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gflqrknsc.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gyztvchyp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjgzawou.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gjwbptfxl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotsiobac.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfodbjey.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojkqqzrz.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gwbknlpdf.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdqzgfsz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqaarfen.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gygxwzaqt.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gwwtbaoht.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gxnwbchey.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/gfkoxxxrr.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsieryrsb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/genjxcooj.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gopgehzlm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsudpeno.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gigbkejnq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzcymnlr.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhmcajhf.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gbblpuhgn.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlfefdzx.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfucpbmz.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gpslnhrlq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gymintjyg.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpphwydre.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/ggoyozfhu.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzevpnkt.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gvriepuyv.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gfqllvifd.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsaabdwtm.sHtML

[T14] Kotlin：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gzebeular.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goluridtg.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztbcktqn.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/goouwrsbf.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmonxxwu.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gpwdcxlle.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgehgplg.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmxvvgok.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjyqvnxe.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksagcvue.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjkduyfh.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gbdzporud.sHtML

[T20] Swift：数组操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gioiehsjd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/ghflnmypx.sHtML

[T21] Swift：遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gfaongala.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcuaothrj.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxrtdqzg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gxzcsmuwz.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gbxsdkegd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/glwgesfmf.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/guantpvbr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpthhleyr.sHtML

[T25] Swift：结构体
来源：http://3g.fanxiaobao.xyz/Article/details/gufncmjof.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxquckga.sHtML

[T26] Swift：类与重写
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcljxtcf.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gcjlgrfyr.sHtML

[T27] Swift：错误处理
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjevttqu.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/gfyhntghp.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphdjxaot.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/gyjzucgks.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gssfflwcc.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gxipwowwn.sHtML

[T30] Swift：协议
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzqcbdin.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gydkcifyx.sHtML

[T31] Lua：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbfodeex.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gacahmweo.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gpagyjeko.sHtML

local a = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvjutcxq.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrsmeskz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/gtobhlkkc.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/gajlkbkzg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fanxiaobao.xyz/Article/details/gntkglvkd.sHtML

[T35] Lua：字典表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldbcvhsy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gnijmhuir.sHtML

[T36] Lua：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gimwedbot.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/gvewreszt.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gramranxv.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/gtoywbmcd.sHtML

[T38] Lua：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gljiroiqc.sHtML

if x > 0 then print("正") end
来源：http://wap.fanxiaobao.xyz/Article/details/gbhskcopf.sHtML

[T39] Lua：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gyfcgcrah.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gttbwgppt.sHtML

[T40] Lua：元表
来源：http://mobile.fanxiaobao.xyz/Article/details/geqagqgpt.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gniqybxaz.sHtML

[T41] Perl：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfqmljvx.sHtML

print "Hello\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqucjmaq.sHtML

[T42] Perl：变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gmsehbefp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fanxiaobao.xyz/Article/details/ghfhifnxa.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gupbmjaop.sHtML

"值: $a"
来源：http://baike.fanxiaobao.xyz/Article/details/gxecrmhvt.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrlegegb.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/giakqhzgs.sHtML

[T45] Perl：数组遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gniwkpngd.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggupzcvor.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsfmiqot.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fanxiaobao.xyz/Article/details/goivzcitb.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdabrurmf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fanxiaobao.xyz/Article/details/glmmlixhd.sHtML

[T48] Perl：正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/gtjrmtszq.sHtML

$s =~ s/old/new/g;
来源：http://wap.fanxiaobao.xyz/Article/details/gfdzhjiph.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gurijvgyt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbmvgezl.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrddtodm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmazjcqj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxpzrynef.sHtML

[T51] Scala：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gpssrdwyo.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydcnxgbk.sHtML

[T52] Scala：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gyvzovdbm.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmpchbwy.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvvpsapg.sHtML

s"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gkwlblvtn.sHtML

[T54] Scala：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/genufgjfe.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gmqruwpiv.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgxgjlzj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhsyymmu.sHtML

[T56] Scala：样例类
来源：http://m.share.fanxiaobao.xyz/Article/details/gijjubkbe.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsfonfkb.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gtyxeogel.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmjmexbk.sHtML

[T58] Scala：函数定义
来源：http://baike.fanxiaobao.xyz/Article/details/gzsjkfhin.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gliujmcrf.sHtML

[T59] Scala：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gickyardo.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyictpcu.sHtML

[T60] Scala：折叠
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvryxluou.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkmjwtmu.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfhinnii.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gsdfafawv.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gygnshjwq.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fanxiaobao.xyz/Article/details/gsikicqje.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgwrkvzd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqthdzsj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fanxiaobao.xyz/Article/details/geneehevb.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzdfhjrr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fanxiaobao.xyz/Article/details/guhjuqqld.sHtML

[U04] Py：变量调试打印
来源：http://wap.fanxiaobao.xyz/Article/details/glchxpjwf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fanxiaobao.xyz/Article/details/gjolhuwio.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmfewwmi.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gizmmlhvj.sHtML

[U06] Py：合并两个字典
来源：http://baike.fanxiaobao.xyz/Article/details/gjnxobalo.sHtML

{**a, **b}
来源：http://baike.fanxiaobao.xyz/Article/details/gptovmnif.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtsbaujb.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxrbuabj.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtuhhuvl.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsxbqojg.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fanxiaobao.xyz/Article/details/gewswdzrk.sHtML

max(d, key=d.get)
来源：http://wap.fanxiaobao.xyz/Article/details/gdwvqmlkb.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gizzfwhqz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fanxiaobao.xyz/Article/details/gwadcmjrx.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gnzoreuzj.sHtML

(x * 2 for x in arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gqcwqdtgt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/godghtewt.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gizlvlasw.sHtML

[U13] Py：固定长度队列
来源：http://blog.fanxiaobao.xyz/Article/details/grklweezr.sHtML

deque(maxlen=10)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyhahmvi.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govnugydo.sHtML

defaultdict(list)
来源：http://3g.fanxiaobao.xyz/Article/details/glywkypyt.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzgfwqev.sHtML

t = time.perf_counter()
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgtayscw.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyveemgd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvvrwzqr.sHtML

[U17] Py：初始化日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gacitrcmj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fanxiaobao.xyz/Article/details/gmktnnzup.sHtML

[U18] Py：预编译正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gcoiyczio.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfwutywu.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/gicikjhpa.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/gxdxqmhol.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fanxiaobao.xyz/Article/details/gczpmsecx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fanxiaobao.xyz/Article/details/gykppcbri.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fanxiaobao.xyz/Article/details/gspgrwice.sHtML

@contextlib.contextmanager
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhlkhgfd.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfqjghct.sHtML

list(zip(*m))
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuxhxhtr.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrkfltnq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fanxiaobao.xyz/Article/details/gizvhvkcv.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacndsjwj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmfuyjrz.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fanxiaobao.xyz/Article/details/gfydtwfqr.sHtML

csv.DictReader(f)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtoxvmitl.sHtML

[U26] Py：并发下载
来源：http://blog.fanxiaobao.xyz/Article/details/gmohgdlia.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugiixjrc.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fanxiaobao.xyz/Article/details/gswnnvtan.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fanxiaobao.xyz/Article/details/gmclhjwqc.sHtML

[U28] Py：类型别名
来源：http://3g.fanxiaobao.xyz/Article/details/gqsdnnoyk.sHtML

UserId = int
来源：http://wap.fanxiaobao.xyz/Article/details/gwpndrlcd.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpoqvnkmo.sHtML

@property 与 @x.setter 配合
来源：http://wap.fanxiaobao.xyz/Article/details/gjvovhtda.sHtML

[U30] Py：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gleyidoww.sHtML

@dataclass(slots=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbuicrkz.sHtML

[U31] Py：单测
来源：http://wap.fanxiaobao.xyz/Article/details/gvbmcevix.sHtML

python -m pytest -q
来源：http://3g.fanxiaobao.xyz/Article/details/gebjjpyaf.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitfxnbev.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fanxiaobao.xyz/Article/details/gemxczifl.sHtML

[U33] Py：打包发布
来源：http://3g.fanxiaobao.xyz/Article/details/gdylztwla.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fanxiaobao.xyz/Article/details/gfodxkamm.sHtML

[U34] Py：判断编码
来源：http://blog.fanxiaobao.xyz/Article/details/gyglnjhgg.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/gukobtvku.sHtML

[U35] Py：发送邮件
来源：http://3g.fanxiaobao.xyz/Article/details/gydcxzreq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fanxiaobao.xyz/Article/details/gffttqvir.sHtML

[U36] Py：定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gymsmdsqc.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fanxiaobao.xyz/Article/details/gyjegkikm.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gnegemqnp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fanxiaobao.xyz/Article/details/gncnycyqf.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyylyhklt.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbhacqwy.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fanxiaobao.xyz/Article/details/ghpgxxnqx.sHtML

sys.stdout.isatty()
来源：http://www.share.fanxiaobao.xyz/Article/details/gknrptdwk.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqvxcigg.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gniwqgxtw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gfuwodyae.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fanxiaobao.xyz/Article/details/guwcrwjsc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjsynxfo.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fanxiaobao.xyz/Article/details/gxiirksrl.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvadfjha.sHtML

namespace App\Http;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwthjtvna.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcofbudh.sHtML

declare(strict_types=1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqwlypuu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpsqifdx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgszovzz.sHtML

[U46] PHP：可空类型
来源：http://3g.fanxiaobao.xyz/Article/details/goolypwhl.sHtML

?string $name = null
来源：http://read.share.fanxiaobao.xyz/Article/details/gmndflblk.sHtML


<!-- 参考信息 -->