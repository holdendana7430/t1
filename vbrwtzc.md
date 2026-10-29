代发 wailian999

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/guflhvdcw.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gcsonsgil.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gtceczonf.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gblsoopzx.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gdljtswew.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/gqfflslmw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/gkrtzbbsp.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/girgrhbso.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/gwakfkhru.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/gsbswtgxk.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/ghspvbhii.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gaqifbrah.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/gvvsjxstg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gjbuknive.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gqqntkhmi.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gqfirpmbm.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/giskrnuga.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/gsgpvdbcu.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/gqojmrxzk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/gdjbmukxs.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/groappskd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gddbrahfi.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gzukqfyal.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gwgzvocxo.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gxqszjufq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gbwlngjcb.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gngkjibse.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gtvhggyyc.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/ghfbczqlh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/gxnevohng.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/gjejxynrb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gbhfzuunq.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gfecfilvg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/gmtmlswmp.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/gforymfrc.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/gzcsmdwxj.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gqmsehhyb.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/glhionrro.sHtML

[S44] C++：引用传参
来源：http://baike.hesvh.cn/Article/details/grftuduyg.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/gourlkhzo.sHtML

[S45] C++：lambda
来源：http://wap.hesvh.cn/Article/details/gxajaoeqo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/getchbrbq.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gqnltdoev.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/goqpbnptv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gnkbcfkki.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/gnhhzuxpn.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gqtensrfz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/gumpsxifk.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gmvkjrzcy.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gsukytjmg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gizorvrib.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gxalcbgaj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/gztyybker.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/gdgwwfgxy.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gwojomaei.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/gdkagpprz.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gwkwahelw.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/gybfwyzkf.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fehbvm.com/Article/details/gpuyrrtjq.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gjywnotrg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/giseleaqq.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/gvealwici.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gljdkebtn.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/ghztkiydn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gkxffbuqm.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gbkfwdqbz.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gnuazsezj.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gysvidbcs.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/gtjozoftj.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gsrknkhfu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/ghjauuwpb.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/gdmqiajjk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/grcjyueic.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpvymiids.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/glpawjlrs.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gynuflbrb.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gpbzlnebz.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gxbrtmbqy.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/ghxjtcvyd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/gamzfalrf.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gymutampt.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/gifbxtqts.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/gsimfcvsu.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/guliojeiu.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gcbujvqos.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/gbxrbhvxc.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/ggosahqqp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/ggadzmxom.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gcpxwmqxm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/glzzgcjup.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/ghncqoqcc.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gtojeugbt.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/gjodyljfs.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/gdghsiddi.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/gaqnvzfiq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.hesvh.cn/Article/details/gghvadlrc.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/ghjounnlg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/gznoynuou.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gemcnpdyg.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fehbvm.com/Article/details/gnfnafwje.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fehbvm.com/Article/details/gdhuohwya.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/gjuytzwna.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gnsuishzl.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/guoxiybag.sHtML

[T15] Kotlin：接口
来源：http://wap.hesvh.cn/Article/details/gokxtmiqp.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gbsdmsupf.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fehbvm.com/Article/details/ggdmetbpo.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gaeqmnssb.sHtML

[T17] Swift：变量与常量
来源：http://baike.hesvh.cn/Article/details/gedsbjggi.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/gzejduauv.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gapagloyo.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gmekhazfe.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gecfvexei.sHtML

if let n = opt { print(n) }
来源：http://mobile.zdbjq.cn/Article/details/gnymnmxts.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/gmqglfavm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.hesvh.cn/Article/details/gazpmqptd.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/giqbykntj.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/gagjgpbjv.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/gimuhxxyi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/genusyvmc.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/gvbxajivw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/grocuwtvt.sHtML

[T24] Swift：闭包
来源：http://blog.hesvh.cn/Article/details/gexanivyy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gmnthmlhx.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/gjwuusbap.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/gsyeduvkv.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gzaknkwyz.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/gicwsztut.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/gabgicjgs.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/gmxvujzdr.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/gtqydrglj.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/ggztnxggf.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/gukgfdeel.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/gtgxxwclv.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/gtuaxgmnd.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.hesvh.cn/Article/details/gvrtoqpnj.sHtML

[T31] Lua：Hello World
来源：http://blog.zdbjq.cn/Article/details/gjbvzljqm.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/girattjrf.sHtML

[T32] Lua：局部变量
来源：http://www.blog.hesvh.cn/Article/details/gkwevuxuo.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gvmakfhyy.sHtML

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/guykwnett.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/geeuhlcwh.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/gxqfiauqi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fehbvm.com/Article/details/goyecruqv.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/gbegbvjwj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/gimdsyfel.sHtML

[T36] Lua：函数
来源：http://www.share.fehbvm.com/Article/details/gqvmnmdea.sHtML

function add(a, b) return a + b end
来源：http://baike.hesvh.cn/Article/details/glhoubqid.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gxnffoqqo.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gtudilxky.sHtML

[T38] Lua：条件
来源：http://mobile.zdbjq.cn/Article/details/grspdgmel.sHtML

if x > 0 then print("正") end
来源：http://mobile.zdbjq.cn/Article/details/gkmvqsjhj.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/gohmugzbr.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/gexmndhqh.sHtML

[T40] Lua：元表
来源：http://www.m.share.fehbvm.com/Article/details/grchafvuk.sHtML

setmetatable({}, { __index = base })
来源：http://wap.zdbjq.cn/Article/details/guwczcklv.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/gvxuhsqui.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/gmvuijweq.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gwjpnjppc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/gukkpfnge.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gejuraqqs.sHtML

"值: $a"
来源：http://read.share.fehbvm.com/Article/details/gwzrouwnv.sHtML

[T44] Perl：条件
来源：http://www.m.share.zdbjq.cn/Article/details/glxwtixcu.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.zdbjq.cn/Article/details/gbrhopuhi.sHtML

[T45] Perl：数组遍历
来源：http://read.share.hesvh.cn/Article/details/gchqhjcvn.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.zdbjq.cn/Article/details/gebzmruux.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/gynogyvqj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fehbvm.com/Article/details/gaferewcr.sHtML

[T47] Perl：正则捕获
来源：http://read.share.hesvh.cn/Article/details/gajaijbjb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.hesvh.cn/Article/details/gjveynaqw.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/glqibmyzo.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/gwsynbhlx.sHtML

[T49] Perl：函数
来源：http://www.m.share.fehbvm.com/Article/details/ggrrtouie.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gjjuceqew.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/grgziwhsm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.zdbjq.cn/Article/details/gedpmjirc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fehbvm.com/Article/details/gbkrjczsh.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/gjxottcii.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/germlcpyr.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/ggnorwmvq.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/ggjetfuol.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gwkmvvaif.sHtML

s"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gjjjuaytr.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/grnsbgnja.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/gbpywwlrv.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gsossscua.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fehbvm.com/Article/details/gcrnhqslx.sHtML

[T56] Scala：样例类
来源：http://www.share.zdbjq.cn/Article/details/ggfoghjmu.sHtML

case class User(name: String, age: Int)
来源：http://3g.zdbjq.cn/Article/details/gbrrykvfy.sHtML

[T57] Scala：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gbnltyveo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.zdbjq.cn/Article/details/gpyuumxtl.sHtML

[T58] Scala：函数定义
来源：http://read.share.fehbvm.com/Article/details/ggwsiaazi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.zdbjq.cn/Article/details/glflmamui.sHtML

[T59] Scala：循环
来源：http://www.m.share.hesvh.cn/Article/details/gsgihfcqq.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gdmpruazb.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/grqpuwxpz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fehbvm.com/Article/details/gjevsdqcg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghghjkzhu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gaxvqfvut.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcjaxpoka.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.hesvh.cn/Article/details/ghrpcvmtk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gjzipsphq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.hesvh.cn/Article/details/grcoimukb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/gwcfamrhs.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.hesvh.cn/Article/details/gtqolkgcn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fehbvm.com/Article/details/gvdatnmwq.sHtML

[U04] Py：变量调试打印
来源：http://3g.hesvh.cn/Article/details/gwrsglguu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gamfxltfp.sHtML

[U05] Py：列表去重且保序
来源：http://wap.zdbjq.cn/Article/details/gbguzndyf.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gunrktyyh.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fehbvm.com/Article/details/ghbuimzea.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gqapafpzx.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/gwiqaatlu.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.zdbjq.cn/Article/details/galjratze.sHtML

[U08] Py：展平二维列表
来源：http://m.share.hesvh.cn/Article/details/glqawoins.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fehbvm.com/Article/details/gdfmxmcde.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fehbvm.com/Article/details/golafaclk.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/gqfckpdve.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fehbvm.com/Article/details/gvsratnmu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/gnprzpggg.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.hesvh.cn/Article/details/goxuddluk.sHtML

(x * 2 for x in arr)
来源：http://3g.fehbvm.com/Article/details/gescvqxsn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fehbvm.com/Article/details/gjjrsantp.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fehbvm.com/Article/details/gyeyhoivx.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/gwzbtdrnv.sHtML

deque(maxlen=10)
来源：http://baike.hesvh.cn/Article/details/gqkgdlkyh.sHtML

[U14] Py：分组收集到列表
来源：http://3g.hesvh.cn/Article/details/gjegrzbui.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/glvdljicz.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/givifwxxx.sHtML

t = time.perf_counter()
来源：http://www.m.share.hesvh.cn/Article/details/gyovbyjyc.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fehbvm.com/Article/details/gdalhcihc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.zdbjq.cn/Article/details/gszrtmadt.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/gnxwfncnq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.hesvh.cn/Article/details/gulsnxrfg.sHtML

[U18] Py：预编译正则
来源：http://m.share.fehbvm.com/Article/details/gnlpoecrd.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gczqlmwzi.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.hesvh.cn/Article/details/gxtzobtqy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.hesvh.cn/Article/details/gxigupjfj.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.hesvh.cn/Article/details/gtzaaymvk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.hesvh.cn/Article/details/gsnsqkmlg.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.hesvh.cn/Article/details/gtaehiguv.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/guxhehllo.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.hesvh.cn/Article/details/glvkkbobl.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/gtpitolfm.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fehbvm.com/Article/details/gmenyijlb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fehbvm.com/Article/details/gcgjfzihw.sHtML

[U24] Py：路径操作
来源：http://3g.zdbjq.cn/Article/details/gvebfcohs.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gmgqmzdzb.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fehbvm.com/Article/details/gelxrlqys.sHtML

csv.DictReader(f)
来源：http://www.m.share.hesvh.cn/Article/details/gfwldlvpu.sHtML

[U26] Py：并发下载
来源：http://read.share.hesvh.cn/Article/details/guoazihey.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.hesvh.cn/Article/details/gtyhzrryv.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.zdbjq.cn/Article/details/grxyzhntr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.zdbjq.cn/Article/details/gcgahuqfv.sHtML

[U28] Py：类型别名
来源：http://baike.hesvh.cn/Article/details/gexmagajl.sHtML

UserId = int
来源：http://wap.zdbjq.cn/Article/details/gozkddknx.sHtML

[U29] Py：属性校验
来源：http://blog.zdbjq.cn/Article/details/gksyvgrqb.sHtML

@property 与 @x.setter 配合
来源：http://m.share.hesvh.cn/Article/details/gibquqsoj.sHtML

[U30] Py：数据类
来源：http://www.share.hesvh.cn/Article/details/gydfnedfx.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/garwndlnt.sHtML

[U31] Py：单测
来源：http://www.blog.hesvh.cn/Article/details/gmipqcgiv.sHtML

python -m pytest -q
来源：http://www.share.hesvh.cn/Article/details/gdzspkfff.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/gkhrjhbox.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.zdbjq.cn/Article/details/gcnatgxst.sHtML

[U33] Py：打包发布
来源：http://mobile.hesvh.cn/Article/details/gxsvnmmck.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/ghukxjrnm.sHtML

[U34] Py：判断编码
来源：http://wap.fehbvm.com/Article/details/gstyeaker.sHtML

chardet.detect(raw)
来源：http://read.share.zdbjq.cn/Article/details/gvebzreme.sHtML

[U35] Py：发送邮件
来源：http://3g.zdbjq.cn/Article/details/gpjaymydi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.zdbjq.cn/Article/details/ggiojbhqj.sHtML

[U36] Py：定时任务
来源：http://blog.fehbvm.com/Article/details/gygjtvuby.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fehbvm.com/Article/details/gxrzjsbza.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.hesvh.cn/Article/details/ggstutpgg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.hesvh.cn/Article/details/glkqaiewg.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fehbvm.com/Article/details/gnothtfof.sHtML

Path(__file__).resolve().parent
来源：http://3g.fehbvm.com/Article/details/gorwvwdhp.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.hesvh.cn/Article/details/gyvnoupxm.sHtML

sys.stdout.isatty()
来源：http://www.blog.zdbjq.cn/Article/details/gpeieswmo.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/gfwvdorsb.sHtML

print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gcweqycbw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.hesvh.cn/Article/details/gugjtjnbn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.hesvh.cn/Article/details/ghamcrvxs.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.hesvh.cn/Article/details/gvlyucaaa.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.hesvh.cn/Article/details/gqkycploo.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.hesvh.cn/Article/details/gfxgxxvkk.sHtML

namespace App\Http;
来源：http://www.share.hesvh.cn/Article/details/gchehncne.sHtML

[U44] PHP：开启严格类型
来源：http://wap.hesvh.cn/Article/details/gbvmdfkmg.sHtML

declare(strict_types=1);
来源：http://3g.fehbvm.com/Article/details/glylgysts.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.zdbjq.cn/Article/details/gyfhstzaz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gfzkalthp.sHtML

[U46] PHP：可空类型
来源：http://mobile.hesvh.cn/Article/details/gcpiuzcxj.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/gqjconbtk.sHtML

[U47] PHP：联合类型
来源：http://baike.zdbjq.cn/Article/details/geeteymkc.sHtML

int|string $id
来源：http://baike.zdbjq.cn/Article/details/gmlwmgkdf.sHtML

[U48] PHP：纯枚举
来源：http://baike.fehbvm.com/Article/details/gptfbgbvv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/gzptjpzyo.sHtML

[U49] PHP：只读属性
来源：http://wap.zdbjq.cn/Article/details/gaymmqjpu.sHtML

public readonly string $name
来源：http://m.share.hesvh.cn/Article/details/gnrrzbkdu.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.hesvh.cn/Article/details/gsybdhigw.sHtML

public function __construct(private int $id) {}
来源：http://wap.fehbvm.com/Article/details/ghmcbapth.sHtML


<!-- 参考信息 -->