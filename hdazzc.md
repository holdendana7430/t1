代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3fnmfnvmx.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3bsomulmi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3azcycxek.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3fzybaxhg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3slregteg.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3lugfalld.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3txphniqh.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3ahognoqb.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3uvqtrfkr.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3etxnicpg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3nyjrybuh.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3bljjmcso.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3boeiflit.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3lqrxcnuy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3jmlaizre.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3eclujgki.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3sexulqus.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ujjnabsy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3aytucauq.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3uczzkkxp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3lnlbfdef.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3tzduxxgm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3dzazvdcp.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3kwdcbnuj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ajdhdhsx.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3zjtabhkg.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3nmefbejm.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3atknwbld.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3axayfrle.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3pokvvget.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cuujthxv.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3vminftvv.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3swkougpg.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3thatqvfq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3uwbzimyq.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3zxdzgdkd.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3syqfonng.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3gsggcunb.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3otkcvwzj.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wzyfabiz.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3pndumadk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysgbewcs.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qzvshfru.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3kpixlonj.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3xjyqihcf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pdpezmqw.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3htjmagts.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ygqgwlsu.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3adgkzrhh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xnpsnsxx.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3kiaaysjk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3anbxgnbf.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3jqnfeafq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hpsfxlsq.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3blhtwyfo.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3xdkeiaoi.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3jiwahcns.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3bupkaanu.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3dbwgcuko.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xmgiddyf.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3jujmqybs.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3skvxahjs.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3cbbzixlv.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3adxawmjg.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3tbdxyiko.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3zfddwhhw.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3fsmhfaos.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3qlsuglqd.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3oonijcpt.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3cxtjnifw.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3muyjqvhs.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3swkcdacs.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3etamnuni.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghbbsvpc.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ktxeilon.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3oamyuvzs.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3eslghxnj.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3atahtzpk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3vertgqnl.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3iyfzijfl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wwxadybp.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3lflobwwh.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3bsaxwwhd.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3ceomuffb.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3nxqxwjor.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3nmgezcog.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3yczzuwdo.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3wqspftwt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3aiavvjwa.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ovbmkysq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3pnpxephd.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3blihlfqn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3rqfqczby.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3qfbvcpwb.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wnjzhpyy.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3wweuocki.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wvndhzpr.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3avdntyyn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3nekahglv.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3bakwjuhw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3admkqwbo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hmkthntt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3mfmkipnk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jbwgodgg.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ylgyyipk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bsoqxbwl.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3lzrzffxq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3zlkvblfd.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3lnnmgbwm.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3twddwphu.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3yjtsrqym.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3kzgekcuv.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3pwdnjclk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3ordyvkfa.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3lnysdkcl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3zrgmkqwf.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3mzfzgcrd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3fyaaybtp.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3zmnvrifb.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3wenmvtfp.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3nltlumrz.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3ifrinvcr.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ladjlhee.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3upnnhmby.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3iebmbugr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3tonrblip.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3fgvmclfx.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wxqknfpa.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3oqyuxcmb.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3hcwwrkyc.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3vigwhsdb.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3fbqwixoc.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3papqqxnk.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3bkkvicef.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rvvnfhbl.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3krgbwumg.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3avfrwqnb.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3nobitctf.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3dijcvubi.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3syaqvccn.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3sgawrfww.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3rhhctkto.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3fnxjbacp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3kzgasdyy.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3epydxhmz.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3zjmiukzd.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3byfjqwty.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3iatakrnj.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3laefzvgj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ejmtocdt.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3zfpknfcr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cavhlscz.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3oxtfkjny.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3imboyipu.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3utbmumcq.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3dawdwdoq.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3ifiobjti.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3cuzpvcbe.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ivfmzuqv.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3wxwmlzvh.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3lloucegp.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3kgpdaqzt.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3bnmjfejl.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3xhklgmbp.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zeprlqta.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jjvqxbju.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3evkxywmp.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ddfxucep.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3kpxtvbhr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3nfjeavxu.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3hozklnbd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3olygjtdp.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3cmbvblue.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3rbgyrmkj.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qnrsgrfm.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3luceyvhu.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3eetuyzmo.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3faypfzkj.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3mblaomax.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ldtjcoia.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3yitsmtde.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3oqgcptuz.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3iathgtso.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3ostpgtpn.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nebnwuqn.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3atrdbowo.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ahhnvepb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3tgqlwzxm.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3drbncbeu.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3ldbrueym.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3wowdwneu.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kazzogqn.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3snssjrnc.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzanbdhv.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3cqqgntsz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qukjjtwt.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3jzuxrcct.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3sglsvsih.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3hzybbvyn.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3cfjetgph.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3jiiulxpj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wifzqewr.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3agxacjyz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3dphjojuk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhejlsyh.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lxqrfnvp.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nxcktzpd.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ajsyklaq.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gsovzaon.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3dwxsawec.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3jrvakcda.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ssxplnrm.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tuoolouf.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hpoguhwc.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3odhxbnpb.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3rmayvecz.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3khhodmpq.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3moezdvpc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3bdvcmavp.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3sdknrpij.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3oqvisiej.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3xbpwyswv.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3tctdaiww.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3ijfhkxok.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3ykefthin.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qwttfxtz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sjndtnfq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ldcengye.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3reixihjd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3hgluqyjs.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3vlcjgnru.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3knygpgnn.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3pwvzrpil.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3ikpllouc.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3wpfvgtnv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3fmwdmjps.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3fqeqocfw.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bpqwyyjv.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3lnunmnox.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3gyncduzn.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3snhbbmui.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3aaeexevy.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3fshczuai.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3izpuurrp.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3ikngdqvt.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3iqnmdczi.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3nmbegsmg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3jrmplmms.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jxboyuuy.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rkirkmav.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3qeuiujds.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3apbachyy.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3pfcctndi.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3tcpcxfka.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3lxtcyggo.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3hmisgcng.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3csvptuez.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3behnujgq.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ygsybmkd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3pvcjucvm.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3kmzuodlp.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3logxuqdn.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3vetpoidx.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3pycyfnal.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3wrbzdttl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3bcygzbol.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3bpnbwdoo.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3qtqsjrca.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3wmjeuduk.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3momgwyfg.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3bxntmsse.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3sjbyndng.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3smwwcljq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3nmmodpwp.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3sidfiuxh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3nbgtfkst.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3jlzplknd.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3atllweez.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3iopsmzxi.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3hwvtnqcb.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3ykicmdbl.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3nccnsqpj.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3mtwlpfbo.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3wzybkrpz.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3uizwrjep.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3iedbnryc.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3vhnvsgqp.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3mehjkfgm.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3vraeitnx.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3jamzuqlc.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3hubewkyt.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3bzapdvvo.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3hpjezutn.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3kdybasht.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3iffsbmzb.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3tepsooqo.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3vfuvicxs.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3khhrerdl.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3qdlqjypy.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3elqaxqci.html


<!-- 参考信息 -->