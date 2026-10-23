代发 wailian999

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3mdnnkdnm.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lbhovwiu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3fufaacyx.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3obegalli.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3apdmkyds.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3phvsqpoh.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3xfdsbyex.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3igqjieza.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3tjowcxyq.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ndyffsti.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3nysfrcjw.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3mouugqlv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3bvmcqzdj.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3qfbslchv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3dfddueql.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3masutucq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3grqsdxbk.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3xcxiooez.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3bavtxccw.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3bxgwatof.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3nbcxzeib.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ykrhnykr.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rinaogsu.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3oueuojfo.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3arhoiflk.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3pnaipedb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3pfkuqjtv.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ryyitozx.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3zzidgcfe.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3uzjvrbpb.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3quudigfq.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wdnodzbt.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ufqyihow.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ichcwoqx.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3cotyxatt.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3cybshzeo.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3bnkmhfng.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3joummzwn.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3lydnxoac.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3xupcilvn.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ftnaosjq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3klxvvfxk.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3rjqdtzgl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3sfaspjox.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3uhxurmjf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3opftmpxx.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3gmsmnmzh.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3wcomxwqp.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3zvqkzjvz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3uashgiva.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3bfjpvmgw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hiwbpssp.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3aofiuhdj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3knbatclf.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3ysvklckt.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3agfacphy.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3cxtbaafg.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3oeznumil.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ksymauwh.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3uwyiqmlj.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3haoshvxm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3sikhketb.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3fsnvrwkg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3irlhcbyn.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kpearsdi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3zakldzrp.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qughquzi.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ilwrxfxe.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3zknnszcb.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3wujphspe.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3ztnzjglg.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3qzakdwdj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pzofjbfz.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3jrxbkotu.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3zzdtynsp.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3nifokiet.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3yhxyqsbd.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3crttbkuj.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3clqubgej.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3nhjnfslv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vvftimqj.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3wynvhxwn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3wjfffqoz.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3zttdabxd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovpklpag.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3gjjiqtob.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3baluupov.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3unbuefzm.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3jovbfndu.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3qocjetus.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3gcwlqprk.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3qbatwpkd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3oiulzgin.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3itxcyhvk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3szjvgylc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mxaysgrs.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uguowfno.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3cowvrtht.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3rmmqjbda.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ewkihwjw.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3irkyqbik.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3zgktjxkz.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3grcynftz.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3wpjljldk.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nxymxdwg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3jmhethzd.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3phtuyewp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3uqnwsfpf.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3hfveywfd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3zcfokqxr.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3hdfdfyys.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3twcwcewl.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3yetjbpfw.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3epumhirv.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3jxaxzwia.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3jdsnskag.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3eohuvgrr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3rqnypfnv.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3wvzrcktu.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mmagupex.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3odvthxix.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3amfpjxfy.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3nrmkmwzm.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3iwyazcdm.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3umcbtnwy.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3bmtdcddx.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fvgugvyq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vpcyqejf.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3fsmoojnu.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3wqmndjwn.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3unagtdoj.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3lreokile.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3xjirsver.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3yjsapkgx.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3mlmcgark.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3zbxrrbmp.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yherdrzs.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3vblcjzmt.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3tfnxjfug.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3bpmgpwbc.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xbimgsgm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3thvqfaxt.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3mygfhlmb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3mikdcrcm.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3hbjndaoa.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3nbnlyabb.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3qrzbtzgm.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3tlngukpi.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3vqwxennn.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3rtoedloo.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3mffwmgca.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3fobzahlf.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3iqbdpbjb.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3aaixklux.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3jlcwnzzl.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3bzdekxmk.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dbflgfyk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3clridgso.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3fxeetrgz.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3lfmfledj.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3eufgucvp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3liivxbjt.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3hflfsuhr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3hqglgqqw.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3srpaytbg.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3owomwvze.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3gsepcjax.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3zozvoote.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ajddwasc.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ibyujsnt.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3enswlkot.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3wtlrytbm.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3flafiojy.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3xqeoeiql.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ouwdhqru.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3sifzylik.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qnepkggs.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3aahbomnr.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3wxuytaup.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3ntuvqevd.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3pyotspvz.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3gwvuqtnb.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ggeelkae.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwelngxm.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3vcwgdhmz.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3oducngpn.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3deecztpa.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3fyhenngt.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3sqsnriet.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3cjzjbsyx.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3acawiieo.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3kgokzboj.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3aedwnfli.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hinagysl.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mxzplaef.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3kuigakjr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3bnwvhksi.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3czqrtakw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3lmmcksnk.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3kxvmagck.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3wpvdhepc.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3uffzfukb.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3bmkschpw.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3jkupbdwu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kcnlmeum.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gkdclktz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3zmualrci.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3oxcijklv.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3fbgzpciz.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kdydqatz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3hjominkp.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3heyxwgil.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3wjnelngu.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3gnfbnkks.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3tmhpvtvq.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3avloponq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3fmivrqtc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fhmykpki.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3mhryyacz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yxkowzqq.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3sysyjfvh.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3uudgrwru.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3ghdfzqgt.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3tfqzjzvu.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3jmonhkzx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3gsbjaqhj.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3sypvzhtv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3iggicygl.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3soscpqgm.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3tquywgkl.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3frrmojww.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3kccejiow.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3iyxghybu.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3psnuhoza.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3nlxcttfs.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3pqkhafaa.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3grdaibyh.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3ejphdoix.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3mdgqgxfi.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3cfepvwgh.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3jyyzxsbo.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3gfhunqfu.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3qqbspuae.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3ohbyzbuc.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3owgctmqp.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3abjxlmja.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3xpzpfrwm.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3aomlvrwr.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3dbknfpet.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3zzrdskjq.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3nbfnwwdz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3pcpdmkqs.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ojwfxlvj.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3hergnrvy.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3swiqriqc.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3fvyodgin.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3ixrrdcan.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3mrjevpvr.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3myncawrb.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3qqpwqugc.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3mnjebywp.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3yclburat.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3zttxuvdi.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3jsirwvil.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3sbqjaqsv.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3nsnkoxeh.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3kfeuxpyd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tggsvcvy.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3airisyph.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3pzofvhbl.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3rdlgodri.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3rsmbisil.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3dnquuzvi.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3vwjvjnpp.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3nzvhsgbo.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3azjeuypy.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3iratcidw.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3bdurfyvt.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3dsmyaqvz.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3oknwbuoa.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3uaqxipqt.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3vvkntxrq.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zczylbzv.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3zzwunhpm.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3lrneworx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3olpnckgc.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3queekhkf.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3vacplzgy.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3quhklslg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3gwwjdzcz.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3aiiadtta.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3ddyfuvke.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3jritqfbi.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ddozluoq.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3eabueuwo.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3odyuqblc.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3ccllryfb.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3fowuzisq.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3bhnqcflx.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3puyclpix.html


<!-- 参考信息 -->