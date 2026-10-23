代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3hjfpsncq.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3raomzozk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3dxfaczwp.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3fthszzpa.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3yjodrkte.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3jquidzya.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3otijylgx.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3cubpuyim.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ivznqypd.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3nhtctooy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3mbivpbfk.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3uddnguzx.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3gjzfhwvq.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3glwswrnk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ywsrglui.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3cxyfbewb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3uueiapzj.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3fcveiank.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3edezgiva.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3tsdiujlc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3kmmibfij.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3nvpwwvqa.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3mvqsomxq.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3ugkenwjq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3oigkmvls.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3cdkauove.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3qzvqtjuw.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3ptskhcxc.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3coxycgdf.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3gdagudbg.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jzfcfjlw.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3xxsxovtv.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3zztgvqhm.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ogkjulnv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3bmlrxpzs.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3vgdidueq.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3mtjtxqsg.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3luqvwvav.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3wkmgzzep.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nxoyfkpk.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ocxgayez.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3qfpsvpoo.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xctovwis.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3dllavjck.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3oaagqrag.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nnrvzlkn.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3eeytxech.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3iypzdqrz.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3scitgpez.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ozkkhvzv.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3mlqxwrfm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3menvkjjp.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3ehxdjlfd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hogdadyo.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3mlnztcsb.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3vmgehvvh.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3rtehjazw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3qtyjetpz.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3oivbkyvh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mbxhhspz.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3eladstki.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3gktasaou.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3kassxpiz.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3cntjwdxr.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3kvxshrps.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3ytlpxvps.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3rhnqvdcl.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3qtiswhor.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3vaweqauz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3kysaodaf.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3uieirdnj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrdrmrdn.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3arzhhgjb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3cuvxfiju.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3btzqnczt.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3kpdkcbvy.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3egeeeuzd.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3abcdphtv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3cmcpknik.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3usczstzi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lmhbbdbh.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3tvneyvvq.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3zkmziggv.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3nkywsztn.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmpzyldu.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3vvvaqrnk.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3wavrexys.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3cycrlkeg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3tjgiijba.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ftbarfnl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rlxbumdo.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3vjifetvm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3zkcpwkte.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3brteftza.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3hdszygbh.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3bvehlzbx.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3huxigubm.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3msiizzal.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3mbyolzfo.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3tjozxmgp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ysmygnqx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3marjtwio.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3lquacfoo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xvymijig.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hwraleue.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3uqutlugb.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3txyjrfhs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3gshvaidj.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3bnzivthh.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3firgalew.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3rwsqzkbr.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3udbimcfj.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3cxxwfobq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3ifnqjhwb.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3piejvwgx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lwwwmqgq.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3voagvtep.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3lphaotnq.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3mcabyrpx.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3pnxwwrms.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3wamaevpr.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3ajoawpsv.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3keaxteip.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3dlxoolyy.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3vzpivqka.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3qttvdurl.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3kxjcewci.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qhfqjqto.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3nrtmrbrh.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gfxgymaj.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3prxjejle.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ugpveero.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3rfeoulhm.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3udotuqaq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dkrozmbh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tyuaayxz.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3kerryeel.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3txgutqqm.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jegvmdyt.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3jjpqcosv.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3nqphhzbp.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3ghrntnsl.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3goekuejb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3vwninmdz.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3qsisfzms.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3mbddidrx.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3jounadpp.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3hleuixcw.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3kkvfgilq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zmjbifrs.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3mjspilkh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xtfhhjfe.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3fhbactql.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3smnnlrsh.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3harjssfw.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ontpiyok.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3oydizbsu.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3pgiyuzlr.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qizarcav.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3gcodnjbt.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3sqgskmjh.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3cmpwzsqe.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3oznxqsyt.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3sxtmefqc.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qcklrchz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3djvbblxb.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ztedhbiv.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3wiwjuvus.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3opzvsoqa.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3wybqoabt.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3kohzdegj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3zzbeiefn.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3iodnlryy.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rxgybxpk.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3fapynutw.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3fjsibklu.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3gjajdhay.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3vjzckuly.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3jehboqlb.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3hvhqgmjo.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3piqatheb.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3adowpmay.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3upsioxvb.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3ihuxvurd.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zvmzmdzr.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3dpnkekfk.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3fyjeyorg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3efbqtowj.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zghqgirk.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3zbauyesr.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3jfwzimri.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cyhklqvh.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3ymfmlztg.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3fbqbxzkq.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3mfdmwiiz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3icqkkxlo.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3yfrgcjln.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3enwmdupt.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3cgpcagfu.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3syqvacnc.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3bufdfuqa.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ibfkvdhd.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pvpjjjrt.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3hjtpzdif.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3hcgxksns.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hqgvcwyn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3fjgmtxeh.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3iadexzzk.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3ujfhxerb.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3cnygbzzf.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3icujfpru.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3xlnqaziq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3segsjiqn.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ygonkdug.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lvzkulsq.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3bbdtjjwb.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3vhnpxzvr.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ydlqgjqq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3xgyjccmw.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3htqsnbuo.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3chsbtdmi.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3cajbalvl.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3wttqdeed.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3fqmzvryt.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3wmnsyiir.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fmolseip.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3malfifit.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3duosfczp.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3qvdpmpeh.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3iyocdbsn.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ahgdyrea.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ezgizpaz.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3oulpuwjy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3dniaaxff.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3qwuyztfm.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3idpsmevx.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3gfohvnyb.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3suowjdyx.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3omimahdv.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ftqqmbws.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3hnetsqbo.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3itrxcjeh.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3xaiohone.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3upteelzj.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3aunnnthd.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3tchixpnj.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3nqrhobbh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3gecdaksq.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3iijherph.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3aciljptm.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3agitlgry.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3dilyozjq.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3zylxqwid.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3wojcuenr.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3xczgnixz.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3alqphjdb.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3nulrsgbc.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3baxbknqm.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3srmoxwae.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3qejjnrxo.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3ldjazgcv.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3qfludyhj.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3qrqxnzit.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3wmpgzfau.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3luwqcqji.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3tpqlbovj.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3efmyorgp.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3yznjwbis.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3dlxwhohs.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3fvplrzke.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3tlcxykdk.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3nzcydvcs.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3helooxva.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3ddkcwkax.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3lslaozar.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3cieaeoov.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3zxgqqsjl.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3lxpfepwd.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3ijkvllbg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3heoifrgu.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3thjxswpn.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3fxtqxgxb.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3wuqxewrh.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3igvnhenm.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3cyfhgzeu.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3uuifjlmi.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3hwzfssdg.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3xdkppcgr.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3iqyaqxna.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3ncityfsl.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kbhcashx.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3xwcqtofy.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3cgedflzo.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3msqhddrb.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3tceopoth.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3wmrhpown.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3edxnobfo.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3npjssxia.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3fvmlgooi.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3jltjkdme.html


<!-- 参考信息 -->