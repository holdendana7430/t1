代发 wailian999

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3jfjqrjyw.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ujgprozt.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3rhefocqz.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cfowfehw.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3wenrzwrw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mlytxzff.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yhmpvgzc.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3sjfennzv.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3utydwjaa.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3hscizrat.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3bgfhopgn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlsrrbfr.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3lchkjxnk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ftlqxzqs.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3tnidfdao.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hslawifw.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3qccbmiqf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3gsccznfe.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3pulnpxgw.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ceqhcvow.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3ukkdlpnv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3jyxlpdbd.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3iizbkchh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3rdahszkx.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3cvhgalvp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3irisqazf.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3moqnjlnk.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3vanwtjkb.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ufjkczui.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3cvfrhsfj.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3aylvsugr.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3qgperafa.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3umypyegg.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3sqouabsd.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3xnigvcbc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhkowlhn.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3eufmptcv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3atfccmis.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qtmhkrhj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3vqkwlubh.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3kcevgujx.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3vsofvqgj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3xjkcjlmp.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3ojjlwlsp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vjoeapkt.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3kwoqyesn.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3eiypthvy.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3mnqxuhkd.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3dbeeealw.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3bkrtolyw.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3lugbzjmz.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3wgrllfiv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3rlwavfwn.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3dvisxdlr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bvwoowwi.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3tujswkgx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3wklxrhfi.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3fxqmcybc.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ewftvogf.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3fmakuffo.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3vqbzxrqz.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3oflmdzpz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ohnkhbte.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3awzigcpv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3notujapd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3reyxrohq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3gexnjotb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ffwzlwye.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ufdyhapm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3brpybhxe.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3cdjkuskf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3ecwzmyds.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3cojyzwvq.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3rhsgktui.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3tdydposd.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3hvomomob.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xdolqlim.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3ojbycmmm.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3rgvonlqw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dawhofqg.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kyxuuctw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3dczehixt.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3hjvtsguy.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3minxuycv.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3bbahjkct.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3europuir.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ldakrjzf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3blbnfpka.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3nyucwvqc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3exrazvmm.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3uydfvuyu.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xhrikmlt.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3pdkmomiv.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lpoltecy.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3cxlkvsry.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ccephzyx.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3befdjxtu.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3xjnetlza.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3aynnrbwk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3yixjggen.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3xnhjsdzm.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3sudfpyru.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ayclaogg.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3bfhyrcga.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3arjuiggb.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3bhufglvv.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3nwgakmcf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3gfsbpiqk.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3rfgrscyt.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3egztpdey.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3fchtbwml.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hzqdxruc.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3gudafjlf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ednzfhqh.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ouqasdur.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ppiuqpim.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3lxcfrzdz.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3yrupqnvz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3firqgdvr.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3uamjcxfd.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3nmasfgxr.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3utsyxcet.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rlvipsot.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3tvieffzg.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3mjwlgsgg.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3kifacsud.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3pgxdinxv.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3zoecmqdw.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fattmncw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wmsexfvb.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3xtkxrmxz.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3fwzttgvc.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3nnnoyzdx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3xbpwamkz.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3dunjcksv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3jtyuqotd.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3okcbcaot.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3prmphqge.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vjjvxnpw.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3himewplt.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3mlaweulv.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3dnnmrfcr.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3yqabqtga.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3dvtikmiz.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3hykueulo.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3lgxtgrgs.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3scgsqnut.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3xhxzljtk.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3axqsaqql.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3toyvdmko.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3mmsmwxsb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3lpfepuil.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3eaxfejio.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3ulnmrcas.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3vlpscfzi.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3lxpfnvvi.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3klfotfcg.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqsqeqzb.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3omifuyhb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3jlrufmtl.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3bfhgkyso.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3fyjcnnke.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3jgjnpdgb.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3qoeempai.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3urgdsyui.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3yadzztpr.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nqwnkppc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3iwksibwp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3vrzdcqtt.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fdpbztag.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hmhwtwjq.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3jqjkeewv.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3lykpiujz.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ntxxbsej.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ilvaejqm.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3jhantuxd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tvyxwjka.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3fcxscbry.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3niwwfpvl.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3fdjvjxdn.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3lpjjnjmi.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3feldybco.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3iyouuypl.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3wlrdrzzu.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3kcnblskf.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3nopsrlsf.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3xazfhxyu.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3zrzbhwhy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3kbcwcinm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uwpctosd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rtekreom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bkoepwkk.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3bhijjbvj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3xicrqhaa.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3gcpleweo.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kgidnxnd.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3zxbttyqi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3acgwralm.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3glvvvlij.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3khvxpoxk.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3wqgzkbju.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ycolgleq.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3nyyeafke.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3lkyogfwo.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3iyaklndt.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3majlvlgc.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3qlfmhurn.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ewruofbf.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3qlhjhweo.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3mmuxgkdo.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3spwrsapk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3vficxsoq.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3ofvrhixo.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3bssenakj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3amtzsshj.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3nizfmukd.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3oqmfvqfd.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3cgfafhfh.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3vvpiolsi.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3dydepxuz.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3zaofgcty.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3zhcathnh.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ktalrcmn.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3tmdnijjj.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3qftdlwtp.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3vwcvptqk.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3umrkwnjs.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3uxqatbmo.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3ojvgglnw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3qnzxpgpg.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3xprpmsht.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3unmjogko.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3xqarfggx.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3hswlvncw.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3jtqknnuq.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3kpybnqqm.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3fsnddgos.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3ofsstxzy.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3ihtjwexd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3isropemu.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3jcbrfjno.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3rcikgvji.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3idsuqgfb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3fttcjmql.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3ccsaklnn.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3etsdearh.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3rpxwydxr.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3vwxzoxpt.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3zofpotaz.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3wcvimwks.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3otalgvps.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ojmabvrq.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3jgownxra.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3aopbsrze.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3omcnliic.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3hhqimixp.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3extpuhho.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3zsfnggpe.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3mawitwaa.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3ftpdnglf.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3yillhtsd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3wrdgujzs.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3tpzbstsx.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3jehhrzko.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3tqvanyyb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3uekltylj.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3eustoptj.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3fchebbtr.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3qvjllfes.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3tdrrvmyo.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3dybyaedl.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3hssxbshh.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3aiqtnpxo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3ycpwaagd.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3iwtssscu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3vhhywtoe.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3gznypfhw.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3tomtddkl.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3ndvrqlce.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3curjeldv.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3rtzzayqf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3izrncmys.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3prpnmwkl.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3yhhcddxh.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3mfcgscjf.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3hpjqajiq.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3wkdggnqh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxzlumzj.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3ffprrcsp.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3elecjrjy.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3wbluvqyd.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vuzruxeh.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3aogfzcty.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3cgjytwdq.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3kddgwxqn.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3tzimvyqg.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3yotcmobw.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3dpaqwgxs.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3ggggxqxn.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3pbtttygg.html


<!-- 参考信息 -->