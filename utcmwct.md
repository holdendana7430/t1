代发 wailian999

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/gnnkkqugw.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gtqamjhdb.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/geodfygcb.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gfmfcrqbi.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gycqqprim.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/gdfbhewku.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gudfskobd.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/gqrnbhejr.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gvkbgcxwi.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/ghhkjjfom.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gxdaxxpja.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gytahhhpg.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/glhxrmvll.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gghphphwn.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gmjwetcsn.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gwwrazlcb.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/gcbtwkfds.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/gexpwtbda.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gxfmlplqq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gdexvyqhs.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gwsktgbdb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/ggwqliayk.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gmegxhten.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gqetodjxk.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gfmrdibty.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/gfpihwose.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gduflysfn.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gnugqwzed.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/gjayvehni.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/gtquyqzot.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/glmyciqxz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gxdhdhsnj.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gbmykloju.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gqougnqhv.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gfdtymrmm.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gxdenxhge.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gscytkdjq.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/grekkgibs.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gfykvldpk.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/guioebgjy.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/gqqthrxze.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gzasiwyfq.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gvuvffqri.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/gngqbjjxx.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gwbyreuuw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/gstotjqrn.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/givyoesao.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gscizbgew.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/gilganhgy.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/grbzwrrsh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.zdbjq.cn/Article/details/glwnsoiao.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/grfxlyvjr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/gcrxjelgp.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/grggjhsow.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/gaqsjaqwe.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/gvmjxesiy.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/gnopwevca.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/gdpxpmune.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gnsuhtplg.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gsjrkpqmx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/gkhphmrnq.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gqeuotftw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.zdbjq.cn/Article/details/gpfrbhxla.sHtML

[S56] C++：optional
来源：http://www.m.share.fehbvm.com/Article/details/gfbnojesq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gbufytuxe.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gqrujgfhn.sHtML

constexpr int N = 10;
来源：http://m.share.fehbvm.com/Article/details/gonmiwryt.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/gnofldlot.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/gufkqadeq.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/grhjhzrsc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/gnapcktmp.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gqkmblywc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gwtmrbiyz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmscwbprb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gnhfbcbbx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzidjeugh.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/galnmxffi.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/grorppjor.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/glyyagwuq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gguhmsauz.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.hesvh.cn/Article/details/gkjapbsez.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/guwjverql.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/gdyuhbcpo.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gkwufgnny.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.hesvh.cn/Article/details/gqsxszgwl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gdpjczakr.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/gkbbrbwnn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/gurxyvlyc.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gxtifooya.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/gecvudpat.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/gkrmosvcn.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/geftrxsey.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gbdjshhsw.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.zdbjq.cn/Article/details/gfhwkygxj.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/gbyzncggf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/gzfduwgwm.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/gjqzkjsse.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.zdbjq.cn/Article/details/gnhfzwypi.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/gvocksnei.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gyvtblyax.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.zdbjq.cn/Article/details/gbcljsjym.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/grpbczabn.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gokzviwus.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/gafqrrsva.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gajrccnev.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/glidkzrqe.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gknhsscug.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gffeckjas.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/geiittosi.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gsntcibgv.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gyygyymzc.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/gfwevuluc.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/gjgnckodw.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/gcyvsecaa.sHtML

[T20] Swift：数组操作
来源：http://blog.hesvh.cn/Article/details/gvszmzizi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/gdqxohlin.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/gptgihsnh.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gutjjscyd.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/gflxzxxlj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gatmprtxf.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/ghafitezd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.hesvh.cn/Article/details/gaaurcyjk.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/gpyjrtfdg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/gwxjenwkz.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gcqbzuvbe.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gezjrdkgi.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/gvpcslwlo.sHtML

class A: Base { override func f() {} }
来源：http://www.share.zdbjq.cn/Article/details/gzycwlerg.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/ggulzvnug.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/gdxecplzl.sHtML

[T28] Swift：枚举
来源：http://3g.zdbjq.cn/Article/details/gdfhfmmgw.sHtML

enum Color { case red, green }
来源：http://www.blog.zdbjq.cn/Article/details/gecmgvien.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/gugsxkjdo.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fehbvm.com/Article/details/gbuffiqfl.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gtjtbbwdd.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/goocmhlkc.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/grwaamekc.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gfqrqjzey.sHtML

[T32] Lua：局部变量
来源：http://baike.hesvh.cn/Article/details/gaussvgvl.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/gypkzpraf.sHtML

[T33] Lua：表（数组）
来源：http://baike.zdbjq.cn/Article/details/gmgduupvd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/gtuiqyedz.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/gpqhpxhdj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/ghnsuknkk.sHtML

[T35] Lua：字典表
来源：http://mobile.fehbvm.com/Article/details/gyzkxrokr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/grhgxwfcc.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/gptaoqzvk.sHtML

function add(a, b) return a + b end
来源：http://www.blog.zdbjq.cn/Article/details/gwpjzoqze.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/gjdambxsu.sHtML

"a" .. "b"
来源：http://www.m.share.fehbvm.com/Article/details/gtceoejuh.sHtML

[T38] Lua：条件
来源：http://3g.zdbjq.cn/Article/details/gapbmtakg.sHtML

if x > 0 then print("正") end
来源：http://read.share.hesvh.cn/Article/details/ghfkkbfgf.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/glddvuosi.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/ggelbcvql.sHtML

[T40] Lua：元表
来源：http://www.m.share.fehbvm.com/Article/details/goxfqquud.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/ghptrvjkb.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gvjqudyar.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/gknfmfksh.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gnxeeexja.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fehbvm.com/Article/details/gjrrdywsg.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/gskvkgovb.sHtML

"值: $a"
来源：http://read.share.fehbvm.com/Article/details/gyclvyejo.sHtML

[T44] Perl：条件
来源：http://mobile.zdbjq.cn/Article/details/glfhooiat.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gxnbjfrrv.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/gillbmiyo.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.zdbjq.cn/Article/details/ghjuyyuov.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/grfylqzda.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/govnchvym.sHtML

[T47] Perl：正则捕获
来源：http://baike.hesvh.cn/Article/details/gyesnqmdn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/gfvzpkuqn.sHtML

[T48] Perl：正则替换
来源：http://mobile.hesvh.cn/Article/details/gtrnnubgo.sHtML

$s =~ s/old/new/g;
来源：http://www.share.zdbjq.cn/Article/details/glizhyojf.sHtML

[T49] Perl：函数
来源：http://mobile.hesvh.cn/Article/details/gizemoqav.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gtivbcnxd.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/grzeihujk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/gjbmsvcub.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.zdbjq.cn/Article/details/gzxqrhuxg.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/goeqmiysm.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gjhjtxjbx.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/gasjzdvno.sHtML

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gdqlcnaaz.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gcyqadeph.sHtML

s"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gnyleknki.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gwkixmdwh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gfdpjvdib.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gvlwfyyhr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.hesvh.cn/Article/details/ggpyyweda.sHtML

[T56] Scala：样例类
来源：http://www.share.zdbjq.cn/Article/details/gdsbiifca.sHtML

case class User(name: String, age: Int)
来源：http://wap.fehbvm.com/Article/details/gbeumvrxw.sHtML

[T57] Scala：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gxdbcfwec.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/gnmutogyn.sHtML

[T58] Scala：函数定义
来源：http://wap.fehbvm.com/Article/details/gmkxnwnhj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/gzrztkego.sHtML

[T59] Scala：循环
来源：http://baike.hesvh.cn/Article/details/gyhqcnmac.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gkfvybcju.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gpcuhhyhg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.zdbjq.cn/Article/details/gupimolre.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyisizopq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gznjqqssq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpfskfnqw.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/ggqcfkvzq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.zdbjq.cn/Article/details/grdccwjcx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.hesvh.cn/Article/details/gmhmlxuop.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/gocsymhep.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gknhpbcon.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.hesvh.cn/Article/details/geoinmebh.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fehbvm.com/Article/details/gofotkqew.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.zdbjq.cn/Article/details/gjltvrhzy.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fehbvm.com/Article/details/gkgggzsuf.sHtML

list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gtwklcqun.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fehbvm.com/Article/details/gxcvgblkf.sHtML

{**a, **b}
来源：http://mobile.fehbvm.com/Article/details/gslfqghtg.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fehbvm.com/Article/details/guhrwzgkh.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/gnvtpnxpc.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fehbvm.com/Article/details/gxfkefywx.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/gcofowisy.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.hesvh.cn/Article/details/gxowfdtwm.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/gkicxmpxk.sHtML

[U10] Py：按值排序字典
来源：http://3g.fehbvm.com/Article/details/gheystwzz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/gombphuoz.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/ggbcmtkzp.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/gtmzdoxsr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/gbnesthnm.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/gvtzotazu.sHtML

[U13] Py：固定长度队列
来源：http://www.share.hesvh.cn/Article/details/gqhmwabhp.sHtML

deque(maxlen=10)
来源：http://www.m.share.zdbjq.cn/Article/details/gkvpdizzs.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.zdbjq.cn/Article/details/gzetixpdh.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/gbnvcerxd.sHtML

[U15] Py：高精度计时
来源：http://wap.hesvh.cn/Article/details/gvbgliasf.sHtML

t = time.perf_counter()
来源：http://read.share.zdbjq.cn/Article/details/gnnhvqydg.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fehbvm.com/Article/details/gmaqmapdm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.zdbjq.cn/Article/details/grehqbjed.sHtML

[U17] Py：初始化日志
来源：http://www.blog.zdbjq.cn/Article/details/gbkllfdcn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.zdbjq.cn/Article/details/ggloinmnt.sHtML

[U18] Py：预编译正则
来源：http://www.share.zdbjq.cn/Article/details/ggiwsyrij.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gbtlszekn.sHtML

[U19] Py：正则替换带回调
来源：http://3g.zdbjq.cn/Article/details/giywzuwuk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.zdbjq.cn/Article/details/gcqqdwxqq.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/gkacvnjqz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fehbvm.com/Article/details/gzrssymqv.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.zdbjq.cn/Article/details/gesuawmnb.sHtML

@contextlib.contextmanager
来源：http://mobile.hesvh.cn/Article/details/gdcdkgmfc.sHtML

[U22] Py：矩阵转置
来源：http://www.share.hesvh.cn/Article/details/gjtifuych.sHtML

list(zip(*m))
来源：http://wap.hesvh.cn/Article/details/gygtzoxub.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fehbvm.com/Article/details/gtjxiuclc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fehbvm.com/Article/details/gjrigmrls.sHtML

[U24] Py：路径操作
来源：http://wap.fehbvm.com/Article/details/gmjbrbgfj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/geahabhfq.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/gvyaykokk.sHtML

csv.DictReader(f)
来源：http://www.share.hesvh.cn/Article/details/gclpoixzt.sHtML

[U26] Py：并发下载
来源：http://www.share.fehbvm.com/Article/details/gvhlimsar.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.zdbjq.cn/Article/details/gocopkvca.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.zdbjq.cn/Article/details/gcywybrwa.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fehbvm.com/Article/details/gadhkyost.sHtML

[U28] Py：类型别名
来源：http://www.share.hesvh.cn/Article/details/gmtyzubfw.sHtML

UserId = int
来源：http://baike.hesvh.cn/Article/details/gsuelonms.sHtML

[U29] Py：属性校验
来源：http://mobile.zdbjq.cn/Article/details/ggijmgten.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/gnkafjjuk.sHtML

[U30] Py：数据类
来源：http://3g.hesvh.cn/Article/details/gtzwvxdgs.sHtML

@dataclass(slots=True)
来源：http://baike.hesvh.cn/Article/details/gsrpslxbc.sHtML

[U31] Py：单测
来源：http://blog.fehbvm.com/Article/details/ghxroexxo.sHtML

python -m pytest -q
来源：http://wap.zdbjq.cn/Article/details/gznovdzhv.sHtML

[U32] Py：代码格式化
来源：http://read.share.fehbvm.com/Article/details/gnlbchtaj.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fehbvm.com/Article/details/gdkgeiggx.sHtML

[U33] Py：打包发布
来源：http://blog.hesvh.cn/Article/details/gaotlaryu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/gfwffsgfe.sHtML

[U34] Py：判断编码
来源：http://www.share.fehbvm.com/Article/details/giipwzryq.sHtML

chardet.detect(raw)
来源：http://baike.hesvh.cn/Article/details/grljnktsk.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.hesvh.cn/Article/details/gdshktedu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.hesvh.cn/Article/details/gkevpelec.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/gnmifclkl.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.hesvh.cn/Article/details/gdofcpfru.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/gyiucwwsp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.zdbjq.cn/Article/details/gzenrhkyi.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fehbvm.com/Article/details/gguhfxebu.sHtML

Path(__file__).resolve().parent
来源：http://blog.zdbjq.cn/Article/details/ggnrxicxp.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.hesvh.cn/Article/details/gomniobaq.sHtML

sys.stdout.isatty()
来源：http://www.share.zdbjq.cn/Article/details/gxinvmpjq.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.hesvh.cn/Article/details/gayfpxxhs.sHtML

print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/ggnkxhdwl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.zdbjq.cn/Article/details/gkdbjulnk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.zdbjq.cn/Article/details/gjijwdlzo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fehbvm.com/Article/details/gsornouev.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fehbvm.com/Article/details/glmgutclk.sHtML

[U43] PHP：声明命名空间
来源：http://3g.hesvh.cn/Article/details/gxvrxjehc.sHtML

namespace App\Http;
来源：http://mobile.zdbjq.cn/Article/details/gozjhyhhb.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fehbvm.com/Article/details/gfvbgshuu.sHtML

declare(strict_types=1);
来源：http://3g.hesvh.cn/Article/details/gxumdaaov.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.hesvh.cn/Article/details/gajmookze.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gkxlebgit.sHtML

[U46] PHP：可空类型
来源：http://m.share.hesvh.cn/Article/details/glaecjifw.sHtML

?string $name = null
来源：http://www.share.hesvh.cn/Article/details/gopwzccqd.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fehbvm.com/Article/details/gwucyduul.sHtML

int|string $id
来源：http://m.share.hesvh.cn/Article/details/gkowbltqh.sHtML

[U48] PHP：纯枚举
来源：http://wap.fehbvm.com/Article/details/ginyzzavu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.zdbjq.cn/Article/details/gopqzhasu.sHtML

[U49] PHP：只读属性
来源：http://m.share.zdbjq.cn/Article/details/gmcsoundj.sHtML

public readonly string $name
来源：http://www.m.share.hesvh.cn/Article/details/gofudtwug.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.zdbjq.cn/Article/details/ghchzazfk.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fehbvm.com/Article/details/gaqzvalur.sHtML


<!-- 参考信息 -->