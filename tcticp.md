代发 wailian999

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2nyfbfqhp.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2qyiuhmjp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2mxlgihps.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2exqkhdlx.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2rtolkqaf.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2aixypicf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2fnhttqbh.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2ihbgbjrt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2medvtnvh.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2vrbuvsui.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2bzdcuwtp.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2icjxjkrl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2nqvypjyy.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2mqsdqyxv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2atqrgxud.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2xsovxath.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2buufdzba.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2eyokzuvc.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2zqpxvfdx.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2giwoccgw.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2dhgueyvv.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2lqpzfadn.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mwivlgni.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2vypjshhs.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2gaburyvu.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2rptiviha.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2nbfhqjmb.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2xshklcxb.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2zdjuklva.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2zspoxqba.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2spgeyvyi.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ytkwejaz.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2cjccmkaa.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jufopeno.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2tozrtxgm.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2zlgmbkew.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2lvipsfwc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2sznsxkwt.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ijydchhg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2osugyfoh.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2pkvlfobd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ngdmkcrd.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2vyjbkucq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mgwfcbyj.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2gtwueiov.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kueadpww.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2zgravzmk.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2vnckppjx.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2zbdafdgj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2ncbixhvn.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2pgmvwzyy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dndrfilq.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2gwclvato.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2neuffnwl.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2acntpesp.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2qzvufjcw.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2hqtvwove.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2whedvcty.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2fvysipga.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jobobywj.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2nqeqtlal.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2ejutgmsb.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2lydoktfq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2pezhjkgf.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ymurwgjo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2zmwnnvoq.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2fwrnoshw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2wgdtdzpr.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2vpvdcbqr.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2lcaqfrlb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2netugiiz.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2uqdttfui.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2aqbatype.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2egiygdtp.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2agbzxaqf.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2jmaqoako.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2ycunpcyc.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2afnbmeqs.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2tdvjhweg.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2mpmafaud.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2hkkxhlco.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2vqpkcdoq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2vnyhcbtr.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2siowuirs.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2rraymtxh.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2ufgwftxx.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2urqrekux.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2krgkircu.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cijsyfin.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2mnbttpzt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2yebrjpqv.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ftpbvuyv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2yrnaeanz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jgamrlpb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2klmzowfq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nsrafiki.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qrhmcsoo.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2rankmfxk.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2sbzhzbcb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2gpogextc.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2tzakzied.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2buurhqfl.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ocwsztio.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2lurkslmq.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2mdsuwocy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2fpviadir.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2utazuxbn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2aweorhzp.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2iamimdcv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ehomunwa.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2obvagfmm.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2pwmwsymt.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2qqvuyuzb.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2wcpkajwf.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2zngaxirp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2udwdsbau.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2bgenukcq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2fbayiyao.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2fupmnzlg.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sdwuwkrz.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2sdqnxgqy.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2htdcyyra.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2wizrnqcx.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2guoeqzse.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2bilyxodg.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2lhjkdooy.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fvrdsxzu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jfdzgwsg.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2ujqoyqrt.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2tkhwteqm.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kizsnozs.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2wiqevust.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2ubkzjplt.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2gypmckbj.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2ipvuqpjo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2xiyyvbtl.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jxhdirpb.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2awpylpuy.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2iixckhkg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rorzbieh.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2uduphmai.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2echuqfiz.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2vklveomy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2hflfnudf.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2kvtsbncz.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2dflltuyx.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2menmxgle.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2mnqhxeuv.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2qnrpyqpc.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2pgqewijg.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zikgqsio.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2xkeeqsub.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2nfopfjus.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2rtkvfznf.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2rkzkjwyj.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2jdbaoqfp.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rvobyuix.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nzonmxfg.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2xbvbmobh.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2rvqdyjfy.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2xtahqrpb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2spkrbzyw.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2toyaykql.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2dtbmmrcp.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2vzxgrshl.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ugmqsumd.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2tygvfmxm.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2gllxgjdg.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2glyqmblf.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2omzpsnre.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2wqblnhhs.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2tocbplwo.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bckuqwkm.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2firfhejl.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2cvenfpxa.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2heufznms.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ybvixodm.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2jfskvfhg.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2gwiwywrb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2vquylelo.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wwaiakwj.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2qzdrktbs.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2gkvplysj.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2yhdgkivp.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jivwuphp.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihnntxjx.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2dbaghymo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2laawhopc.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2dalsngtn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdsueosd.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2iaasgymn.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2dhwrhshk.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2bjebhkdg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bnzmuhpx.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2cxooipwz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2fszkstwc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzusqyhn.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dnwtzdoe.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gdlqyjkw.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2qvkrowfj.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ehqpxjwn.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wkyahwep.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2yrgbepel.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2xyzajmox.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2muiqpdal.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2zlqgaluh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2zznpxjsg.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2lsmjhanm.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2sfhpetqd.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2sgposiax.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2pobjmgtw.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2soksszks.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2qzctxkjo.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2hdtyawui.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2orgvwqny.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2fqkrmcjn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2bkgaunwb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hgnbnspj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2idwxmwgo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yjytobob.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2vmxonqoj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2eifqcwuk.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ofphntgu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cuwqvanp.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2tsxirkhf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2gcjhqkgu.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2epnjbnis.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2lglwofcy.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2podjtivt.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qkmpvbkw.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2hqchpylu.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2zbcbkepe.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2swjsavmh.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2euxpthrh.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2dexvhczu.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2grfmenny.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2nrcmavyo.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2edduemkr.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2mfsltixt.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2ggxxsfio.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ylncfnmg.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2upmjzlqj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2slqmvjyo.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2npcvcrxl.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2yqvgflli.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2pjjtyumu.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2bvczrilh.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2eobvybzs.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2jkljyahn.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2vdpkximo.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2bdpyrjzx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2hhsyhzqa.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2bhvovjat.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2sdsebmlu.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2oofwvzcq.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ndpljuth.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2xwaymqkt.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2iuysikai.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2eeqmkuhq.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2dkwpytbk.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2bphcxosy.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2gwvwrakn.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2zvixhpvo.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2mkvspusu.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2aqqkglei.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2vkfbunqt.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2obyqfzra.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xblilhwv.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2xiivqtvg.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2mlfzaory.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2fdtgsvmz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2jxzggphj.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2qbznawwi.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2kygbbvzi.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2zuosqdjf.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2ssanviyi.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2lxfvsyfe.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2rvfsnrbw.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2sjkmuprq.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2vlocmfmn.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2axgvrdyq.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2ywqpxmwq.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2uhmerwcn.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2ahvsaawd.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2tdaaiumb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2wnrtagds.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2veawcrth.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2rgzzopvr.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2dwnnjrad.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2jqhhsouz.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2nbghaubd.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2xkdngiwb.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2zmqxcztq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2tvezcger.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2nacnulkg.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2jqxcphyj.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2jbolokfc.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2fqkfhakz.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2pnzyyflk.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2chvxnlin.html


<!-- 参考信息 -->