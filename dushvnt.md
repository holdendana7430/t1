代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/gwifyzisn.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/giztdwkwq.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/gzsyumggo.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gheenvlbj.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gqwjwgrzu.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/gfzvpnyec.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/ggyliejgr.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/gpdflttjw.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gxmvbaasm.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gvonomsdv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/gdjiabsxu.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gqofsbyyl.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/ganqklnjs.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gnvkzvfib.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/gjaoxakbk.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gvgkkktlw.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/ghmnkffoz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gjhuxzqsm.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gvsbgnfym.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gzpkimvcy.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/gjofjjotx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/gzafmeseb.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gylzcgjsi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gcujdjujp.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gewbsoult.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gtcoqnbvf.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/ggxfbxpaf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gosvuqiwj.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/gblmdvmzi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gtyeavpiy.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gfhjtiscb.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gyjdixfcr.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/gvcbhwbsu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gcgutfpvn.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/germxtezh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/gnexmxzzb.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gyufpeoqh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/guoawzsic.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/gydceatwm.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/grugofhgr.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/gotlxykyt.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/grgzwisuq.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gyiccfjli.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/grbrabutx.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gcefflsbb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/gdjikhsas.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/gdkfqxffw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gjjaqwtny.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/goerbannw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/grrfvxehh.sHtML

[S48] C++：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gvcwgvetn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/gwabqapxx.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gvcecejiw.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gytovhzak.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.hesvh.cn/Article/details/glkgnibok.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gcpsvhpbl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gnpwgsiwh.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/gceikugsq.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/gkvhvgywu.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/gqfulqtqi.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/gdedgikbe.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/giinvvysc.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gaizaoudl.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gwaldztdl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/gzyunlayh.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/ghzyncjor.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/glzmijwxi.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gmiudnnnw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gnqgbdaph.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gyvyrsokc.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gbjblbpxb.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gfnpyzeie.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gkbhepggm.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gyvkhgwkr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/gycwxxdqb.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/guuvervxh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gzlnvlfcv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggdnmthbc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gjuksbvuv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gipgadfbo.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/grccsxhkj.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/grwhfmosm.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/gvbgbufki.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/gocsekydt.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/grcfhgpvf.sHtML

"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gamkqwxfw.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gzbcbuswd.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/glgojpyxo.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/gxhybamaj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gemcgremp.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fehbvm.com/Article/details/gjvmkjzhs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gjmexpfaq.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gorqxpkgl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/gydnsbspj.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gzvsybkhm.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/goanuciie.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gwxmihoky.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/ghfbwgxdu.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/ghzcppkra.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fehbvm.com/Article/details/gzanqmqxz.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gwzzxpnpq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gtblxqjsw.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/gnrgxlqiq.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gefivagmd.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.zdbjq.cn/Article/details/gylovpnzh.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/gvcoizuyw.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/gnblquqmn.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gyzkskgqy.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/gwcmexjfy.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gtohpztbk.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/geazihmqg.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gybehopms.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/glfgjssci.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/gnbjvgpcy.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gwhvxolds.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/ghdsoacik.sHtML

[T19] Swift：可选绑定
来源：http://baike.fehbvm.com/Article/details/gwcskremx.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gxwraeijm.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/gtjkaujdq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/ggaupuweg.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/glfupdvem.sHtML

for x in a { print(x) }
来源：http://wap.hesvh.cn/Article/details/glkzvvdlt.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gexacfjoq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/gihjumykz.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/gstrjjqfh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gxmmxhoob.sHtML

[T24] Swift：闭包
来源：http://m.share.fehbvm.com/Article/details/gynojnejm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gzcbblrbj.sHtML

[T25] Swift：结构体
来源：http://www.m.share.zdbjq.cn/Article/details/geqnceqkm.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/gkwihzgav.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gkohlurhq.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/gzcrryupm.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/gyezmhwrl.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/gsfdmjjaz.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gtqzlwlfr.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/gsuapdlxa.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fehbvm.com/Article/details/grbpookcs.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/gsmpxifru.sHtML

[T30] Swift：协议
来源：http://mobile.hesvh.cn/Article/details/ggjyhlsba.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gxrjqhkeg.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gkimpzalf.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gfwvqvqec.sHtML

[T32] Lua：局部变量
来源：http://blog.hesvh.cn/Article/details/grxylnzrj.sHtML

local a = 1
来源：http://read.share.zdbjq.cn/Article/details/gchtjpsmg.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/gvxqyufuz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/gxooehcbg.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/gqhjhldtv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/getnwdeeo.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gohfumfwn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/gqfcdwebj.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/ghkyyvenu.sHtML

function add(a, b) return a + b end
来源：http://baike.hesvh.cn/Article/details/gguyicymd.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gyoxtiuiy.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/glehzzlmm.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/gealofwjd.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/gldfyznsi.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gqqoawllx.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/gqbciuycw.sHtML

[T40] Lua：元表
来源：http://baike.fehbvm.com/Article/details/gydbzghuh.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fehbvm.com/Article/details/ggeavlfdu.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gznliiaub.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/gmbgozusc.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gmvjdiqpw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/gctfpfcew.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/goqeshwkh.sHtML

"值: $a"
来源：http://baike.fehbvm.com/Article/details/gywyanank.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/gwlxjtsrn.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/gcvybisrv.sHtML

[T45] Perl：数组遍历
来源：http://wap.zdbjq.cn/Article/details/guinrxyls.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/gqunyfbun.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/gurbjrlqr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/gdbicbsxg.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/gldxveelk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/gqgzosuns.sHtML

[T48] Perl：正则替换
来源：http://baike.hesvh.cn/Article/details/gwvxpwlru.sHtML

$s =~ s/old/new/g;
来源：http://baike.zdbjq.cn/Article/details/gjuqudffk.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gvsfhujqv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gfyqlzorx.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/glysrresn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.zdbjq.cn/Article/details/gbmulbigj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/gllywoslp.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gvonrtpri.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gsghprtuy.sHtML

[T52] Scala：变量
来源：http://read.share.zdbjq.cn/Article/details/gwimwjoal.sHtML

val a = 1;  var b = 2
来源：http://blog.hesvh.cn/Article/details/gjqjikygj.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gttcpqpxq.sHtML

s"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gukmuwwov.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/ggwvpuvch.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gnmirfoxv.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gytpjqgll.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/gryqjikyf.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/gbcueogiy.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gcjqoczlg.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gnuqftdrw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/ghhnqqpgy.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/gcgrtqesj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/gmwwxgmel.sHtML

[T59] Scala：循环
来源：http://blog.fehbvm.com/Article/details/gyzydvpqa.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gktmbtamf.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/gagggomls.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.zdbjq.cn/Article/details/gybmhabeq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbomnfghz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gebnagdhg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxoflhzgy.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/gxkroitbq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/gozushzic.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fehbvm.com/Article/details/grpduwahq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/grnqwjian.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.zdbjq.cn/Article/details/ggzxzattd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.hesvh.cn/Article/details/gdvixdgxs.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.hesvh.cn/Article/details/gltcxjure.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.hesvh.cn/Article/details/gtogfuada.sHtML

[U05] Py：列表去重且保序
来源：http://wap.hesvh.cn/Article/details/gcjgaucwh.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gvruhdqwt.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/ggpsruiuj.sHtML

{**a, **b}
来源：http://blog.hesvh.cn/Article/details/gsbnedkaz.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fehbvm.com/Article/details/gjidmideu.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fehbvm.com/Article/details/gauzdfgxo.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/guesghwth.sHtML

[y for x in nested for y in x]
来源：http://www.share.hesvh.cn/Article/details/gljhpvhpq.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.zdbjq.cn/Article/details/gmumefbwd.sHtML

max(d, key=d.get)
来源：http://read.share.fehbvm.com/Article/details/gpfkpilgm.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/gmrlaoiit.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.hesvh.cn/Article/details/gvrgxgvai.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/gofpsbxbf.sHtML

(x * 2 for x in arr)
来源：http://read.share.zdbjq.cn/Article/details/gmvecvaan.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fehbvm.com/Article/details/guckntikm.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/gxumuxkzq.sHtML

[U13] Py：固定长度队列
来源：http://m.share.hesvh.cn/Article/details/gonemffut.sHtML

deque(maxlen=10)
来源：http://www.share.fehbvm.com/Article/details/grvclqomx.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fehbvm.com/Article/details/gowknubzg.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/gjgiprmse.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/gckebjckc.sHtML

t = time.perf_counter()
来源：http://www.m.share.fehbvm.com/Article/details/gdhnudsta.sHtML

[U16] Py：命令行参数解析
来源：http://blog.hesvh.cn/Article/details/gntovogox.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.zdbjq.cn/Article/details/gngkepete.sHtML

[U17] Py：初始化日志
来源：http://mobile.fehbvm.com/Article/details/gzkqemwgc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fehbvm.com/Article/details/gllkusfgs.sHtML

[U18] Py：预编译正则
来源：http://wap.hesvh.cn/Article/details/gglizoahx.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/guhxxijvj.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.hesvh.cn/Article/details/ghrrmswji.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.hesvh.cn/Article/details/gfzpvgkeu.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fehbvm.com/Article/details/gvdxbfrah.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.zdbjq.cn/Article/details/gnckdirzp.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.hesvh.cn/Article/details/gfzgtzuxv.sHtML

@contextlib.contextmanager
来源：http://www.share.zdbjq.cn/Article/details/gfxgsozca.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fehbvm.com/Article/details/guichitiy.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/gwmactuum.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/gnutcbcya.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/gbaybwqax.sHtML

[U24] Py：路径操作
来源：http://www.share.hesvh.cn/Article/details/gfvxinldb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gnzyybaxu.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.hesvh.cn/Article/details/ghpxsyrkz.sHtML

csv.DictReader(f)
来源：http://mobile.zdbjq.cn/Article/details/gxzmorexx.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/ghnosrmbb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.hesvh.cn/Article/details/ghzejxhkc.sHtML

[U27] Py：异步 HTTP
来源：http://wap.hesvh.cn/Article/details/gzeucrifq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.zdbjq.cn/Article/details/gmuyybedo.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/giruulcyg.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/gbcmpbikl.sHtML

[U29] Py：属性校验
来源：http://3g.hesvh.cn/Article/details/gzcbnldog.sHtML

@property 与 @x.setter 配合
来源：http://3g.zdbjq.cn/Article/details/gasggxept.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/ghhmuujbr.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/giqnmryjw.sHtML

[U31] Py：单测
来源：http://www.blog.zdbjq.cn/Article/details/gpcgtlzyz.sHtML

python -m pytest -q
来源：http://3g.zdbjq.cn/Article/details/gxeonppty.sHtML

[U32] Py：代码格式化
来源：http://mobile.hesvh.cn/Article/details/gqezvhkrc.sHtML

ruff format . && ruff check --fix .
来源：http://blog.hesvh.cn/Article/details/ghloextxv.sHtML

[U33] Py：打包发布
来源：http://mobile.hesvh.cn/Article/details/gpcgvmgqx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.hesvh.cn/Article/details/gtusowtcf.sHtML

[U34] Py：判断编码
来源：http://wap.hesvh.cn/Article/details/gaolblyfg.sHtML

chardet.detect(raw)
来源：http://blog.zdbjq.cn/Article/details/gbohvqdnc.sHtML

[U35] Py：发送邮件
来源：http://read.share.fehbvm.com/Article/details/gthzostue.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fehbvm.com/Article/details/gubptlrjk.sHtML

[U36] Py：定时任务
来源：http://mobile.zdbjq.cn/Article/details/gorluzezy.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fehbvm.com/Article/details/gflhiglfv.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fehbvm.com/Article/details/gimjbisme.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fehbvm.com/Article/details/gvbjkhvtq.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fehbvm.com/Article/details/gzjhhcves.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/gndaqtjph.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/gvbhyqoww.sHtML

sys.stdout.isatty()
来源：http://www.blog.fehbvm.com/Article/details/gfkmhnzgx.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fehbvm.com/Article/details/gvybptinz.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gmqchdfuy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.zdbjq.cn/Article/details/ggdcwlces.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.zdbjq.cn/Article/details/goecahkmu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fehbvm.com/Article/details/guywekvus.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.zdbjq.cn/Article/details/gfwgovyjk.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fehbvm.com/Article/details/gqfthofdh.sHtML

namespace App\Http;
来源：http://read.share.fehbvm.com/Article/details/gvxhgfzsc.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fehbvm.com/Article/details/gvfafahby.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/gwiobqygp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.hesvh.cn/Article/details/gxrhxulag.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/goqvnotif.sHtML

[U46] PHP：可空类型
来源：http://www.share.hesvh.cn/Article/details/gmuxkrxnh.sHtML

?string $name = null
来源：http://www.share.fehbvm.com/Article/details/gyfbfaqgo.sHtML

[U47] PHP：联合类型
来源：http://baike.fehbvm.com/Article/details/gklovfzin.sHtML

int|string $id
来源：http://www.m.share.hesvh.cn/Article/details/gdspemees.sHtML

[U48] PHP：纯枚举
来源：http://3g.fehbvm.com/Article/details/gejamcffo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.hesvh.cn/Article/details/gnjwebjew.sHtML


<!-- 参考信息 -->