代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gscksabpy.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkwcautq.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gieoxvszd.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/ghpsmwwcd.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkqvrmqn.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goegojbcq.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/goygdrdkg.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gahkfmmql.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddcrgnwj.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxhgmzdy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gtarkclzr.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehcagbeq.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebqnfshb.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gjomlhcby.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxmrjpgx.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gjmppabni.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gnymzppdw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcoequnsq.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gswthuspb.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gdyjeowrf.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjdzwura.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfrejqjv.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrvgqseb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gojgqzuvp.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gspliyivg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/glktrwtgd.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gdaxmkxzt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gtegxtabr.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhxkvzof.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/getouniug.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdldmrhek.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guclqgtzc.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupkdnwqi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtejpgpuf.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gmagvlreu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkhjwcas.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghetjrzip.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjdzdvax.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjaaeizp.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gnskjdhav.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqsbrbkt.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gbzxbptuq.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/ghmavloki.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbokvoxbk.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpylgnxq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gykdrapmg.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/gectruadc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxgipcxu.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrpzjjnf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnzidyiqk.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gzpmijvbh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gobygmwgo.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsekbbabe.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/goqyungnm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhwjkooe.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gwtegrcrd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gopmeprlq.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gabeuelzv.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gibgrguwz.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gpecexusu.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurcpjuhs.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwygexxp.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvqsvubt.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gaclutmip.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gpnpcypde.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkpcqbue.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrkpneuf.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtkherke.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvxvlyzc.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gdnsblksn.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/grzsixxfd.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlwukiju.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gkxkejako.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gxklwnfoq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gcmvfjzbq.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/glbickhkr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gphjfltix.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gftnndzni.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbcxlzux.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gghwbhulq.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/ginojdude.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnoatktjq.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/grpucfhbs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gcfcvobln.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gmajqgjey.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/giwogyvlu.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glliothhq.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/goumshbey.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebyiwjml.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/ghavwjwzf.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmjcgrnj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/glrhtbmph.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuunabgf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/givjrshut.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrtvubbc.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/grfgjyfef.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/ggyrkyjzl.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunvrocgm.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzznruca.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/ghiclskgy.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/grdognfkl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdoagtabz.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlunbplo.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/guulldnlk.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gheuuihnr.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/glbpnjzjj.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gklodkgpm.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzaonsedu.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtuezofv.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlbbdkgt.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gfloadotr.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gdiborqcq.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdqeadyf.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gerzrgcoo.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gaayiumfh.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnmogxdx.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/guqrixjeo.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/ggfeydlql.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gsahytcrr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbilltlzy.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gylkwzjge.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gramstfma.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/grbtzqams.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gaznpavlt.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/greihbueh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gfshsuvyi.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyzghceu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gcbxxnmva.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guohinozg.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/guerjgytj.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/gzdvratlp.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/goodzajso.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvabfqqn.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fanxiaobao.xyz/Article/details/glxknegsk.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/grnvgjgfp.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/gexvcutdm.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/grngmcnty.sHtML

guard let x = opt else { return }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmstrnhi.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhsagkjd.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/giglsicps.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gmllncqnm.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gcodkbtxx.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkhwagna.sHtML

local a = 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjyfuebo.sHtML

[T33] Lua：表（数组）
来源：http://blog.fanxiaobao.xyz/Article/details/gevzrqoim.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fanxiaobao.xyz/Article/details/gpzjtorua.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/gwsbrnunz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gupdrkcnk.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giunmjklc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwufjrhu.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gzsozapyx.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhycpcve.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gxhacbkhl.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/gfokpihnb.sHtML

[T38] Lua：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcacyruoi.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/gotbeqnyp.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhnebtvh.sHtML

string.find(s, "%d+")
来源：http://wap.fanxiaobao.xyz/Article/details/geyaliqeb.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxzwcnai.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkdjmnjr.sHtML

[T41] Perl：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gxukdtzhe.sHtML

print "Hello\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gzurpzhsr.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gatfedlvd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/ghwzhnzzb.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzhuluyy.sHtML

"值: $a"
来源：http://wap.fanxiaobao.xyz/Article/details/gpooqdwwm.sHtML

[T44] Perl：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gadfcbttn.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gldsgduel.sHtML

[T45] Perl：数组遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gyeogqujt.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwliyzobo.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjjydego.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrqsbrzc.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqvjdnvc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxgehwmn.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaurfubwp.sHtML

$s =~ s/old/new/g;
来源：http://baike.fanxiaobao.xyz/Article/details/gwndicmkp.sHtML

[T49] Perl：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gvdtlecyc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbarqxayw.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gylcuaert.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwurttyj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghkzghtoy.sHtML

[T51] Scala：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gkiefxgco.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gaadgvcax.sHtML

[T52] Scala：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/genuhwuri.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gknamjwxm.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqhcajrg.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gsaynuseb.sHtML

[T54] Scala：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gvepnmdre.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/golsxzqcs.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gydzdrhvi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgqmfkej.sHtML

[T56] Scala：样例类
来源：http://www.share.fanxiaobao.xyz/Article/details/grvlumlbk.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfulcbqcc.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucmtwowk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/gnyunbcox.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/ggcusuxdw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gdonvxynd.sHtML

[T59] Scala：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/grixihvkw.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtgtcojs.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvzbfock.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fanxiaobao.xyz/Article/details/gszgmvqqb.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/glmzwhedu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgzfjetu.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqrlynqj.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fanxiaobao.xyz/Article/details/ghhyholzm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjtunwfo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrqabwsn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/grogizfbl.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gynljmcmp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofmnccqp.sHtML

[U04] Py：变量调试打印
来源：http://3g.fanxiaobao.xyz/Article/details/gilvlmhfw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuimasus.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fanxiaobao.xyz/Article/details/gjydmsvcv.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gzubwwnzq.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcdyipyv.sHtML

{**a, **b}
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrenwoes.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwiafokq.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/gopbevgef.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/gaglszvrn.sHtML

[y for x in nested for y in x]
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnkotmhl.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrkjsncs.sHtML

max(d, key=d.get)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdpnwlmr.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdrlmtmq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmdzbqsx.sHtML

[U11] Py：生成器表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gcnimejdl.sHtML

(x * 2 for x in arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gksaapstg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagdvngdf.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvhmnusd.sHtML

[U13] Py：固定长度队列
来源：http://blog.fanxiaobao.xyz/Article/details/ghyveeudq.sHtML

deque(maxlen=10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygqzcbdu.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fanxiaobao.xyz/Article/details/gwwmqqkuo.sHtML

defaultdict(list)
来源：http://3g.fanxiaobao.xyz/Article/details/gpyokqbwg.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdlgykyb.sHtML

t = time.perf_counter()
来源：http://m.share.fanxiaobao.xyz/Article/details/gohyhhovc.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fanxiaobao.xyz/Article/details/ghsmilthg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fanxiaobao.xyz/Article/details/gsnnsfyve.sHtML

[U17] Py：初始化日志
来源：http://3g.fanxiaobao.xyz/Article/details/gxhrlznkt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcrgxfbx.sHtML

[U18] Py：预编译正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gwaikdfpi.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelfvleli.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpreungl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govrcspuq.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fanxiaobao.xyz/Article/details/gehbvdati.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/gakggfxwo.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fanxiaobao.xyz/Article/details/gqdhuacqf.sHtML

@contextlib.contextmanager
来源：http://wap.fanxiaobao.xyz/Article/details/gazrkmfjv.sHtML

[U22] Py：矩阵转置
来源：http://wap.fanxiaobao.xyz/Article/details/gvdtlongh.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwitfdkbh.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsbbljfk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fanxiaobao.xyz/Article/details/gnpfuoipg.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqnzufwh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gvmwptxqu.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fanxiaobao.xyz/Article/details/gystywgnt.sHtML

csv.DictReader(f)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkfylpyd.sHtML

[U26] Py：并发下载
来源：http://m.share.fanxiaobao.xyz/Article/details/gpezrmgxd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fanxiaobao.xyz/Article/details/giditoqhn.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcsszepq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fanxiaobao.xyz/Article/details/grtgmoyoh.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/gbxodfwcd.sHtML

UserId = int
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmensjbb.sHtML

[U29] Py：属性校验
来源：http://3g.fanxiaobao.xyz/Article/details/gkhsjpasb.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdkkcsbo.sHtML

[U30] Py：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwonblyn.sHtML

@dataclass(slots=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/glqyreuxr.sHtML

[U31] Py：单测
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmogecvt.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/gwcttpgmh.sHtML

[U32] Py：代码格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gypjgnubm.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fanxiaobao.xyz/Article/details/gtgdauylz.sHtML

[U33] Py：打包发布
来源：http://m.share.fanxiaobao.xyz/Article/details/ggeltirdl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fanxiaobao.xyz/Article/details/gtebgwxop.sHtML

[U34] Py：判断编码
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqxnwoqp.sHtML

chardet.detect(raw)
来源：http://read.share.fanxiaobao.xyz/Article/details/gipenmesp.sHtML

[U35] Py：发送邮件
来源：http://blog.fanxiaobao.xyz/Article/details/gyqplwbmo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqhfikiy.sHtML

[U36] Py：定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvklnogd.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fanxiaobao.xyz/Article/details/gqnkwmhto.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtudrxagb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gefsjttgg.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxwzjvth.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geeitmjem.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fanxiaobao.xyz/Article/details/glarancpk.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabpgzbqk.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fanxiaobao.xyz/Article/details/gpqtlqmvy.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fanxiaobao.xyz/Article/details/grxecoenq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gsaoysnat.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubfbauyf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmhhhbjr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fanxiaobao.xyz/Article/details/gcwtmrdyi.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgntsaha.sHtML

namespace App\Http;
来源：http://3g.fanxiaobao.xyz/Article/details/ghbrbnqde.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fanxiaobao.xyz/Article/details/gojuflroq.sHtML

declare(strict_types=1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghedvvxuj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/ghwayayie.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghevkswfo.sHtML

[U46] PHP：可空类型
来源：http://wap.fanxiaobao.xyz/Article/details/gajpuemdz.sHtML

?string $name = null
来源：http://baike.fanxiaobao.xyz/Article/details/ggfwodagp.sHtML

[U47] PHP：联合类型
来源：http://wap.fanxiaobao.xyz/Article/details/gmyqnvkqb.sHtML

int|string $id
来源：http://blog.fanxiaobao.xyz/Article/details/gbyeudxsq.sHtML

[U48] PHP：纯枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gxzeiizew.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqefckgx.sHtML


<!-- 参考信息 -->