代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3edxjmoar.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3smefzbyj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3pgakewto.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3httjedxk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ebgwzcaq.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3kwtgdztd.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3nvnocqtu.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3frwmrwid.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3tmoxyoqy.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3fyebtmsm.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fbowbauc.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3fqialmfp.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ucgmspvx.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3pgtyspqg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3qmtthgoq.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3cpvkssvz.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3mdukygwy.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3vkenzbjt.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3vswthdip.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3agvlmnbx.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3yixbaggq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3zirskgjy.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dxzjgyro.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3cbskrbuv.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3kxannruy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3kludqhef.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3wcaoeceq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3zxqjdgzo.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3llujelej.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rojpgaza.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3surfjzsl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wiutwqyq.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3klngpoeo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3eypskfet.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3hmzxhscm.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3unvvxlqv.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3eulvdnrv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3fgvlalwl.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3wbwmighj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jqmcopxd.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3kfhflgun.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3pdfvchyv.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3aevboiaw.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3hubwlzpl.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3cwwxihde.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3hijpylgl.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3kqbdhamo.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3rvmkstmv.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3fyrxejml.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3bamlkkwg.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3yqeacvnf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3frdwtqlc.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3oywfpcgq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3atladgnv.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3oityqbsx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3qqjdhvga.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3taofvuos.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3pwmfocci.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3intjpwjc.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3tpysqotl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yqpekfcm.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3qcqumxzv.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3kjosnsgc.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3scsyqhdi.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3yzjywtai.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3sziebwyg.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3cqfyngdo.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3rzuwuvog.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3lbzayaap.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3mvnuelzn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3vwdgkpga.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3fdqthfxw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3twwzrtoq.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3ixsugeqe.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3pcelwgyz.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3xhqvnzmp.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xdfatfis.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3aikhmnxv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3kjhktsjl.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3rmtxlwhd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3zpnxshny.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fbymqacn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3zcpqsgtr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pcmsmery.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lvfotoqi.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3eqcwcsqt.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ltxwsllv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3bxnuqxgw.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3zhlbtujl.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3glelxxaa.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3ojpkkkqc.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3bdvpcxgi.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xcbusamh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3ibuomtrf.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3knyxvdrk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3objlimwz.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3gogatvrq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3grroqeox.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3aeolknlc.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3avywcsjd.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3czgeyjtt.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3uiiiinpw.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3jtgwftwx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3ijumiydh.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3sbzlylqq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ytkwsulm.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3banygxny.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3aoympdzv.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3rsniyuys.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3lvwbjeqb.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3jotdawhx.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ejylcbhn.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3yzzaubti.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3hdpatmib.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kvmvnxuv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cdmhmvgn.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3qtylaqqh.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ehmtcvkj.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3isaoweim.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3vacpsgau.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3dssbxsfb.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3cgeunmfi.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3kazwxsyz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3rpnczgdt.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hlbajbzm.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3velbqtff.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3zoobhwbw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3qugctwjk.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3rabfveui.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ylikjzff.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ftbsfzty.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3frnwzmwr.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3jaovhmgc.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3wolecjnv.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3hcksphlv.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3hzjanzko.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3sokmjzij.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3zihjdnip.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xhjittsp.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3ydjiytsb.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3amvcpzua.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3zidfahdj.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3xbsmhybm.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3lknjomwr.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zhtipqrc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tiuvpcyw.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3plhfuogf.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3atxidgrq.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3iwfllenc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ggfqrkti.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3rankwsho.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3yzrjwfjs.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3ohpnllzq.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3vcclnpaa.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3wfcargdp.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3qenarlww.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ofuucbpa.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3enoszted.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3bukkioxd.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3pegufdfu.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3cifnhphp.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3gymrnqsc.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3idrimatp.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3iketvgxn.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tooitbtw.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3oubgdsqi.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3qtribibs.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3vvvvhqng.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qguadebv.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3jqqpzncw.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3fisnmwud.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3whdzmajj.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3isoajclv.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfhtappl.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3giblugvo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjxrdqwk.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3saofvhak.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3fvcpfxtc.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3npwswsai.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3lfwzlysl.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3cszjausd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kwpnmohq.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3egppockl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3hdobwzff.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmewiwoo.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cgrlitul.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ncbqbkgo.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3ocvcsbkt.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3dmplfuyd.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3mibkfxze.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3slhsmbmh.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3radysqzr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3bvhspomn.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ybkuyyfu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3zvxxzvpg.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3borofnun.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ypxwolqh.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3afywszqw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3fczmfyry.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3yjdojtmx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3lvghnsfd.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3rqnhclvu.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3wpryreva.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3zdljxabm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3tshyplrv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3flbacrdd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zsjjhwwr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ubofayop.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3ovrpwrft.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3xeoacurf.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3asnddygo.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3gjzoenjz.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3vbeamkgk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3grjufhbh.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3rxdnklzy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3rrzlyxwz.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3vzdpnhdp.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3uthzeyfp.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3aqmdlrqd.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3yrqafxrm.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3mlwznakv.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3xhkmvhnd.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3rvhvzpar.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3nwsbbffd.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3ewuaopif.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3xshuwpwz.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3twppztmj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3wqtrpkwp.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3mdgofggm.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3fgouenqc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3reifhcex.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3aptbpzzl.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3nhlykkqn.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3pxlmmtkh.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3rvifpokt.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3mulsehmh.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3xkaeeqcy.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3xtvsaxjq.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3uzgcbsqd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3gusnjzsr.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ufpkjyqn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3qrxuzory.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3xdqxgpms.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3xfsflrwv.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3wjcstsei.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3mbtcypxt.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3usouxdqf.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3jyvvkihp.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3ebnvqawe.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3cvqsndyt.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3appazudl.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3bentkqou.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3zxgeygvr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3ysbarvzw.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3wmpiawjs.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3khaqrszc.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3dwllvxtp.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3ttatdeff.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3mwpsbbiv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3nxyyhfnv.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3gsljmrmz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3xervpuxd.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3qtlumies.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3caiheuiv.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3uwubssth.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3fuyccafr.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3nhkimjrs.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dpltizgu.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3pvobxqhn.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3exeqihdz.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zbnhehud.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ptsazxrr.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3gyiblyqr.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3fxltsvho.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3ovixiivb.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3uwijvapz.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3czfolznq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3sokywfsf.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3fmoslzsd.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3urfjrokb.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3pzcgmlqz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3kxqwzgcv.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3butpqhco.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3yxmjilsa.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3tjlthoeq.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3zpwrpopl.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3fxbefmbk.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3bqdxchqo.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3lwxnwrmw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3rwrdqaea.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3qtfejkee.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3pwtrhhyn.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3jjkgoizu.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3ucwmlfyr.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3nnvcyhbg.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3czgsolcv.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3meybhcnw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wzqwvqfk.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3lbxyasqr.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3lfkduefn.html


<!-- 参考信息 -->