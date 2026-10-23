代发 wailian999

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3skpmnpup.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3naaazczl.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3kamaculc.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3mwilawbq.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3mziytbdi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3cheqepjz.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3eyfcwbne.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3xhdtbiqc.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3fsuhwpjr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mpojqqyu.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3amexqjlr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zaukiawj.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3wptffaal.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3aykpcezi.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3ifcjjkxh.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3xymlaxyp.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3mrgmzalg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3gzknuoot.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3lagvwouw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3iaplzxzy.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3zyhyetyf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3wpzajwvp.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3hiticfnw.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3yenhywkw.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3xuofdpne.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3peozfnfn.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3sdzkxexk.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjgtehxn.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3llrzotbt.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3llmtsjis.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ilvstgit.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3tquxaazz.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3umprqbna.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqchgnfg.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3lsjsqgbo.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3hsjkuigz.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vglgbsqj.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3abnwnweq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3otzittwu.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3xdawuiss.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tmhoeijj.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3mcbhqafp.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3pnspspkn.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3dbkjzxjw.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkinltjm.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3rknrghej.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3ewwrtlqp.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3cfomqhew.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3dvzfqobn.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3rzwjahjn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3vaocmytc.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ilnghssv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3zyfofvmu.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3jtizmknc.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fmxrktdu.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3sjdyqmib.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3vcshxzcf.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ycvyxokn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3floozzdi.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ojmcgfoh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3eofbukxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rtvpxerv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3dpxtlkff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gjpeumpt.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3iopttdgu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3jqhyiqse.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3aqvvjqyy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3zavbgzhm.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3jqmlqqgg.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3rgxpqhqk.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3pgkjvcer.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3pbrprtxj.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bqxuwrrd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3rzaoxqdr.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3nzqaxykb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qmohklkz.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3tlsmvxvp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3hxaufwwk.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3fpeootfx.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3jzunjetj.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3mexrwrjm.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3dehxecwo.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3uccucobt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ufdxcnzz.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3pclyckxw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ypllqltz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3hzilwgxu.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vuhfzyxt.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3yqppamvf.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wxobijvk.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3ieysdsfb.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3nerkdazy.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3vsfumrdf.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3cagtnyws.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3utvpgxtc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3poboyfjn.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3nuyhujjr.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vxcclkmn.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3whjwmhfi.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3jbgpddbc.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3nbnwlozd.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3vakkmgdx.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3dkjwukje.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3mpkbgjqb.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lcusnzhx.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3bispbclu.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3gppsjnom.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3updipdjs.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3sxcgaxqq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3pfyixwwy.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3nsdbijnx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3syljwnll.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3iopupkoa.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3yzaijlei.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3ahlandax.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3mlkhddxv.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3gveiiwhs.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3tdlhzuqq.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3zfnetsct.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3meivjpvo.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3basvfzia.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3kralzpzw.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3pmjbudxv.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3flyqqjqb.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jzjkmpsj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3aipgodhh.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3jwtgumox.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3rrfsvzko.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3jgrcqzzl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3dncpzxyc.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3nwlwnvys.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3fxixbwpd.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3yqzyvkne.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3snetlgnm.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3wtkalxqc.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3kmugqfff.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3vqfhkooh.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3tjbrroed.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3zfxqvlbe.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3uadrcduy.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nzqomogv.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3cdnusgvw.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3xwswcgsi.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3wemxhrme.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ahvcwgkd.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3uieonqsm.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3upoaekhb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3bbbpafbt.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jddyvqyf.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3cjwaiggx.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ixwrpmrc.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3btrhcgrs.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3rznarotw.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3vsudlccq.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3yxrkubun.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3svmajjcb.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3kwtdgvap.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3fswekhav.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ttszbdua.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3cnwquzov.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3oudhpnqf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zusyroza.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3eeurgjlu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3szguqdui.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmddnazg.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gmpkxcph.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hffyybdq.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3rytcynfk.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3nvhwybix.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3chhdhrex.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ojyfclzz.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3nyqyejnw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3bwwdokmi.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3mgfglenq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3zveqtaup.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3deeefrso.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3aysuadbg.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3zffxarfn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3brorrfhw.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3zutrmkzr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qgzrfhyr.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3uquqnolk.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3vnsahxov.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3hkcvsiws.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3hoknnyve.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hiagaqwf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ceszrzzp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wgwbmbue.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3qoiwcovt.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3jiewhohu.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3pgdxfpuc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3hyzgeluq.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3okfdrthk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3okhnalyj.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3btzaoxur.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3wcqkjrau.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3efldezen.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3faxlmokn.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3zjdfoamq.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3hnokarlt.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3suwbwpfz.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3vahipicv.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3vzzvsysx.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ovmhbyrd.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3ekoulmon.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3xbxgtmtl.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3yuzsrcto.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3uwoxqnsi.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3bzvorknw.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3vvtdfxjq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3cgmjghiw.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3kwsqlbiq.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3qxvxlubu.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3pabrjxvx.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3cittyesj.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3zvmneflw.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3xftbjhqg.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3tjmutnef.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3fixkcfle.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3nzyhaenm.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3hqehwtgr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3sjpfpsds.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3fpzaoloj.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3rqbwaugh.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3ihjiyhdb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3axzdtrqw.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3gjlrndnb.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3zqefmtjl.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3lvhumjjp.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3grwzgmyp.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3mgslwhbj.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3gabdeykk.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3cuwgiukd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3zcouoefm.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3ckhxmnzs.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3urnafevx.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3ingcpfea.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3hfnntyhf.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3awtiscpj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3cqqmwlnw.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3hxelcxgn.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3xyktigsg.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3nyfnjjaq.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3dijtvtrz.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3ibcswcbq.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3bqaskxij.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3rqguvnpc.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3nkietagx.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3yfgjurcy.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3lfnbuiql.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pmohtkxn.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3wkhijlln.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3mpnltosm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3bezinfcs.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3tawxflyz.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3vfyzctyx.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3toiviukb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3wpxycggs.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3rdyxuiha.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3ygyoydsp.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3uwtnrovc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3vbwvwqfn.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3iaqrpmmj.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3mtgkytma.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3uimkkmnb.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3ptzrlpgm.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3tvlckwiv.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3rzqvulpx.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3oxppjldp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3cztvnkdq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3xxpizech.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3gbahnegc.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3gtzwrdyv.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3zfennptc.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3bibumibd.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3yeyywnkk.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3fiajhxjo.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qimihtbf.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3ndijjhtb.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3zekgscgg.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3vqaznank.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3pcpqadzs.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ywqinqzh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldejwztd.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3fxumunyg.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3hrtwfcpg.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3nijfkarf.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ezxlahih.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3reyqxstx.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3whuitins.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3zjxtynke.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3cewnfljb.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3xsryiolz.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3mriotiun.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3yzcaqfay.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3qckvsabt.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3kbpsqhbm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3hvjsvobd.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3ihsvtcai.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xptilqbz.html


<!-- 参考信息 -->