代发 wailian999

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3nlmgyxyv.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pyzmlfgx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3eyodeqdf.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3sqgfysdg.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3nzllghty.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3yoppaxxy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3koyiwuxf.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3lhifhxlu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rsqjlxcz.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3dqxuituh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3xdoaaxmd.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3uoiqazea.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3kzdpanwn.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3gjbearas.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3frdwlrmm.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3ajtbkzvo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3fhrzjcbg.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3iptdotxy.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3dwtgmwbi.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3mfvasgcj.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3angaocsz.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3mfstemwg.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zubzjaqu.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3ksxlszro.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3gtqocxdq.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3gwebetyb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3gujjmees.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3pvfbrpmm.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3kgzpmdmq.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3rrtqkfhl.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3bjqxucip.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jyoqxawm.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3phdbwdfn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwbapvta.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3fnwjjhul.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3yvvfwvfo.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3fnmlkjyf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3lkatdnve.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3jfnmhymr.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3parerwxn.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3vfmryooo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3idiqlplg.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3rntmkavz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pbvsfquf.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3jntdinwr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pszftfsc.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3rynrsioo.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ksjciyeq.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3lbvogmpw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3hyeejzvm.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3njxlhaxs.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ukkmibzf.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3okvhcnab.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3uapasytf.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3wkluqtgt.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3heutpnyy.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3qtymcuus.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3iyduwwjz.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3zdnivxps.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3jdpidsiy.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3akcmczbb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3qeejqbmw.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3ywwfnhoc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmgpqmvp.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kquvwsin.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3qhiawmuz.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gbihqomf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3tykwtnkw.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3khkngjdx.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3knqdtpww.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3pvidkpuv.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3xrtzemht.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3twcofakf.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ameovomz.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3pgmeubbm.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3nbpncnyb.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ojwiybrt.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3pxyydhhq.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3rsluyysf.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3npkriktm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3okhpszxi.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3stctvzxg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3cntnkmdc.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3zhrdxvwh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3oohhbzyd.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3ekekgmki.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zmwvfeyb.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3rkkrlfed.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nyvffpkq.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3enjcwfxn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3rlpzdwxl.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3txfdxjey.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3dwedqnjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ggmnlftd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3vvqkvjtp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ssukmwel.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tfmocelk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3yzcmgtgf.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3gmndqsrr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3nciwgeuk.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3afboblot.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3molhpquj.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3jpdrzscd.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ntghijgz.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3pvicmpfm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3dpbtgkkc.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3agjaiwao.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3oepnquus.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3xmgusxts.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3dejhckqb.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3xqgkmzoi.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3rzqyabem.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3trhtyufg.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3gktllpys.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3kcngkrjg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3hncadegi.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3susudxfv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3dhjrvkga.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3vxmniwyj.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ewdhfrej.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3ltyupmgq.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hrrltuar.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3bsrpvebn.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3glqliywu.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3bwowlsda.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3wphxntil.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ufyreqzs.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zauasgql.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ztqvykkn.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3glabvxxe.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3yrozvxcu.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3wmoseekr.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3pkaaaywp.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3xnvxrxla.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3ekvgukfj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3ahroaosc.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3eyjlcqmk.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3aewvrbvt.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3rttsxrpp.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ewtsomvk.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3ofdecuoz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3sqdzvieq.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3rimsobbi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3pgndzimp.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3ohrcrgqs.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3zncyammp.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3qaqgurqd.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3rnvczdid.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3keextyvm.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3yqxktxsn.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3xvxqlpbh.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3mwhqhhen.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3nyutlbnb.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3wuqublhk.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3evqllfts.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3gwdykuvj.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xcunknzi.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xwfhzpsk.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3bsqpakwh.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3qpcqywub.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3foseobri.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ttgajdhx.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3cffxmhts.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3fposrxnr.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3luuourmi.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3sxyhgfnp.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ogvbjfvh.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3dzdzlncy.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3fvvbhrrj.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3dtwuqsle.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3fbfqsglq.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3zdfqguul.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3jmcspunb.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3qsrhgmqb.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3ncknugdx.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3pcckertj.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nctmpzcr.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3ksazkvua.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3xflabfmp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3lhfuertq.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3casgbglp.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3ylfujlrb.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3pggetuwy.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3eduhoequ.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3ttuwrajy.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljnbvxvk.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3xtrsuwke.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3pjpkmodx.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3lxgzjbce.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3yucjapcj.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3djhwshyx.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3oyxxqlvs.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3owwkaknt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3llycwsvh.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jexicqme.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3ajhvphxo.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3nindspcg.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3anvgwvxt.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3lmikrxmj.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3smzkjdnl.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hvxksfdh.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xznkfybt.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3jmlevvml.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3jnawwmad.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3lucnflko.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3czceznrq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cazkiqin.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3adeptjrg.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3pezrdefs.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3shamyzvm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3xsctzxek.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3dorvmwux.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hbwpyrlw.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3jjbbqzou.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3eftmcuhx.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3jnkrslyy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3dxdzqeqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zkmgwaqh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lbukkftq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sumauyof.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3jmfzdzus.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3zfturoae.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3czxpngzj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3xtrcrsni.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3dptflykp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3lprlogsa.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3rdfqbdyy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3pzkuqgzv.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3peckuscz.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pjmmrdxt.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3jnsfgpvy.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3xttqdhgl.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3tmkchrcf.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3qaiuxwec.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3ijzdaize.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3znyyhlsa.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3kitxxujy.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3qmfpvosr.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3icguxhap.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3nznixwxv.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3ndszhqic.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3hwjknijz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3jztqthho.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jtboxkzh.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3epoaxkcf.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3tfweiwhn.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3blydzgzv.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3lyxdecuv.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3krzxiihm.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3nsivnskw.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3qtftkkch.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3lsahtvyj.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3vhecklry.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3ewaiiqkk.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3yzhouamr.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3cmcicaxg.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3scttypno.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3zmryqtzf.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3soacwcar.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3xjslusze.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3zoneivlu.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3cfprvzlo.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3qpxtvqtn.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3sulfftzn.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3gubnfxpf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3ouvqfzsz.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3cnlaeycj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3roplofvc.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3ebtdfobq.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3pctrmfht.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3axrcanmn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3dznzpzqw.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3tzgbpihr.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3iaguqose.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3lqhudjab.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3fycmipux.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3nfliadfz.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3vjeddivq.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3evnhisnf.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3nuubbmrp.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3hoibrlfa.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3etcfdpbr.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3hglnbsth.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3fajypqcg.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3cggxcgkx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3uqypyrne.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3ntopobzk.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3fvbchyck.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3pxvhecad.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3vvwkhflx.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3ijooumlm.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3vobphnvo.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3bscxomql.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3tdqvcunf.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3yggsxzff.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3fexjkjlu.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3myfgtrdp.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3vhjoewmi.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3zbjsoykm.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3gygepgwt.html


<!-- 参考信息 -->