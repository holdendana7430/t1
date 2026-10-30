代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/geysmysfv.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlypvgaa.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gucalngqk.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gcmmbascu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfekhynug.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdwwypoh.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/ggsualghs.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gdnixztnm.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/glamgsxbc.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gerxyiwvl.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/goikaxzty.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gpezcpoxg.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfeefwulv.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gfgwqiaar.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gboliagjg.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjhukjdr.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gcbepzche.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gptfvrdjh.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gagjvcncv.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gfgcltnqv.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gktqjzcos.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggkomiblc.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyyujehm.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gjjoiwdhq.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gceadtguy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/ggfqcnbcn.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/guyrczxpg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmsrmuwy.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gloteyhyq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrnmddpd.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gxdfmhlot.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gifbkmrtq.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gguiaokiv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/goensmmer.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/ggbsxgajw.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvoqjcpe.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gyxnnussc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyezbwtg.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gfcttlfdl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gogstvjjl.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/grsaaakvv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/getynlmqk.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/glweqggyq.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccfxvxrb.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/ggrrxubdd.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/ghzoyzibm.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gbfuxfetg.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzyrxialk.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gsmjgcylg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyxgutuu.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhucfpxd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadxdqqce.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowabodor.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gesywhljp.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gqtdvglzh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawkzgxzt.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnayvydfy.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gyoswupdg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhhikvrj.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gqcchgcho.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guuxcvgjn.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gelkmuhss.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gvroqheen.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsndpqtn.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvwrbyfdc.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/ggoiagfjh.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcizcyzsy.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gweulibsh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gtkyormdd.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwchbbjx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpotixye.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gslzytksa.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gihxlqkvw.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpubyygw.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogxemmeq.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gjvuqcayx.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdduoxlat.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gjmoijolo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqiliczf.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/guobjzutt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gknofgkzo.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvyuqxvw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpuazbsn.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gfhlelnlq.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvngaysg.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcceuzdt.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gvxqoimfr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/grwrnmdum.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gdewztmeb.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gapgjlvfn.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/gxsogpxmp.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gqilnoyyh.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gtfdjcgaw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqgdxnri.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfkzpmhs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyirwavgl.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbblyuint.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/ggwlymgmt.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnypxlqmf.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkszpjbvc.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzeaudua.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkngtnkm.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/giindmnmc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbecqqrig.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gfdlvkdei.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbnftolx.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaepscfsf.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqaptqspf.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/ghblhezux.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjbmksmp.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gawrwrnke.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/glflqngaz.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gsygwnjrd.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gjqoiaser.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gugrvluyc.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnglfiphp.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gfkdeknfx.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlevceou.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gtopoklcu.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/gkapusheq.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gxkwlhrpi.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdkqrmdy.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gstowxkmx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwujqazfb.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gmeearvgh.sHtML

for x in a { print(x) }
来源：http://blog.fanxiaobao.xyz/Article/details/gperkwzyj.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/ghmaashlm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxacoexuu.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gyhkzpstm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpsoadsk.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/grrgfvtmr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwizgpwh.sHtML

[T25] Swift：结构体
来源：http://3g.fanxiaobao.xyz/Article/details/gqrlqipqx.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpqbvxpq.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwltltrwi.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gszgzggqx.sHtML

[T27] Swift：错误处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gscqygaah.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjavpsxg.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gfzszytho.sHtML

enum Color { case red, green }
来源：http://mobile.fanxiaobao.xyz/Article/details/grdacdium.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godyjrrgh.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwqzfngs.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcptnqxp.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gydflplay.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/grhqlfylo.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghodzrvtm.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvltwsif.sHtML

local a = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmkkwnpu.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjierruwd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvmeiilq.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/gitgmbrak.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmorqcjxq.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/gsnmwoykc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcyifohw.sHtML

[T36] Lua：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/giwbsgwrk.sHtML

function add(a, b) return a + b end
来源：http://mobile.fanxiaobao.xyz/Article/details/grxjikgcn.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gfoytiorg.sHtML

"a" .. "b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhfjzevm.sHtML

[T38] Lua：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpsuoknd.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcfaxtgv.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqjypcpm.sHtML

string.find(s, "%d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzunfuui.sHtML

[T40] Lua：元表
来源：http://mobile.fanxiaobao.xyz/Article/details/guxcqstke.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgeummsu.sHtML

[T41] Perl：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwpebrqg.sHtML

print "Hello\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqigglet.sHtML

[T42] Perl：变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuqvcwbl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/glrnzearg.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxbrccxa.sHtML

"值: $a"
来源：http://baike.fanxiaobao.xyz/Article/details/gibjluevr.sHtML

[T44] Perl：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmbgsgoy.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhzvrkiz.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/grkvftoyq.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gazrnapoa.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/gmcivsyck.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grldrqmaw.sHtML

[T47] Perl：正则捕获
来源：http://3g.fanxiaobao.xyz/Article/details/gmrlnocue.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytfdjrvf.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhrqubkw.sHtML

$s =~ s/old/new/g;
来源：http://wap.fanxiaobao.xyz/Article/details/gfzogsbnp.sHtML

[T49] Perl：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjnpvbhg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxdvlebg.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkwpruhm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsgjaxon.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbiieodba.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvipnpiw.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwztzkkek.sHtML

[T52] Scala：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gxsezthxm.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gdrngxmhy.sHtML

[T53] Scala：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gpjdqahzf.sHtML

s"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gaxxjpssr.sHtML

[T54] Scala：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gylqlnbby.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gipxgenpn.sHtML

[T55] Scala：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gqucrbhmh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gjgkoghpj.sHtML

[T56] Scala：样例类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnjegdzn.sHtML

case class User(name: String, age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gfbewpudi.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfvnpouw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/gjbgkmzwo.sHtML

[T58] Scala：函数定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdnftehg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fanxiaobao.xyz/Article/details/gvmxkfeyl.sHtML

[T59] Scala：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkgehbqm.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gvpwtbmht.sHtML

[T60] Scala：折叠
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjhifxzx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxhwdjni.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gqnsbfmlr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gadjrrylm.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ggizwgjqp.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fanxiaobao.xyz/Article/details/gjkfpddmo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fanxiaobao.xyz/Article/details/gaektejhm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjustryz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gnjlwgnvx.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrxzqife.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fanxiaobao.xyz/Article/details/gahisprvt.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobzqsbld.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjctwjdnv.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/gxpzmrelu.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gthxqdmno.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fanxiaobao.xyz/Article/details/geomgghue.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkpqusgn.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlayehpw.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fanxiaobao.xyz/Article/details/gtagtmcfw.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/gdgqmckhe.sHtML

[y for x in nested for y in x]
来源：http://3g.fanxiaobao.xyz/Article/details/gifvutlor.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fanxiaobao.xyz/Article/details/gnqhykwnm.sHtML

max(d, key=d.get)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxowgifa.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gkesavfok.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fanxiaobao.xyz/Article/details/gmwkmfeyx.sHtML

[U11] Py：生成器表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gdavymgfl.sHtML

(x * 2 for x in arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/glkbyezsw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogcohadt.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gbuzbhnct.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrigsugb.sHtML

deque(maxlen=10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprggclad.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fanxiaobao.xyz/Article/details/grqfgvllb.sHtML

defaultdict(list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtngenyzv.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/gpvjsjytb.sHtML

t = time.perf_counter()
来源：http://baike.fanxiaobao.xyz/Article/details/guelxcdux.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/gtwpbajtv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/gnceqlotw.sHtML

[U17] Py：初始化日志
来源：http://3g.fanxiaobao.xyz/Article/details/gajsdjejs.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fanxiaobao.xyz/Article/details/gfnxuzsew.sHtML

[U18] Py：预编译正则
来源：http://wap.fanxiaobao.xyz/Article/details/ggknxcesi.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gxxhkhqls.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fanxiaobao.xyz/Article/details/guemvgubw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjesfryb.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fanxiaobao.xyz/Article/details/gwfcyrzfl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/gydiutbxr.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fanxiaobao.xyz/Article/details/ggbbdwewx.sHtML

@contextlib.contextmanager
来源：http://3g.fanxiaobao.xyz/Article/details/ggfdkkbfj.sHtML

[U22] Py：矩阵转置
来源：http://wap.fanxiaobao.xyz/Article/details/gjtpfzzkm.sHtML

list(zip(*m))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylxlfvdp.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgtcgora.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fanxiaobao.xyz/Article/details/gwmwmyzjg.sHtML

[U24] Py：路径操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyihygsf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfccvfnqo.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fanxiaobao.xyz/Article/details/gbmbkcdbw.sHtML

csv.DictReader(f)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqgwunbv.sHtML

[U26] Py：并发下载
来源：http://baike.fanxiaobao.xyz/Article/details/gbgsfbkxd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fanxiaobao.xyz/Article/details/ggisnrmcj.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fanxiaobao.xyz/Article/details/gygcbanwb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fanxiaobao.xyz/Article/details/gamesdstw.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhpwyxvy.sHtML

UserId = int
来源：http://www.blog.fanxiaobao.xyz/Article/details/guaxybtfg.sHtML

[U29] Py：属性校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gewaotgxf.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/guwdtyyqb.sHtML

[U30] Py：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gpnvrmopt.sHtML

@dataclass(slots=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/glxbtmgxr.sHtML

[U31] Py：单测
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhersmdu.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/ghajjwcij.sHtML

[U32] Py：代码格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/ggalpwwig.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fanxiaobao.xyz/Article/details/gaoestrur.sHtML

[U33] Py：打包发布
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbcahcng.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fanxiaobao.xyz/Article/details/gzahzlorz.sHtML

[U34] Py：判断编码
来源：http://wap.fanxiaobao.xyz/Article/details/ghxwsxziz.sHtML

chardet.detect(raw)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkczdxbq.sHtML

[U35] Py：发送邮件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtumtkjbp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzhpfsfd.sHtML

[U36] Py：定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gacsqchmp.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggodydspl.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcremsvyf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fanxiaobao.xyz/Article/details/gtyqfndso.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fanxiaobao.xyz/Article/details/ggrafboox.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfwvhuhb.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fanxiaobao.xyz/Article/details/glvqgzpby.sHtML

sys.stdout.isatty()
来源：http://3g.fanxiaobao.xyz/Article/details/gdkpdbtyq.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxqjbkhg.sHtML

print("err", file=sys.stderr)
来源：http://3g.fanxiaobao.xyz/Article/details/gyelgqhcs.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxlallvv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fanxiaobao.xyz/Article/details/gloiacddx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwbehvud.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fanxiaobao.xyz/Article/details/gjswgdppa.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gbbcpmbxb.sHtML

namespace App\Http;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrxdforq.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gnetlqboh.sHtML

declare(strict_types=1);
来源：http://3g.fanxiaobao.xyz/Article/details/gjdajgqyc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbxacxvc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giyxawcra.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftmbxxzm.sHtML

?string $name = null
来源：http://3g.fanxiaobao.xyz/Article/details/gndytbljk.sHtML


<!-- 参考信息 -->