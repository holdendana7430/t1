代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gyqgwbmjd.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/getdowcwi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gmjcnzjuw.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gitobxcuz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gbhagrrhf.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gucfixqxt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/griacvvpw.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/gkzqycbug.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/grobprocw.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/gtisgzvly.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/ggzshltpz.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/gmnkyditz.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/gdvmjrkrs.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gbrdkoaqc.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gglqhpxrb.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/ghbnizzca.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/ggshgehbd.sHtML

[S29] C：变参函数
来源：http://mobile.hesvh.cn/Article/details/gihfctjzc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/gytobauxd.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/gutbltxtn.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gjksaiqcs.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gjbctyqsf.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/gtmzorxvu.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gdbmkzshi.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/gonxlylhr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gfidyldgt.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gcaefcfba.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/gvuwvgjyk.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/glfcornyj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/gldaoseus.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/gpxdgffit.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/gvbabuimk.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/grqdhykxk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gpobsmnkp.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/gjrurqkgl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gosibdztk.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gvhlybbpz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/ggpetzbkk.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gjoyqxbnb.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gkeyomyhk.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/geineyach.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gjtmzuhsf.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gkrfskuyd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/gmndeccoi.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gtwbmqaoa.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/gneavgpmj.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/gajcmexfm.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/ggofpelju.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/gofjygopw.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gyufrbtsb.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gaeuounul.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gufcijvwu.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/gvbbpzxnk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gymisummu.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gymeblomb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/gpfqrcwcc.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gkzuymufu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gobdyisoq.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gxqpgbxgg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/gbubawmik.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gtvewzmvy.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/gvpldxiok.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gjeactnaz.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/grzajzddr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gzzbxfyud.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/gizqcbvmy.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/ghxvuuptu.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gibrxqrxi.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/giaidanwa.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/gduuproic.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gcfvegkql.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/gyalzpxux.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gxuoleiaf.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/glpfutixy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/geoaskdke.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/ghdidsdso.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gboankgsd.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/grxpamino.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/gdwifzogh.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gclucimyb.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/gsgyrmthw.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/grytcnkdx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/ghqmddwkv.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/gqjwgetly.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/grupvlymj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsknxqbri.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/gpyhfcptu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkqefkkkm.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/gojubqoba.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gqakenmrr.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gmiptqceq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/gnhorojpa.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/ghcqhzing.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/godkkvalu.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gludfaqdz.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/ghlpiqqgp.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gqdbonoot.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.zdbjq.cn/Article/details/gafjcssju.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/gpflojqoz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fehbvm.com/Article/details/gdjgpslmt.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gesryvrpy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gwlxmqjpw.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gdyluhjhj.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/groufmkwi.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gxcepwwzo.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/gabbhhbgx.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/gfmszrdfn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/gapketbzt.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/goirzufgm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.zdbjq.cn/Article/details/gazfobufz.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.hesvh.cn/Article/details/gwztwuhuz.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/ggbjiwloa.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/gqbqxkyfb.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/gyalgnees.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/guuvciiyj.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/gmvstsqez.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gpeqybmib.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/gwwyxiiew.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/ggotdtkhq.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gybxnbmwq.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/gaxubujje.sHtML

var a = 1;  let b = 2
来源：http://3g.zdbjq.cn/Article/details/gvnaislmd.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/gwbslzgya.sHtML

"值: \(b)"
来源：http://m.share.fehbvm.com/Article/details/gxryghjew.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gkdtlfuly.sHtML

if let n = opt { print(n) }
来源：http://www.share.hesvh.cn/Article/details/gseueyesd.sHtML

[T20] Swift：数组操作
来源：http://www.share.fehbvm.com/Article/details/gejhdbqxu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fehbvm.com/Article/details/gqyljmzji.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/gesywpqzs.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gmzagsidn.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/gjqgrcbah.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/gdotxjeyt.sHtML

[T23] Swift：函数
来源：http://read.share.hesvh.cn/Article/details/gqnblbosb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gfrznabwq.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/gdhuxvbsh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/gnnjcxhug.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/gitvlxhiq.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gieiedsbs.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/giazxkhog.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/gqbqbruhq.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/gtuferdua.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/geuzzftng.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/ggsrywgli.sHtML

enum Color { case red, green }
来源：http://m.share.hesvh.cn/Article/details/gvawiqvdc.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fehbvm.com/Article/details/ghmhrrcnw.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/gspyzxada.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/gwfyhzisf.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/ghizjozgg.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/glthbfoqu.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/grnwtzdnh.sHtML

[T32] Lua：局部变量
来源：http://wap.fehbvm.com/Article/details/ghkffqcii.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/gktjkfaqt.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/gcjofxwea.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/ggqkvxmdm.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/gjgrnxxcj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/guwuctjsh.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/ggqadptdd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/gddniecvo.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/gmlqhjhmb.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/gpchqgtyi.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gcyziggha.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/glsvandyz.sHtML

[T38] Lua：条件
来源：http://read.share.fehbvm.com/Article/details/gmzvyctlo.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/gmwyqvajz.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gpasqumay.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/gllhxpwkf.sHtML

[T40] Lua：元表
来源：http://wap.hesvh.cn/Article/details/ggmybheag.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/grlskcday.sHtML

[T41] Perl：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gntkyxhno.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gvenshhke.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gbtrxlgpk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.zdbjq.cn/Article/details/ghtvguonw.sHtML

[T43] Perl：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gmqopndcp.sHtML

"值: $a"
来源：http://wap.fehbvm.com/Article/details/girmvmamz.sHtML

[T44] Perl：条件
来源：http://read.share.fehbvm.com/Article/details/gajvbuzhc.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbbruvstv.sHtML

[T45] Perl：数组遍历
来源：http://www.share.hesvh.cn/Article/details/gzrlondah.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.hesvh.cn/Article/details/gudsivvwd.sHtML

[T46] Perl：哈希操作
来源：http://read.share.zdbjq.cn/Article/details/giubzatqn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/guvgzmrjw.sHtML

[T47] Perl：正则捕获
来源：http://blog.hesvh.cn/Article/details/gvykmmhke.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.hesvh.cn/Article/details/gxcqccczs.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gxamoguhe.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/gkpfasovf.sHtML

[T49] Perl：函数
来源：http://m.share.fehbvm.com/Article/details/gnhyzlqhk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/guqhaaqxk.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gpbleagqg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/ghfpozguc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gpqeqpioq.sHtML

[T51] Scala：Hello World
来源：http://wap.zdbjq.cn/Article/details/gcwkzluzv.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gxogrecdl.sHtML

[T52] Scala：变量
来源：http://www.share.zdbjq.cn/Article/details/gnykzgddz.sHtML

val a = 1;  var b = 2
来源：http://baike.hesvh.cn/Article/details/gewbzrqvl.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gohizwrps.sHtML

s"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gcxbmvqdp.sHtML

[T54] Scala：集合映射
来源：http://3g.hesvh.cn/Article/details/ghxpxjnid.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.hesvh.cn/Article/details/girqotheq.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gbtuunxrz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.hesvh.cn/Article/details/gmsjagdus.sHtML

[T56] Scala：样例类
来源：http://baike.hesvh.cn/Article/details/gegywydxs.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gzxlbqmuj.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/gobyoqpry.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.zdbjq.cn/Article/details/gxejlnbyd.sHtML

[T58] Scala：函数定义
来源：http://baike.hesvh.cn/Article/details/gdvyyneid.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fehbvm.com/Article/details/gqpbasycr.sHtML

[T59] Scala：循环
来源：http://blog.fehbvm.com/Article/details/gnytdvkjz.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/gvxqqotlg.sHtML

[T60] Scala：折叠
来源：http://m.share.hesvh.cn/Article/details/gitbauddu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fehbvm.com/Article/details/gzjwgmoff.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbfakmmuv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gyotwryva.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbyeygryt.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fehbvm.com/Article/details/grzbhgzjt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.zdbjq.cn/Article/details/gqcaewavu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.hesvh.cn/Article/details/gzyivvacx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/gvxehmvtx.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/gpahmgoun.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fehbvm.com/Article/details/ghywscdav.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fehbvm.com/Article/details/gwbhrpynt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gttgwxwmg.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/glhcurnvu.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gqinkawdz.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fehbvm.com/Article/details/gzngypkuz.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/glvbyyknf.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fehbvm.com/Article/details/gkvjtjtgr.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/gbqxpvhqd.sHtML

[U08] Py：展平二维列表
来源：http://read.share.zdbjq.cn/Article/details/geibbyicj.sHtML

[y for x in nested for y in x]
来源：http://baike.zdbjq.cn/Article/details/gornrmwjt.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.hesvh.cn/Article/details/gjwydpzzr.sHtML

max(d, key=d.get)
来源：http://www.share.zdbjq.cn/Article/details/gdfkchfzo.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.zdbjq.cn/Article/details/gixvgleja.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fehbvm.com/Article/details/gbdgperxi.sHtML

[U11] Py：生成器表达式
来源：http://mobile.hesvh.cn/Article/details/gibufylpa.sHtML

(x * 2 for x in arr)
来源：http://3g.hesvh.cn/Article/details/gdjaaxtxb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/gccwbiupj.sHtML

Counter(arr).most_common(3)
来源：http://m.share.hesvh.cn/Article/details/ghqoufcwy.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/gdwyinork.sHtML

deque(maxlen=10)
来源：http://baike.fehbvm.com/Article/details/gbedqlykv.sHtML

[U14] Py：分组收集到列表
来源：http://3g.hesvh.cn/Article/details/gbkjiimin.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/gdozjxsen.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/gzsoccunt.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/ggbydhycc.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.hesvh.cn/Article/details/gcelepdxx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.zdbjq.cn/Article/details/gzwroulwv.sHtML

[U17] Py：初始化日志
来源：http://mobile.zdbjq.cn/Article/details/geyxuducl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.hesvh.cn/Article/details/gxcdmdflj.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fehbvm.com/Article/details/ghrbmpkpg.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fehbvm.com/Article/details/gpmivlitd.sHtML

[U19] Py：正则替换带回调
来源：http://3g.zdbjq.cn/Article/details/gcdhzgtma.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fehbvm.com/Article/details/gxesmabfb.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.zdbjq.cn/Article/details/gnzggcrdb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/gyqdaqfti.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/gilmswyhj.sHtML

@contextlib.contextmanager
来源：http://www.m.share.zdbjq.cn/Article/details/gtgejqdtt.sHtML

[U22] Py：矩阵转置
来源：http://3g.zdbjq.cn/Article/details/ghduwljev.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/gusrpjrac.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/gtsdhwutb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.zdbjq.cn/Article/details/gdlkuegkm.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/gtbjusugb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gnggrgtsy.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.hesvh.cn/Article/details/gzcdptfnh.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/gcpqupjpr.sHtML

[U26] Py：并发下载
来源：http://blog.zdbjq.cn/Article/details/gnzmxkkok.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.hesvh.cn/Article/details/gtqumrevg.sHtML

[U27] Py：异步 HTTP
来源：http://wap.zdbjq.cn/Article/details/giibrjvqr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fehbvm.com/Article/details/gwlapwxdj.sHtML

[U28] Py：类型别名
来源：http://mobile.hesvh.cn/Article/details/gjodsirif.sHtML

UserId = int
来源：http://mobile.fehbvm.com/Article/details/grzbbmjyp.sHtML

[U29] Py：属性校验
来源：http://baike.zdbjq.cn/Article/details/gvudcxgkf.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fehbvm.com/Article/details/gksmnvyru.sHtML

[U30] Py：数据类
来源：http://wap.zdbjq.cn/Article/details/gjdeiayyv.sHtML

@dataclass(slots=True)
来源：http://m.share.zdbjq.cn/Article/details/gaprfkkgn.sHtML

[U31] Py：单测
来源：http://www.m.share.fehbvm.com/Article/details/gqzsyykwl.sHtML

python -m pytest -q
来源：http://www.blog.zdbjq.cn/Article/details/gjgxhjcjn.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/gqgtilsuh.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/ghnmkoqih.sHtML

[U33] Py：打包发布
来源：http://www.share.fehbvm.com/Article/details/gpovjlefu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.zdbjq.cn/Article/details/gcdqzqdkb.sHtML

[U34] Py：判断编码
来源：http://read.share.zdbjq.cn/Article/details/ghxgflsmf.sHtML

chardet.detect(raw)
来源：http://blog.fehbvm.com/Article/details/gpgwutser.sHtML

[U35] Py：发送邮件
来源：http://www.share.fehbvm.com/Article/details/gwebrcwti.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.zdbjq.cn/Article/details/gfqtqxraq.sHtML

[U36] Py：定时任务
来源：http://www.share.fehbvm.com/Article/details/gpfqsrlmi.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/gbqqivttu.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fehbvm.com/Article/details/gmgjpgdvv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fehbvm.com/Article/details/gmvhncxvp.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.zdbjq.cn/Article/details/ghkgnhswt.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/gzuyupsdx.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.zdbjq.cn/Article/details/gtirooxpr.sHtML

sys.stdout.isatty()
来源：http://m.share.zdbjq.cn/Article/details/gbbhufrco.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.hesvh.cn/Article/details/gaqvvvhpx.sHtML

print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/ggkqfjtgn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.hesvh.cn/Article/details/gyrmobjqb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fehbvm.com/Article/details/gtlwhhbcb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.zdbjq.cn/Article/details/gyyuurnlx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.hesvh.cn/Article/details/gekwedpnx.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.hesvh.cn/Article/details/ghkoxqmld.sHtML

namespace App\Http;
来源：http://wap.hesvh.cn/Article/details/gqevbsyev.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/ghrhtlhyi.sHtML

declare(strict_types=1);
来源：http://www.blog.fehbvm.com/Article/details/gxkyhojux.sHtML


<!-- 参考信息 -->