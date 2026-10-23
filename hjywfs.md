代发 wailian999

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dpwpnpko.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3igazwyof.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3dchaiqss.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3pijgrjus.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3czehnytr.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3yhsmbgsl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3qqaxvsym.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3vmgthumy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3zmaaynrp.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3mmqhivlr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3rrnkuims.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3mpupdyme.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3fwfieddz.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3mhpeftrh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3briwygtw.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3bsshdfqj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3jckclajq.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3iuavenwi.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3gfkvcpcs.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3kodtrnnz.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3jfucqttr.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3hizmqzdg.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3grqmwkti.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3tsogpkwx.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3vpxwwddw.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3rfwfjjtx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3olpkitcz.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3zzzgsjsa.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3pmmxqqcl.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3wqrmijyd.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3gwxnarzr.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pzfyyozh.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3jtglkgkg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmoyystv.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3izdgitot.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3nysvydqb.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3ryvkqgwi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3doznojao.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3sfpvfpfa.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukeycism.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3egnuhkzi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zrceysav.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ggjdikis.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ubcuthtu.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3hkubrqya.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3psighjbt.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3zhmnoiip.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3rbglrxxq.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3sjjzspsp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3oiprffym.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3bnordhmp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3xdfznzgr.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3vyugtyej.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3povfipbi.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3mciqcxbg.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3atytvopl.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3btyrdjml.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3vnyddltk.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3khabdsda.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3csqzxmdv.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ydlphevj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3rqvpzjtr.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3usjobvvp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oiekfjxa.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3duzjlnkh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3cpfnslwn.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3uauqujyk.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3teduruhz.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3kdaegdsr.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3rvmnofad.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3gpkpvnst.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3ftzjoqmh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bsynczvp.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3tffyznqx.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3vhvxjvvb.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3vywbpvxn.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3dqesrtge.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3lomahcop.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3utlxwdzb.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3etjdbsja.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3yvggfnel.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3sorxuzfp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3dswrvjjq.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3lszjvgqa.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3xdhaeakm.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3qvhvizvj.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3uqmscamg.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3guwaptcz.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3mtzgawak.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3hnzesjoi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3ysdsclnd.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3gxygokba.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3pyuzamtq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rzpqwxxj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3gnxusvrs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3whtbhnpj.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zyfzcddu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3auvmcmuf.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3qlurkogm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3hxsdzlac.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ukbcvmzy.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3uhnmbejj.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3mzeubxod.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3vwgvluzi.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3frrnqled.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3iqlhwurb.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3dnxyjxjr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xzrvclso.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dzuoubab.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3gdclgwjd.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3dayxkipg.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3bqexsxoz.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ifmrqkje.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3hmxnyxry.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3xecaqvxz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3mpssiyzu.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3womdomel.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3ybixzcnt.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3xkpcowgo.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gsofdypg.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3aapbxoca.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3bseeouzb.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3nrdxzrws.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3idoimlnq.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3jgihkwyh.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3hzlamhmc.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ftokqops.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kbmtylal.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3kvnmpyhk.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qtyumlqn.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3omselexe.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3rdfyoxye.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3thwriwtg.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3limsounz.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3fwvurkfo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3hhuwybpf.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3npdqcvgc.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3srtnltjc.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3pdnofmjd.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3zdtirloa.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3wipfivzk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3eynevzba.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3nsbdfjbo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3atqrictg.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3ahgoxcsg.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3dgrtajyp.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3hoaftftg.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3qzeeksww.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3bwvukqfr.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3idmwsjai.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3eylbrwxz.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3kyecbjag.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3rhgucgbd.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3txwhlnwv.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3cvhueutf.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3meevkxta.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uzgmntpq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3cfhdpdwx.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3tzkitytm.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3axmokmax.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3gtyhmnch.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ajxhlklr.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3gioyrcib.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3evuvmqci.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3cnleszze.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ulkwzawv.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3zwvwamkd.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3dmpplwkx.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3tqmjunvo.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3bhjlmjth.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3ieysgwiu.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3zicdjizx.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3bxqkknsn.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3yvqudzww.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3gqixluks.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3tpjwrovi.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bwgelvvx.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3ztzmkvyh.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3aesdtddo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3hpqkschu.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3oumabxll.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3xfmjskij.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3gpsdgmri.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbtqiaic.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3ksbkpuvf.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3krczpzwp.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3rsporphu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yyfflfpl.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3supduhnv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3fypqosxm.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3cnrrezmg.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3krudkizb.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3nlgyiifu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zaovfxrc.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bzvktafx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3pgxvbiew.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3dwwudfne.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3igotkmcm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mlqwwdvj.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3waroovpl.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3sxbvxpjn.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3paplpvxw.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3eithckdp.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3vhegzkch.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hdsqodjn.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3cnddrpzo.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3rromyaog.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3uxrdyhpn.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3supzyrnz.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3xwltuunt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3paanzerq.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3cfxxcnei.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3gbyjddtp.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3bkglsspo.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3uwsebaio.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3hucnpkac.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3fskkecoo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3chrbhgvl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3xnjsumyo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bubfhhmy.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3tvjbbhzd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3bgtyjapq.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3bzyarybi.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3glcetynk.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3hivbtyas.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3luahrmas.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3ijqnnygr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3jxwgbeib.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3qvrwjcql.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dljkooap.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3dimullvh.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3svpgtgzl.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3xbqthvbr.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3ferqjqpe.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3dyrntivz.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3nrutacos.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3fongvgez.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3dytnvxwp.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3fwtlspzr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3wuncvfuh.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3sjstcqes.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3xqmtyiaf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3mldfhwkm.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3avsunypg.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3zwwwuifp.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3ameuumkc.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3havyfzom.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3aftfhuyt.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3iantnodj.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3bjzyhrhf.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3lrjqwzkb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3tyiodcjj.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3fvosjvcw.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3uxzvrkyh.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3flzfxsno.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3mjbavxdd.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3frddtzxl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3uhzxfmdu.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3znzkqeac.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3yqliwaxg.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3hibazbgu.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3nvrvjdtl.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3rorjhtau.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3ynwtsncx.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3rjaephcy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3gfrbilmj.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3hwxoklis.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xzziopcr.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3izpxuigf.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ixcumdlv.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3wkbwsynj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3wjtteapi.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3jebfrnuv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3ebopnjes.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3lamljfjo.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3srrwwpay.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3vegxtgcx.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3lukljcxv.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3ohqrnwxx.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3glisjykc.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3gscgsacp.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3ddtulndm.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3dpvoqsid.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3fsasxjzx.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3crzpgqfy.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3ojnslhjl.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3gkqgigfl.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3jqctrdbx.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3eofjueux.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3wijmzpht.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3tmhmceaw.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3ddaviazh.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3kdlcyvzh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3yjyesflz.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3lqtawokp.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3gktbkvho.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3cmusgfot.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3lcnpjixg.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3pgcbfise.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3hqzmuucs.html


<!-- 参考信息 -->