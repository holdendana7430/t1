代发 wailian999

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2juyniouo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2fipdcbrt.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2awuobcem.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2opwlxksp.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2yvsnjetk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2zpmpqhkv.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ljpberbo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2yipcpvhx.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2jtluzmvr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gnorccyf.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2rypfddff.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gywiwgms.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2quclkbcm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xmzulmbj.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2jyllfqjs.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2wnqphpfx.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2jefcipwu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2cmqjvljq.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2rkibxila.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2amjtmhho.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2dxytcmmp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2wjyzccll.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2cnjylfka.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2kuallctb.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2wstwibgr.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2xhedmvjt.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2dbvtbexr.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2swzdbsoo.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2iyprxibo.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2sjfypaqq.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2ozpelaws.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2bfxlbjfl.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vjonrskn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfjxtvwv.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nwsfmeyd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2zshgptrb.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2wtlglros.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ibklhkqj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ahawsetn.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2taarvzat.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2efcfanvf.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2phxisgus.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2sskhdiwr.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2tksmscei.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2dsglspnb.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2yrciiedb.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2iquxbguz.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2cmuakrdv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2lptyvkcj.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2xckbpohn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fnengjzf.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2jutsndjd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2sgdxjano.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2lkhwwixt.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2jvnrqknv.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2masfqlqo.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2qyqhkgnl.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2ujggnwcd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2tcvmblly.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2klmdcpfz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2jdltxmhd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ljdmqrxz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2qcfymzam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aajczeox.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mwzrbwgk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2dhltaalp.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2icdephks.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2cfdjgozy.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ieqpytkb.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2qemzbtwj.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2aqusbvvs.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2gdwzriop.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2pxgfmvpm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2zilsjnak.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2smqmcdzz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xvhdjbxv.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2oefgdnqx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2kisqzcwp.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2xfyidpah.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2gxzqxmtv.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2ucbrhrfb.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2jkxcvndn.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2alaeuagl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2preavwgx.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2njyhmblt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2gkuxyqro.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2bfsodfjv.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qmqiaobq.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2hegdhvqw.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2hjdeennw.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2odmfront.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ojtjxpfe.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2ehzxhbss.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2zbefbtmc.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tjkhdruu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2pjgjynta.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2yatllbxw.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2bipodhqi.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jcanhbiu.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2myeluaqq.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2wxtojfrx.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2mfjhyzdf.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2frwtdiin.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2gynzctkb.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jrktstrs.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2qlqxtpzz.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2guswutxs.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ilpkepxk.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ndtxpsqw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2utbfqcgz.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2uixamnrk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2xhzonyij.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2xhahxmrn.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2rhvidgfe.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2qcihwtmj.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2rtkflhmx.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2fyahpqvn.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ulwffwja.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qvbaivlh.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2zzhozwej.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2abfxctxg.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ojeyuiij.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2pkeoszqw.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2uukztpeb.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2doisejrt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mfioqxkk.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2cxvtdijq.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2hyyspyid.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2lpibwtwh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2brvhwccj.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2kkvwphtd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2kphxwryr.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2ykqqcgdl.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rjiunftp.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qvlcuieo.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2nbfnonsi.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ahvxiltw.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2unztpkxw.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2aybpaitl.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2wewwfmhe.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2lhyhblkn.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2ycbygosb.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2equmbxee.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2cuvpfnts.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2srujlntb.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2gtucozjc.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2rfwgxaqz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2rqnxyskv.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ktcicwko.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2qyhqjyql.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2edckoqbe.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybitkgxd.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2xndknmic.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2iysvyzyc.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2wkyhduao.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2powsiikm.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2lcdzmvdy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2xvqfmxdx.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2psziaiod.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2cvqgnqfq.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2qoikiayv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgbqimtg.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2oybcbxjx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2hxlstlvm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2xhlsennm.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2umgccadt.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2dhhgemzw.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2veawqgss.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2niqhdxgx.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2quuvfarv.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2hqdeivtg.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2nxiiteth.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2rcjgezoi.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xncrexpo.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2fwmsuhqt.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2tnqnsffb.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2kuupdkmc.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zzwzkyyu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2pbxltueq.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2kdcvsavs.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2slquvkuk.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2xfzzppzi.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2jxtqybca.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2hcjjcsws.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2hpmcxktm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xguzvpym.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jekfzefg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mogdvqjp.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2oncdlchg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2iyhpgnkr.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ewhndzuy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rbtakskb.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2wgjiqlao.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2uauwzchc.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2xcqpjacz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2lsljhmbx.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ptqcadqo.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dktapgcv.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2zlhysuij.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2jecpmivb.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2teftybsk.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2nredjkkk.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2pgjbqknh.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2yooxgwcn.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ddclxrem.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2kqsfqutp.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2vofarnnc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2loxlutsx.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2prjmavuz.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2eiijaksd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2dpomrcmo.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2wdleywoo.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2xinavyyd.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2ytkglfvt.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2urdzozpj.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2wnxddrto.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2wvdcpyws.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2fztlxdkd.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2flrbbjkn.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2vhtvuuag.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ramoueqf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2lfdlmlgk.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2spbqtdli.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2rzxwsznb.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2cwwzdbly.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2ngrylrie.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2uhyapcax.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2ojgswvuq.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2gbaijarz.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2htwvochs.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2shrfgjal.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2yzzxptav.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2wrhglkdu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2tdmcxeog.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2scgkfieq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2zbxukjeb.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2okikrpvb.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2ojoievmu.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2likbntnj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2pupftpty.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2hfelvotp.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2ymdrsezx.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2ekkevwxj.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2osxzjnoz.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2xktszdir.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2ptipdjdg.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2zgtotsqz.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2frkyokvx.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2lfsqnhbq.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2ukrwjzkl.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ztjpharv.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2bobhzfqk.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2saxynjyh.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2iilcxljg.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2qvwjahbx.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2xdbvhuji.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2bvdfmrxm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2fhjbbyah.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2oydxtwra.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2ittcttka.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2rckjbcad.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2cabloymi.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2kdhdsoci.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2kdqmffxe.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2mgvfbtxh.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2tcqhxvmh.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2tadgkrad.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2gsfwpxva.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2yvdeqslj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2xbqrswyc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2bpazytef.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2ofddhiua.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2zspjjvmw.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2acuqscfp.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2eaombmmb.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2cslouuaq.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2dejjrtcw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bdezbnew.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2ijzjidbp.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2bpswbdzm.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2kmjufgjf.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2vfnmchdz.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2gtuollaz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqhqzmzp.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2sievpyqe.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2nljvcqmx.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2pbbnotyo.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2utxxpkbw.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2mmmxtpqc.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2psoocvre.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ijfesphm.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2iqbogwba.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2hsidqneb.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2wtakfwyn.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2phkffpxt.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2fhesezey.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2aicbothz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2fpwyeucw.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2hzimhxsr.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sjifzvae.html


<!-- 参考信息 -->