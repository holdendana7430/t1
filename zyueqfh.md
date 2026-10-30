代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gttxxlaoa.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/glehekrid.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gpozgtejk.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/gjnylpxzs.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/ggfsuqveo.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/guqjdiowd.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/gukhwhyem.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/gdajkkkks.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gdxcunxle.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/gfyafzkls.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gphjhjknk.sHtML

[S28] C：静态变量
来源：http://wap.hesvh.cn/Article/details/gcupmdsts.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gwhltgpsz.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gmuzepfoe.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fehbvm.com/Article/details/gpiqvvvun.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gjnshvrfu.sHtML

#ifndef X_H
来源：http://blog.hesvh.cn/Article/details/gbcswdngy.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gwjlazztw.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gfxvlimps.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gtigueskf.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/gsglrvtrv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.hesvh.cn/Article/details/gsdgwpopj.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gfzwapbws.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/gqfvkkezt.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/gqyyphvuc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/gikmrjxvj.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gifoxrkgh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gsmsaqjcl.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gbsbhaihd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gusqdcaeh.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/gpejqknzr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/grutzywwj.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gcoogfhry.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/gybqerifs.sHtML

[S38] C++：排序
来源：http://read.share.hesvh.cn/Article/details/gbmzewfts.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/ggclzkfqe.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gvwnjpmfx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gaesowpnq.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gspljnjpj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/gpezakfrz.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/ghfzxldwm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/gizthdtvk.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gmmdfcclh.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fehbvm.com/Article/details/glshvxynu.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gmwoggobg.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/gdwltcrnr.sHtML

[S44] C++：引用传参
来源：http://wap.fehbvm.com/Article/details/gobchlucy.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/gywyjyybd.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/groawdbpt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/gvdexekie.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gvjtmreke.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/gmhnlkhxw.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/grmoezmgw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/gfiyawypq.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/glinmoniw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/guaimjmel.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gaokjrhvr.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gsabaverh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/ghgneshqs.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gnnjuqucc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.hesvh.cn/Article/details/gxihiwujv.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/geuwwyjbz.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gavggikkb.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/grsofhkjn.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gknxncohf.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/gihkmjide.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/grxklkokh.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/glyqyczva.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/gqheakpbk.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/gptkjzfhg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/gjvixkwuf.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gdquqfmkd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/gxjuxgkoy.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/glyejbjtr.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/gfevggaqs.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gyzskacaf.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.hesvh.cn/Article/details/gkcmjjvao.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/grtgyikil.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/geheexnmb.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/gxpyrxygr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gxlbawvxr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grvdnrakm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gkylgvqmc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdiucxxex.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/gullzzspg.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gdjynwgyh.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/gncpazqeh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/ggpykqigf.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/grifljtxi.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gnyuakvcf.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/gbqhpmqbi.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gucqnbvel.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/growwovgt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gtbjcmkbn.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gvkusmfpl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/gcbrthhse.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gvrfckjqf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/gjphrdjyx.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/glnqzgwbw.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/geqsnobtb.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/gosoknuqt.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gcnxttqny.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/glxrzcnkf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/gmcufzgzv.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/gxgqywfnj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/gamrgbqrp.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/gnktccidq.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gksatviix.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gsixiblwk.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gzfmwdxox.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gyerskdta.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gylmidwuc.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/ghfzhjcuz.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/glbozvqpb.sHtML

[T16] Swift：Hello World
来源：http://mobile.hesvh.cn/Article/details/gpuurdqec.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gevudvtym.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/gwxdzrshz.sHtML

var a = 1;  let b = 2
来源：http://read.share.hesvh.cn/Article/details/gdukgwpnn.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gvxnahqfc.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/goopzccng.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/gyhqpwgjv.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/godnalezm.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/gilpnauux.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.zdbjq.cn/Article/details/gtbahepez.sHtML

[T21] Swift：遍历
来源：http://wap.fehbvm.com/Article/details/gnsfffibb.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/ggqfholrm.sHtML

[T22] Swift：字典
来源：http://baike.fehbvm.com/Article/details/gzvfiqpkm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gvpzgnwjb.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gyfmxgmyh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/goscqemkc.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/gmfevtepj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/gjwdmbdvt.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/govddfslg.sHtML

struct P { var x: Int }
来源：http://www.m.share.zdbjq.cn/Article/details/grxujvker.sHtML

[T26] Swift：类与重写
来源：http://www.blog.zdbjq.cn/Article/details/gmkfsphru.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/gtpallqwx.sHtML

[T27] Swift：错误处理
来源：http://blog.fehbvm.com/Article/details/gpuyqsuyj.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/gichmymxy.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gnmnhbcyh.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/gqaduvqvz.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/gqaeewtbg.sHtML

guard let x = opt else { return }
来源：http://mobile.hesvh.cn/Article/details/gjbigworu.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/givvitmhe.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/gzllrhvrf.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gcefoteqg.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gqymedigm.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gdgijrlra.sHtML

local a = 1
来源：http://read.share.hesvh.cn/Article/details/gjvtxcrdd.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.hesvh.cn/Article/details/gzufonhcq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/gutrwahcl.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/gwnymrihq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.hesvh.cn/Article/details/gdfbbkokn.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/gjieskedz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/gkngkansa.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/gqyhgxcdk.sHtML

function add(a, b) return a + b end
来源：http://baike.fehbvm.com/Article/details/gtibtopzc.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fehbvm.com/Article/details/gzsigpwye.sHtML

"a" .. "b"
来源：http://read.share.zdbjq.cn/Article/details/guwvyuqiv.sHtML

[T38] Lua：条件
来源：http://m.share.hesvh.cn/Article/details/gtywnhkul.sHtML

if x > 0 then print("正") end
来源：http://m.share.fehbvm.com/Article/details/gnifqgdzq.sHtML

[T39] Lua：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gmktxulai.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/gfuavpzdc.sHtML

[T40] Lua：元表
来源：http://3g.hesvh.cn/Article/details/gnywufmbd.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fehbvm.com/Article/details/gptkyasuo.sHtML

[T41] Perl：Hello World
来源：http://blog.fehbvm.com/Article/details/gqhazqupw.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/godmxnkzz.sHtML

[T42] Perl：变量类型
来源：http://wap.fehbvm.com/Article/details/ghoatxbae.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/gzhlovfdl.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fehbvm.com/Article/details/guxuhegnk.sHtML

"值: $a"
来源：http://read.share.fehbvm.com/Article/details/gxyjkxznu.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/gbphdjlla.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/gyzeazxiy.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/greextuez.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gdlgyfcro.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fehbvm.com/Article/details/gnlmggysc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gkxygimnv.sHtML

[T47] Perl：正则捕获
来源：http://mobile.hesvh.cn/Article/details/gucmmxtwi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/gkbgvhsiv.sHtML

[T48] Perl：正则替换
来源：http://3g.hesvh.cn/Article/details/gygbtlnbv.sHtML

$s =~ s/old/new/g;
来源：http://blog.fehbvm.com/Article/details/gusloyjrp.sHtML

[T49] Perl：函数
来源：http://www.m.share.fehbvm.com/Article/details/ghbimrizr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/ggxpbktpm.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gtvaxgclg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/gtxeoigzz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fehbvm.com/Article/details/gxlqqmzvk.sHtML

[T51] Scala：Hello World
来源：http://baike.hesvh.cn/Article/details/gwtbxewqh.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gqivbczft.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gyqojlgfs.sHtML

val a = 1;  var b = 2
来源：http://www.share.fehbvm.com/Article/details/gvdnakkwl.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/ghtktssbq.sHtML

s"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gqtkujngu.sHtML

[T54] Scala：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gquxkszcw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fehbvm.com/Article/details/gaeietluf.sHtML

[T55] Scala：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gplcdwict.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.hesvh.cn/Article/details/gkjtaglrj.sHtML

[T56] Scala：样例类
来源：http://read.share.zdbjq.cn/Article/details/gknfcoyah.sHtML

case class User(name: String, age: Int)
来源：http://3g.zdbjq.cn/Article/details/gdooqnacv.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gotnbnhmu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.hesvh.cn/Article/details/gkveyvrpx.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/gxcrxociq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/ggefoixbp.sHtML

[T59] Scala：循环
来源：http://read.share.hesvh.cn/Article/details/gmcagsrhl.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gzpjfsgyd.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/gdwimsmzu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.zdbjq.cn/Article/details/gtmzwjucj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/glgsjpcwm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gxnbsksuy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ginosiamv.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gshrcgxhs.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/gtucbnbvs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.zdbjq.cn/Article/details/gbgatwtxy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/gexmoptgq.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/gjybiljla.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/gnvryyxna.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.hesvh.cn/Article/details/gxlqjxqep.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fehbvm.com/Article/details/gikacvjyw.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gvkuhxfyo.sHtML

list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/giojoqofr.sHtML

[U06] Py：合并两个字典
来源：http://www.share.hesvh.cn/Article/details/guqaqblzj.sHtML

{**a, **b}
来源：http://3g.zdbjq.cn/Article/details/gkzdrngwm.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/gezgelxnh.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/gwwepovbd.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fehbvm.com/Article/details/gfrzbowpv.sHtML

[y for x in nested for y in x]
来源：http://3g.hesvh.cn/Article/details/gnfwbntuc.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.zdbjq.cn/Article/details/gjdoobrtt.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/gqjrcxanq.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.hesvh.cn/Article/details/genleodaa.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.zdbjq.cn/Article/details/gwvyhmzcd.sHtML

[U11] Py：生成器表达式
来源：http://read.share.zdbjq.cn/Article/details/gkvvkdjnq.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gqjaqnvsd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/ggaygteig.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/ghxhfxbdo.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fehbvm.com/Article/details/gqefpapnp.sHtML

deque(maxlen=10)
来源：http://blog.zdbjq.cn/Article/details/gujxwlkji.sHtML

[U14] Py：分组收集到列表
来源：http://baike.hesvh.cn/Article/details/gcqeaclnq.sHtML

defaultdict(list)
来源：http://wap.zdbjq.cn/Article/details/gmmmiwgve.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/giusdgjdk.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/gzlqcbihh.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/gfiqmkeqd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.hesvh.cn/Article/details/gstukgvby.sHtML

[U17] Py：初始化日志
来源：http://m.share.fehbvm.com/Article/details/gakrvscbi.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.zdbjq.cn/Article/details/gxgkrjhxg.sHtML

[U18] Py：预编译正则
来源：http://3g.fehbvm.com/Article/details/ginrqmrwl.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/ghfyhlubt.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fehbvm.com/Article/details/glmulmvqv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.zdbjq.cn/Article/details/goyzdmtec.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/gtjnyeqde.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fehbvm.com/Article/details/giuikjehf.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.hesvh.cn/Article/details/gyihupjcd.sHtML

@contextlib.contextmanager
来源：http://www.m.share.hesvh.cn/Article/details/gcjobgwgz.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fehbvm.com/Article/details/gttygodnw.sHtML

list(zip(*m))
来源：http://www.share.hesvh.cn/Article/details/gaqynntrv.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/gclcdzvrj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fehbvm.com/Article/details/gkfljlghu.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/gkdbndtim.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gncokzfif.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.hesvh.cn/Article/details/gwrjoybtw.sHtML

csv.DictReader(f)
来源：http://www.m.share.fehbvm.com/Article/details/gcgzpmrwm.sHtML

[U26] Py：并发下载
来源：http://read.share.fehbvm.com/Article/details/gyvzdrumi.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.hesvh.cn/Article/details/gzuibcfhp.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fehbvm.com/Article/details/gkvksmjab.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.zdbjq.cn/Article/details/gtnuabnmb.sHtML

[U28] Py：类型别名
来源：http://baike.hesvh.cn/Article/details/gvldrtbpx.sHtML

UserId = int
来源：http://read.share.fehbvm.com/Article/details/gcikaanjx.sHtML

[U29] Py：属性校验
来源：http://www.blog.zdbjq.cn/Article/details/gcnprhqsw.sHtML

@property 与 @x.setter 配合
来源：http://m.share.zdbjq.cn/Article/details/gbxaedehw.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/geafpowdv.sHtML

@dataclass(slots=True)
来源：http://blog.fehbvm.com/Article/details/gcfqhijpe.sHtML

[U31] Py：单测
来源：http://wap.fehbvm.com/Article/details/gsmxpqjir.sHtML

python -m pytest -q
来源：http://baike.zdbjq.cn/Article/details/gwwscjjdf.sHtML

[U32] Py：代码格式化
来源：http://www.blog.zdbjq.cn/Article/details/gnqlpkxsq.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fehbvm.com/Article/details/gpqlsmlbq.sHtML

[U33] Py：打包发布
来源：http://blog.zdbjq.cn/Article/details/gmubamhlw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.hesvh.cn/Article/details/gpshbgdgd.sHtML

[U34] Py：判断编码
来源：http://wap.hesvh.cn/Article/details/gebtvkddx.sHtML

chardet.detect(raw)
来源：http://www.share.fehbvm.com/Article/details/gklzzabve.sHtML

[U35] Py：发送邮件
来源：http://baike.fehbvm.com/Article/details/gwfgobywi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.hesvh.cn/Article/details/gacwzyfqx.sHtML

[U36] Py：定时任务
来源：http://read.share.zdbjq.cn/Article/details/gboktoefw.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.hesvh.cn/Article/details/gynrlvdwu.sHtML

[U37] Py：读写 Excel
来源：http://blog.hesvh.cn/Article/details/gtvnblzhn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fehbvm.com/Article/details/gxvayvocc.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fehbvm.com/Article/details/gtbdldbwh.sHtML

Path(__file__).resolve().parent
来源：http://baike.fehbvm.com/Article/details/gadnnobaq.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.hesvh.cn/Article/details/gmvbgqwlv.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/gujwomoyo.sHtML

[U40] Py：打印到标准错误
来源：http://blog.zdbjq.cn/Article/details/gemrgnbmd.sHtML

print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/giewqlabd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fehbvm.com/Article/details/gtwjivnhh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/gauzvwfuh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fehbvm.com/Article/details/gvpmqezsc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/grdnipdsm.sHtML

[U43] PHP：声明命名空间
来源：http://3g.hesvh.cn/Article/details/gpyhpcvgy.sHtML

namespace App\Http;
来源：http://mobile.fehbvm.com/Article/details/gkhwecfta.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fehbvm.com/Article/details/goeccxlcj.sHtML

declare(strict_types=1);
来源：http://blog.fehbvm.com/Article/details/grxkrmzgz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.zdbjq.cn/Article/details/gpqcqjyqf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gncoaxbbl.sHtML

[U46] PHP：可空类型
来源：http://m.share.fehbvm.com/Article/details/glccwsvuc.sHtML

?string $name = null
来源：http://www.m.share.fehbvm.com/Article/details/gpqxegpiy.sHtML


<!-- 参考信息 -->