代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gywpyskcw.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/gwjvlzgdy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gufmkickv.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gcusgemuc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gzajsiivy.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/gxaxwsqcu.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gvegcmrok.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gsxxidltc.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/gumufkbbs.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gqckpyedp.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gejnjmxxn.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gxmmprswt.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/grcvdktwj.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gpoziqncx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/gqasynfnp.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/gggaicwjp.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gvrliyeiv.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gbktpjcpm.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/ggrmvkgfj.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/ganuosbal.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/ghhtjbolg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/glocgozlg.sHtML

[S32] C++：字符串
来源：http://baike.hesvh.cn/Article/details/gjjfmcaqo.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gudepemtq.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/gvfmicynn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/gvwxaxrbi.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/gohgmpjmf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/gwmutkrso.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/ggjgjeiue.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gjmeazdkx.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/gxpvzcegq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gclmkqefi.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/gcmpkbenq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/gjavnrbhb.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gpxobgble.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gbqawhhwu.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/gfmrmruzb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/guokwhxkt.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/glvbdjgrn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gwrsoyabo.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gucoqgpti.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/gyudpqxvz.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.hesvh.cn/Article/details/gsznzpqob.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fehbvm.com/Article/details/gwqdiguwj.sHtML

[S43] C++：智能指针
来源：http://baike.zdbjq.cn/Article/details/gbkshddty.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/gmfwfnuja.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/gunkyelji.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/gytjekkyc.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gxiwuwgtv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/gtvojcvpr.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/geqkdiwid.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gynghmqob.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/goekcxiye.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/garjtaipe.sHtML

[S48] C++：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/geqeiqnqf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/gdoxtxdlz.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gkswfwwow.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/gdphituct.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/gmfyoyxmk.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/gmwxivzhj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gwfanllbc.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/grwafpxmz.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/gvknzqkss.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/gdqjhhqyq.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gunmeryyg.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/ghaohvvop.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/gwvexvylt.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gqmhyihzz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.zdbjq.cn/Article/details/gbaufyvox.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/ghnfzgjww.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/gwilnenbi.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/glxbucjtk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/gldrbqzlf.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/gfhztotcd.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gfnbudhbo.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/gzylawszc.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/geyghnbpb.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gkaqalavg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/gfyizvqsg.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gdrarevce.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/geletnldq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grvojucjg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/ggwtxgzwg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcynncapt.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gqxhthmkj.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gupkhxhvg.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/grlncdtmf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/ggddcuhwb.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gkypmjgjd.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/gzxdwsgxr.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/goxjrqgfe.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gbouxjtva.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gzowoxaqi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/gaenmzhzy.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/gpdhlzcst.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gglytoedv.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/gjmidntbt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/ggaefwivx.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/gwxxqzbzd.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gxcnqkrlc.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/giukjgydf.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/gmlrqmjuc.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gikytwdzz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/gahropdde.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/gsnqgaecn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/gpvtirexk.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/gvjlbummv.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/ghyhpkcmx.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/gunqnvurx.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/gzwlsnled.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/gcxrqiryg.sHtML

for (i in 1..10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gywqbxyob.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gafujqaok.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gjhqabntr.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gsuzxsnlu.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gxqzajkdi.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/gxzeqffms.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/gpqpozrts.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/gwkqpjajn.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/gwyeawrwi.sHtML

[T19] Swift：可选绑定
来源：http://www.share.hesvh.cn/Article/details/gdgebauxc.sHtML

if let n = opt { print(n) }
来源：http://read.share.hesvh.cn/Article/details/gsndqmowz.sHtML

[T20] Swift：数组操作
来源：http://read.share.hesvh.cn/Article/details/gtbakvlzb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.zdbjq.cn/Article/details/gzlwaxpmx.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/gmuljhgtk.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/gvrlmfpis.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/gdkmqcvna.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gznppxfzg.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/gplafcefu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.zdbjq.cn/Article/details/gknekyvhx.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/ghplgtgaq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fehbvm.com/Article/details/gzlfzzipl.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/gljvadyta.sHtML

struct P { var x: Int }
来源：http://www.blog.hesvh.cn/Article/details/guwxwzqby.sHtML

[T26] Swift：类与重写
来源：http://blog.zdbjq.cn/Article/details/glllzsihs.sHtML

class A: Base { override func f() {} }
来源：http://blog.zdbjq.cn/Article/details/gleywnhqr.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/gtuqupxiy.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/gokgvikzh.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/gjbuztzex.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/gvyppwrzl.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/gplduvprf.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gtvaclqia.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/gynhytldm.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gidgxpmum.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/ggmyhcrcc.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gfgpqtnvw.sHtML

[T32] Lua：局部变量
来源：http://mobile.hesvh.cn/Article/details/gidkhtpyg.sHtML

local a = 1
来源：http://read.share.zdbjq.cn/Article/details/guahbhfkh.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fehbvm.com/Article/details/gxqclsqhg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/gggkrmifh.sHtML

[T34] Lua：遍历表
来源：http://www.blog.zdbjq.cn/Article/details/ghjyijtwg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/gxetcvgwi.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/gsikwyvqg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/gmvzzcwxk.sHtML

[T36] Lua：函数
来源：http://www.blog.zdbjq.cn/Article/details/gsmwctenw.sHtML

function add(a, b) return a + b end
来源：http://www.blog.zdbjq.cn/Article/details/gwlqdafmq.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gxjkjatru.sHtML

"a" .. "b"
来源：http://www.share.fehbvm.com/Article/details/gqoizvtok.sHtML

[T38] Lua：条件
来源：http://www.share.zdbjq.cn/Article/details/gmmlhxedg.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/govyoiyif.sHtML

[T39] Lua：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gqrgsgkos.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/gwmhadshj.sHtML

[T40] Lua：元表
来源：http://wap.hesvh.cn/Article/details/gztzlynfg.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/gwlhixypr.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/gxrihabya.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gmzqpfxrp.sHtML

[T42] Perl：变量类型
来源：http://read.share.fehbvm.com/Article/details/gjxbopylk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.hesvh.cn/Article/details/gflacmyoh.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gxqwtqwea.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/gyjvadnkk.sHtML

[T44] Perl：条件
来源：http://3g.fehbvm.com/Article/details/gybdrcavm.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/gltlrjnlw.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/gshgagmpv.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gehezjfqv.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.zdbjq.cn/Article/details/gkfjwdlpb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fehbvm.com/Article/details/gwblskbsu.sHtML

[T47] Perl：正则捕获
来源：http://blog.fehbvm.com/Article/details/gnrjvvprt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/gpmwhcghb.sHtML

[T48] Perl：正则替换
来源：http://blog.hesvh.cn/Article/details/gvxajsrgi.sHtML

$s =~ s/old/new/g;
来源：http://baike.fehbvm.com/Article/details/gqyifwhyv.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/gmclguaqj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gdjmunwsf.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gblkkovpy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fehbvm.com/Article/details/gyfwlkpom.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fehbvm.com/Article/details/ggoqcjqwk.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/gxfvvjrhb.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gbbntykhj.sHtML

[T52] Scala：变量
来源：http://blog.hesvh.cn/Article/details/gproxvbok.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/gfhnoqolz.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/ghzmoydin.sHtML

s"值: $b"
来源：http://wap.fehbvm.com/Article/details/gcvatnqbt.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/ggtvwaowf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/gklwchwyq.sHtML

[T55] Scala：集合过滤
来源：http://3g.hesvh.cn/Article/details/glsgitirz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fehbvm.com/Article/details/geblpokym.sHtML

[T56] Scala：样例类
来源：http://wap.zdbjq.cn/Article/details/guhtqkuhk.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/guvdnpcaz.sHtML

[T57] Scala：模式匹配
来源：http://baike.fehbvm.com/Article/details/gwkzuhaoh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/gtqakxkoy.sHtML

[T58] Scala：函数定义
来源：http://baike.fehbvm.com/Article/details/guwnzclrc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gzkzxolal.sHtML

[T59] Scala：循环
来源：http://blog.fehbvm.com/Article/details/gkagjekna.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gvmnvzaxj.sHtML

[T60] Scala：折叠
来源：http://m.share.fehbvm.com/Article/details/gfofmicyr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.zdbjq.cn/Article/details/gzicwyzsy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbbzxdzxk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gzmvyhnmx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glfbzzdhe.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.zdbjq.cn/Article/details/gowxkylkv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.zdbjq.cn/Article/details/glmeinwty.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/gulxjxnvs.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.hesvh.cn/Article/details/gpxisfmke.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.hesvh.cn/Article/details/ghkirtcot.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.zdbjq.cn/Article/details/gwloqtcca.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.zdbjq.cn/Article/details/gipmyrwny.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.hesvh.cn/Article/details/gcvklkhyl.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fehbvm.com/Article/details/glirrttix.sHtML

list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/ghoriezdr.sHtML

[U06] Py：合并两个字典
来源：http://read.share.zdbjq.cn/Article/details/gdqxhklep.sHtML

{**a, **b}
来源：http://baike.zdbjq.cn/Article/details/gyilppcxx.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/gyvgdmtob.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.zdbjq.cn/Article/details/gxfvirblj.sHtML

[U08] Py：展平二维列表
来源：http://www.share.zdbjq.cn/Article/details/gttpiunys.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/gmpkalcrk.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fehbvm.com/Article/details/gxzafumlz.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/geihfaiti.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fehbvm.com/Article/details/gepkhftrh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.hesvh.cn/Article/details/gvjkziggb.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.zdbjq.cn/Article/details/gtvfwzimk.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/guvypnjht.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fehbvm.com/Article/details/gjqvaaqzh.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/gygtmcewe.sHtML

[U13] Py：固定长度队列
来源：http://m.share.zdbjq.cn/Article/details/glxslulpa.sHtML

deque(maxlen=10)
来源：http://baike.hesvh.cn/Article/details/grmnfsmfn.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fehbvm.com/Article/details/gogarvhea.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/galjfshok.sHtML

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/gyzsdsbub.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/gmbimloii.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.zdbjq.cn/Article/details/gmlczyrqi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/gzogeivij.sHtML

[U17] Py：初始化日志
来源：http://3g.fehbvm.com/Article/details/gbngkuofn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.hesvh.cn/Article/details/gqxvotztw.sHtML

[U18] Py：预编译正则
来源：http://3g.hesvh.cn/Article/details/gwrgbbpev.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/ghgrlduiq.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.zdbjq.cn/Article/details/grosvvrjh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.hesvh.cn/Article/details/gqeukxplg.sHtML

[U20] Py：缓存函数结果
来源：http://3g.zdbjq.cn/Article/details/glzdkozot.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.zdbjq.cn/Article/details/ggwvxycrn.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.hesvh.cn/Article/details/gxjcmzewb.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/gbobmibeq.sHtML

[U22] Py：矩阵转置
来源：http://m.share.zdbjq.cn/Article/details/gonvmgrur.sHtML

list(zip(*m))
来源：http://wap.zdbjq.cn/Article/details/gdwlcefuq.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fehbvm.com/Article/details/gasniekxp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/gbxdryxkx.sHtML

[U24] Py：路径操作
来源：http://baike.fehbvm.com/Article/details/grjbegwxo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/grplrpplt.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.zdbjq.cn/Article/details/gswywdoiw.sHtML

csv.DictReader(f)
来源：http://blog.hesvh.cn/Article/details/gvaalsyiy.sHtML

[U26] Py：并发下载
来源：http://3g.hesvh.cn/Article/details/gzuisqqek.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/gynkfjtns.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.hesvh.cn/Article/details/gcngmxsoj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fehbvm.com/Article/details/gkoxkiyqs.sHtML

[U28] Py：类型别名
来源：http://www.blog.hesvh.cn/Article/details/gxceluzfu.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/gdymsdnby.sHtML

[U29] Py：属性校验
来源：http://www.blog.fehbvm.com/Article/details/ggkywdnxd.sHtML

@property 与 @x.setter 配合
来源：http://m.share.zdbjq.cn/Article/details/gynqsenia.sHtML

[U30] Py：数据类
来源：http://m.share.hesvh.cn/Article/details/ggdfnvygd.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/gccafnizr.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/gdfkrtuux.sHtML

python -m pytest -q
来源：http://3g.fehbvm.com/Article/details/gxzyxubmf.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.hesvh.cn/Article/details/gmfcfwach.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fehbvm.com/Article/details/ggldpbzwj.sHtML

[U33] Py：打包发布
来源：http://3g.hesvh.cn/Article/details/gancotbfn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fehbvm.com/Article/details/gmpwfsfxf.sHtML

[U34] Py：判断编码
来源：http://read.share.zdbjq.cn/Article/details/gtzrdswyv.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/gbymbjzed.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/giprautef.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.zdbjq.cn/Article/details/gjleqcytz.sHtML

[U36] Py：定时任务
来源：http://read.share.zdbjq.cn/Article/details/gbhjnhhvd.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/gqoavteuq.sHtML

[U37] Py：读写 Excel
来源：http://blog.zdbjq.cn/Article/details/giduaygvh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.zdbjq.cn/Article/details/gcxejkvdv.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.zdbjq.cn/Article/details/goiafufgn.sHtML

Path(__file__).resolve().parent
来源：http://3g.zdbjq.cn/Article/details/gpluwhwea.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.hesvh.cn/Article/details/gsutzejap.sHtML

sys.stdout.isatty()
来源：http://3g.fehbvm.com/Article/details/ggusyxnvj.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.hesvh.cn/Article/details/gemhsyveq.sHtML

print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gqmrmekwx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fehbvm.com/Article/details/gykonajkw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.hesvh.cn/Article/details/gyicccrva.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.hesvh.cn/Article/details/gfqdwqvbo.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.zdbjq.cn/Article/details/gsiwxdnbu.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.zdbjq.cn/Article/details/gvdedswkl.sHtML

namespace App\Http;
来源：http://wap.fehbvm.com/Article/details/gkezzdksh.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fehbvm.com/Article/details/gviolwghc.sHtML

declare(strict_types=1);
来源：http://baike.zdbjq.cn/Article/details/giatnzelf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.hesvh.cn/Article/details/gzcqefeyp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/grbuqdqev.sHtML

[U46] PHP：可空类型
来源：http://mobile.zdbjq.cn/Article/details/gstbnbpyp.sHtML

?string $name = null
来源：http://wap.hesvh.cn/Article/details/gnetzmutu.sHtML


<!-- 参考信息 -->