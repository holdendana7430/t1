代发 wailian999

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2dtnpwgwr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2opnjgawm.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yjegnpyg.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2orardzpw.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2djjbhyro.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2olejvhta.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2rxygnfpo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2hccjafqv.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2tpapniii.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2clfdxcsp.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2wdhkuioi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2emfapyhs.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2ylsglqxe.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ffznbabi.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2uvbdahze.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2xifdtupa.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2nrdusjiw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2qxfhxlld.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2jhovusdd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2ztvzufch.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2tblcsasc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2kskwcglg.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2gwuzbeqr.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2smrupejr.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2tzzxhlre.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2vuvbozhg.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2flibjqyk.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xkdxvsgu.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2pchfpbhy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2sdbbmuhy.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2vnrynajj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2rycqqfdx.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oohxkobs.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2gfmpapku.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mupfxwbj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2qlnhjlju.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2eidiqckl.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2yddjxaaz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2eevvujgz.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2gpmpxkcf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yxygcxcj.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2ytfxtias.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2lwyttwle.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2wlxwajgk.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2hllcmyos.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2ymzgwybc.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2rzrfjtgi.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2fdslgjlr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2fxykervv.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ppslvuwx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2vjueduxd.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2znduiwvc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2docqsjmt.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2urrsqdst.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vcrfmqpy.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2zsighsar.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rmlclfhc.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2sjqitgvr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2mdmwqqin.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2hyjeyskv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2vlzkfsmb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2awrrbxpp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ulfoydor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tlkmcgxv.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kbphbdae.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ewjrlldr.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2aaqnllbo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2oudxjqle.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ejylafgn.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2jjqlvgdp.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2wpqusdfe.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2mjxxkosl.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2vmrzobsj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2wzgvahyj.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ifpumtvo.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2agtcevac.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2opfgwjiy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2hezcmakf.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2pvogzira.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2rpnnkfmc.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2dxjmxxbd.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2nrnqehjg.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2fpcdyxgs.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2rltklqln.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2fohxutzn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2byrkyapb.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2yyaqqfjr.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jirjhzdu.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2grxagkdr.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2novrzxyg.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2cwkqfayi.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2bhedfolf.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ulbqeaxt.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2atoggrqq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rftndqio.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cailvspx.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2zusdkpnd.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ugmwsjaj.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bhhwvicw.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2zltrtrww.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2xqucurhj.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2zwxwbeuk.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2zdlfukky.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2nkrraysd.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wvuomsbj.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2txtbtlkl.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2rjiyavui.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zkxseuys.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2aduswtak.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2swtfzyud.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2fcnmlckx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2piyypvqn.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2fgbkaqui.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2fspcgkww.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2cignczba.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2upbzlgtd.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2ycgayedc.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2vjeterab.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2ycxsblvm.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2mfznafhv.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2izlsmdbb.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2svzdeoii.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2cmvmqoex.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2ytnxivii.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cqlobtrq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kotcepli.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2lygwzxia.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2dqzqbnqu.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2paypyfhq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2vqedkkhq.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2szsocuiy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2hrlyccos.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2hsdxsxhb.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2akncipqo.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2apshhveo.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2dxxnvpud.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2oztsknqe.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2bchkppfr.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ttqqzalb.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2qsfxhrbb.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2gbjfxmet.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2ijnbnmkx.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2rgrzjljw.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ybcuqjqv.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zbhbtyfk.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2oumfyerf.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2dnypjrht.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ddhxwizy.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fupcngfd.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ekbmcmnb.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2hcjpyaft.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhxvjdwg.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2drbdlqlr.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2mkthwlyu.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2cyetoqov.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2tjjuezut.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2iappqkav.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssbbrmks.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2qmfqjafa.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2enxzjcmb.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2bwosdejy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rlyowsrt.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qkwqmyfl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2udwpemvn.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2nhcqeojo.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zxwxnkmc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2bermgssa.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2xzftvrnz.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ootqgfre.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2slvbvqit.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ygpqazle.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2wwbpxlsb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2hvfcacln.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kxrieyup.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2odqidodx.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2ajhahpdc.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2qdadhias.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2aygazdom.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2wytzuyic.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2fkewtvgv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2sbpmtset.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2tcarhfac.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2bxyrygox.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2haocyxeu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2qzacyndo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fllikjop.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tdhekaoe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hbrtgajd.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2yqloxwle.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2quahxkdx.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2vsjyoyuq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ycokoawn.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2jqjnxbfl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2yvjkqbwd.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2tpuxtqnu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ycftunjv.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2bemuclxo.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2yyjkptku.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2gopfrocv.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2qtunoyjd.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2bghjnzef.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2wqraofpp.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2cvowlotz.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2vavitxqv.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ejhdmjec.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2lhghhzwo.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2xvbsxdcj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2szwtlhae.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wmzsgwps.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2gbfwzato.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2rylcmehq.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2igcctvcg.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2ynawabxp.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2fsbnvpmo.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2wlaloeaj.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2vnjngmne.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2lqbjimwt.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2thxquwcc.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2cxjnxrdx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2zkiicppw.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2wdszcial.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2jbdhlavw.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2neowamuc.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2mgmdmgjv.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2rwttwdks.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2rykcchtf.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2sjsqyorf.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2wcsrkwac.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2difgzthg.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2ardwlmwa.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2ggshfzie.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2ddodnrde.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2fipvckab.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2ujxzxtlw.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2qtkwmqid.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cbclaevw.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2rcgyttcq.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2yrdowrzp.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2myrumqut.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2yirpibfi.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2lqlnikaq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2hmkbiwmb.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2ulgjxqjw.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2aoztjrqb.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2ajjlaksh.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2bfkvwcdf.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2nuxenjwd.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xgbllayk.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2qndqejvu.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2gkywunsg.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kqwsgijz.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2wiwxiagv.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2tdcsgofr.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2xtczrlmf.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2hxovrdam.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2kkyzobbx.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2ilyxscsy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2szkqgdoc.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2vgagidaz.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2nobvshga.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2wlilnyfa.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2jjttoryt.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2autcgves.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2jqqikprg.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2udlhatdb.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2droxhljo.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2hbhzjity.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2gtsjqjss.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2aqgeqskz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2owphvphd.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2xdjlxqvq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2akuselhl.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2vldgwhsl.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2haqqjnct.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2afdkpklw.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2jftbbiwg.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2wugevqrn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bypodggb.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2tkxxjhys.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2trabwwuj.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2uxsxqpmk.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2aokfdgwo.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gaysedpu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2hplsynhg.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2ejxdjnls.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2uplkflfw.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2dbjcwwqj.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wcasufmv.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2leofbyyp.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2brbbeytc.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2frjthqrr.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2kgmoiraw.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2mtfxljub.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2xtpoexaj.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2gycblonp.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2wdbzbcty.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2mpzczzhx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2xioukbdv.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ebsouhrz.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xcipqwmg.html


<!-- 参考信息 -->