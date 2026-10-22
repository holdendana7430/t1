代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2qzltekat.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2kgdzzoey.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2pfkocbas.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jengetwm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2ybgecxrx.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2qwwtfqvj.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2bfavpamj.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2yboxrfxk.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2urrdnvwu.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bxbxhhvx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2nkzpkfiy.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2vkvgrler.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2udrqgrif.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ccjbgloj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2immseeip.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2xcypngzh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2dlkfqzlm.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2rhzyjwrl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ejfziwwo.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ezqwftoe.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2qxqzlhpu.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2kuhzvyqt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2acmouavb.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2khfjicxe.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2xgzxyptk.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2kmvprqvy.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2boobjmtc.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2uynyeatl.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2tiprlhan.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2lejbasgn.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ohqcddne.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2lmertfrw.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2vbspjwif.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2rrtbzqjo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2msefgfrm.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2jkozfyki.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2iqccjndx.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2mehzfmfa.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2zldlysgw.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bswoqmen.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2ajhfhjjv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujiutews.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2xzcayylw.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2urbzvqli.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2gbcscrbu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2siidupzn.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2xkcwgumd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2asymkhcr.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2deuyfbee.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jnonuine.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2fmqosdpj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lvfjtcei.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2afddnvhb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2qkipfkjy.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2pxbzrlyy.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2lodkszbg.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2sylwycxe.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2bmeyjdnq.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2yiwvwucw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2fpanujot.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2mgsltheh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2khpngsdr.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2dtophffh.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2parvmzbu.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2fmgvswrc.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2quozdwrq.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2ioijvcun.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdkzcmaq.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2geymjlow.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2yxfuhyyw.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2jnthiagr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2msgnvhfj.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2uugrjvnc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2mmfrmqhg.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lvvgmwzt.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2mfugfivb.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2lmcwmakq.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2toyqqdfi.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2bmstiwta.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2dfnadjil.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qjvgsmlo.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2qczdedkh.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2kycighzf.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2mrcanemk.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2bcmagbxc.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2epbeyvso.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2bibtlyzh.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2cnjshgcc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xgdzixhc.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2emdetnwa.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2dsdbxusd.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2rzlhyzyd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2pibdyzkj.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2kouaxzlt.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2xwvyfhay.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2kvsulyla.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bhmwcbjh.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2vqdqmlgu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2vvmbvckz.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2xpsiqnqo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2pmrjncma.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nfbhhbdf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2gstzmouc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2icmdctdd.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2flromtgd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2epsytlzf.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2espyhhfq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2lnruuziz.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2opewqmfe.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ehcusycx.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2gbwzbqcx.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2zulsvpwz.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2lhfjhzgp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2tdejdgdb.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2gmrerbcd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fjjtfoqb.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nvclbjgv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2lvbxehjb.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2nwjhwhzt.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2qqsnuurr.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2aqkkrlsn.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2hcovqhdl.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2uxbbnneu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2agoynqtj.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2unjozcvg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2ngvclbhp.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2kszgxpst.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wxxgmtaq.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ikprgpcn.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2ckqpedou.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2nejajoiy.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2bmmfmtrb.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2auizugvi.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2khcpnfkb.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ggmviqua.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nxzkzalv.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2yxdjcnhf.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2xrhasyxx.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2prcooufl.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2khfnuqel.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2iogieohz.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2kjqeprqb.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2uhesqvbe.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2fwegxbsu.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2nacdcgru.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2mtngkeyn.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2iozaeior.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zranxizk.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2njehlrlx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2yenvmtwx.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2etxkojvo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vwoimoyb.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2pcbprqtr.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2cjjyulmc.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2pcbvaond.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2xxonfmdy.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2rtalsauh.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ktvbowvq.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2gybeejwx.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2ywpjrbrd.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2dgyqdatc.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2poduqvnn.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2gbgyeosi.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2iurrkgty.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uueddqgl.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xzstqbyw.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2nlxzwzxu.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2sopcycpc.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2bvnulyki.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2fcdzdfnr.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2bqpvkweq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2cfyxckxy.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2cwxdcmyp.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2cdexzibw.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2cqzlvrdf.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2tgpbsmca.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2pjdydnak.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2hdzojdty.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ouossycm.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2femtizvs.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xvstrshz.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2yqqwnygc.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2ljfmbbls.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2wfyyexvd.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bdrxyebx.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2zunjgawm.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2puiyfffz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2nkgevzud.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vshudpgs.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2bujgbjid.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2jmnnjpqq.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kajfadbf.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2delajubu.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ditwiprx.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2wprgopty.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rcxarhgv.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2hniizlxy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2gnuduhct.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ppbebdgz.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2akjbuayb.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2vbspaqbu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2gsrpexny.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2skslhkqx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2svsolija.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2gmqiwpal.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bvmnnyxn.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zzfxiniy.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2nwjwlkbk.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2ruhsuizb.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2lbcspunf.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2slqtlduk.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2jlfijrqv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2irpxcqba.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2biaxdyrd.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2cotofwww.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2irvcwlip.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ksmiglpz.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2cbuzrvov.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2klmnayty.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2ucknlwqv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2hqrlwicm.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2msadvrjz.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2rlyawydg.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2tturnknh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2ihqybtvm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2shlgunsq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2hwlkjyht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lqcnxala.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2phnrizpb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2ggczpyum.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2tznhvnoc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gubxpzub.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2mhdtgbnw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2lhnlughw.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2mqnygmir.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2qhlharuh.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2pmsvqqkb.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2kuerfzkx.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2xmtwjowo.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2vyrahsxg.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ffnyiriy.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2hxhocvon.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2bbpojzop.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2yuuqaniw.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2cyfjsdwg.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2chtahlra.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2mlfzcifg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2ydujhmdd.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2sowapmld.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2fpgwjatv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2itvixlwy.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gvvyojkh.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2kkozltcf.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2qhafrdnt.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2xgvnpnzi.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2xbqdwqla.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2cdyocfpx.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2cvttncnr.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2npcchyzr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ajjqyxwp.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2odgrcyqa.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2ltsjbrwe.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2udjxwlck.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2cgouqqov.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2fevupxrl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2nryznzsh.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2nnauidoo.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2ecfbszdn.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2gmhkdqcu.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2dnggtyzf.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2kaxxdofh.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2adazqmvw.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2ykgdosxe.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2qhpkltbp.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2ligohldm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qshrbrmp.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2kbpqtuqz.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2wpjfgjbt.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2vslevxdo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2ieixdgnx.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2rvxjfdph.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2reubnvuy.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2vbyihrmx.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2njjiemyy.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2gdwzdyvp.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2hzirnhmc.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2nmxnwtyx.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zaoadsly.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2hjbfdnxu.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2czbzauas.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2olcmupta.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2ifslclaz.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2ogoryjkm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2vtqnbacs.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2ufhlfvuf.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2axsqlpad.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2cppgpkwe.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2yiibqewu.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2fqdgppbm.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2chtfehvs.html


<!-- 参考信息 -->