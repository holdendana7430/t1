代发 wailian999

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gsoxtdvhr.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gxikyuncp.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gjjkrxedo.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwbjgbvp.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/ggmamcrwq.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghentrtuy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfrqygop.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gamseledl.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrstyowa.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmthrpqr.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gvdjrwcmv.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcffyxivi.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbonvdwp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gywvqzyvy.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfuqvhwq.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gfwixhhuy.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaaljklnf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnbsemtv.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gffsbsbir.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtaebnpzm.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnaxdiesf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grywkamhc.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gieyicvvo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gnxevuhjc.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gomkxyygz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqoblztnd.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/glzyrmjez.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzvpedvu.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsasongh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/getjrpntx.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gwenbnltt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gskfdujpu.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcbmcdxb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/grekgtmzc.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmjdfmcc.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gcckqulap.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxwahifh.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsbqjung.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gztzqzetk.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmmqvepk.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gjiuordzy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsybobyeu.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplbfkdkg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/goknbolsm.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gsbkrecej.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grmgaakug.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/giipobzyj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gxgrwpnya.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gzzykxjfe.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbybtebe.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gkflbiuyw.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfemhmsh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gackgwpgl.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/goprbskfs.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrscqdzm.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/gsoivhxxe.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjuzyjvfz.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnfsludw.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqourxjke.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gvparztur.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gccspofvs.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gdqdftgfq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdobphytj.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcqjarls.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpnrzvvt.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/grzqbqwes.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gikqlfasl.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/guofryffs.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqllnqlv.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcivgrjs.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbyezzcz.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/guwewvhre.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gpheseuej.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gsdjzwbtx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdegjmyfp.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gncufwfsl.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/geypivqgh.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmfnylgk.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzlzmmbf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrnumabq.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxjbdodn.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gykxnsxkv.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/grygozvzo.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/ggddhtkee.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gehjchufx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcvtsccf.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/grylrztcr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gufnxdsin.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekywvnbe.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjapqqvg.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/grijumhnp.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gwqeioobb.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/geqlpmhbm.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gegywkjhk.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/grdpeompp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/glhuqlhwl.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/glvvtzccc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/goiztyxjy.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdutwhfk.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyacguvvs.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpkbhpzo.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guputvtmn.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/geuziqkon.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/glvlsnstz.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gwhdeaiwn.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gbwhmvgfx.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbwqhucv.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdezyxxa.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/glkghxibj.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gtinesujz.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gogrofyjj.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/gfvwknuky.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gkminvtgh.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/gutmtkhiq.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gggsieviy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnxveoaj.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gedcdcjzk.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuaxtbhv.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gancibkuh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gjphtyjhq.sHtML

[T23] Swift：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwydkrpg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvfkfeaw.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gdqgmstzb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gvaettjhu.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcdtpcdf.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gyeywqvef.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/gokulrlff.sHtML

class A: Base { override func f() {} }
来源：http://blog.fanxiaobao.xyz/Article/details/ggrizdqfm.sHtML

[T27] Swift：错误处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gottzqykt.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqjobtlu.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmyzoanx.sHtML

enum Color { case red, green }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqxtsxjv.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/graoqevqi.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/goukdkydd.sHtML

[T30] Swift：协议
来源：http://baike.fanxiaobao.xyz/Article/details/gdykzefll.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzwesqzm.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gkhpzbvzs.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gbjxkrjpb.sHtML

[T32] Lua：局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gujpfngau.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsudrwtp.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fanxiaobao.xyz/Article/details/gubifrsev.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fanxiaobao.xyz/Article/details/gjhvrtilm.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/grltytfnq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fanxiaobao.xyz/Article/details/gjcpidmep.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/gtoszsxpg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnycfzhc.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gazkvazzo.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gdzpaziqh.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gsadmghfi.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/gbephzcaq.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gillqnpiz.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmqkyvyy.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gslapduyy.sHtML

string.find(s, "%d+")
来源：http://baike.fanxiaobao.xyz/Article/details/glgjqkivt.sHtML

[T40] Lua：元表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsakkzsqr.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fanxiaobao.xyz/Article/details/gnesdqpob.sHtML

[T41] Perl：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gciyrmkzk.sHtML

print "Hello\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gusnmghlh.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatoogkjw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/ggljpiiig.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtsueode.sHtML

"值: $a"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsoudqnmf.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/groebhxft.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyjcbevi.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gofomqbov.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gaizjbhcf.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxajsodod.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmrwbaqi.sHtML

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/gbdwmgpjo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghnorcczk.sHtML

[T48] Perl：正则替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gcursmlfj.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnitghnyb.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gggcsjzgn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfmmmavm.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvinsjhb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fanxiaobao.xyz/Article/details/gaziprhxa.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/geaxkzzna.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwvcqznu.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqmivulm.sHtML

[T52] Scala：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyufghxol.sHtML

val a = 1;  var b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gylcrloua.sHtML

[T53] Scala：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gtehrvovh.sHtML

s"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gavkbltem.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gyofxzecm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gipnkopmp.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowvokzak.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gpipjjeuy.sHtML

[T56] Scala：样例类
来源：http://www.share.fanxiaobao.xyz/Article/details/gsisivtfu.sHtML

case class User(name: String, age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gvyzanmzu.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gzevtbbfl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/gswpkzlec.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhldtaoi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/glgcbkqnu.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkrekfep.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giavbuaoy.sHtML

[T60] Scala：折叠
来源：http://baike.fanxiaobao.xyz/Article/details/gqdfnnknn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzpgmdfb.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gzlirnnbj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosutcxky.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpmdawea.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/grmipwbsx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fanxiaobao.xyz/Article/details/guasqoxen.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fanxiaobao.xyz/Article/details/glyhfextn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gusdkmmly.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gblohjbbd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fanxiaobao.xyz/Article/details/gddancjxw.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fanxiaobao.xyz/Article/details/gelhujjor.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gmptdaxxh.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fanxiaobao.xyz/Article/details/gdidewclz.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjbklyuw.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhpfbpdw.sHtML

{**a, **b}
来源：http://www.share.fanxiaobao.xyz/Article/details/gcptzspcd.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fanxiaobao.xyz/Article/details/griwyjiui.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqrgbica.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gfunmrrcx.sHtML

[y for x in nested for y in x]
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwvchpog.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fanxiaobao.xyz/Article/details/gpmewcqpx.sHtML

max(d, key=d.get)
来源：http://3g.fanxiaobao.xyz/Article/details/gwbtzafhm.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdcryady.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fanxiaobao.xyz/Article/details/gcentomat.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/ghaejfble.sHtML

(x * 2 for x in arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdcjfvuh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmtopxwf.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwawcnsrl.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhavzsft.sHtML

deque(maxlen=10)
来源：http://wap.fanxiaobao.xyz/Article/details/gtgeukdkl.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqqbjmiy.sHtML

defaultdict(list)
来源：http://baike.fanxiaobao.xyz/Article/details/geckczdaa.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkenikpts.sHtML

t = time.perf_counter()
来源：http://wap.fanxiaobao.xyz/Article/details/gqonapnkc.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fanxiaobao.xyz/Article/details/gazmfhiyx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fanxiaobao.xyz/Article/details/gqscfswbk.sHtML

[U17] Py：初始化日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrlgsdxa.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fanxiaobao.xyz/Article/details/grabtfzpw.sHtML

[U18] Py：预编译正则
来源：http://www.share.fanxiaobao.xyz/Article/details/grfknrgoz.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjyopvse.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxhfcllg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gktpfczci.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsyyztpj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fanxiaobao.xyz/Article/details/gzviqwcwh.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grihcecdw.sHtML

@contextlib.contextmanager
来源：http://www.share.fanxiaobao.xyz/Article/details/gpndrlqck.sHtML

[U22] Py：矩阵转置
来源：http://baike.fanxiaobao.xyz/Article/details/glsaygjya.sHtML

list(zip(*m))
来源：http://mobile.fanxiaobao.xyz/Article/details/ggilozvzq.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhiodxvj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxylyyko.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gorzzjabi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giimezyvn.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fanxiaobao.xyz/Article/details/gyosephdn.sHtML

csv.DictReader(f)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjthgguj.sHtML

[U26] Py：并发下载
来源：http://baike.fanxiaobao.xyz/Article/details/gzpcnlhas.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fanxiaobao.xyz/Article/details/gutvygezj.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fanxiaobao.xyz/Article/details/gjfttutlz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fanxiaobao.xyz/Article/details/gsoeasxqq.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyyfennw.sHtML

UserId = int
来源：http://baike.fanxiaobao.xyz/Article/details/ggiroypzh.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulkwdrpr.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlnjnvbi.sHtML

[U30] Py：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsazadxbx.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzsvojme.sHtML

[U31] Py：单测
来源：http://wap.fanxiaobao.xyz/Article/details/gpvlbxoeu.sHtML

python -m pytest -q
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrtkdsoh.sHtML

[U32] Py：代码格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gybwihpmz.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fanxiaobao.xyz/Article/details/gusaktbvh.sHtML

[U33] Py：打包发布
来源：http://baike.fanxiaobao.xyz/Article/details/gslipoteq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fanxiaobao.xyz/Article/details/gfritqcxk.sHtML

[U34] Py：判断编码
来源：http://blog.fanxiaobao.xyz/Article/details/gchqhybzz.sHtML

chardet.detect(raw)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqdzulcv.sHtML

[U35] Py：发送邮件
来源：http://m.share.fanxiaobao.xyz/Article/details/geinivlvh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxqnxfmn.sHtML

[U36] Py：定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/ggwmdpmac.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvixmhltd.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gvobmlbtp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fanxiaobao.xyz/Article/details/gynzdufdc.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowgkoidk.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/gavbddwjn.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fanxiaobao.xyz/Article/details/gdumgzwyi.sHtML

sys.stdout.isatty()
来源：http://blog.fanxiaobao.xyz/Article/details/gqcpzdfdc.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fanxiaobao.xyz/Article/details/gkzvjrdlv.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhtbnued.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gxihhklih.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzqxakem.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fanxiaobao.xyz/Article/details/gvujhjzdn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlsomeyh.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzuvkabd.sHtML

namespace App\Http;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwbiiryq.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxyjsprt.sHtML

declare(strict_types=1);
来源：http://wap.fanxiaobao.xyz/Article/details/gcttfyqeo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fanxiaobao.xyz/Article/details/ggkaedjjh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwvejrghm.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnrsqhjy.sHtML

?string $name = null
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicpvheyu.sHtML

[U47] PHP：联合类型
来源：http://3g.fanxiaobao.xyz/Article/details/gyesloyyp.sHtML

int|string $id
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjfeiave.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/goxxjvtzr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gprlfpofk.sHtML

[U49] PHP：只读属性
来源：http://baike.fanxiaobao.xyz/Article/details/gbslpfztn.sHtML

public readonly string $name
来源：http://www.share.fanxiaobao.xyz/Article/details/gffajrlvo.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwqgccvf.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdlofrob.sHtML


<!-- 参考信息 -->