代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/gxxvvdsxg.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/grogzturb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gvhwionya.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/gjqdroqmb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/ghxybptgj.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/gcagatxgj.sHtML

memcpy(dst, src, n);
来源：http://baike.fehbvm.com/Article/details/gmubuuyrn.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/gokxuplxg.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/ghagqlgwh.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gxzziwsdl.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gdoptmdra.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gebnsnsck.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gdjbfrjsr.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/guaulrhxw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gahaowgjx.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gwttjfjpj.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/gktndntyh.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gjkkqzmtq.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/gddqsyisk.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/guztttanu.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/gxjlwuvhk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gwqbavhzd.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/guanyclgr.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gfkrcqzdw.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gurdaedab.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gqvsbrnxb.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/gcsjezdal.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gnrehsdbs.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gniudwrwc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gojsmsjrf.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/gadgtmkrz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/ggciiwqxs.sHtML

[S37] C++：set
来源：http://www.blog.zdbjq.cn/Article/details/gbfexidgq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gxvsoavph.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/gmqcyyhwa.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gcaukxrnk.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/gzmafepdc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gsaxppnmm.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/gfpgytyth.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/glpxcphow.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/gitjbxmni.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/gikzjdofi.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/gnzgbmrrr.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/glnmgcjlv.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/geahsnsve.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/gohdxxpmr.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/ghbkckwcp.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gzcfgdpcu.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gyhrhlclg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/gdgvshisb.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gnkqfeceo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/ghutwpzwd.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gzaxovtvv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gauwfibda.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gfdpspezw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gyongniey.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/gtcwtuqfg.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/gihurnhry.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/gypwqqeua.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/gdortjopn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gbcjqltoq.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/ggrcefwwt.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/gnnmhhxco.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gtbzemifo.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/gclijajwa.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gtfrrokju.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gcvugyupv.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gcmzhnuwz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/gtzcfjalx.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/ghqhvlnlq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/gvsdaywvq.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/gjbbrjird.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/gqhsktqfm.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/gzszvfnqk.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/gqlaugytn.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gianstlxy.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/gzbbhllai.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gmxdnwmnn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fehbvm.com/Article/details/gwwgozjgy.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gpviqcamq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/gvhhhpwhz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfdigrixt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/ggkddigjc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmclqicdd.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/glgulcozr.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gtevqnjnr.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gpmuwkwog.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gviiuuihd.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/gpvgoxfyq.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gnjuifscc.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gwucdkdep.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gbgswtrhj.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/gcmlxofhu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gubqtquot.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gcnwjkxgy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gehmynaoq.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/gqpsorehh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/gzcertipt.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/grlfuruhz.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gjxejlwuh.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/grynmouaw.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/gxpwnktgu.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/gluynaitf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gigretrxq.sHtML

[T11] Kotlin：协程
来源：http://read.share.zdbjq.cn/Article/details/gqconuskg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/gofxhuwbk.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/gmuddupyh.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fehbvm.com/Article/details/gppfrdgea.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/gktgilepi.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/gpgyecnrb.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/gsfxipkbx.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gbfbctexk.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/gdfxsjmot.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gvnbrhgpk.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gzcojcsad.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gxfmgsnif.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.zdbjq.cn/Article/details/gnkvdjnvr.sHtML

var a = 1;  let b = 2
来源：http://read.share.fehbvm.com/Article/details/ghanoeaer.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/goxpzmccq.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/gvbenqptk.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/gpexixeyy.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/gmiysfjcf.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/gryazomug.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.hesvh.cn/Article/details/gqwqcqshn.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/gekhmthfj.sHtML

for x in a { print(x) }
来源：http://www.share.zdbjq.cn/Article/details/gxrigmrfs.sHtML

[T22] Swift：字典
来源：http://m.share.zdbjq.cn/Article/details/gdylqfasi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/guwuchybf.sHtML

[T23] Swift：函数
来源：http://www.share.fehbvm.com/Article/details/gidalvyol.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/gcnpqdhdt.sHtML

[T24] Swift：闭包
来源：http://mobile.fehbvm.com/Article/details/gxntznjtj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gkjvfsugu.sHtML

[T25] Swift：结构体
来源：http://read.share.fehbvm.com/Article/details/gobjxpvuo.sHtML

struct P { var x: Int }
来源：http://m.share.zdbjq.cn/Article/details/gczeogpmo.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/gizuhwehh.sHtML

class A: Base { override func f() {} }
来源：http://wap.zdbjq.cn/Article/details/glfxclczp.sHtML

[T27] Swift：错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gjumoymib.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/gpckelyrd.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/gdjvmmgfi.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/goguytpam.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gdahevbxb.sHtML

guard let x = opt else { return }
来源：http://3g.fehbvm.com/Article/details/gjnnhzgua.sHtML

[T30] Swift：协议
来源：http://www.share.fehbvm.com/Article/details/gkokskddb.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gvbhyrism.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/ghbdawmdh.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gazcqauic.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/gdtuzzjeb.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/gybgsqpnu.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/gcidzbkle.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.zdbjq.cn/Article/details/gjfdjwqkz.sHtML

[T34] Lua：遍历表
来源：http://www.share.hesvh.cn/Article/details/gcskxhmnl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fehbvm.com/Article/details/ghvoqgcra.sHtML

[T35] Lua：字典表
来源：http://m.share.fehbvm.com/Article/details/gxqpiuruf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/gaffrhhns.sHtML

[T36] Lua：函数
来源：http://wap.fehbvm.com/Article/details/grwgrmekw.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/gouvqnxbs.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/ggrwbsmvb.sHtML

"a" .. "b"
来源：http://read.share.zdbjq.cn/Article/details/ghwumwnpz.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/guweioukc.sHtML

if x > 0 then print("正") end
来源：http://mobile.zdbjq.cn/Article/details/gswhmdkeo.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gpohxthji.sHtML

string.find(s, "%d+")
来源：http://read.share.zdbjq.cn/Article/details/gnvnbcosc.sHtML

[T40] Lua：元表
来源：http://blog.fehbvm.com/Article/details/gpholnzcl.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.hesvh.cn/Article/details/grxoyqplg.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/gfxwsehfi.sHtML

print "Hello\n";
来源：http://3g.zdbjq.cn/Article/details/gogkhfjqg.sHtML

[T42] Perl：变量类型
来源：http://www.blog.hesvh.cn/Article/details/gsydyrkds.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/gymcwievi.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/geidhlnqt.sHtML

"值: $a"
来源：http://www.m.share.zdbjq.cn/Article/details/gcfxwzufe.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/gaodlmaom.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.hesvh.cn/Article/details/ghoxskluo.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fehbvm.com/Article/details/gavnzwadx.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.zdbjq.cn/Article/details/gkzzttjpn.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fehbvm.com/Article/details/gzpnfdqow.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fehbvm.com/Article/details/gbzlbnvmh.sHtML

[T47] Perl：正则捕获
来源：http://blog.zdbjq.cn/Article/details/gotkngrxg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/gpgayvvxi.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/gxmgykyaj.sHtML

$s =~ s/old/new/g;
来源：http://baike.zdbjq.cn/Article/details/gqhlmsusp.sHtML

[T49] Perl：函数
来源：http://www.m.share.fehbvm.com/Article/details/gvgzrzaic.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gwpdovwsu.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gdmumlgvp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fehbvm.com/Article/details/gmskhbpkr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/gvlrwhbij.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gsjdlzoek.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/goddkming.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/gshusfqoe.sHtML

val a = 1;  var b = 2
来源：http://www.blog.hesvh.cn/Article/details/gyzfzzmrg.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gnbpjkbqu.sHtML

s"值: $b"
来源：http://3g.hesvh.cn/Article/details/gcxdghfnr.sHtML

[T54] Scala：集合映射
来源：http://www.share.hesvh.cn/Article/details/gxouxcxgt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.hesvh.cn/Article/details/gfckdtczb.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gsizgtokr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.zdbjq.cn/Article/details/gjmjzzuxo.sHtML

[T56] Scala：样例类
来源：http://baike.hesvh.cn/Article/details/gcpktgzom.sHtML

case class User(name: String, age: Int)
来源：http://baike.hesvh.cn/Article/details/gnxdkfckr.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gkpdzlfop.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.hesvh.cn/Article/details/gjojrofki.sHtML

[T58] Scala：函数定义
来源：http://wap.hesvh.cn/Article/details/gvaziwzxv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.zdbjq.cn/Article/details/gvjmaubfp.sHtML

[T59] Scala：循环
来源：http://read.share.hesvh.cn/Article/details/gtiuggnkb.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/gbrbkmmei.sHtML

[T60] Scala：折叠
来源：http://m.share.zdbjq.cn/Article/details/gxryaqcik.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.hesvh.cn/Article/details/gqykdrbku.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gawjhalhc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gkdtttqbu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grqjnhlfa.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.zdbjq.cn/Article/details/gavfiipxf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fehbvm.com/Article/details/ggaajsind.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/gpoqpnuid.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/gflzgdexe.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/gagxxganr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.hesvh.cn/Article/details/gucrhbnvs.sHtML

[U04] Py：变量调试打印
来源：http://wap.hesvh.cn/Article/details/gxoojoyse.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.zdbjq.cn/Article/details/gcgqbidwg.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/gyeolknnc.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gmrzeahfk.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fehbvm.com/Article/details/gkxezqppe.sHtML

{**a, **b}
来源：http://m.share.hesvh.cn/Article/details/gcusvztzn.sHtML

[U07] Py：反转字典键值
来源：http://3g.hesvh.cn/Article/details/gyyouijxg.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/gagljnlpo.sHtML

[U08] Py：展平二维列表
来源：http://m.share.zdbjq.cn/Article/details/ggqxvhjkm.sHtML

[y for x in nested for y in x]
来源：http://www.blog.hesvh.cn/Article/details/gfmckiqcs.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/gpmoxofvq.sHtML

max(d, key=d.get)
来源：http://www.blog.zdbjq.cn/Article/details/gdwiyqyei.sHtML

[U10] Py：按值排序字典
来源：http://mobile.hesvh.cn/Article/details/gblylzjxa.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fehbvm.com/Article/details/guhusuuyz.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/greymslmq.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/gnqdirxdu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/gbgyaejgh.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fehbvm.com/Article/details/gjkmzrdpk.sHtML

[U13] Py：固定长度队列
来源：http://blog.hesvh.cn/Article/details/gmpaclwrb.sHtML

deque(maxlen=10)
来源：http://www.share.hesvh.cn/Article/details/gvkwtvwmz.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.hesvh.cn/Article/details/gvovbmgyw.sHtML

defaultdict(list)
来源：http://baike.fehbvm.com/Article/details/grvsjlmou.sHtML

[U15] Py：高精度计时
来源：http://m.share.zdbjq.cn/Article/details/ghzudpvrx.sHtML

t = time.perf_counter()
来源：http://www.share.hesvh.cn/Article/details/glbbanqvd.sHtML

[U16] Py：命令行参数解析
来源：http://baike.hesvh.cn/Article/details/gpagsjjvt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fehbvm.com/Article/details/gzagzahfn.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/gyakivokc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.zdbjq.cn/Article/details/gctvngjid.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/gngblercb.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gewmemwpl.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.zdbjq.cn/Article/details/gbexzjfrb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/ggcoegznx.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.hesvh.cn/Article/details/gukehhrcs.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.zdbjq.cn/Article/details/gkmstgkvt.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.hesvh.cn/Article/details/gifyspsta.sHtML

@contextlib.contextmanager
来源：http://baike.zdbjq.cn/Article/details/gbnvhyvog.sHtML

[U22] Py：矩阵转置
来源：http://mobile.hesvh.cn/Article/details/gpbfhvtsh.sHtML

list(zip(*m))
来源：http://wap.zdbjq.cn/Article/details/gqwchogpu.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.hesvh.cn/Article/details/gifpbtrpu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.zdbjq.cn/Article/details/gjqtxdylt.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/gmpgftpzz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gswurervs.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.hesvh.cn/Article/details/ghplvfyyr.sHtML

csv.DictReader(f)
来源：http://www.m.share.hesvh.cn/Article/details/gocxotyna.sHtML

[U26] Py：并发下载
来源：http://read.share.fehbvm.com/Article/details/gccizfwtf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.hesvh.cn/Article/details/gtwzulico.sHtML

[U27] Py：异步 HTTP
来源：http://3g.hesvh.cn/Article/details/glwbtjaiw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.hesvh.cn/Article/details/gyrwebftj.sHtML

[U28] Py：类型别名
来源：http://wap.fehbvm.com/Article/details/gauprageq.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/gfcdsxokf.sHtML

[U29] Py：属性校验
来源：http://3g.fehbvm.com/Article/details/gewujhanr.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/gavccvqje.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/gnnipdcql.sHtML

@dataclass(slots=True)
来源：http://baike.fehbvm.com/Article/details/ghguvcvph.sHtML

[U31] Py：单测
来源：http://www.blog.hesvh.cn/Article/details/gwysdgevp.sHtML

python -m pytest -q
来源：http://www.share.hesvh.cn/Article/details/gntckwyde.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/gdcnsdvti.sHtML

ruff format . && ruff check --fix .
来源：http://baike.hesvh.cn/Article/details/gvufgrvtl.sHtML

[U33] Py：打包发布
来源：http://baike.zdbjq.cn/Article/details/genljbihk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/ggrdmjsyj.sHtML

[U34] Py：判断编码
来源：http://m.share.hesvh.cn/Article/details/gqvhikqyv.sHtML

chardet.detect(raw)
来源：http://wap.hesvh.cn/Article/details/gvvgfazzl.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/gxldhuvtx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.zdbjq.cn/Article/details/ghefzfbhm.sHtML

[U36] Py：定时任务
来源：http://wap.hesvh.cn/Article/details/gksosglbl.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.zdbjq.cn/Article/details/grnhkyfzl.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fehbvm.com/Article/details/glnbfzjxr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.hesvh.cn/Article/details/gizpaihuk.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/gwrjhdspe.sHtML

Path(__file__).resolve().parent
来源：http://read.share.hesvh.cn/Article/details/geeoeahhw.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.zdbjq.cn/Article/details/gvhkygvtb.sHtML

sys.stdout.isatty()
来源：http://www.blog.hesvh.cn/Article/details/gvluolgpn.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/ggwhjvwbo.sHtML

print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/ghwijlnsp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fehbvm.com/Article/details/gqxjboukm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fehbvm.com/Article/details/gfcmdolvg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/gtacmeczl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.hesvh.cn/Article/details/gnzacotui.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fehbvm.com/Article/details/geqehdbny.sHtML

namespace App\Http;
来源：http://baike.fehbvm.com/Article/details/gcshjrfhm.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.zdbjq.cn/Article/details/grviprezq.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/gjwsruwso.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.hesvh.cn/Article/details/gsylhhwgw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gnnxbocmp.sHtML

[U46] PHP：可空类型
来源：http://wap.zdbjq.cn/Article/details/gxvhbmbnf.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/ghggtdcga.sHtML


<!-- 参考信息 -->