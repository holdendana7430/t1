代发 wailian999

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3qynvuolb.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3klmdowxk.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3uameuxqn.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3fontjvsy.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3guxlsccd.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3xfukthav.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3fgxwznas.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ndtmktuf.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3qdeltmrv.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3izkpalqu.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3myaedtso.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3oidjzneu.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3cwuwptjy.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3jcfpwntv.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3cvtrkouf.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3kvkjfkrw.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3jrhmkxer.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3tsbxvxza.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3ttrdmozj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3kfnxovvw.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3mkitksjy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jnqhbgpu.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3xlmldxss.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pnoimglu.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3zhzuzlwy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3galzzibe.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3sbzcqhul.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3wqlhjiir.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3xpszyqtb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3vmfumxil.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3rbknrmrj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3oltynphz.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wetvbkpk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3kqzkcdnv.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3bwxpfznv.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3kxxwagrb.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3qpgacfet.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3gxbjfnkr.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3yukirntw.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3fgwnrhnw.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3hzqahgyk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3baomrwqh.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3tewxfxol.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqpghbhh.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mwoixudl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3suehtetq.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rwmkrcyj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3yxdpoxjd.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3enhtzxye.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3bymbause.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3ctlotzwf.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3loizhkee.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3oyyijkrh.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3vvibzzmu.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ujdpheua.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3iquxmygc.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbavidkp.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3pzlauzlh.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3cqnxifkk.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3biktqobk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mezkbcpp.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3libhjoid.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3bmvkhjtn.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ajpgondp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwcjbjbr.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3jmfvjakk.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3rlbdspbj.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3obxpzvkb.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vefwklkf.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3dzjioocy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3qpzsqcsd.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3fykeuupz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3qvtqimhw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sbmrupyr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3olcdkrkk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wmgzssfl.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xwviyuwe.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3amlyilxt.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3kkidlqvp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3hjvccjpe.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3hzkuzhds.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3edzdmmvp.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3whdhazrj.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3kasalywo.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3lkypgyey.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3yeqwqyqs.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3dzsihewv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3tgoghnfb.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3zekoczdn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3udggsecq.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3xmzolllj.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3iwatmxjt.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3jtmekwtm.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3qvnzdlwp.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3lmnsvtpe.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3jpbwgtjy.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3uitexjhp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3yxkoxgrf.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3hbyxubrj.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3icvbhilk.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3vyevainl.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3pnacmnhb.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3uchoxcje.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3pnuszwmk.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3rtbfqrge.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3rcrwyavk.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sdtpdwct.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ggkrbosx.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3cwljlxww.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3hrtwydzu.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3yttddygc.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3jnxnrydi.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3myfimrhu.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3gwkhrmuq.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3zorigiru.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3lnovhmch.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3yxitbnns.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3pvsmurwy.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3wkhygmrz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nitdxcss.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3hqyhtvad.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3fdhtbfcw.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3psuihwgc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3nwbfjwcf.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3wbtqckjz.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3lvdptozy.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3czfycxkq.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3sygvfmok.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3mreflcaf.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ivbobupl.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fsekhjzw.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3gpxbwsva.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3zgrlfpbm.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3vhgxfasx.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3acrrqnsc.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3cpgcnjhg.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cfwrbvpc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3clwehclq.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ouecgnea.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3wuyscgub.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3vgannsud.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3nscmtwhi.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3toxqbmgm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3zvisbiei.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3rhwgtega.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3opguslpc.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3uuenzoqe.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3iomqeksq.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3khiyrxgh.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3eqpboujc.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3uggmqpsb.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3qjmlejyd.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ljadfzhx.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3uoxmlnzr.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3zzuyzxyk.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3oswrkjjy.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vsimcvrp.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3xxitdguc.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3wyevinfm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3mwtoserw.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ocxmsjzj.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3xrkgmauw.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3idomquyx.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ftgxweum.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3aivhmvxt.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3gcykyvod.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3yxshphhv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nhzufmph.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3drolqwni.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvkadyez.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3htreqews.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3pwqghizt.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3mlrcoaye.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxjemwsh.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fqrwsgsf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3gvafeqrg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtvukyez.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yylmdqyc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wjnrabyn.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3zgbemjfr.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wowbqfav.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zknnujow.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3cmdmabzd.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3skjrynky.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3klvnnmef.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bkhwjnwu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3ppufnbck.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3inmzazns.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ihbldbsm.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zzxolria.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ddhootkc.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3fieipmeo.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3oecxlsyt.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3eeuowwzx.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3rdmnszeo.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3xekfkbfq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3rhhxhtxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qjhnsyno.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3deutzqxy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3limyvxsy.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3uowwesnz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3tgtdtrso.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3aotrsmfk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3sjppwuke.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3zwbezyfv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3lltgvflb.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3twaefctw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3bkpymcsc.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3gkhutaau.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mfatijox.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3aaenzolm.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3lkqjascd.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ysmqphho.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3snengiuf.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3hkicidzm.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3gvsizdos.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3zkovapoh.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3dtkffahi.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3oogjelqt.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3fnqrypcv.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nzcycgrq.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3jxwgleya.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3avpplash.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gkzpxigb.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3xamcvmcu.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3ecbbrhne.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3twihpmxi.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3pafsfdqb.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3kggprlex.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3rptwpejl.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3wsghiyvz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3xmbipxrz.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3otlhqjra.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3kimrsyka.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3wkeklmaq.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3mhqurcyp.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3kxehcpmj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3mmmwpysn.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3yhpfanfo.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3tigxunny.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3nezkukem.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3yogyfmlt.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3lxdecmmr.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3yfhbfnbn.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3uxnmzgjm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3llhbdoth.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3oxzilpsr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3uomrvpyh.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3rjkvzmri.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3rbcycvod.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3mdplvzao.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3qilhfeag.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3vrsazeaa.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3xsiuwium.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3vqufeaka.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3pvcxhukh.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3ivgalnbc.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3sukfrwbb.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3unoovfhs.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3cyjztuac.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3ptpvmqfe.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3uicbfzmw.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3drgmlaom.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ffzofrfd.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3vhjqfbzj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3ipsjrsrh.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3slaqevjn.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3btjsyvli.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3pnkwmzma.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3vghehuwt.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3supzjlxg.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3iznuyqhs.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3oezknyak.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3gbitfvle.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3zroajsuc.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3cgsphhaj.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3tekfysir.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3zmyilbry.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3qhizspbg.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3mfuuarrr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3iihgwvkq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3rgzanmaw.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3bwvyegyk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3rccytoja.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3xywynvre.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3kukhivfe.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3petiiphh.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3uvpulbzl.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3hrnqhnhd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3afghkfeo.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3rzhlzbky.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3dvtkglmk.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3foisqwah.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3vprczzjk.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3fyoaqxrl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ylntromv.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3kpuhsjpj.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3dswtrehc.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3ivyohsyw.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3chsmfycq.html


<!-- 参考信息 -->