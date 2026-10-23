代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3wphgecke.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3kpxyogzs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3vvghlvuc.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3xrnzxurw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3wqigpuzn.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3uktotatw.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3xsyslfbh.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3gfivozqu.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3dnsviiiw.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3orcvvpkk.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3iyhlegud.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3zmcxjyev.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3owfgsygg.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3zbpxmdch.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ecdkngpo.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3kobxxoyq.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3gvkkgfan.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3dkqvpnxr.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3tsmmuace.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bepbhyvw.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3qxestoxd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3wxwjnnpr.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zzakbxfn.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3jaafsmak.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3ouummhfs.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3mecfxlry.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3obcblqfc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3hwzfcufy.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3nzfnczck.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rhdvcdja.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3jrtmiehj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jiulyhzk.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3eefmaain.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jpxwsytn.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3lmjcezen.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3vfqcfpwj.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3brpulbdv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3fuvcqrxk.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3mafvomeh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3vniugbhs.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3vhixsmgj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3gagelfha.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3krpaiste.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3jkhjieov.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3kswlqoje.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3mrqhkmmt.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3kgfzeirw.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3jutdrzou.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3bbwhtzui.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3getlgekk.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3setmxusc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3dgcbtrpo.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3plkhyjzs.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3jwcgbtaj.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gnnpudew.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3sltsgtbg.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qhqahndd.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3qkmqimye.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3rihohefx.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3bmvooorz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zuwhknaz.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ifbvxcgm.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3kcpywffs.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3zdjatpwr.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3cbqqtmlc.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3fzzeahfc.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3fuyckydd.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3jzhjohgb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vpgvjhyc.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3fvnhamgo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rlxljhyp.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3azuqyllm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3qccfehqi.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3ufzhhbvk.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gqbncyln.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3isjiejrv.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3eyjelzej.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3yexckble.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3oxydfooc.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3hrslhpfk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3rwfozkrs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3puceijbu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3zkrbhmli.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fpwcwbud.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pxsiwunn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tjjcxowj.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3xuahjqek.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3oktddsxp.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3vqydokbr.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3mdrpnrwf.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3jvpxmvvz.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3yxewngrz.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3kveiotiv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3hpqgzwsh.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3pqyzlsev.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3sbhycdor.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3tuxygmpo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3barmixpp.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3dmxbqzga.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3bbmetfvs.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3zsuzyunw.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3yjzvhppq.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3eoiesrbk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3xqyfslwu.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3rohtbuvs.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3ejzyolia.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ndguuwca.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qytvdlna.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3sekwlgos.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3gbqnjemp.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3tqxyvave.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ngeqqhhj.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3thfexmon.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3cmsaupzs.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tbahztid.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qahfpmfa.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3lcunyoth.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3hgaizxwh.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hcbcigns.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3tlvlqhon.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ddphxfqy.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3bvwzcplb.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3szslqaty.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3wrjybxrw.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3vyrffwsx.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3glmgohwi.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3vrccdpeo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3osmwtryo.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3nzjauaqs.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3dwuzusxo.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3jvtnpwka.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vjbxnxhk.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3hxaabvcy.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3lkhrxoac.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3kqdcgcnw.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ipnmfgtg.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3mcurknzn.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3ptnlbhyx.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3cqhxjywb.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3jfciffom.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3oyphgvqv.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3sfugghxm.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3rpqzljpg.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3wrlwlaei.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pqwhrcbp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pphyvhzx.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3qivuasta.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3qmqupvxk.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3auiylbcy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3rkhrwwry.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3kbutffuc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3cohnrreh.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3qetrghzu.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3iukivtee.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3rdxskbin.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3oyutvqjk.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ponxcefo.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3mdupyomh.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3fshxegru.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3sdrvocny.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ggfcgkhi.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3vzxpsqkn.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3eawpgaat.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3roekihpa.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3prngtufg.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3dludkhar.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3hfvluxow.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3nvijscmt.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ihdmedoi.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3tmpmiuuk.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3hjnvdgjy.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3asdansnu.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3zzmdxmwl.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ynkabdeb.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3wmuvsojc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3xnlqwmwu.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3xdttppdl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3exmgijli.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3yrnbwlag.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3hemruzqd.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3ewkawbzx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3menuauqi.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fckmbdaz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3myhxxpls.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtykqyul.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zjvlezee.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pxxoqcrk.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3izrowusx.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hjdaamkl.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zipocdxs.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3nwofduqs.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3duzqyzgv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lxphqcyc.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3uewevead.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3rvwvvdee.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3cwnqphyn.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3zfdtgyhb.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wvdjknpz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ldqrhkcm.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3tlwzjmpx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3tvxaiiqg.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3hlqgkvus.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3dxlnrgvm.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3havbfqhm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3yirqyxad.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cclckmod.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3srvuyvff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3maaidxtb.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3dkvsgtkd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3bsolvkie.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3oksnccwo.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3hcdunjwa.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3vkdwlxor.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3mgxokasq.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3edadkvhf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3uouocass.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3miwdmotu.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3olychcly.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3gvmkkhhk.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3dbwoipul.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3kwdtuato.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3eosmjsoj.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3qqqohvob.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3bjphfopk.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3cdzoakxy.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3kpqxwaft.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3kmtyjtwo.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3uvsniswz.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3uqwbnxjc.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vjekrzrl.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3zbntfnmi.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3cubkjuvr.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3sbcfqzul.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3hgemfigq.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3emdmruku.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3rktfufsa.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3mpzzyzlk.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3pxmhmfdr.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3jbzwlyhp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3iefkqdqc.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3qsnjepbt.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3aldnxrgd.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3grushhwx.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3damtxzgc.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3jkwthmsd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3kbeiqtkn.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3gpzqnhag.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3ofdcojcl.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3buoaxcse.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3luwzzhvk.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3wmuefmou.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3kgbztiwu.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3nxittbvj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3doxmpwkp.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3iyxcaxkw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hhqhflyu.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3fgcxnphg.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3aqaicpza.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3tygjmotg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3tkoangxb.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3mghgepli.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3dfzugpfn.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3spfprbtn.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3acagpsdh.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3kuqjozfa.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3bxgfcekf.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ggzvdoxk.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3agzeeprg.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3fonqowek.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3cvhweuqh.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3rzmkuzid.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3xlpkofpe.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3yxhlknvd.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3mboqvdgz.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3bysqaebj.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3djmwpjce.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3lafpsylg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3ckeznnlh.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3pjqzssdn.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3rmpudeln.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3atweaexa.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3uhwfiwlt.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3mxmivtgt.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3kowvismx.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3wsacqyub.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3cwzrsgpb.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3ofuijkcq.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3icjgypkr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3tkqkabpe.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3tcxfwtks.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3qterixiq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3sgtmjcwm.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3ypzqtaqt.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3apymhjzr.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3fsejvsrd.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3kxlrhrtn.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3ihwmghxq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vmlkmhds.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3kquleqya.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3svyhqtii.html


<!-- 参考信息 -->