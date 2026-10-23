代发 wailian999

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3roxfelml.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3pdsrfebx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ciemyvvq.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3lizehbxk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qezwlxus.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3fxmjycoy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3deliefdo.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3zavdepvd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3zpijcsej.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3akzrprxj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3wfmjcbta.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3idfnpcya.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3porzvlhy.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3pogamxzk.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3pxabowrs.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3xobngztl.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3zktrsbdc.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3dqamkscy.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dhirgvbk.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3zkjkykoo.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3gdhnxsic.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3crzeidhb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3bvboprcn.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3varplfbt.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3tvfpoyqi.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3gclezses.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3wyltheet.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mvuziefz.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3fwcjpzcw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkhuhpfj.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sltxiyhg.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ddbfrgaf.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3rhihhxsq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3gecgngze.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3urozooje.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3chriuhvd.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3oxfwouow.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3svqvbyff.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3zusxcrmz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3djvsbowa.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3jznnrywk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3rtexzgza.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3iidaunhl.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3vhgmmqbi.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3zfbqyqgd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3lzrcegfb.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3xvclkakv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nbabpran.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3spqcmsnn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3etuaylom.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3glztseog.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3pfkkxrkg.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3huifygdl.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3aaptwibt.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3hmmibzjd.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3cmuboxjc.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3jbudelkg.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3jlzjwldd.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3wqketmur.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3pikykbxc.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3eusvlwvl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsmibenf.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3uqpttmvg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3vojmeipc.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3dvnlbuuk.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3onblvcyc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3fbfnvzev.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3qkwpxhfb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zboybcyc.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ioerjesj.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3nlauydol.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3ktzvdtgf.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvjvrbna.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3aciikldm.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3pckvvxfx.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3alazdtav.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kqxkvrba.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3vvoaaaou.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3moxhdaay.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3dbqtrukf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3bkxkaela.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3vawlomuf.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3cpwevxui.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3qbrrssag.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3veczcljk.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3iudlizjl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3mgoapzry.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ndoftxvw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3xtivjhik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3esvzmpwm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ihdkcqqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ztsbvyhh.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cbmfnwpo.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3asqxgctu.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3svsardwb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3nayfhlvz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3exuqayzm.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ytwvswqm.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3fhfothun.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3jqohoyrr.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3tyyrjlgb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3tbpvjdfq.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3zodzmqvm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3wyfwgprm.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yngkdknq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3cruasatu.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3hocxhzkf.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3zmbglofh.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3bvjsarrg.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3jibhefgl.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3coyqabwm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3kbnlitqd.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3xotmzwni.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3muzjsqoc.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3nfoiluxo.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wuttkrwi.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3qkyqswlg.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3qirjqrdg.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3wvtjjlee.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3rkenoklr.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3zjnehyne.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3xdeetsog.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yvalhble.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3svbdmjic.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3tgubhdxp.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3unvprddp.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3caklygxt.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3axvegutq.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3bfzxqwhk.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3nzmlbjdw.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3bgueijtk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ikmbdazw.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kaqctdqi.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3hqngpjsl.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3zltxobal.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dpwzdihy.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3opepkauo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3piisevaz.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3pywknupv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mzlvfdbe.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3oeuejjjt.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3hwhvxlwl.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3rpgkbify.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3vllqldmd.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3rhswixpe.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3dqrqulgr.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dlhoahfg.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3dhrmlznz.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3evvfimvs.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3spudlfvq.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3iqkwsemj.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ogvejyyh.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3saakfflu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zevjpyxa.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3yxiqxsso.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ucvnttjg.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3kyuqrxvw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3tipnwgca.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3ybnufebr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3rxevvgzr.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3bdgsfflu.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3umkiyzel.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3wmggtvwd.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3gmafbqth.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3eadpnupp.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3lyczbgtz.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3xbzbxqbp.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3ytekokpi.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qvynuyjm.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3foeuxske.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3knyyioef.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3vfrivgum.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cqsjwsis.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3gjlyxrai.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3xwpkdkqr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3rpkurloi.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3nibihanv.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3ckmejhzc.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3drshjisg.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3rctstahn.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3jdyluuvd.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdzzdrvy.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3sefitdjb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vhuqpqaw.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3xogunxzw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3lpiwdfnk.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ppvnmrew.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3wzyjpszx.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3xruxclds.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rtyqpbol.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lthnjmyw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3umhrcmmu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtrrdjba.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3itufqeco.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wchrkhsz.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3ibhnodui.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lxrocpiz.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fauajnje.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ytmaxbyr.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3szcfxevj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mmxooqjt.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pdmidtoy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gqtbdktv.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3avkcpwny.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3hxfwcnls.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3fxpjhpxl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3wojomekc.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3kfuvciui.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3hkdjrvdx.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3hefcuiqw.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xiskyipx.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3tczcnmpn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3hpkmpmui.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nfnottnh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3miniqhfx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oaersqqq.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3mwykqaub.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3cxgdfukn.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3anzzyyop.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xojyhiad.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3stkrmusn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3itttsqhc.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3wfuonvmh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3xrxrftrm.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3oluzzzct.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3mcdjfcvf.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3ycnfzfpr.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3mygivdky.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3itgwlbqx.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3cdclgily.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3fvafyikv.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3gzrzofyu.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3qkajcjma.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3nwznhqwl.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3yddicpwd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3xioxvhdz.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3iidwnqqi.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3xtfubumt.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3izelczvx.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3dfzmwqgu.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3bqunwglr.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3pfusfjnw.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3eclnawcj.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3txhekgoo.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3tlprqndj.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3opdzagmc.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3mhglseiv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3vfshaqml.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3oonpfmeq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3durpygbd.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3uavghvyy.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3mgmrbwal.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3zcyynigp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3zkzywlnr.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3ssdttmfp.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3qalubyau.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3paglxlzl.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3cosdpsiv.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3enqtaerm.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3nwzkrebd.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3qopuvnmb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3cagicxgg.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3ceaihxvc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3imjuztmj.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3ganiefwc.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3mveuamcq.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3zsindqwy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3bmqgfgcz.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3kzoxkotv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3emgftfnf.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3nkxakkox.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3tqeaqrox.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3oupsyfwf.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3lduftgwk.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3ljzavnir.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3wuxqmvhc.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3akatnjum.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3cijzmnnx.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3tkixejus.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3ipghqcic.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3tniyftru.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3fpmkduva.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3malxyxlj.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3rghgqdcu.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3bbfkmmdy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3fdzwccxt.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3gaakejlb.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3obrrcofq.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3ekmqcjkv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3gmoowrix.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3sqqcisxr.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3qfjwjhje.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3kaoyngda.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3xitmukie.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3xhrudeod.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3wvzznhvx.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3twnqqrck.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3zjdfnabn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3pgspwrbj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3vjeefhlv.html


<!-- 参考信息 -->