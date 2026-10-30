代发 wailian999

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyzlnejh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/giobrzhqz.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrfsokyz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gobnraiui.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gprphvzhp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrefstgz.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gputdkspj.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/goojobmmn.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrvgvbwp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gbxikecbc.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtxspnxl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzipaglbn.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gvifxxrbf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goerqkckp.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnfowdiu.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyfknlqb.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/giizbxvas.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gedhapzej.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gomtfuhvm.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpvmfobd.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/ggezzjkvj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrawqafa.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gbltlmtcr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/guobhyyfd.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqjyjdhf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyfgimcp.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxugeeoto.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gqkvvjlaq.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbggqgfh.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbamsnvah.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatovqhll.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmftcrbtk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/glzzfaxiz.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrwgiyhx.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gsthmadlw.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gjceixypm.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/grlnzwcmg.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gwptqsbvo.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyogozcp.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvjermml.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjdabjcg.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/griqpbejt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gwyjgayoq.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzydclczu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtxivmgvo.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/gnneopbyw.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqejsncrq.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gyotbhjvy.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvxavcjz.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsjhrzqn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gpqpxybik.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gllebziwc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gqlnsawrl.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gboumagup.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gntwarxgb.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/guxgalifu.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/glnkdxwzo.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwbbcgzd.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjcdpmuq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gczaqknmm.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgqasoze.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gobaijknj.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjfkowxh.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/gmuqiruxi.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuqrarul.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxyljhfs.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gqyvlprdz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyefloqml.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/giqovrbph.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gsmqbkayx.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gmdwzxyos.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gdbhatrkt.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gbvmmxdqx.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/gptzdyxvg.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzelpycj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbpwkvlq.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/gccrszgie.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkeneiovn.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/gvjqdjwfp.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gtuceisot.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrewaihl.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/grghawyxk.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gxnztguxm.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gjcevxuer.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gwklgwkpm.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/grslppebw.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjworalc.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpzfgfis.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/gssdbsqkg.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/grrglrumh.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvgxdnpk.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvygyydge.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gpyslrppz.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/guigbtpit.sHtML

[T20] Swift：数组操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsvclmae.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/giqwxhaeh.sHtML

[T21] Swift：遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gebvyxhud.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcytjmft.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/gszjzpxre.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gptesmbsu.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gichcknkd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbniicej.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/ghalempau.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gevqrjjkk.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbqrqyga.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlnbtqxf.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/gvmqkmagy.sHtML

class A: Base { override func f() {} }
来源：http://blog.fanxiaobao.xyz/Article/details/gopwfpkwx.sHtML

[T27] Swift：错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/gqyhrtoxa.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fanxiaobao.xyz/Article/details/ghtfhjzyw.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjhgtcfr.sHtML

enum Color { case red, green }
来源：http://baike.fanxiaobao.xyz/Article/details/gjtegvlgt.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyilrndea.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqimqvgp.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gslilwhsr.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gmjxikwlh.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsvoadqw.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gzsbgxcww.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gwzbqujpl.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzfzzudy.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdotpets.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuimlmtk.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtrrcias.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsewbcjz.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/gbzosqgda.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfqtcwpm.sHtML

[T36] Lua：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gnmeqlnxq.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/gqnxmvsjx.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwehtyoln.sHtML

"a" .. "b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwzvyujd.sHtML

[T38] Lua：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzzukjci.sHtML

if x > 0 then print("正") end
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyyrhvlb.sHtML

[T39] Lua：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gdsxucpct.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gykqffadn.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/gsfsdcmoi.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/gzlyckpex.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxlfofpo.sHtML

print "Hello\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gijozuhot.sHtML

[T42] Perl：变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/gfwgtvnsr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gkdsctsjo.sHtML

[T43] Perl：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gukteynol.sHtML

"值: $a"
来源：http://mobile.fanxiaobao.xyz/Article/details/ggukvnqkg.sHtML

[T44] Perl：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gvhmgvcgh.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxhjghfa.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnlzpxbn.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmiufajtj.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godcmldpd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxgmgzde.sHtML

[T47] Perl：正则捕获
来源：http://blog.fanxiaobao.xyz/Article/details/gzmezeuqz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtodqqrrd.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gimftqbzq.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyyqbjxp.sHtML

[T49] Perl：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gxasyxayl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxzmaxmgq.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gocdkiffa.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxoqjuoy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkiqmoucw.sHtML

[T51] Scala：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuuqlukp.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gfnbzohcn.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gjzsywdtq.sHtML

val a = 1;  var b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gwqynmuyi.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlqhoyle.sHtML

s"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gpdewylrz.sHtML

[T54] Scala：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gvnojrzfu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxiuwlwk.sHtML

[T55] Scala：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gyzftjcix.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjifpzpo.sHtML

[T56] Scala：样例类
来源：http://mobile.fanxiaobao.xyz/Article/details/ggntlufew.sHtML

case class User(name: String, age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/ghthzmasa.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gjubcqpiu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fanxiaobao.xyz/Article/details/ggcfdower.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/gzaungavy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwtwzcci.sHtML

[T59] Scala：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gaimrajhm.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgytlxfn.sHtML

[T60] Scala：折叠
来源：http://baike.fanxiaobao.xyz/Article/details/ghuuyyysm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyeouswzj.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gufkenmhb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbsmxhmp.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrenvcjw.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fanxiaobao.xyz/Article/details/gxvovhdfj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzubhina.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fanxiaobao.xyz/Article/details/gwmysvtpp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/glumqrrxl.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfkxajfy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhkzrhpg.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvewhguz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fanxiaobao.xyz/Article/details/grtswzulj.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrqqzdns.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbgpdwdk.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fanxiaobao.xyz/Article/details/glgwfbhzf.sHtML

{**a, **b}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqmfdifr.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fanxiaobao.xyz/Article/details/gaygbuhqh.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fanxiaobao.xyz/Article/details/gggvclbxz.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gejejodlt.sHtML

[y for x in nested for y in x]
来源：http://baike.fanxiaobao.xyz/Article/details/ggjscorgo.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fanxiaobao.xyz/Article/details/glxgsuxhm.sHtML

max(d, key=d.get)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuzschlb.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/glevgmhiq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fanxiaobao.xyz/Article/details/gwzscdlfh.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gthtconol.sHtML

(x * 2 for x in arr)
来源：http://wap.fanxiaobao.xyz/Article/details/ghjaqycio.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbtkkavu.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblkmbygf.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkjciuch.sHtML

deque(maxlen=10)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbiieltfz.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpkldxgb.sHtML

defaultdict(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvgpywao.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajacpwxb.sHtML

t = time.perf_counter()
来源：http://baike.fanxiaobao.xyz/Article/details/ghymepebs.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fanxiaobao.xyz/Article/details/gaxbqtzol.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fanxiaobao.xyz/Article/details/gfjkucbpe.sHtML

[U17] Py：初始化日志
来源：http://baike.fanxiaobao.xyz/Article/details/gdeyvodyf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfukgsogx.sHtML

[U18] Py：预编译正则
来源：http://m.share.fanxiaobao.xyz/Article/details/ggemdrsww.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/godvdqaar.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvinswhe.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fanxiaobao.xyz/Article/details/gqcdrciyy.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fanxiaobao.xyz/Article/details/gahbhamrn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fanxiaobao.xyz/Article/details/gszghfsgi.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpjezzti.sHtML

@contextlib.contextmanager
来源：http://www.share.fanxiaobao.xyz/Article/details/gcttjidqm.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljihidhs.sHtML

list(zip(*m))
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlglrank.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqziwrtv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fanxiaobao.xyz/Article/details/gvmnkxjyj.sHtML

[U24] Py：路径操作
来源：http://blog.fanxiaobao.xyz/Article/details/guewnmtkg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gynvmfmvr.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fanxiaobao.xyz/Article/details/grhrsbihe.sHtML

csv.DictReader(f)
来源：http://wap.fanxiaobao.xyz/Article/details/gjbhrpqhn.sHtML

[U26] Py：并发下载
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwywvbzu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fanxiaobao.xyz/Article/details/gehpefizi.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuogrwjf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fanxiaobao.xyz/Article/details/gkhvrrtvx.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/girxbttol.sHtML

UserId = int
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqrfdjxm.sHtML

[U29] Py：属性校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrikxnbs.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fanxiaobao.xyz/Article/details/gshwdhyun.sHtML

[U30] Py：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gvdsduurf.sHtML

@dataclass(slots=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gcnpuzbqq.sHtML

[U31] Py：单测
来源：http://read.share.fanxiaobao.xyz/Article/details/glcahnoki.sHtML

python -m pytest -q
来源：http://read.share.fanxiaobao.xyz/Article/details/gilvetrls.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/grmnvdgux.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwxlveup.sHtML

[U33] Py：打包发布
来源：http://mobile.fanxiaobao.xyz/Article/details/gspsuoqha.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsmpenfm.sHtML

[U34] Py：判断编码
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbbfnycq.sHtML

chardet.detect(raw)
来源：http://baike.fanxiaobao.xyz/Article/details/gyobsmcia.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgtgdewd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyyytfbp.sHtML

[U36] Py：定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gkusojzya.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fanxiaobao.xyz/Article/details/gseuwakjt.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexcrszpj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gmegsfzfs.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fanxiaobao.xyz/Article/details/gpbuapkvv.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtbainwa.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fanxiaobao.xyz/Article/details/gpnokebyr.sHtML

sys.stdout.isatty()
来源：http://3g.fanxiaobao.xyz/Article/details/gjomcaion.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gxeudtlct.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuzgfsox.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fanxiaobao.xyz/Article/details/gtvuyfvfg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gouqqsdqg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gluemqljc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfnxcmpo.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdlgxszn.sHtML

namespace App\Http;
来源：http://m.share.fanxiaobao.xyz/Article/details/gekvnpnfw.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fanxiaobao.xyz/Article/details/gzxrtqupp.sHtML

declare(strict_types=1);
来源：http://wap.fanxiaobao.xyz/Article/details/guiecosmi.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fanxiaobao.xyz/Article/details/gfpfilzhq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gousuqovu.sHtML

[U46] PHP：可空类型
来源：http://blog.fanxiaobao.xyz/Article/details/gmoqpbrwz.sHtML

?string $name = null
来源：http://baike.fanxiaobao.xyz/Article/details/gpeotgmib.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfusbovpa.sHtML

int|string $id
来源：http://mobile.fanxiaobao.xyz/Article/details/galacogit.sHtML

[U48] PHP：纯枚举
来源：http://blog.fanxiaobao.xyz/Article/details/glxqrxlrz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fanxiaobao.xyz/Article/details/grjqhsfay.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakowymyt.sHtML

public readonly string $name
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgugjnrd.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyppxqrbj.sHtML

public function __construct(private int $id) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gvopvmywa.sHtML

[U51] PHP：数组解构
来源：http://mobile.fanxiaobao.xyz/Article/details/gsycmibcf.sHtML

[$a, $b] = $arr;
来源：http://blog.fanxiaobao.xyz/Article/details/gxwldyjfg.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gubkuzwqq.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/gdextvprw.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fanxiaobao.xyz/Article/details/gkywqjrxv.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzczilwe.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjfkyqte.sHtML

$obj?->method()
来源：http://baike.fanxiaobao.xyz/Article/details/ggvtalwfv.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjaznpnk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilfnewcc.sHtML

[U56] PHP：命名参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkhxcnhy.sHtML

f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gflxsfunb.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkfyzwjx.sHtML

"值: {$a}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysvvmxdh.sHtML

[U58] PHP：数组三件套
来源：http://baike.fanxiaobao.xyz/Article/details/gtcklihvb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahguntds.sHtML

[U59] PHP：自定义排序
来源：http://blog.fanxiaobao.xyz/Article/details/ganesvjia.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnenqglrl.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fanxiaobao.xyz/Article/details/gmhpfosfh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfsetzrb.sHtML


<!-- 参考信息 -->