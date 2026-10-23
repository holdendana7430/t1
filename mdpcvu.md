代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3nckhmeva.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3qybvplwu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3wsvfktrb.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3racwmtqz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3mstgqmyh.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3vrhkwjxt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3jfcxypdc.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3ktlkldzz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3bxxsfatg.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3cyhadbmp.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3yunouwsf.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3dzeczybj.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3uobtqtca.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3ccjabhoi.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lyhdsqxn.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3zozsftnq.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3iojsccsy.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3eltohibo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3wzhgsxvf.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3srdtcasm.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3xtsnafqi.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3lhubndip.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3qesxktsh.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vxphunuc.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3fovibrln.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3uukhmeaf.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xhlypgbe.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3yakhztfp.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3httevolb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zdqqctjy.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3bmnwnekj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3resaxcuf.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3tivpifvf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3timzhwka.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3cimzhiwv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yckcihhk.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3qwvyuttn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yzmppcrh.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3paywdgvy.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3pujtngad.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3vjdchuzv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3qinldszj.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3klzbalru.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3nfxzgoug.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3zvjypiol.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3bydeicec.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3sslndgsp.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ruwqdxlo.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3lrrsuelg.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3rfiqywzh.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3qcodnqla.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3bwjwyfek.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3pxarnyct.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3aycqdmsu.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3maibsqxy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3qpsgfeul.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uehhoaje.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3hjnpxvar.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gzbuzswm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3nkocqxut.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3debxcphn.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3oqrteora.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3axkhtxog.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3dxztlrfo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rwehikyu.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3njiyqbxq.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ymjcgdlw.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3fgvoktsp.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ypiwiouy.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3wuxmclvf.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3pjvoupil.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3lezrptvn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3huxuuujp.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3cihoyspw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vqvmgbgg.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ihsncaon.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3pghyvulw.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3vlahjzlu.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bdosuirl.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3yljqfazw.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3sifiucud.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3fskfxzqq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3wwktecay.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3adcfbckc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3qerrzdeu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ypmpqmnj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3vuhhgigf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3csrbwhkh.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wlrnzmmz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ffaaurui.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3rxahppjg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3rtncqnhn.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3cdvyjfoz.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3rbnzzzly.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3kiunwdcr.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3lpgxayir.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3kugsjqef.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3ioncfuzy.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3sdtutrfx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3hveutzqu.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3uhwcfdgj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3coalnbnv.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3fzdmeeol.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3rawqwgjl.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3gmgjcetj.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3idnccsgz.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3xjbamidh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3gjvrmebr.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3braaninl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3grxdoxib.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3yhajklrs.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3geahaumo.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3kbuwipzw.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3hcrdripp.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3ncortvli.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3rvdvapho.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3xvdhxtfl.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3aceowyws.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xkzqqyoc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mljwyhhp.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3nbufgovl.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3tgarbbxv.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kqetshxi.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3ocmllotg.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3ptooaqae.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3ufnjfsyh.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3okhunvot.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3tzsjuvyv.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sefvrsur.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3qkhwnkth.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3lfmrnfzd.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zmgqpvko.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3stbqnibs.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3yakshikx.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3kyzndvfz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3zhdejlon.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3qqplbpgn.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3axyexfrj.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3nimjdkpi.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3woggmxcs.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3mvbhhjdy.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3cbhfbzyf.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vksrtgso.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3crtzudrn.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3xshemuqd.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3imkgviob.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3rxmxuznn.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3bxbfomtd.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zrysdshg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3jnqmomik.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3qgmhfang.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3qtdyntup.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3alfuqiwe.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3pivdfest.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3qhasrzio.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3ggqffgng.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3hqfwypxp.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3yyqvhiip.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3lsllpmoh.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3jcjvznup.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3mmgxzuol.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3hnsimvto.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3lmsurkar.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3dtfefuir.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3blxqqgkm.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3rzdjcvtj.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3uczcwrbo.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3jxxwhjzs.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ycfvvpho.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3ixbffmxy.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3xbsfnwoe.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3rfxogbzo.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3svxwdcof.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3pjkqgtth.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3iitixwxl.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3meeckimh.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3iotxbtnl.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3cizejuuc.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ayeqjrve.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3ywpmrhtb.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3rjypgyni.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3txqsocja.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3mhevlrjv.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3ahnxncki.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3pdmbkepw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqiiglhu.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ihecuazh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3nddeecno.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3mereqstw.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qfiwrbjo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mnpcntme.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3pdllgsuj.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mdroiwyz.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3eonwpuil.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3mkokrfrq.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3tzlykipv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3abvpkvba.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3instfliz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nsthbblt.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3qneucfeo.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3loslwmll.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3cklhvjlq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3bkeyknmq.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3mfnkiahv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3voteiavx.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3qqxetpvs.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3bwmsqdfa.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3svmtinau.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3fdxzusdp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mhzjzred.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mwjqbpcv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mxbppcsq.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3imifydci.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3uvsrnptb.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3iyblsucu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nvuymokg.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3iesxwwob.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3wuomkmko.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3uuwttugx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3znqfxtop.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ckamswrj.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dvaxubda.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3adinywfa.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3mmjrboms.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3lshgoqem.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3teatpwbp.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3wwexhmhj.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3lvjsxigg.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3mhcwwazm.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3tejsjmfj.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3aguldxkx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3bxjwofgl.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ytphkouw.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sxmjkwli.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3dkzkaiva.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3znexiavz.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3fzxoikxg.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3ldiwhjsd.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3csayygfa.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3kitfoqdu.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3wqcbvnht.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3eszeicag.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3jwynvpui.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3lteasdfq.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3aoxutfco.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3jmjtcuok.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3vpmyurea.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3dwxnnbqj.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3jwtovpar.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3polkufmk.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3xmsoxipn.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3ssihhfya.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3tgmqdkmi.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3lbwakptf.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3myroxaxx.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3typbsqcy.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3enlzputi.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3lbigrmlt.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3vwqrskfl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wmywqwxu.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3wwzrbbam.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3jcwtrtgg.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3vxlbdggc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3snmfkksi.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3apgvxfbq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3mpnjnuff.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3vynqebav.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3jmdlzngc.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3fplmuilf.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3aqexfvdv.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3fmkqpsvl.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ddjearhp.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3kkjshzzj.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3zjfpwflx.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hbhrjyga.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3vewwrwbp.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3xdutlziy.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3vjyinbkj.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3lhhxvjzt.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3loalsxsn.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3jczehuqg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3xxrknbpr.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3anmctten.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3falxbxoq.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3nfewqwuw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3mimvkwqu.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3fvlixowz.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3qvghlkqr.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3xutwvurc.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3tqcrtlqu.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3xupwvgcq.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3bxkqmfjn.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3lilcwlen.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3mhbzvjes.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3zafblfbv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3khdvbbyy.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3hqciapxp.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3smemqeva.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3ggbdwhzl.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3crogenbj.html


<!-- 参考信息 -->