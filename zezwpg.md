代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3lqrjsqhs.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3zxdtfrug.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3wukhcxii.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3zyogmluj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3zpiowkua.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3vbfacxwi.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3zkqtvksu.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3czgjesbb.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3solpznwo.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3nwbjsmge.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cynsbjio.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3buhlzzqx.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ttxrhqyn.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3uoyyqyzj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3mffbsrbr.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3mexiwnjr.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3dslawkpc.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3sgtummcn.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3jskrcglx.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3suvqzjsp.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3zwgbdvpw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3nqxedofz.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3jngyypzk.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3xrqlnkxy.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3wktvlpys.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3xffxjcad.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3piewbeva.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ywpckinc.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3zdglrcdv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3brkslavj.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3lebgdhmj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nairapqt.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3dsqvmvnn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3vfxukpmp.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3bukysnoc.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ttlolvoc.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3wtuhwyvh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3wlnwwxcu.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3cpouinty.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qgjpgbiq.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3zifrtkwh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3mnxremct.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3mltwhvlv.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3fyonyyla.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3etgituyv.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3lvgmgpuq.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3vasfczqz.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3upzyitqm.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ztijxbok.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3qppekxrv.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3gzudgnyp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3avbrvpei.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3cdozkqhp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmajssji.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gymvpsgo.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3krbmdsue.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3wyimaxxv.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3aglfpzpp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3veztrdjo.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3rvwaitrj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3obwegrhk.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3dxprzfam.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ggaeammb.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3snjeormp.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3jexouqcb.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3venhzcoz.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3rrygxzpz.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3ieqpbnwv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3sshtarbn.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ujyghjlj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bnzkmvxh.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3aujdayil.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3bumsjjjt.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3dqlslygl.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3njbpjikx.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3aeocprdw.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3whpqhjmx.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3nfdhejnw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3onqkmaqb.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3puvckitd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3goqzdytt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bseauiwc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3tjlyiuxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wbowpqee.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rgkenzip.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xconcqgh.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3kaxzevuk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3xfaxmsrs.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3wfgejtnj.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3hcdphvlq.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3kqoabsof.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3kttjpqix.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3ahpqeyhf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3uakieeaj.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3jzhpmxmb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3aheeljqi.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3xolatcam.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3hcgntnva.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3meoooneh.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3crofqnto.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3dzsrgcse.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3lftxdltb.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3uwswjhoi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ccmzacbu.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3fypukfzb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3jxkxzrrc.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3bicesqnx.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wslvdkgm.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3edvfkzda.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3nccofdit.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3hvhibxbz.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3vjnohnkf.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3zntfaidd.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3vscdjedl.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xtqcglzx.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3htzfnpyn.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3tdpohygj.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wdozhwgz.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zlrvcyvl.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3vhueofkm.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3acozrsnu.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3mosfnowj.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3xgozweok.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3rxmbcnsq.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3okqnvptq.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3mnqbcriv.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3gygtpncx.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3tzakcwja.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3uulswmvm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ewkzhrfd.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3aqftvuze.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3asxkitjy.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3rafupnus.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3nlrvvyri.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3fziwgern.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3nvikixqb.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3eebqrrre.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3yzkmzaoo.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3mchswvdn.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3dkogyopj.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3fakxwwqo.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3dwwgckot.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3qpigofgv.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3fckzuinl.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hhzigyys.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bzjgzils.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3bjzrubys.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3wwtpdsnu.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3xvcemtkt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ledymnpj.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3kmhmbimb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ureuzwyt.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3gbhebkmy.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3bdqjnuof.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qzkweqfy.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3merkevwj.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ksrgelpz.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3wvfqxcod.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3lydrikep.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3mijapmrw.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wcetavtc.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3vymtodie.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ejhtdvlf.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3wqktgnqv.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3upfmaont.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3gqpetowf.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3gqeytkya.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3eafocywf.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xooajswz.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3pmnlyagl.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3qnobanol.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkpulbav.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3carcicqo.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjiuerup.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3moqdlycp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3rcimfyst.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3mkcdzgej.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhqciogf.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3kjtgndna.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3anwruqvc.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xcuxehzc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fgsdhtks.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dxivcotc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3pqwwzeol.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3jlaxssay.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vvhdriti.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bzoyjhju.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3vhvdgikn.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3htlescup.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ymctfcat.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3pbhuacve.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3feuvrfng.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3grkfitmd.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3wybsivrk.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3qwpfzwin.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3khrprmjn.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3edsccqby.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ufurshrq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3hncimegw.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3fwhbzdvq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3opazuzru.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3pljwoabq.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3gfmzmfva.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3psqgwraq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3etxcxgfh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hdodrcab.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3crjgeyrn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bzyjhkvv.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3kvcgumun.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3mogohykn.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3itcbwkxq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3eisiosff.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3dmwgrclp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3jpxsznoj.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3kzgrzcsx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3wprggqxy.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3bvqjxnlh.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ylopwbuz.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3xmbmzuqf.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3kmfxfzka.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3hmsmhpcx.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3qqncngmv.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3eemrzhdw.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3isijtvwj.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3damltcvp.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3giigcvrh.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3vmqyutvj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3tzxnnbhu.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3tgzdzclv.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3jscpjbuz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3qzvdpskw.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3hsjultgo.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3krgvfzwy.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3sylzreha.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3yxeepcsn.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3gqlodupp.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3zzbajlfn.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3werqmyyl.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3eoegwsna.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3cahklwvc.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3mihemfwh.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3orphjawc.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3jlrirguo.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3khgxntob.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3yjyewsen.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3mhmwgsts.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3bvxywdaz.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3nkofgbkj.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3tiensukf.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3bldvtlzg.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3xpwlesjx.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3pyyntguo.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3lxucvlrn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3jwxpqwbj.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3mrkwkief.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3depkdhms.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3guaeutaf.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3sjpdvxwa.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3cjgolcjm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3zdxitkox.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3xdosffba.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3nrfxjzrx.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3xcfvkxlx.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3vunlfmbb.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3aaulcrss.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3ocregopw.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3gecfzrci.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ijfklbxz.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3azihypei.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3nwmmrjtl.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3ebfwyioz.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3vgqtsixt.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3vemfuxzk.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3ochplqdz.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3qnevpgye.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3ohnqepao.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3yafeouyz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3runwcygt.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3iaswqygh.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3mupfiumg.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3optdwiax.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3mrqooeor.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3celoysoa.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3bchwskyd.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3vdieqjeu.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3lkdxsiwq.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3pxcxejca.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3druxviie.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3pjksllze.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3zcfljjcm.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3tnkzxquf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3olvrpwxi.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3dydsnfmc.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3rzkyxguh.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3zguncful.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3sfmuadmp.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3gxfnnfot.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fygevpat.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3xjmahbil.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3ihomhdju.html


<!-- 参考信息 -->