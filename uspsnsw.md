代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gaxypzdzv.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gieyylaps.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gasvvzbti.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gxeqqcqio.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gastacccn.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/ghkhjnzsf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmfzepcn.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gbdgxmltd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gpzqnybhu.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gdodchdub.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gzjixamjh.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gxziuojlb.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqcorbhg.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgjtcoyx.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdosnmdqm.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gckacdyrc.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqptylcp.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/ggtegtack.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpyodiwe.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gcbyfzsoy.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzysvdpb.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/goosqzwmc.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvllsufs.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsaacdno.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwxpeetf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gratoyfne.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gyrtcpsaz.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gofioaugy.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdpwtypx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giulxuvie.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gijtpehlq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grmkyackz.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gpgrwfdin.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdpfsuny.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbtkgbjk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gbctsnslo.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gjljfnzmf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnufuzpha.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gvodkopmw.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gsvudwgrr.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedfizkse.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpcbqjua.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gfvdbztnl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gczsfnhat.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldqtbrhl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzrzezog.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqmdsuxp.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gfptfuhgy.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giafuvjqy.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gneycymiy.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutdlvdwp.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkifmrpyq.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gtklzqqjm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gusbneslo.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gmeavzxub.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtxsypfx.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavjsqvdt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gayibisem.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gxtkqdbvf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbcsfkac.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhnbggtl.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubmwkjns.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghebxyvmp.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcimczgtf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gzojnspni.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/ghffpsmvv.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gtjjuguxc.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goynvzjcy.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcewlykm.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznljzvnm.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/ggvvnqfty.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqcmnsme.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzsqrrfc.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/glmpjznky.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gwlblkvnv.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/grcawhtzv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtjwyuhos.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdbimzas.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfwlrokp.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gfkprmviz.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gvlgtkmpv.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/godkthaiq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gsegtwfpf.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gxrckcrme.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhuldybn.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrjfukjl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/glkmwnsyc.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gszwnnqet.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgnvbmjn.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvoewlikp.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gketsekhv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gmuvaxkjf.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/glghbcsed.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjqmkhoa.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/giunyzyrn.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gbibkpfdg.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhniltpk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdxenqxf.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqiefrdm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gibljqbga.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/grzdpabpd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gauzzolww.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gapmejqir.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gozsvvaij.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwpcauzv.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/gutzhfmqo.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gtgxuqnxd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvagiaye.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypzmjuje.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/giwgugzfm.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsbqcjjl.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gzvudskdm.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/glofntqml.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcplvwxyx.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/guchtmvkt.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhdllces.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/gcwecmgjq.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gynszwfzn.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecgdfcqs.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/ghvvkvwde.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/grhghepeh.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gtbllyulq.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gicfgwozh.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/gipdelxhy.sHtML

[T19] Swift：可选绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gisiqpyex.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfnqxsiq.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gghowdbda.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fanxiaobao.xyz/Article/details/gxndectmi.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gcjzlmsuz.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/gyjxzcoym.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gggnkzsjl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/ggffrfyav.sHtML

[T23] Swift：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnvmpvvx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyauldhx.sHtML

[T24] Swift：闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/glqwknbki.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnbfawpj.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/gaendnark.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/gpxwhuyda.sHtML

[T26] Swift：类与重写
来源：http://blog.fanxiaobao.xyz/Article/details/girocbpjd.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvdkxceb.sHtML

[T27] Swift：错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/gvbaivyjp.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/gxkyfugsu.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gcnqfndva.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/gjizfxxjh.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqkquldf.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvudsyfsq.sHtML

[T30] Swift：协议
来源：http://wap.fanxiaobao.xyz/Article/details/gtphxusvt.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlofydsq.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgjvppqt.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gjhkaedam.sHtML

[T32] Lua：局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgqxwljo.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gvrmnxwhm.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefvfakeq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwhzfbks.sHtML

[T34] Lua：遍历表
来源：http://wap.fanxiaobao.xyz/Article/details/gcjzrubga.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/gcmzruzgw.sHtML

[T35] Lua：字典表
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhqknvmd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gfayuarew.sHtML

[T36] Lua：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gktafatfs.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdamjjupd.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glliuosfz.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/gatdpmqrw.sHtML

[T38] Lua：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpxsmxsj.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/gbuzgnvak.sHtML

[T39] Lua：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/glnezlcxl.sHtML

string.find(s, "%d+")
来源：http://wap.fanxiaobao.xyz/Article/details/ggbfbmeqn.sHtML

[T40] Lua：元表
来源：http://blog.fanxiaobao.xyz/Article/details/gbnfwoavt.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/gdknsdzpt.sHtML

[T41] Perl：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gzccskulu.sHtML

print "Hello\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gylwrwdgl.sHtML

[T42] Perl：变量类型
来源：http://wap.fanxiaobao.xyz/Article/details/geyrvxhff.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gmumxdait.sHtML

[T43] Perl：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/glahnnqqe.sHtML

"值: $a"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrsxfcsm.sHtML

[T44] Perl：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gvjvmpbsg.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grmiszlhu.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnhsduyx.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvtvfzga.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdcaughr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/govcbusib.sHtML

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/gdoukxzcr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnujomuko.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gynpnlkbl.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxbokeme.sHtML

[T49] Perl：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/ggabcsqkl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gngluopmb.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gjvugnvin.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwsnfylq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtobvhwwb.sHtML

[T51] Scala：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gzexhqnzo.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzzmfbui.sHtML

[T52] Scala：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gjvnaqxwt.sHtML

val a = 1;  var b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqyvkeby.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrnpburs.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmsxgenh.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gwczxipfi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gssdsjhhz.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxtirnht.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/grpuqcbsh.sHtML

[T56] Scala：样例类
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnduxjei.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gczjgoskx.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixgrudyp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqivwykq.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpausidd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gpwcdayzo.sHtML

[T59] Scala：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswkxscas.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gnpkzscoe.sHtML

[T60] Scala：折叠
来源：http://blog.fanxiaobao.xyz/Article/details/gyctwezwi.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/gatgznwas.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/grgujyrlq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdpsaxlt.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gjvcyuulr.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqrmwkpt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fanxiaobao.xyz/Article/details/gsxxaipte.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fanxiaobao.xyz/Article/details/gqyvtfwvj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczmpbsge.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwvetemo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fanxiaobao.xyz/Article/details/genantfkm.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fanxiaobao.xyz/Article/details/gyddlagnp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fanxiaobao.xyz/Article/details/ghwwgjniz.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbaaidge.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmetxquht.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocupiitd.sHtML

{**a, **b}
来源：http://mobile.fanxiaobao.xyz/Article/details/gvujebhny.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtobsmpj.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnfiverm.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskindvib.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypeturtm.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fanxiaobao.xyz/Article/details/gonuurgjg.sHtML

max(d, key=d.get)
来源：http://3g.fanxiaobao.xyz/Article/details/gatvdhhgk.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbuqcdqb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsxzsmyj.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwdnrjur.sHtML

(x * 2 for x in arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbigxjynh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fanxiaobao.xyz/Article/details/goejesetc.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gdexahqcl.sHtML

[U13] Py：固定长度队列
来源：http://blog.fanxiaobao.xyz/Article/details/ghsfkytnt.sHtML

deque(maxlen=10)
来源：http://baike.fanxiaobao.xyz/Article/details/gcppiholj.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fanxiaobao.xyz/Article/details/gmgxnxvbu.sHtML

defaultdict(list)
来源：http://baike.fanxiaobao.xyz/Article/details/gxjyuxtij.sHtML

[U15] Py：高精度计时
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlzkpuqm.sHtML

t = time.perf_counter()
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjnlzanz.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fanxiaobao.xyz/Article/details/glkjvpzoh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhqqwcoz.sHtML

[U17] Py：初始化日志
来源：http://3g.fanxiaobao.xyz/Article/details/gikizfgdz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhfzgmrt.sHtML

[U18] Py：预编译正则
来源：http://3g.fanxiaobao.xyz/Article/details/gjeyxtowr.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/glrmweryr.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpukvqnek.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fanxiaobao.xyz/Article/details/grcvzhjxa.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fanxiaobao.xyz/Article/details/gzwtokfwe.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzsrncsa.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorhaglhn.sHtML

@contextlib.contextmanager
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjsguauh.sHtML

[U22] Py：矩阵转置
来源：http://baike.fanxiaobao.xyz/Article/details/gndbjlute.sHtML

list(zip(*m))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyjuhcnm.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gutpeulwq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fanxiaobao.xyz/Article/details/gropqsjvj.sHtML

[U24] Py：路径操作
来源：http://wap.fanxiaobao.xyz/Article/details/gkonhpced.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/glgsbeobr.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fanxiaobao.xyz/Article/details/gacrtftvs.sHtML

csv.DictReader(f)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzdmvsev.sHtML

[U26] Py：并发下载
来源：http://wap.fanxiaobao.xyz/Article/details/gkvdnvguv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlyuincs.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fanxiaobao.xyz/Article/details/glsoflbeo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fanxiaobao.xyz/Article/details/glnvraobc.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdwhoptv.sHtML

UserId = int
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfmxevxi.sHtML

[U29] Py：属性校验
来源：http://blog.fanxiaobao.xyz/Article/details/gpwikfyqd.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/gvdsrlwfd.sHtML

[U30] Py：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnudkhnln.sHtML

@dataclass(slots=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gltlcfncu.sHtML

[U31] Py：单测
来源：http://mobile.fanxiaobao.xyz/Article/details/gttczazwx.sHtML

python -m pytest -q
来源：http://www.share.fanxiaobao.xyz/Article/details/gagjpilhz.sHtML

[U32] Py：代码格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gpqfzinec.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fanxiaobao.xyz/Article/details/ghpffoxan.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxtniiim.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fanxiaobao.xyz/Article/details/gkeoahnyh.sHtML

[U34] Py：判断编码
来源：http://wap.fanxiaobao.xyz/Article/details/gzeskaolc.sHtML

chardet.detect(raw)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geapnjaxc.sHtML

[U35] Py：发送邮件
来源：http://baike.fanxiaobao.xyz/Article/details/ghcbmxhpi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grziegnjd.sHtML

[U36] Py：定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgjnqkwt.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fanxiaobao.xyz/Article/details/gurxkxpwa.sHtML

[U37] Py：读写 Excel
来源：http://wap.fanxiaobao.xyz/Article/details/gcbneimal.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fanxiaobao.xyz/Article/details/ghekuazbk.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fanxiaobao.xyz/Article/details/gwcekfvyd.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fanxiaobao.xyz/Article/details/goymaaxay.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fanxiaobao.xyz/Article/details/grnkszdkh.sHtML

sys.stdout.isatty()
来源：http://mobile.fanxiaobao.xyz/Article/details/gahgzewsv.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyggfezch.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtykkvova.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdxsokfd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjqwssgq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fanxiaobao.xyz/Article/details/glkbxxxcl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fanxiaobao.xyz/Article/details/gouuvkolm.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/giagtyinc.sHtML

namespace App\Http;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzmrywbk.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fanxiaobao.xyz/Article/details/gwtrzyzcx.sHtML

declare(strict_types=1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwgmovgc.sHtML


<!-- 参考信息 -->