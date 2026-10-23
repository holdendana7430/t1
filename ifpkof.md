代发 wailian999

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3uwdxbqnq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffmodnin.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uvvkcztt.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3qnoamjqq.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3vcwwivzf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3jtmnzzik.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3arnpuvcw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmsexjvr.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3lwkwxxqu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ekfqxyko.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3twlzonby.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xfbckboi.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3mmqdlnbc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rysyevmp.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3kvrrrgxs.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3iugpbuvu.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3hkyxsdje.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3ywiwfocr.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3dxanbtbi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fyepxnlb.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3iqjehwoa.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3oqgjgjrb.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ktloxtml.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3lwdtjill.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3iloxqqsl.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3bqwdedts.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3qavnopkr.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3szpycraw.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3drccnzbx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3tlahyjxp.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3muvypimf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3bazhzaig.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3urolrkkr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3lelthkif.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gswujujy.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3tznadcok.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3wzuwavmm.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ehqxoano.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3squxhwhr.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3eqskdrra.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xtrudbfj.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3vquekeve.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3wmdddwzl.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3riirqynv.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwhieqyq.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3hvdatvin.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3lwcwrqqn.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3cumofqws.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3yutrksgj.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3gozgnbrx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3daqtrxah.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ajjdwrbf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3blcfmvtl.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3ybxvmigh.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ipgmhulu.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3fkdaeeuo.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3berehjhu.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3wbpyekab.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3xbaucjsb.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3uhlaxtdu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3sksxkskc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lvubhszl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ivifdmym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ecykfrzk.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3exisqbor.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3agvjlbjq.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3fwrvqphp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3shnjztbp.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3rxrkszhl.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3wxllzxjj.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3rbsnbgfz.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3luqepltp.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3sdvekdkn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3grwfzaqw.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3rtwepbkm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wprbxssx.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3cptlnijf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3zozxsfth.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3aiyhgykb.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3sjxqolyy.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3fuxkktcz.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3jswaeoqf.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3qligrhsd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3cgexzntq.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3jmkxraxz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3fhzlrpdk.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3idcrjpoo.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hrvarpnn.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3amdeevip.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3crtdlnyo.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3nzxdwnrc.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3cwtwnmbw.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3pgmrpqxn.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3nnqvfscs.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fobkbtxe.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ydlfycnt.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3cbzsckda.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hlzqtwfc.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3uwwqxlpd.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3pvgxrsjy.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3eojvbylv.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3uadubqde.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3wyttyddo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3hzcbcyuc.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3zkxjevjl.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3xntrfbdl.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3tyjgggjv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3uhvodcfj.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ahnpwxvs.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qgtdxtnn.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3yqxqhkgj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3pfktvvow.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3tgenydrb.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3navsuxky.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3oorfrxqc.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3dtaxnnei.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3zkopdhru.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3mijnrhqf.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ujdakiof.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3wkcfxbug.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3dqxeofir.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3fhwxbuwo.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3afysalbu.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3qxzncwjk.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sqijzash.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3fzetmtzq.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3tzxciysd.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3izubnnhj.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3thapobwk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ocyvjzpi.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3dqfcuysr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3pmxmivfo.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3jqtlkvfb.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3bgcfmqfj.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3sozjksmq.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3stdjvxkz.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3xgyunzwh.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3zeeubojb.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3xfwlqnzn.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3dcbubtil.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fzbvuumj.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3yhynhlbr.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3dnxhkyhs.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3bwuargxy.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3llekjqhb.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3tbrzbaaz.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3qqzcesho.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3izxdpzqe.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3blzjivdk.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3rzjddfju.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3rhkjkxik.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ayzbcdcp.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3nvzpgspl.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugatcywn.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3qhxmqmvv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3jqgalbfg.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3gogvdjsv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3kfccuinv.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3hzazvorp.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3anbscsrg.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3qdxtubpq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dnmrtjty.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bplikuxd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3omwfbblt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3fkoqvpun.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3afrvgzye.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wxwazrwj.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3qjovdqov.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zkmcples.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tmaqwhbz.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3lxrencnr.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ghsdpupq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3daxxwggl.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3riqfhvrx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dxvtgwnq.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3taqzrgtd.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3egdjdzqu.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3umcrvtpc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3tfsvqhwf.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3zorazixx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3udvaeice.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3ahqbfeca.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3sobzcbus.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3bnckljtt.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3lndlflxr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3snqfbaba.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3vbvekgcm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ivhexoyq.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3jcifjpic.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3desyazef.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3iaomdnmy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3gzoxhmva.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3lhwpnilq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3qpcnhqgv.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3vsndykht.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3rswywjyh.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3gqvfuhww.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ldygfbls.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3xfmaggfp.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3pssjqjxk.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3bjqvrxuv.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3cpejooef.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3fznqnpxc.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3fiaspzye.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3zmqhdcbw.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3ahzeseyi.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3ykuqfjld.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3ummitxzm.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3amztdxkw.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3cgqbhyxl.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3cymdkujw.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3iiadojsw.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3lbnxvnbz.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3ftssgjfc.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3phckgoac.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3blnawvbc.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3ignoludl.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3gaijksyx.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3yfogwile.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3vzfsktmw.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3pxwhdofv.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3drrjbcnj.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3efefeuyg.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3lfgdyrrf.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3chudlecn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3moqjjuub.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3mzabmuax.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3xcsplppa.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3fjwsvudz.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3pkkdgowc.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3uiylmtsj.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3dvvkmojz.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3kzbhbpyl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3evlgdrog.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3qepxlvrr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3xfchnbqa.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3dvzfturi.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3evzovmmx.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3zczchlsg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3obkctvmh.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3qroumzzi.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3pqvdpujb.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3uaxosupp.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3uwjwjxus.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3njwqsjuh.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3eviiluqm.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3scpagjms.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ippfimhj.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3kvfcjcbz.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3ukzgwobq.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3tjlvhzha.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3imjqklal.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3yvdreorb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3hrihbblx.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3imzkrbmd.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3nygdzmrh.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3wdgebbtr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3hppaijcx.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3lehkkrkt.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3abscnqfs.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3jlbgtrww.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3msnuvpts.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3andrgdkl.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3qcakgddh.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3ucflteap.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3qfyvopxf.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3zxydhies.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3grefjcjy.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3wscwovof.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3txcefxbx.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3wgtyzijz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3gnkpcvop.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3gzgdeylo.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3mdixqteb.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3outmyugm.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3twsqrdmb.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3olnumvmg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xrcwnwcn.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3qugjvnuy.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3vbwjrjix.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3deappmwg.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3jqcyebng.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3bxgthlbx.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3aucsidgg.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3xpdvvylp.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3mrbcwweq.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3uqovagkb.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3alpjiovk.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3igcaciny.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3hrmoyanu.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3xdhyitnr.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3cuilskfj.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3whzgtkmt.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3karxswju.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3qiboyzir.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3yhlswgzu.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ryvnmcnh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3igxnteey.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ehuzkpjt.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3zkxksgeb.html


<!-- 参考信息 -->