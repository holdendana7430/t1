代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2cmifdesg.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2hgocvvdw.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2zqghlnhw.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2umtostnc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2mlcvmoam.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2kknrpnyb.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2qmvpzbma.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ffehoouw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2aewwsaqa.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2wgxjlndb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2vnukadpl.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2teqwvzds.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2upgdglos.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2oeinmrgq.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2nfaperns.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2jzriaqww.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2azaagyiv.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2wrratdfv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2kbooeshk.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ntkckxps.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2drahyaie.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2tssaajyn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xsywgvwx.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2dczfckge.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2hzbtthsi.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2sdjnfnzg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2bdjlvpzk.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ekzlssps.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2jcdmwuvw.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2yhuzbtey.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2nypeyhef.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2mbtixoye.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2lmufemqq.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2gxuowbak.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2cltgpaua.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2grwjtbxv.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2wgvddieo.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2dduqyjig.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bhauprgy.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2yutqgrbc.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2spomlexz.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2upqrqdej.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2pkjwlxtd.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2vuwhkriq.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2fvrgsxhk.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ogviiolx.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ditzvhgn.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bcmeohsd.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2axdflpqo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgypvmxh.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qkshlagt.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2jdspjmwn.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2azhehgud.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2oggmzrtq.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2fobrfytt.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2jgexpfon.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2zofauuju.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hqdphkmf.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2uhxagjqe.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kqoqwtui.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2rfsyeskw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2apkntngn.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2gngyrbum.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2xdgkehja.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2tmgjjtvq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2gqyyjfrp.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2vhwervsu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2frazoufe.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2boiabvoa.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ipnvqtpq.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2pvgasjoh.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ltjzrydh.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2qpbmfgaq.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ymdtdfup.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2efggyasg.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2acjsadpt.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ngzkzhui.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2qydtaxql.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2puasxfwu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bracinfi.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cqfljkxj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2awuvwcfr.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2neayhgve.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2zmyvyjap.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2csczucbo.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2hzqyxrjz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2hxoojhif.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2haqprwje.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2trucowcj.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2aobjgbfb.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2pupqkprt.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2lkmgprhj.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2icdbuskk.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2uhcijoaq.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2iyiouyrf.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2tdxgwgbf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2vdlhjwen.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qqozqgtw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ettyyfyl.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ylmnrrho.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2enmxkozm.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2udcpboim.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mqsapkyu.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2rewexoey.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2zpeovcyb.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2ldqihfgb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2dwqlwfqk.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2oppbdvdq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2nmwfgcng.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xkdejbge.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2eaexunkn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zlevktxh.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ifnlubwq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mzusjiec.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2eaevkkii.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2lnmdqplo.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2dmwopifb.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2dfpaukvw.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2lumlsgmj.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2cbloxyjt.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wcfxzvra.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2cpmfdnrp.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2acczxkhv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2weewgsot.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2oqdwsjze.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2patxembq.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2pxmpollv.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2vyocxtjn.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2wycasoci.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2tdvwssgn.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2mtifbvnc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2cvdwokix.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2nhulzydl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2qdxqyjmx.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2meyeyujb.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cmtrtumk.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2mptzyyyo.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2ddxlskia.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ishhuozr.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2tstrxgan.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2crvdtvnj.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2wgfajjxo.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wlxjmjhn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mbsfdsjj.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2kfagpzsz.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2zvknrwyt.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2epjqyvds.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2itkvfehv.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2nggvxyyj.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ssuevgbj.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2fhnzgyio.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2vhoqhazl.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sguyggki.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2mjnghoif.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2bqhbujil.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2vcydshza.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2qfnzdgqh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2nxgxekts.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2oyunckht.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2gklqudwi.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2kdiohhzp.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2gnwocgkz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2hlcostah.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2lymtzgvr.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2pouxbbhg.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2krvuepkl.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2cbqhylqd.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2ulmbcpvi.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2jkchkuqd.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2dinjkhss.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2njfuztzz.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2zjykickx.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mgtwcfhu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2oosffxhl.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2xrthorls.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2hqhvnsug.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2zpqxqjkr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2kiuimpfi.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2qqdbwyes.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2lrjwylae.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2woqxphij.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2lqnmcqls.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2exmqptvg.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2myskywgz.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2wrbzbkmo.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2powydqay.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2cmxwohyt.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2lbrkgfnp.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bvtxewfb.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2migjyxpf.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2migsyfbn.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2vvlbojxd.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lvywxski.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2nvbmtnhw.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2hwdvuoab.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2csxvfxag.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2oceemofk.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2qatxixtd.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2vmmflwah.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2sotalwyf.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tcdesltq.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqkdavuu.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2wvuwpucc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kuhuyqsg.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2qdqolnzu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2uuwywisk.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2uhpnnoxi.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2wihdgftf.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2tmndsfgw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2klntmigl.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2leuiikbw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2ltbhjmxj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2hnhaudvp.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xflbclwr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2uxalholr.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2ijjqcdzz.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2mrfuqali.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xbnfeiez.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2wizdftzh.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2injhpomu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2quvzoeps.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kzcasrov.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uokzqvru.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2lkqrdxjo.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2xivlqvxg.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2bzvogpsp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2wygntsfj.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2rkcaucbu.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2qwvvghww.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2bkigqgqg.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ytupwtzy.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2bgboflek.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2uouhkvgh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2omefmpir.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2lxztarwt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rjfiuqfz.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2auabmihh.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2qxlxdvie.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2tgxjvggo.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2xoywsqry.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2mhuyazpu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2vskyecze.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2gukuldkf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2wadssohc.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2evzvnseo.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ncknfyzl.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2rdlaygfy.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2kemjitbj.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2pjrnqayb.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2dpzrugdg.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2bzwlliuq.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2pkfxobip.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2vhggyscf.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2zmjbcbew.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2xyygdcjh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2azcutlcv.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dzjznyea.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2ypicwwtd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2iahulamj.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xicbxhkg.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2mdywlqgl.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2dvmcptsc.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2zgomhtrr.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2spgqqrrt.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2oxnivxwz.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2nhmcpmzb.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2ozxegxyp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2gwoiryjm.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2jjbybogb.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2tzpmigxb.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2taejugey.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2roeabbhc.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2lrciqxao.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2ajrtlnua.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2prmlgfub.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2jiyfzpgw.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2csiienux.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2gtwbwxqn.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2yyugearn.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2xrqyfgyb.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2spyppohj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2wieugren.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2vhohmyif.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2cojagyey.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2wuqpcdmn.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2fhffrjuv.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2qwbfgtnk.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2eelprjej.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2uguaqdoh.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2auhgulal.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2dcnldvgt.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2bycqctkg.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2iyuxfvor.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2zrhfftuw.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2pprwdowu.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tzxsbdqt.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2flwbupyg.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2vedgykmt.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lhjibdgn.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2hkokyqrg.html


<!-- 参考信息 -->