代发 wailian999

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gdkaacunk.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/grfuuwggp.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gqsysdzqt.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/gwfbzhvnz.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/gmrtgwkzy.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/gyzuymqij.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gqvqwdnja.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/ghaifnqsu.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/gisyglapa.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/ghfxnzbib.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/goavoxqgr.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gjrtbgznb.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gmpyqzyam.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fehbvm.com/Article/details/glswaayxi.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/geqrqoldj.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/gqvejptwu.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gjhotickk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gwjxlarvw.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gpscvqgqh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/gxfiwjgfy.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/gjtzuaqsq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/ganengura.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/gyvfgmnqp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/grqrtfego.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/gupynkxoq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gnixmrfsq.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gmfbiirzn.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gqqcciezw.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/gdopawydt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/gtbjfovoj.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gsmuitmum.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gpuyetfuo.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gqxdavapd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/gcvlemboc.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/gbkeocfeo.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gueumawxm.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gfcqnuriw.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/gpudkeycz.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/gkocdkgyb.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/gmgtwmybg.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/gjmxpovjg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/gusamwxjt.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gyxiupllm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/grlmufaew.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/gmhmisbda.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.zdbjq.cn/Article/details/gdnohweid.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gcovohxxa.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gbhacptwj.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/goqysnlwg.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/guodnrlys.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/gahconydp.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gwgjerwsn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/ghniklxdi.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gvbsbcxfg.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/gbqyphzrf.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/goevhpkgy.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/gejtgykdq.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/grgghiivj.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/gnwwurmki.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gpqkcfxvd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gkzruhavc.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/gtpdubyun.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gkqghkovi.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gcjqxpjyb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/gffyytlod.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/gbiftkczi.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/giozcwfcl.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gxlyyoybq.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/ganmbwkts.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/guswhuwnb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/gqppatbql.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gsbmeuhjw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/ghgkiiokl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gedofdbsm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gzohzlpgz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gamynotqy.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gnslixrie.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gjwujryfw.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/ghjezztgm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.hesvh.cn/Article/details/gkcfywqtu.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.hesvh.cn/Article/details/gmdvtvrao.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/geaivbvio.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gonxudzeh.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/gyerxddji.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/grfkvnfqu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/gjotbcoan.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gufxuhzol.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gtkdfvbex.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gobztrvoq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/gnigiirfk.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/ggxxqrdoi.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/gwbymeuea.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gusqfznrg.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/gpezjlvfp.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/gshjqifoc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/grglotgjx.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/gvlctmkys.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/grebnegso.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/genofdapq.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gvklrgfjf.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.hesvh.cn/Article/details/gkdkfzhkh.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/gthdtbfhm.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gxqysknjj.sHtML

for (i in 1..10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gicencoyu.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/gvajvdzag.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/gbqamyqpq.sHtML

[T16] Swift：Hello World
来源：http://baike.zdbjq.cn/Article/details/gumbbdjtz.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gsdhhfxmc.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gmdqpzmox.sHtML

var a = 1;  let b = 2
来源：http://read.share.hesvh.cn/Article/details/gtsaigzws.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gflpholpd.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/grpblbuid.sHtML

[T19] Swift：可选绑定
来源：http://baike.fehbvm.com/Article/details/gbdqazlim.sHtML

if let n = opt { print(n) }
来源：http://www.share.hesvh.cn/Article/details/ggjslbzto.sHtML

[T20] Swift：数组操作
来源：http://baike.zdbjq.cn/Article/details/gagxxnxhc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/gdibturza.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/gltmticqi.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gulrcubdh.sHtML

[T22] Swift：字典
来源：http://read.share.fehbvm.com/Article/details/gjpeylere.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.zdbjq.cn/Article/details/gojknpawi.sHtML

[T23] Swift：函数
来源：http://3g.hesvh.cn/Article/details/gxvupnekt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/grysfzkao.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/gfvlphius.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gdphvyqnu.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/gpqshophu.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/gbrkehtdf.sHtML

[T26] Swift：类与重写
来源：http://blog.hesvh.cn/Article/details/gjzxnkwbi.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/gbqnhbmiy.sHtML

[T27] Swift：错误处理
来源：http://mobile.hesvh.cn/Article/details/gsmrlfrep.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/grlznrrye.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/ghnzlvkyy.sHtML

enum Color { case red, green }
来源：http://m.share.hesvh.cn/Article/details/gcdvpipkr.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/giktoawfl.sHtML

guard let x = opt else { return }
来源：http://baike.hesvh.cn/Article/details/gvrmpiipx.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/gvebwpolk.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gxfwnbfon.sHtML

[T31] Lua：Hello World
来源：http://3g.hesvh.cn/Article/details/gmlqhpqrl.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gxqdcmxxs.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gxoulryng.sHtML

local a = 1
来源：http://3g.zdbjq.cn/Article/details/gdtjcrcms.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fehbvm.com/Article/details/gaccyascu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/gywjppdcu.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/gbpkcguon.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.hesvh.cn/Article/details/gjpvuetwy.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/gadqistdw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/gcslezbmo.sHtML

[T36] Lua：函数
来源：http://baike.zdbjq.cn/Article/details/gceuoliwb.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/gttyofguo.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gedasrxyv.sHtML

"a" .. "b"
来源：http://read.share.zdbjq.cn/Article/details/gkbtwavbc.sHtML

[T38] Lua：条件
来源：http://wap.hesvh.cn/Article/details/guqgbrdnd.sHtML

if x > 0 then print("正") end
来源：http://m.share.fehbvm.com/Article/details/gnfkspnnw.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gngszzsnp.sHtML

string.find(s, "%d+")
来源：http://baike.zdbjq.cn/Article/details/glqwfdzny.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/gasmlwkfx.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fehbvm.com/Article/details/grwwdeiow.sHtML

[T41] Perl：Hello World
来源：http://3g.hesvh.cn/Article/details/glcarnmpk.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/gjvoyitsa.sHtML

[T42] Perl：变量类型
来源：http://baike.hesvh.cn/Article/details/gahwmljbm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fehbvm.com/Article/details/gzvtnyjqq.sHtML

[T43] Perl：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gqfwwfjzq.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/gwytpimwv.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/gnaqbiklz.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.zdbjq.cn/Article/details/gpjzxrtvq.sHtML

[T45] Perl：数组遍历
来源：http://read.share.hesvh.cn/Article/details/gfnnnhxkn.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.zdbjq.cn/Article/details/gdbsnegis.sHtML

[T46] Perl：哈希操作
来源：http://mobile.zdbjq.cn/Article/details/gbitkdhch.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.hesvh.cn/Article/details/gzwanwyun.sHtML

[T47] Perl：正则捕获
来源：http://mobile.zdbjq.cn/Article/details/gzcctbzcl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.zdbjq.cn/Article/details/gxhyytcoj.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/gznqmscpu.sHtML

$s =~ s/old/new/g;
来源：http://www.share.zdbjq.cn/Article/details/gjogbxzlm.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/gzygfxgug.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/glurwrjwu.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gaawbnpzd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/gyvxwdscg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fehbvm.com/Article/details/gcdggjofn.sHtML

[T51] Scala：Hello World
来源：http://wap.hesvh.cn/Article/details/glhutsgdf.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gnwanyalb.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/goujrwfyw.sHtML

val a = 1;  var b = 2
来源：http://mobile.hesvh.cn/Article/details/gqkaagzbh.sHtML

[T53] Scala：字符串插值
来源：http://baike.fehbvm.com/Article/details/gnbudeuzq.sHtML

s"值: $b"
来源：http://baike.hesvh.cn/Article/details/gcxbaxydl.sHtML

[T54] Scala：集合映射
来源：http://mobile.hesvh.cn/Article/details/gmikqqhkr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.hesvh.cn/Article/details/grpohxjdr.sHtML

[T55] Scala：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gxoyjnnej.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.zdbjq.cn/Article/details/gnnrakksg.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/gxwgxrrpv.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/gfssjtmkh.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gnlxsywri.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.zdbjq.cn/Article/details/ggbiagjvw.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/gfzkwmkcn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.hesvh.cn/Article/details/gvvpqyvrv.sHtML

[T59] Scala：循环
来源：http://blog.fehbvm.com/Article/details/grnvprtug.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/ggrscoweg.sHtML

[T60] Scala：折叠
来源：http://www.blog.fehbvm.com/Article/details/gfqfqfjgi.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fehbvm.com/Article/details/gptuztwzi.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkqlcldvz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gqkxlsupf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxmmdxzmj.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.hesvh.cn/Article/details/geiqqmkjm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/gvhtljqrd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.hesvh.cn/Article/details/grqycxmqm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.hesvh.cn/Article/details/gtsyiaqwh.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/gbjpqvktx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.zdbjq.cn/Article/details/gtoqvceee.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fehbvm.com/Article/details/gkjkhrrdf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gpxepxumf.sHtML

[U05] Py：列表去重且保序
来源：http://baike.zdbjq.cn/Article/details/gyczssylx.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gkxygatym.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/glviltshm.sHtML

{**a, **b}
来源：http://baike.fehbvm.com/Article/details/gaffljbes.sHtML

[U07] Py：反转字典键值
来源：http://m.share.zdbjq.cn/Article/details/gikmsnyez.sHtML

{v: k for k, v in d.items()}
来源：http://baike.zdbjq.cn/Article/details/gbypgorgd.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/gxxlbarwr.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/gmahzoqlm.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fehbvm.com/Article/details/gxwxbcjkr.sHtML

max(d, key=d.get)
来源：http://baike.zdbjq.cn/Article/details/gozkswske.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fehbvm.com/Article/details/gptuzndvv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.zdbjq.cn/Article/details/gbxhfuzlk.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/gvqsuarnk.sHtML

(x * 2 for x in arr)
来源：http://baike.hesvh.cn/Article/details/gdgxatoad.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/gjterrigm.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/gszdklzgw.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.hesvh.cn/Article/details/gbwcxdzsv.sHtML

deque(maxlen=10)
来源：http://3g.hesvh.cn/Article/details/gecmdzuih.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/gkbalxtqa.sHtML

defaultdict(list)
来源：http://www.share.fehbvm.com/Article/details/gseqbjewa.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fehbvm.com/Article/details/gmqispees.sHtML

t = time.perf_counter()
来源：http://m.share.fehbvm.com/Article/details/ggviayuzb.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.zdbjq.cn/Article/details/gkmyuxval.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.hesvh.cn/Article/details/gwzdxdqxk.sHtML

[U17] Py：初始化日志
来源：http://wap.fehbvm.com/Article/details/goidbnurc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fehbvm.com/Article/details/gqdwmjtbb.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/gebqzxsjq.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.hesvh.cn/Article/details/gasdxdjrz.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/genkgabze.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fehbvm.com/Article/details/gjhoaatme.sHtML

[U20] Py：缓存函数结果
来源：http://baike.hesvh.cn/Article/details/gbaswdfnt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fehbvm.com/Article/details/gdwulqqbs.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fehbvm.com/Article/details/gkuvywocg.sHtML

@contextlib.contextmanager
来源：http://blog.hesvh.cn/Article/details/gtsgbkzco.sHtML

[U22] Py：矩阵转置
来源：http://mobile.zdbjq.cn/Article/details/gchrcpyox.sHtML

list(zip(*m))
来源：http://mobile.zdbjq.cn/Article/details/gtgihmdqg.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fehbvm.com/Article/details/gazcpdlgr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/gojoytqgi.sHtML

[U24] Py：路径操作
来源：http://wap.zdbjq.cn/Article/details/gpxjuwawt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gvqzmhokt.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/glfinuxsa.sHtML

csv.DictReader(f)
来源：http://baike.fehbvm.com/Article/details/gtsjgyobs.sHtML

[U26] Py：并发下载
来源：http://baike.fehbvm.com/Article/details/gxfhalyje.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.zdbjq.cn/Article/details/ghfvwevml.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fehbvm.com/Article/details/gbqtoporo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.zdbjq.cn/Article/details/gtwehfrrr.sHtML

[U28] Py：类型别名
来源：http://wap.fehbvm.com/Article/details/gvpiblhax.sHtML

UserId = int
来源：http://read.share.hesvh.cn/Article/details/grrngxlgx.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fehbvm.com/Article/details/ggvkpdjpl.sHtML

@property 与 @x.setter 配合
来源：http://m.share.hesvh.cn/Article/details/gmrbwsken.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gaahbegtt.sHtML

@dataclass(slots=True)
来源：http://3g.hesvh.cn/Article/details/gddknzugr.sHtML

[U31] Py：单测
来源：http://m.share.zdbjq.cn/Article/details/gnccdaimi.sHtML

python -m pytest -q
来源：http://3g.zdbjq.cn/Article/details/guyexsrhn.sHtML

[U32] Py：代码格式化
来源：http://baike.fehbvm.com/Article/details/grwdevscs.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/gasazvifp.sHtML

[U33] Py：打包发布
来源：http://blog.zdbjq.cn/Article/details/gwdzyizhk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gnbwmdsxj.sHtML

[U34] Py：判断编码
来源：http://www.m.share.zdbjq.cn/Article/details/gkemuhgfd.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/glqktnhls.sHtML

[U35] Py：发送邮件
来源：http://mobile.fehbvm.com/Article/details/glvzudhdp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.hesvh.cn/Article/details/gxqntwvmq.sHtML

[U36] Py：定时任务
来源：http://wap.hesvh.cn/Article/details/gmgzumnjx.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/grfkteyyv.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fehbvm.com/Article/details/gabxjncxd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fehbvm.com/Article/details/gaomoldqe.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.zdbjq.cn/Article/details/grouccinq.sHtML

Path(__file__).resolve().parent
来源：http://mobile.zdbjq.cn/Article/details/ghkkeerrg.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.zdbjq.cn/Article/details/gltqdispb.sHtML

sys.stdout.isatty()
来源：http://mobile.fehbvm.com/Article/details/gfafgecct.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.zdbjq.cn/Article/details/gltyyszob.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/ghkigftwx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/gmmsbeajk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.hesvh.cn/Article/details/gxqheulib.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.hesvh.cn/Article/details/gpwkidiau.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fehbvm.com/Article/details/gpeawlouu.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.zdbjq.cn/Article/details/gmewfotuz.sHtML

namespace App\Http;
来源：http://read.share.hesvh.cn/Article/details/gmyzrxjeu.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.hesvh.cn/Article/details/gwxomamug.sHtML

declare(strict_types=1);
来源：http://read.share.zdbjq.cn/Article/details/ggykpoesv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.hesvh.cn/Article/details/gtxhnfaia.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gzprtmvir.sHtML

[U46] PHP：可空类型
来源：http://read.share.fehbvm.com/Article/details/gjqpfcwfj.sHtML

?string $name = null
来源：http://www.m.share.fehbvm.com/Article/details/gnszxrknp.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.hesvh.cn/Article/details/gkupkusbp.sHtML

int|string $id
来源：http://baike.hesvh.cn/Article/details/gqagzaqsc.sHtML

[U48] PHP：纯枚举
来源：http://3g.hesvh.cn/Article/details/ghthqoszg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.hesvh.cn/Article/details/giekxsjny.sHtML

[U49] PHP：只读属性
来源：http://wap.fehbvm.com/Article/details/gpdqflqaz.sHtML

public readonly string $name
来源：http://mobile.fehbvm.com/Article/details/gfbhvtrwp.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.hesvh.cn/Article/details/gsgvfassh.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/gmiwtpkcw.sHtML


<!-- 参考信息 -->