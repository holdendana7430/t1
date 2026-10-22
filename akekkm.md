代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2dzrfessm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ubjikclq.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2kxvbfqda.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2qpzfotum.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ctvbxuot.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2spccvisa.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2gwshevob.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2noxrfqxn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2prullbpt.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2kmwskshf.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2wvfcywdp.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2szbzshta.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bxjoofqz.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uzqwegrz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ovnciaks.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2cdbwvvkl.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2akczocpw.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2xelqaymk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2sippfdhq.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2trltfick.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ufupgzqn.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2wmvgyeyj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2atntpmhc.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2eoaajuxl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2gryslnae.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2tfcuurdy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2swkdsuia.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2qwienpxh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2jlnctyhc.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2uupbiuwr.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ydywuuoj.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2jgjzlill.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2apuptflo.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2nknhixrr.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kqvyjjqj.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2xwgvnssc.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2zrpssbfg.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ysnfkldf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2ysvxvcwj.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2hqnjtipg.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2rypnjsus.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2hnteaspa.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ifdauuhm.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2csppsaaz.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2qdncgmqc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2stezydvc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vqhhzogf.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2pnxjmsaq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2uomqepdi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2pjqtrqyz.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2qeytmxxs.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbcjgvdd.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ycsdyrll.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pjplcjqc.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2uptobdyk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ofgujbvu.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2xtugbmsu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ticiliay.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2njilrxjn.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2nfsgplod.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2kblvsyur.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2qbuejuxn.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2rovqamba.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2xlqbimmi.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2lhlwclmw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2fvfnljrq.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2keekuajh.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2jrpteush.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2hdqlxyhe.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2tzlkudqh.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2gxvsbusg.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdfkckqn.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2psineyva.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2qxoikdlt.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2xddkbpan.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eaixnikt.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2mxsydlra.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhymhtsf.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xwxexcdy.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2yymkzugv.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2gxoahxjj.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2fxnrwtks.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2djmdvdkw.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2yrzslebm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dtgcjluq.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2xxouukgs.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2afovoxdg.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2vrohnyuq.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktwtcffj.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2dtjrfnni.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2jhcdmzam.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2bbluoxmj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2gfeelhit.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2wmoltzyu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2bsrmwfxy.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2mseusyqb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2rkqfemdu.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2hvtackjp.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2umjifelj.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ebcokjsf.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2qreswmgo.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2tbbdfiez.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2yzepxgrq.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2apjippry.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2gmwnednm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xlgxdbly.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2qqrlkazo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xgoqnlhb.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jwtpntki.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ygfmgkrq.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2eueleupk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2wxjprgse.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2mcnbhtkf.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2lhignowz.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2vwbziruf.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2tegxruqv.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2jmryvfep.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2scahudwe.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ffvnuurt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2sdkewdaj.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2qyhpexay.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2ijffriac.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2yjdaxpti.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ncfaksfb.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ypevhafq.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2xtnqpynr.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2xgaddrmf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2klwoplhn.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2bqnjtmbi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2eifzmzkj.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2mmhmyjuq.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mwuodklf.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2brrbwmym.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2ulhpioft.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2iffzydfg.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2lvrvqbod.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2zeonxigw.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2wunfxiaj.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2affghsbn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2dzzpoqeh.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2owwtfnhv.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xhhghqia.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ndoqzhjn.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2iihspewt.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2rfvozgfl.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2ssvhchjt.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2qhfnnbnp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2hfdzfslc.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2cwalsqkb.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2ixrrakeq.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2gkgklrmi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wwjeezic.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2qivsdqgk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2sdmpnqvg.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2hauyznxj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2nigehkos.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2hzbbwhuu.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2xwtscxhq.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2dszqtjqp.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ontgzkoj.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2uxlvqqsp.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2etoqpffy.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2dbftcwaa.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2cvgnwukn.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2gyzxmdgf.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2aoxuqhgg.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2ajnfbpoe.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ybmqejzx.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2osneiguy.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ziupdnqs.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2itnkdvln.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2wnzclcgd.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2lqqsedoa.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2qjxccotj.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2pinfatkj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2fmydfmic.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2gziiudno.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2wepahlwx.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ysyiidfq.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2iluheydt.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2oqwwjhqx.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2elnlhdnd.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2kuvwzkhk.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2auxkyxwr.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2gwqzbqbv.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2wgirspyt.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2gwinbick.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2wzpsvakh.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nmrxguim.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2zrnpmlgv.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2icerdwkf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2haldnavv.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qdytjqzv.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2fouzlxib.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2byhljjsg.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lcgrcfar.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2gwdtqbbk.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2ceifureu.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2zlqkbvyh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfsyyqns.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2hmfhbdcn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2mivxtlqr.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2tlnfckem.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2agshvhib.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2fhkpcurk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfnwzrtk.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rxxzcnzd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2denjncsz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2hnqhowun.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2smmoaaqw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2pysehpws.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2buupfzud.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2urffuoxw.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2djgjzqpi.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2vqtggvbv.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2bajomjgo.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2zqicnpqv.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2zpkmdumr.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rmurqfyn.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2juztbjps.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ueprrxzc.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2tbabwehf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2anhjsxjd.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2hrsllouv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2lnoebhjg.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2oyemeuxz.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2nqfyceml.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2mtiextfu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2lkgmkwqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hwmzthrm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zwikugqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tiqtfiro.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2uqazwrbp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2evdkupvz.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2xrbonfye.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2omoqbouq.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2aefjqltm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2flpenzcw.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2hollhvtk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2rxgjstvk.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2sxcpxfai.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2batfkymj.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2kmwigjjy.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2ndrkhxqx.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2clsawhde.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2dtcolhop.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2dunidgqd.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2lbblamth.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2rhhryhur.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2thskziwy.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2ukbnrrmm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2kszhfhkp.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2nhuxckki.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2garwhkoa.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2narzrnaz.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2aimzesyy.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2vxjvdptg.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2skpoviky.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2yhgaarfp.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2lzkdxaao.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2ngocygks.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2qsmzifxj.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2bftnpxvb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2aovassqa.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2rlgmjpfy.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2touoyump.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2mivlahnp.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2nxsnjaoy.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2bobcgzmb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2thkidbsv.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2iatddxgk.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2xfqulscr.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2zcqvjurh.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2armlcmzb.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2xguzqnpb.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2mvqyhxvm.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2kidrzyic.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2utonqxrq.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2uhbfonlv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ncykrhpi.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2iumfftfg.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2edilcbtc.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2nclgarkn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2slaupxgr.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2doxkthzb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2snulycky.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2hwnazkzv.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2fllbdzww.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2pkfajqbk.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2llizkzdj.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2esqoaiqq.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2odyjynob.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2bfbwqysb.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2dkdgrfzv.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bllyhzei.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2xytqznwh.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2olsookfr.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2gbprhzlg.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2vimlmsgd.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ecduypon.html


<!-- 参考信息 -->