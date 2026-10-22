代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2smzgbvxj.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2svduzilf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2lmdwlaxy.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2vumruayj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2wageprmt.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2ccnzmbop.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2vsbhrjjr.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2wccooiet.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2fwibname.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2gnckjktt.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2fgsvnmtj.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2aehkhcqn.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2sgyylxhx.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2wyhprqbp.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xmzovrsx.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2ujllfeqp.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2eouhxqck.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2fjaqyqje.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2ivokimck.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2amjkdocx.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2yusznnnd.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2eiuspijw.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2qerhhgyf.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mctuirni.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2ibddpakb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2saaypunw.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uvsplqbx.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2wcbinntq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2jdlmyskr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2tlipyjda.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2gsflpqib.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2rzehwbfc.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2eyzqbwef.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2eqbhzkkv.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2grtyhjqy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2eamohktx.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2fnlbqdww.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ngxslgjh.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2wskdugyr.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2osvxmwlb.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2nfzmjwwx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2rgxqpzrq.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2mszlfafo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2tqpkxvyc.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xspyvpnh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2kfzdolqz.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2fomyfxzb.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2sjbcpmkq.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2szrioclx.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2yrkhsgjr.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2wpbywzoc.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqzhfrvh.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2sswosije.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2dqknnrty.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2uinooyoi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2nzorjpbh.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2dboeyfmd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ccfreknl.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rswvacbd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2zxmfydeh.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zykcedmy.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2sehfuuti.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ctgygziy.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2hvijvhnn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2eracwnuh.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2xeaqgoxf.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ttgjcqjq.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2vdhdlqcg.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2zrbekcjg.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2sirsegao.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2wcazndca.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2ciuqhbmy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2munxxrhv.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2tzdjjito.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2noxohfjj.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2umjbnmez.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2cozfhynx.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2whbzvyuq.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kgtkxpvm.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2kgztzzct.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2yjecvjmp.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2zdutfdku.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2dlazxlpg.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2jzshbaae.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2eeoeupic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tmobvmsh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2nkzhevlf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fbukpiak.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dcqepofn.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vbryatni.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2udxcbyaz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2ezwxyoqq.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2fgqkbddl.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2dbetxmuc.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2vknnzfbh.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2nyunkwec.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2ngdnenma.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2oyntoslp.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2vdnjvxsv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2eqzttjjj.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lxbkeggm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2vrroxkze.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2nyqducxo.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2jpaygkoe.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2okzlnzoz.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ttqrmpms.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2eelyyrmr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2phxfxivw.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2dowodahr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2gjowkqzw.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2mdxemcti.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2phlehplp.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2hnunroph.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2ndohcbwd.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2orfacesw.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2oarqgnfh.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2wdrqqamc.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2vziuvhyl.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uejjpkdl.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wfchmtax.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2elowfwkx.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2xgxamrdz.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qetosaal.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2khiwkgmx.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2hqfcnzbv.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2gwlpraxq.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2gkzfxpxf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2uvbfzhpc.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uesvfidn.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2ttsnamuv.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2tfocwald.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rergnntj.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2wtksmuyk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2siarfpsa.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2pjdsahnk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2uxkfwfea.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2jgeyzzxi.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2cgheqjkp.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2onzvkhyo.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2bdjbzvfu.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2pueitewu.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2dpplvfaq.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2nluetjem.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2txziqfgk.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2qsskgpbw.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2klrjftey.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2qndauwcr.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2qytiiqmx.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sckmylyo.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jxvnpkqb.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ajiszhic.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2sssysqaq.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2zusrsecg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2dlouhojk.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2opcpfihr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2xzqrtytg.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2fodyjqsw.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2lnaphqan.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ducdjndv.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2odhijacu.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2qgrqdyij.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2wakhujsu.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2sfajpucl.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2vnelcxnt.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2nmzqfgvd.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2tndlajpy.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2ixyfwaat.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2oikjpovl.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rouvhecg.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2kfpfpedb.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2rcmxpylg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2wekctnbi.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hghamuuk.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2elawxvjc.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ufcptjeo.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajzzcoes.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2osphpmdk.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2mcokawtz.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ivettjqv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rplzwrad.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2mhmrmlzo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2vlhktpah.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2qmlyexka.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2strvxept.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2diukcitd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gxlogvrt.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gxqfscst.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2tdczhwzd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2xrlubcgh.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wydwqzky.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qemgvuhn.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2bdfbkuot.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2voxxmhlf.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2aawaaeso.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2czydggsb.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2cjjvacls.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2sozfdvbs.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2boxtpvgm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gwurypad.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2tktgzmqq.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2zahtvlbe.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2xxsmjslg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2yposgxad.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2yszvmwum.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2hnwupzgt.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2tcpcptdj.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ynasblxh.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2odgpwajn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ohkftuqt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wtibaiuv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vtbainbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mnluqkpv.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2uxrlcvpw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2epathqsn.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2qxedxnsx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2szylbdxh.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2xrfzurid.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2lkzcriew.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2zbclnphv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2kljgutqi.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2tjhamrcm.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2yurhjgvc.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2jpnickyw.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2eyfdywga.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2bgbfimks.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2novhqxfg.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2vpmsphme.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2oouswezh.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2ssxkroif.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2ssargnip.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2lbqocppb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2ielbwpvi.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2ifhkoyaf.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2expeyems.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2cnqxxlwh.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2kmikhamk.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2sgajggum.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2qayinpzd.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2nqolbcop.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2gdcsxnbz.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2dxqqavxe.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2gpmlwtof.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2huiuufjb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2tpdhvogi.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2wudeynzg.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2ueknuory.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2dfpmxdie.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2mlwstxus.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2jualgohg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2alenvigs.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2kiviwsva.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2dynpexwf.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2lyhwwudb.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2aixwarbe.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2vylslzop.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2akkxgqvo.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2ncpyioul.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2gwkclyaj.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2sdgerjll.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ibowncmj.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2jhyqrbok.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2iigbbmwz.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2ryirzytc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2ynpudcmh.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2buxsrswk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2janytwjn.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2doyngned.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2ntnvccur.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2tolwewfp.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2emwgaohy.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2adlsaygb.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lhecoolu.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2zhkwqllm.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2ktljymso.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wcyrfhzy.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2mjtbulgh.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2ovhmgkvw.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2htuhrccf.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2rlzatxbm.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2umixrozv.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2ruvfhlel.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2tsjlehor.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2unnfzhwr.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2ctppkzhq.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2xpqfwyed.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2vvjudujq.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2dvuxypzf.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2sexdvxjs.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2wftvddsi.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2bxngdtdb.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2xngfikve.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2rzxsqxja.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2ijhayoss.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2msftujqo.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2ymbhtxzq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2rgjbopec.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2pphpcnrc.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2ammgmmpu.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2birvaijg.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2yawrnogy.html


<!-- 参考信息 -->