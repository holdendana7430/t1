代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/gkjcjpatz.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gtgzxqvsl.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/gsggyfrtm.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gbmvlbyme.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gddithpwp.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gqajampgz.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/ggwcrtolu.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gbucephjo.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/gutgfmpgy.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/gtelcxzzr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/gsepjhfbd.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gokzuznng.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/ghizjrrba.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/glgydoecg.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/gcdlozqfx.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gcgvnzjjd.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gokdihixf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/goiinqcml.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/gcaapzakr.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gskwybqei.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gwbyrbyde.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/gxnltdvjq.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/gizrgghys.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gcgzvosjt.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gkbcarcpz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gnqzkjrsk.sHtML

[S36] C++：unordered_map
来源：http://wap.fehbvm.com/Article/details/gwkjenwxd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gpkfxbyhh.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/gjwonoxce.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gpwvhyqky.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gfifykwef.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gcyxscsbx.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gwnieanzi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gaesgrcik.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gxxddgtzo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/gjapwfslj.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/giaeqayzq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gcpkbvzot.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/gpdralbvk.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gsqjwcuja.sHtML

[S43] C++：智能指针
来源：http://blog.fehbvm.com/Article/details/gmofkkqge.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gvczztfpi.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gfmamurpa.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/ggqrlkljg.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/glwhaartg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gedtifzov.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/gxpyeqdho.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/ghvscygcb.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/grxozwlnp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gqdatiydz.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gjxmbxoac.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/gtbatruxl.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/ghsgjfvyi.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/gkfhswacs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/gxwmqyuvb.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/gnwvpmusc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gusorwejm.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gujjwktcx.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/grcrnbmsu.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gdypctrxc.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gmrzxnqtk.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gnbofawmc.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gqzdusono.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/gghncehsq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/gybmsfnes.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/gzhtpdxex.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/gcuvfzyju.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/gytpeaebj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/godybgdgn.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/gyrwvlmjy.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gzmrlxjru.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gcwdtaumb.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gpyohvuuo.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gzbvzbtpj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/grjmfyvue.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/geoqwufon.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gvoytmjij.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gobwxnyws.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/ggcgbffor.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggzpguxul.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gswzzsmas.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gfujxjnyp.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/garnxfloe.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/gtkyllyvr.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/gzwmdbbxb.sHtML

"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gtyffdraf.sHtML

[T04] Kotlin：空安全
来源：http://baike.zdbjq.cn/Article/details/gttwdihdi.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gdijdsiac.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/guzedkafa.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/guwvpxdwn.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gopaiwlin.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/gscktubfs.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/glkvhauxq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/glvghhavh.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/gmiugiamp.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gddcyhoxx.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/gdzuqppgv.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gxbltzbaj.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/gakvatihl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/gwjeewbpq.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/gxwmmzsva.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gleaxqoau.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gofabdpee.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gwqsejdxx.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.zdbjq.cn/Article/details/gfecvgvvf.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.hesvh.cn/Article/details/gvydexzwi.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/gstngtfii.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gfvgxklgb.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/gylhujeik.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gentpdpcv.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gocecppcv.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gkixiusrs.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gblkobijd.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/gbzghasoa.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/golahzbcp.sHtML

"值: \(b)"
来源：http://wap.fehbvm.com/Article/details/gaeahkbcm.sHtML

[T19] Swift：可选绑定
来源：http://blog.hesvh.cn/Article/details/gwubfeoal.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/gwqpjphfo.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/ggzlbmgfz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/gkinfqmhv.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/giizuhxzu.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/gpsasgihe.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gflktpokl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/gbtnwiacp.sHtML

[T23] Swift：函数
来源：http://blog.fehbvm.com/Article/details/glipssuye.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gwsjnixri.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/gwsvlmxwv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gfaaiebsq.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/gsndnbdab.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gqriedyei.sHtML

[T26] Swift：类与重写
来源：http://www.blog.hesvh.cn/Article/details/gyzqoilvh.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/gyqgosvbk.sHtML

[T27] Swift：错误处理
来源：http://m.share.fehbvm.com/Article/details/govgeinww.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/gabbhaoth.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/gifuurvvx.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/gljkjnlkg.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.hesvh.cn/Article/details/grpkbeykw.sHtML

guard let x = opt else { return }
来源：http://m.share.zdbjq.cn/Article/details/gomzcndam.sHtML

[T30] Swift：协议
来源：http://mobile.hesvh.cn/Article/details/gonncewre.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.hesvh.cn/Article/details/gvynfhqba.sHtML

[T31] Lua：Hello World
来源：http://blog.zdbjq.cn/Article/details/gofwdwmrg.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gohgkhquq.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/grudcrpfo.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/gngsbsxbm.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/gosvwhhcc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.zdbjq.cn/Article/details/gjdkqflhc.sHtML

[T34] Lua：遍历表
来源：http://3g.hesvh.cn/Article/details/gatajjulg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.zdbjq.cn/Article/details/grzlzyzow.sHtML

[T35] Lua：字典表
来源：http://www.blog.hesvh.cn/Article/details/gnwycfvao.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.zdbjq.cn/Article/details/gmbvmsfbp.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/gfnuxjvyb.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/gejuinepx.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gxoffvkze.sHtML

"a" .. "b"
来源：http://m.share.hesvh.cn/Article/details/gbstzcsse.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/gikmginkb.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/gsszbskvm.sHtML

[T39] Lua：模式匹配
来源：http://baike.hesvh.cn/Article/details/gmgmfatdj.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/gqmwdcydy.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/gbpfzxdwy.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/ggxulnyoa.sHtML

[T41] Perl：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gvqoptayr.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/gxpcxhpvb.sHtML

[T42] Perl：变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gzgdxhaub.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.zdbjq.cn/Article/details/gyuuxlmfx.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gtnewbrok.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/gbvshtgnp.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/gjstleclj.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/gpdkwuead.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/gygbyndgm.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.zdbjq.cn/Article/details/gjqcgvpcb.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/glcluxnwj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fehbvm.com/Article/details/gyihzfgky.sHtML

[T47] Perl：正则捕获
来源：http://mobile.zdbjq.cn/Article/details/guzmyctuo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/gqrrdelxp.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/gushpcuue.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fehbvm.com/Article/details/gjvettwuq.sHtML

[T49] Perl：函数
来源：http://mobile.hesvh.cn/Article/details/ghpjqzhwf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gydhkpikj.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gsijrdhnp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.zdbjq.cn/Article/details/gdxllbrou.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fehbvm.com/Article/details/gadclaqru.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gsfutprdo.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gifjhugbr.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/gogrlruvq.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/gdshloals.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/grapqwsmv.sHtML

s"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gjhurjeeu.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/gwfafnldx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.hesvh.cn/Article/details/glqmghjrr.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gpqnincbf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/gdpleymzw.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/gotuavpum.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gjkaubgts.sHtML

[T57] Scala：模式匹配
来源：http://wap.fehbvm.com/Article/details/gcpsitizw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fehbvm.com/Article/details/gfesdomat.sHtML

[T58] Scala：函数定义
来源：http://3g.zdbjq.cn/Article/details/gxsytwjhb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.hesvh.cn/Article/details/gimnplieo.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/gqgpjcdzg.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gwcguerqe.sHtML

[T60] Scala：折叠
来源：http://blog.zdbjq.cn/Article/details/grsmkysbq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/gzoteamig.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjagcnhbt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gcxxlkdxo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gexjrbybq.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/glrigenfm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.zdbjq.cn/Article/details/gpxvjwvmt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.zdbjq.cn/Article/details/ghgoszciz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/gzcpkyxgn.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.hesvh.cn/Article/details/gtnrhpfmz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fehbvm.com/Article/details/gaiwxddhx.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/givestqoq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gustelhpo.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/gvdrxohqp.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gccfkeenp.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.hesvh.cn/Article/details/gxabatlfx.sHtML

{**a, **b}
来源：http://www.share.hesvh.cn/Article/details/gaifwzkgt.sHtML

[U07] Py：反转字典键值
来源：http://3g.zdbjq.cn/Article/details/gnrunprlo.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fehbvm.com/Article/details/geijrfwop.sHtML

[U08] Py：展平二维列表
来源：http://mobile.hesvh.cn/Article/details/grahyuywa.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gfnbyvfrq.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.zdbjq.cn/Article/details/gqgdsxied.sHtML

max(d, key=d.get)
来源：http://www.blog.fehbvm.com/Article/details/gzfpfrhoh.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.hesvh.cn/Article/details/ghopuemfb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.zdbjq.cn/Article/details/gattrjbmc.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/gctwrrkbg.sHtML

(x * 2 for x in arr)
来源：http://3g.fehbvm.com/Article/details/gvldaquoc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.zdbjq.cn/Article/details/gcgsvgbwf.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/grzxvhdfc.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/gbkmwnhns.sHtML

deque(maxlen=10)
来源：http://blog.zdbjq.cn/Article/details/gxtkojwby.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/gmcmshwph.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/gmciwxjll.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gfepvashy.sHtML

t = time.perf_counter()
来源：http://mobile.fehbvm.com/Article/details/gpsabymuf.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/glsagdqej.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.hesvh.cn/Article/details/gvihlaiuf.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/gxnwcrzrc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.hesvh.cn/Article/details/gmpxmcrvy.sHtML

[U18] Py：预编译正则
来源：http://baike.hesvh.cn/Article/details/gitymngov.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.hesvh.cn/Article/details/gtsunnokz.sHtML

[U19] Py：正则替换带回调
来源：http://3g.zdbjq.cn/Article/details/gothxrsfn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/ggqgvdkby.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.hesvh.cn/Article/details/gyizhtzsv.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.hesvh.cn/Article/details/gkqtczlec.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fehbvm.com/Article/details/gxnhjcwza.sHtML

@contextlib.contextmanager
来源：http://www.share.zdbjq.cn/Article/details/gtytlkwly.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fehbvm.com/Article/details/gqcsaulpt.sHtML

list(zip(*m))
来源：http://www.share.hesvh.cn/Article/details/gyybkslrc.sHtML

[U23] Py：分块读取大文件
来源：http://baike.zdbjq.cn/Article/details/gokezpwrm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.zdbjq.cn/Article/details/gvieifwdy.sHtML

[U24] Py：路径操作
来源：http://mobile.hesvh.cn/Article/details/ghrdnbcqa.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gzfuliulu.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.zdbjq.cn/Article/details/gwxlojfrq.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/gomfflkhd.sHtML

[U26] Py：并发下载
来源：http://wap.hesvh.cn/Article/details/gmdahgeqy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.zdbjq.cn/Article/details/glyxuenzw.sHtML

[U27] Py：异步 HTTP
来源：http://baike.hesvh.cn/Article/details/gfknvsguk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fehbvm.com/Article/details/gldplrkww.sHtML

[U28] Py：类型别名
来源：http://mobile.hesvh.cn/Article/details/ghnhfzzly.sHtML

UserId = int
来源：http://www.blog.hesvh.cn/Article/details/gbcurhtzj.sHtML

[U29] Py：属性校验
来源：http://m.share.zdbjq.cn/Article/details/guefazohl.sHtML

@property 与 @x.setter 配合
来源：http://3g.hesvh.cn/Article/details/gpqyfaaxx.sHtML

[U30] Py：数据类
来源：http://www.share.zdbjq.cn/Article/details/garbgibqf.sHtML

@dataclass(slots=True)
来源：http://www.m.share.zdbjq.cn/Article/details/ggnsznvml.sHtML

[U31] Py：单测
来源：http://baike.hesvh.cn/Article/details/gtgkhzmdp.sHtML

python -m pytest -q
来源：http://mobile.zdbjq.cn/Article/details/gqsovhqfu.sHtML

[U32] Py：代码格式化
来源：http://read.share.hesvh.cn/Article/details/gfjzjamxd.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.zdbjq.cn/Article/details/gpseyktsd.sHtML

[U33] Py：打包发布
来源：http://read.share.zdbjq.cn/Article/details/gkeedodss.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/glsmmlbzx.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/gdlpriqsz.sHtML

chardet.detect(raw)
来源：http://mobile.zdbjq.cn/Article/details/gltysksec.sHtML

[U35] Py：发送邮件
来源：http://www.blog.zdbjq.cn/Article/details/gnirhhxfz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/gpkabnxxc.sHtML

[U36] Py：定时任务
来源：http://3g.fehbvm.com/Article/details/gnggluyjx.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.hesvh.cn/Article/details/gvwycbkry.sHtML

[U37] Py：读写 Excel
来源：http://read.share.hesvh.cn/Article/details/guanwrcmi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gypuziaul.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.hesvh.cn/Article/details/glbdkrrpg.sHtML

Path(__file__).resolve().parent
来源：http://m.share.zdbjq.cn/Article/details/gkqukukuj.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fehbvm.com/Article/details/gjlojhquy.sHtML

sys.stdout.isatty()
来源：http://mobile.hesvh.cn/Article/details/guuqswepe.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/gjvutjqlw.sHtML

print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/goocpaifk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fehbvm.com/Article/details/gzrcsthne.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.zdbjq.cn/Article/details/gkogkfdma.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/gjuetblog.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.zdbjq.cn/Article/details/ggavyvdgg.sHtML

[U43] PHP：声明命名空间
来源：http://3g.hesvh.cn/Article/details/gvhokkgyp.sHtML

namespace App\Http;
来源：http://www.blog.zdbjq.cn/Article/details/gglntddnw.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fehbvm.com/Article/details/gemgoddqg.sHtML

declare(strict_types=1);
来源：http://read.share.fehbvm.com/Article/details/gtllvpkzy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.hesvh.cn/Article/details/gotkwmusj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gshfaqwgd.sHtML

[U46] PHP：可空类型
来源：http://blog.hesvh.cn/Article/details/gndmkqmsm.sHtML

?string $name = null
来源：http://m.share.hesvh.cn/Article/details/gcdkgiydp.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/gtbrddvhn.sHtML

int|string $id
来源：http://www.m.share.fehbvm.com/Article/details/gfcayueer.sHtML

[U48] PHP：纯枚举
来源：http://blog.fehbvm.com/Article/details/gfouxwxsl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fehbvm.com/Article/details/glxhlkqmg.sHtML


<!-- 参考信息 -->