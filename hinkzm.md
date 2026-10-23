代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3gstmqhcf.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3pddsmsmu.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3jjpirtaw.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3bqbryail.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3pjymatts.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ubotypfc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ouxzoanu.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3bgomvbsd.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3hfdordfp.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3odwyynpv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ijlfzwqg.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3zoboxbcx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3mmqtzyqp.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3wgqtlhvv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3oziukbbn.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3skilxypf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3sszmhkln.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3xbzokybb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3kzsovsce.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3lihdrhqs.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3hwmfzxcq.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3gzukofxb.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3rdktcntw.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3vyjaayfw.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3cpnkexkw.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3pxomwbza.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xzqrtxym.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3oyqpugla.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3qelgciyk.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3rbspbodw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3ctxtlvhn.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3noyltmsn.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ysclbhhl.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3zahmlogs.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3etyifohn.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3isumdivm.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3novdgzwo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3hcifqwqg.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3towhecjm.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3zkqsdiha.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3izgnedxn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3ugihdqmj.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3dihjnxzy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3hlvhmnih.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3uimorcgh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xkqbjsyz.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3dithtcbv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3fqlhlxwy.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3rbbrbkav.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3hnkeuktc.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ldopoxav.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3zwavtaca.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3vmolamjs.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3hnazqbej.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3ydhwszeu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3sptavmez.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3bhyzmftd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3qtbifrtf.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3tmrnprel.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ockixjzy.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3qtzgeofa.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3cnpqhakg.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3ftduzsck.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3rfauuxhi.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3zatzdbjb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3doqvpbee.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3rtvufksx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3vtosjjzc.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3edxotfgh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3qhodflyl.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vrbdjubj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3gwzyngcq.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mefpldbo.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3inrdtsic.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3uorznyrj.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3jrdqfjkv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gpzclocv.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3wwkgrcbb.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3cezgzcwi.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3sumbmihs.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3rllhxmrr.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3sgridqru.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3jzuxswup.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3wuubealf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ggplzywk.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3udyiqzan.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3tpczgmac.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3cnzmtrok.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3saqccnvi.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3iqpyhetd.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3grpxlodo.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3rfqfzzqu.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lvmmmskp.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3mejbwreh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3mbabitod.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3fqkzbchp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ulawvfrh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cpappncg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3kaiifkua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cfablndy.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ixphbuuz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tklhzjdb.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3dqxfcjbf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3rmyyqtbm.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3gzkadczo.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3njmkwfue.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3asovhkna.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3xfhqxfmd.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3yszhzhkl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3jglxnqkc.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3uatxpgxr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3olhbtvtq.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3bdrsjxzs.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3uxpiilij.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3nmbzeqtg.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3fujkrevz.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3vxftxlqz.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3opnzrkpq.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3jihcmbvn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3qqffvbes.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3jnvfeiti.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3vdaflwfk.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3mxnwwoyt.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3onjwbmmt.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3szurbikx.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3fsirwnnu.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3talhdkgv.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3wkzkmjny.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3sedgbvgz.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3bkxricau.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cxevcbmr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qwvdppxx.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3fhwtxzyq.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3deschbst.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hrvawfko.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3jdobsbya.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3tcxiggyh.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3yjfbuufd.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3wlobauvu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3babzicov.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uokzwknd.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3eakannuf.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3gcdcsybr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rbmjqexq.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3ieaycdjg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3yqjnztke.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3ovncwbjd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gedaaffb.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3jdbhzpxd.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3hwrhbqtf.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3lbjvzrrj.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3xwikmerv.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3rvlimyib.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3dvyayimc.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3oknqzond.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3szcouykm.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3pdhtqfww.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3uiqzgujx.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3dkljdcew.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3exfpodej.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yrwbuljt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pzzfrivg.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3gnsmhtvi.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3neniahuq.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3mujmlisz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3rarwvgik.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3ytxmhqph.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3zjmryoib.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3newkvhew.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3bsrxmuen.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ialqhnvb.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3nnyhfkel.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3augshnvp.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3rzzymckd.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3rgsrvdvq.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3iwbgsfnr.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mfnklsdm.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3gqolktew.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3qtqvnfxz.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3csnbtriy.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3oqeftnpw.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3wcykwpiy.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3ktxopyxf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3venjmbbl.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lvahmegc.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3jmkdmjwt.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3hexqjhlp.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cwqifhrw.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3phrblpub.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3yhsblfkp.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3qcvvsgxc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ktoqhjwk.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3alpgdhib.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3axyyoanq.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3vfjenses.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3vwijuzob.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3khzlleut.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nhxcanmr.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bezimqdx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3cnjauhvt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3ayjjniff.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3knqyurgv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zufspqwm.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3ohwyeqnq.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3ccmokbwa.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3cjvoiaop.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3pjfadelo.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3dffymcpm.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3ipsofphm.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rlcxzyxa.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3brciesfi.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3iwwzdgpt.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3foufkabd.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3awabikxw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3pqxvzpyn.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3iecqinml.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3tcwoeuot.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3kgvapgqm.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3yspkoxsu.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3maalgxzv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3frpiljdn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vberryqm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dtrmwbkz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jmxaiqpf.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3xjxjtzrt.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3hixjrxip.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3iqevykro.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ffezcqqd.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3jzgwglbi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3ewcaqegd.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3jtjnehgp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3qwcactav.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ioacauyn.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3yyolybak.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3dvbosyvo.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3gtxwozlr.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3oiepkuih.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3exxkopmx.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3guqvtiln.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ndeoncop.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3wyiqwywe.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3ypeqvjbu.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3reyuyfgf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3hsqxkyyp.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wwbapbwe.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3gawrcgrc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3feoaaery.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gxdyogyj.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3ishqcpsl.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3odsqeazg.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3jnvsvmyl.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3cdhhdqmt.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3jnhixuzv.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3komsgdil.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3fyxftrok.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3ofrihnzp.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3dlohwgrn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3zpeejruq.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3xtlwffea.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3pclbtzpf.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3wipdjpov.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3hwvrmsmb.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3hwyevnle.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3hklwfzjb.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3ivpnywyq.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3bjljozwc.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3kknxoxox.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3ktiltxfi.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3xvmceneb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3aaannnkd.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3hyacsxua.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ghzvwwtm.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3ysgxepvh.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3qwszmihj.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3dnveyexs.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3bqnnqewy.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3ctcycmjl.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3sfjjotxb.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3hwleeesb.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3edqymwjc.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3wrvxnynh.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3advjlsyq.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3ttgcdttd.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rmwiopmj.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3tlowgppe.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3wjbhjlka.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3vqijbuqh.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3qzokukli.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3iaawdhxc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3mbqkmggv.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3yznugmbd.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3rmpsqnpt.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3vnntfdkt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3xchcqbxx.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3jltovmso.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3qfphwolj.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3memcfcyk.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3sgkhjibm.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3lzctfovi.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3absztlng.html


<!-- 参考信息 -->