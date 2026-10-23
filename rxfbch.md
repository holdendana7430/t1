代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3pmhxjxfv.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3soofyzbt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3ezcrqvtw.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3qhjazrpj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3mqihwysq.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3kqtpqkaz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3qsoohciq.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3jptspvoo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ikymotoz.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3ullypbsi.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3vuexofox.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3pdnvtkaj.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3euekmsxb.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3yghmayda.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fzbthmzo.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3hsgidnyq.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3slmyvhhj.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3xurvccra.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3nwhimpwo.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3smxtbxug.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3gateundg.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3senhsewo.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3nhicmupu.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pocmwaiz.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3emaibmmd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3hwtcbvsm.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3daggores.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3qubgpmjg.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3ilfyocdz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3xayyovrm.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3vvysbntg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3opuvnuhe.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ummscwbv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lslzxcbc.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3nacpyqhd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3djuqvqaf.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3tmzlqqet.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mctzwtuz.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3lxtoxpmi.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3uppxfmim.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3bgbvblad.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3awnlpvaw.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3kukwmlwj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3rfimrvnu.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3alhbrctt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3pzhdkuei.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3jdwcvohh.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3oscxihet.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3ykkowwvr.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3akysedok.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3kqwfglag.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3kjuubflp.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3gajxmbrk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3bmrmkkwj.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3hkbbxrlb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3apybppkz.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3mhdiqsqt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3opqpsbkc.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3cdvddvov.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3fdnfqqog.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3mazuyjhi.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3vwiplpgv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3eosxnxnh.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3tuldiibh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3usefdlxp.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3nxbubxtd.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3xszeksfx.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3rsxcxesu.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3muuaddas.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3wpelajtz.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3hyialdag.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3uuxhqafd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3qzsnjcqi.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3uoghgoql.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3whjlzigq.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3drihaiwu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3wtjneovl.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3nypxweuo.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jmqivhav.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3audtjcqj.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3mcjdzqgh.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3omwllnhe.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3zvawdlhf.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3gxwegfaw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3mggxrifh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3itphnhzg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3jdypwdys.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yegecsxj.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gweftolk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ntfyryos.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3jlwyrtnj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3zsosrbjl.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3zgxzkyus.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3llyggmzh.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3qwzilqst.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3uqnvofld.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3pvxtkpag.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3rtmjizly.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3oumqilip.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ahbbxhcx.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3laqtlkzs.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3anpeprvg.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3oalkbspx.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ksrdubkd.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3qxmwzsoh.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3yqncnglt.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3zukygezs.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3bzhkvxgn.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3bsqrlqpg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ncukkybn.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3mqammidp.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cpbdqejt.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ewuzamfa.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3elkfcime.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3bnilfzga.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3vmowfumn.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ltjyvigs.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3rjyqvtvw.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vqsktifw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3aqlehzvp.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3rplzrhfh.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3aaxqwbgx.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zwajgzie.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3wtppftii.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3emmskfsr.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3kxgenamx.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3smcmapjn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3fwqolzkk.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3qpkswwqr.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3xxmptfbt.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3aleeanlf.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3fhtkuvls.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ljcctlyq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3skmegktt.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3nhafjwon.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dwxfuptj.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3jkyarhdr.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3bpodieqq.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3pgclhiza.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3zpbzypqb.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3knljjxsm.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3euzivnsq.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3pvpevuam.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3omhhgbvg.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3szjqlfwk.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3kghquxqp.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3umgwbser.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ywfoyozs.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pveelbeh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3nqrwnznr.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3zzdtaxnf.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3gwqzapvy.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3dniljrbl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3omkonysc.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3sqeqzazm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3zbifxtrw.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3hfntbaan.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vtuhochj.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xzxusmsw.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3pzquxglo.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3jjgzcsog.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3wbopsnip.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3ubrwfqpg.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3nlvvmpqy.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3seckrhst.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3bjocispc.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3rmotcmgm.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3poguziik.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3exnbkldw.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3mukfovpf.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3rehhdlhz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3topdquyx.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qfnxbilk.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3gxteoniz.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3abifvxqi.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aglyqqzz.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mddnqtis.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3bdgehpmp.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3pwxfdwov.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3mstxebyr.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3pnyahycz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3defseakj.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3rbqwudtq.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3xagwwgpk.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3tmxoeemd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3isfzmjdx.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hljqighs.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3hwienwlh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3cigeunlb.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bngweiwm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ldihamyy.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3onjycxfq.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3emmaqesk.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3awpfytai.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3bvlioqqt.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ycmqshxp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qxxndljx.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gmxmqvlc.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3wpvwpgmy.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3xuzslzhq.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3begijwjn.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3teozeios.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3vdjosyax.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3bxntppyn.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3fnxdtkdc.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3khjrmxhv.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3dmxypitd.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3coinywyu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3nalubcch.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zyouvcba.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3uhpdojyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vlflmwdz.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3pnkcguth.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3bxvhpinc.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3hiolvhnh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3lxdvoaiz.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3nfobaimk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3acytrfaq.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3bshphkgo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3gdlhxyae.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3dwjwyaig.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3brprolat.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3ifxqqopq.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3obhdnmst.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3aytekmec.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3undyimru.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3hasuojid.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3milgipic.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3gylrskhw.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3rnfhuzpn.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3vvzpedxj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3tymeriuq.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bycmtgnu.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3smuqvlmr.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3tikgbqnm.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3bpdqxkff.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3efsgjcua.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3mknbcqum.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3mifdjmzk.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3rwxyfpud.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3bvefvidp.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3nxfcksbz.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3oiqrkaeu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3zzceshjf.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3pmkeasfc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3jbblovwn.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3gxfbnroz.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ezvjwigp.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3lprnwsns.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3zsruzobi.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3qioxqtjh.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3pgbcuphd.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3knemgfkv.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ibrzcdvh.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3pxmxggqo.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3kyegjvzw.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3zpmrwsew.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3dsgldemc.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3unvnqlte.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3eoocqbot.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3cafsizxu.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3ibfcnwbp.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3ypnvwgdb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3xuegkydz.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3ovzcyghp.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3ernbxzjf.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3bewizrnu.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3osxbjvwg.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3kjsswkoi.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3xtmjhtku.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3azjvezfl.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uevjucxk.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3zrgghwon.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3hlvooaqd.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3rautqslq.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3mlrmdmmn.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3fgnhpuzh.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3epkpjurj.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3imomsywq.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3usstvmts.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3ilduqzzt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3usbvrtqh.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3fcsgyfyg.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3tbppdzvj.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3ywrzxhim.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3dixarouj.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3kolebcyj.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3ajjmxyrd.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3msldmaog.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3jjywdyju.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3alydesgv.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3fmcysrgd.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3wyibhsye.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3uvmwhhmi.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3nkiclfpl.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3yletxutc.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3tpullpwd.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3vajvdnzx.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3kmcqulzs.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3bubcysjy.html


<!-- 参考信息 -->