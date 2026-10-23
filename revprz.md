代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3lfhxefkj.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3evmlilkn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3qtguswpu.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3bdicuhni.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3khxyqovt.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3idrvwxro.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3hqisqeto.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3dlkljtkj.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3htritefd.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3hyylcfvr.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dbsfvofm.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3erviguaj.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3nmlauhdh.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3dqkuehhw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3qphhbqzy.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3kyjuaasu.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3tmfrgfvx.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3vfcverbj.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3hjphxejs.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gejcexum.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ftnjigpf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uimhvvyu.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3ozetgrez.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3xyucpdmi.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3pkfqzprd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3muyogqxt.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3rrinyzps.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgkkuxtx.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3psvrllfg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rsycsvgi.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3piztxzqt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hwkgjcvd.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3harfpofr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mbzcsrol.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3zooqblyd.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3driypxyy.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3zdaxyuxk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3horbrjzb.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3nzpeodvp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3bbuylvjm.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3bkgmszfk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3qlkozzty.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3jeryfatb.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3lktushbx.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3bzpjpjup.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3sffwxvow.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3rvimgxmm.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3aylkyabj.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ubpkcbpz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3gpnqpscm.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3unsszmql.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ciysfubn.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3wthattqc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3xboezbkc.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bvixitoy.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3ufvgyvaw.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3okfbbvxo.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3ypnbhjbf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3djkdaxou.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3abragzdm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3aotfzbqe.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3lhnsfgtd.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3qqllgohh.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3lovkalog.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3hckggnek.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3vkzumonq.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3gmiexoqo.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3pacdckli.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fghngria.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3phbxlfrv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pkogdjsn.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3escyecbj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqjxhcib.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3bzcxzsdj.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3hetpcpim.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3bndwdzse.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3jyhzcrbc.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3eyicjoyz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3sggjjhgt.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3jpgefitp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3vsaxcskz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dhsgirvj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3jqkkhsut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gmxmtczf.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vruuopln.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3orqabjej.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3hvfsuwbc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ulrhqrpi.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3oeqiegrs.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3sobnxdyo.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3naoarxdq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3qizoxuwp.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3utbpegrs.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3coxbfjwe.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3uvohpqzu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pcufjufg.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3haketuer.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3qwlqvewi.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3ihtwxszc.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3islmxaas.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3itglvjdy.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3phomktfl.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ipuaycom.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3udlptvfe.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3iyrjdgxj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3rgdmimnk.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3lcwqcpxi.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ovnpuekv.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3uqaattec.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qreiqixd.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3tvapdbje.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3bmqnqjvk.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ynlcalkc.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3bcxcufga.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dpfvgpkr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ysridhga.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3itwrdmef.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3puckcskr.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3nhhpfdws.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3cedmqrfb.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ypvmwopy.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3nzqwtvcr.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3eifafnpc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3vlfeieik.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dmyybybf.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ijlyhvdz.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3xmthowge.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tludhbwt.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3pflgdtaq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3inlffrys.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3xhljfurs.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3kjiwryel.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3dljxhbod.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3chthmpow.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3mrinfzwl.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3tnnbbwiu.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3yuumcvky.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3vlsznvse.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3itwjnluz.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3rkfjkffc.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3cepfgvjy.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3aunvagso.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3mjfrxbss.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3jtxzwrif.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3megqvkcr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3miophfgr.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3fcrvlqwy.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3gruyvlxh.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3hoylktcf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3twnuomnb.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3gmhnfmxh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3elebjvui.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3tbodycpl.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wnmlubdi.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3hobbklfq.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3gxxjmfwb.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ptcmkqiq.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3rxqipwjn.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3ngyuewip.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3vcbxtjlj.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ggiidotw.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ztstfdxx.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3lwcpfqlg.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3zzchehlj.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3iiqaomdf.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3djkjkfnp.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3umcezwkk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3yfyhsfnj.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3aaculydn.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3otwltkmf.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3kjizephq.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ebxmasox.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tdgbjzqu.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3qavpqxbj.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3qboqbkoz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfdzqocu.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3aeijmodb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3wpcloajk.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3xlnwwjdi.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3jbpytrkn.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3urzvwhqi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xsbwgzqn.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3btdvkbeq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3jkjbgpzs.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3nyxgumqp.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3klntoiag.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3errtvqga.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3xqzirdqw.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3nfntbemp.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3oupxnhol.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3pejjevxb.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3oniibnck.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ieentctb.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ayawgmdx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3htdspaal.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3ztuezled.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3cppnvrww.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3lzvozpfi.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3cnjikqel.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3jdchhohh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3guktzgky.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3bpypamhj.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mzcuqepj.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3xpzmwxuy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3sslaqjnf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3somwkszw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wcvbebuh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qkmgcgni.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3heosnpdh.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3dfbidtqb.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3wjaqmdhh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lrfbadtx.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3pgedmznu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3zrvcihio.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3kzrzikte.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3buhcwvvi.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3ivwvdwph.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3uwqopvob.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3xbozvmfe.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3kvvjcrrv.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3bagneidv.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3tbtcyhih.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3lcmnzkxd.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3qvlcmowl.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3btihztsi.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3xgechdjb.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3yirrsyau.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3vddxhqce.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mwxvzjmp.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ixtaakww.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3wqqijtrj.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3vlfjrmxs.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3faavjfdx.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3uzsdgvhg.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3uyzzoxwo.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3rjesscyj.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3uibdiuku.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3lowrysub.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3jlwbraxp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3mpevjdcn.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3psfkpqed.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3sjwhxlnw.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3dahuxwzc.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3uyrigend.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3ogbjqicd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3khrhohln.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3cndqumew.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3lapqwtvt.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3acwdvboj.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3oprzxhnz.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3nrnugaco.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3gozttobj.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3jutzxecs.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3xcyvnpdg.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3tkjsegjy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3mfgxpfdx.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3xgsnhqdb.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3pzwifguo.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3kxrqrjwu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3wozsazqz.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3tnzpiorv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3rvopvhru.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3uztpwwrd.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3dexfdwld.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3jmkhasmq.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3esbzjmfe.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3zueoqwfv.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3ohzhwqvl.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3epvbfrxn.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3zrtxpyel.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pjswhyhe.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3ejanpqjs.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3qtmgkhia.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3qsnmpzqz.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3gmcvljvu.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3fvkmugaz.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ottslzdb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3evhuzemn.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3fnuoeylt.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3mwfcwscj.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3zsjnhxyx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3cuorfjqx.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3xxzwcoin.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3awwyavnv.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3yhsrhkro.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3dipkpdsx.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3titsmxoo.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3tfpiyiuu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3ptrbugvx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3oxlqzmll.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3pnfpvqga.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3uomlbpmc.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3jklxbzrn.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3bpqqsfmv.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3hkjnesjb.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3iakykedx.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3ztqogojq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cagxiwad.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3lmuyziwl.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3meckrmre.html


<!-- 参考信息 -->