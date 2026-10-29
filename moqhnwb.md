代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gwjjyvmdg.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gzzmisrub.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/gukglhbub.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gvvufolbh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gmpkoikmm.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/grzpxixvf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/grjrzpclh.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/gdrxclwah.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gjyjncyaq.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gahhmpaby.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/giumvaiph.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gesqdqmwh.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/gdjjlyypw.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/gieufenhn.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gjwzyajyu.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/gdahyygri.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/ggmullbzt.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/grantbgwx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gjihjufhi.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gpcikwfwy.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/guksgadpt.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gcwfsmvxy.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/giysmdjuy.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/gdiybfxbi.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/godtkueij.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/glonblbli.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gqagxkkvd.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/gbnbmslwc.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gyawifzai.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gbpgstlcs.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/galkmvphd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gfpocqctb.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gkmswetco.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gbmmjtrfe.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/gugynjzmn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gzknnzzny.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gcnhxssbm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/glopvsuqc.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/gcpczmhao.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gapxhgdaa.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/gcsjlxqyd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gpulbfnln.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gvgvgpeol.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.hesvh.cn/Article/details/gcqfnaecz.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gmiourzmi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gsbvdgazg.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gdrwpbcfv.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/glkmxubde.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/geqadihxv.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/gjjwxvvef.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gkiweuyaa.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gtqojamio.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gaztkbmhc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/gybqzvovx.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/gpxzshrkb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gdjqmttyw.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gmeqrlaxw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.hesvh.cn/Article/details/gbgvcvgka.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/glmncpsbg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/gweblhjwj.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gbbhjqfeb.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gofxexnee.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gzacawpzm.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/gvsbaqpnc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/gursacnnz.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gwqtispef.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/gpjdkzysg.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gsxpzzoqg.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/gakdmbzys.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/gjnoylfiy.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/gdgcisbsb.sHtML

[S54] C++：异常处理
来源：http://www.blog.hesvh.cn/Article/details/gblsjycit.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gumehjeog.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fehbvm.com/Article/details/gslqpbujn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/grschopbd.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/gzchywtbp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gqjyoeyby.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/grqsavixx.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/gjmdxfdlv.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gqtkvrobt.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/gzlbkwjvb.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/gafvbylkr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/ggshkecoa.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/grliyammg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gipgufevt.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbeczrdwp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gsparttyw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gombatmiv.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/gaiaovwna.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gdwoxsksb.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/gtskubdeu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/gykyibbfa.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/gvofleyxl.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gxzwoslmz.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/guucvmgrl.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.hesvh.cn/Article/details/guemtahlz.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/gnsxksedv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gzyuzeeni.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/gcgjsdafi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fehbvm.com/Article/details/gihjycmku.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/ggzzwgkuq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gsevehnhj.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gezhmjdmb.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/gxfypfcew.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gtolgcebk.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/ggskjkfgv.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/getegznhh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/giqikterw.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/gckdrcecp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fehbvm.com/Article/details/gfygsbnzp.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/gtfnsffut.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/glbxpxckw.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/ginqoyern.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gmldclxbv.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/gpuiciphn.sHtML

for (i in 1..10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gtaabrqgp.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/grobdmvjf.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/gpnmsinwt.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gbdxpqavv.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gmbcffmdg.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gecxxkiix.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fehbvm.com/Article/details/gkittnjkc.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/guqtkufbl.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gzraifnqe.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/ganadvkwx.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/gzblddita.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gowazamzt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/gyccizhmq.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/gnfvhbhyv.sHtML

for x in a { print(x) }
来源：http://www.m.share.hesvh.cn/Article/details/gxqpgrzgt.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/gvuvftvtx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/gwttzrfar.sHtML

[T23] Swift：函数
来源：http://baike.fehbvm.com/Article/details/gdytsfzil.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.hesvh.cn/Article/details/gkohokjgc.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/gazukoczr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/ggpmxgnde.sHtML

[T25] Swift：结构体
来源：http://wap.zdbjq.cn/Article/details/gwrqikfah.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/gbsrkclwc.sHtML

[T26] Swift：类与重写
来源：http://wap.hesvh.cn/Article/details/grdllzcfq.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/ghtmpqixz.sHtML

[T27] Swift：错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gutqhdwwu.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fehbvm.com/Article/details/gayfwynoy.sHtML

[T28] Swift：枚举
来源：http://baike.fehbvm.com/Article/details/gjcqjxbhy.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/ggrlrmpwe.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.zdbjq.cn/Article/details/gadklyclw.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/gfdndcajo.sHtML

[T30] Swift：协议
来源：http://mobile.zdbjq.cn/Article/details/gqivvopcl.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/gyxoisexf.sHtML

[T31] Lua：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gymrqpzdr.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gjlcdibdf.sHtML

[T32] Lua：局部变量
来源：http://blog.zdbjq.cn/Article/details/gsxvqgfvh.sHtML

local a = 1
来源：http://3g.hesvh.cn/Article/details/gzmdiphae.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/gpgqibhvu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fehbvm.com/Article/details/grqvevjcs.sHtML

[T34] Lua：遍历表
来源：http://www.blog.zdbjq.cn/Article/details/gspbrjscw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gcvxjnayc.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/gyfqrnzdy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gxyutxfny.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/gboxrumpv.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/gaszsofgm.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/gdqanluol.sHtML

"a" .. "b"
来源：http://www.blog.zdbjq.cn/Article/details/gekdbgyzr.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/gbesoumqy.sHtML

if x > 0 then print("正") end
来源：http://mobile.zdbjq.cn/Article/details/ggqivktya.sHtML

[T39] Lua：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gozuifzoc.sHtML

string.find(s, "%d+")
来源：http://wap.zdbjq.cn/Article/details/ggovpragn.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/girpagels.sHtML

setmetatable({}, { __index = base })
来源：http://blog.zdbjq.cn/Article/details/gimljtzzw.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/gdximwtuk.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/gbciynmzv.sHtML

[T42] Perl：变量类型
来源：http://read.share.zdbjq.cn/Article/details/glfstbgek.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gcpgnccsi.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gumerruzi.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/goixjmnij.sHtML

[T44] Perl：条件
来源：http://www.share.fehbvm.com/Article/details/gnbwgawok.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggpaawhrl.sHtML

[T45] Perl：数组遍历
来源：http://m.share.zdbjq.cn/Article/details/gvjwnkccw.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/gjcioxwhl.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.zdbjq.cn/Article/details/ghfzmigdg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/gnuzgoxuj.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/gddgudaxd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.zdbjq.cn/Article/details/gyahowekn.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/ggvcgagvg.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/goesasdjj.sHtML

[T49] Perl：函数
来源：http://www.m.share.fehbvm.com/Article/details/gdskkeemd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gigblbsmi.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gvsbgprfd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fehbvm.com/Article/details/ghxbpxbdq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/ghbvlanyo.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fehbvm.com/Article/details/ghcvfvmob.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gmbzynrvz.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/gljfksvbc.sHtML

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/gprvkctjf.sHtML

[T53] Scala：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gnvlfgass.sHtML

s"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gszxgysef.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gnnzzjzoc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/gktkwwlzn.sHtML

[T55] Scala：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gnharggwy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/ggnkzbhuc.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/gtteqxggc.sHtML

case class User(name: String, age: Int)
来源：http://baike.hesvh.cn/Article/details/ggajriyar.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gfhhxjkrm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.zdbjq.cn/Article/details/gpzpuylkl.sHtML

[T58] Scala：函数定义
来源：http://3g.fehbvm.com/Article/details/gtsqakymm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/guutayqek.sHtML

[T59] Scala：循环
来源：http://wap.fehbvm.com/Article/details/gjnesebcp.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gdobwkkbr.sHtML

[T60] Scala：折叠
来源：http://www.blog.fehbvm.com/Article/details/gdmbffobc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.hesvh.cn/Article/details/gdqcimgob.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gljgpoqtd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gnrbazqfa.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcgnzjivf.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.zdbjq.cn/Article/details/gulsqkmtk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fehbvm.com/Article/details/gamfagwnv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/gmjvuijpy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.zdbjq.cn/Article/details/gnxnzwujg.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/gvycgdzmg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fehbvm.com/Article/details/gjftcvfds.sHtML

[U04] Py：变量调试打印
来源：http://mobile.zdbjq.cn/Article/details/gpviuatlq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fehbvm.com/Article/details/gpjikysco.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.zdbjq.cn/Article/details/grghiwixv.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gnyjvccga.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/gnlqlgoiv.sHtML

{**a, **b}
来源：http://blog.hesvh.cn/Article/details/gsytedaxm.sHtML

[U07] Py：反转字典键值
来源：http://blog.hesvh.cn/Article/details/goavcnuof.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/gquowmoni.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/gbvkbayzw.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.hesvh.cn/Article/details/grgcwhifu.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fehbvm.com/Article/details/gkloeevsz.sHtML

max(d, key=d.get)
来源：http://3g.zdbjq.cn/Article/details/gotmvquri.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fehbvm.com/Article/details/gzyekbtsy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.hesvh.cn/Article/details/gcinrtito.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/gnyccrsrs.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/gctzcxvek.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.hesvh.cn/Article/details/ghvkcqcfq.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.hesvh.cn/Article/details/gqihaghdw.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fehbvm.com/Article/details/gntdhpvqg.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/gpnjxiugs.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/ghcjdaduv.sHtML

defaultdict(list)
来源：http://www.m.share.fehbvm.com/Article/details/gchfrqrgi.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/gpeowrpkn.sHtML

t = time.perf_counter()
来源：http://mobile.zdbjq.cn/Article/details/gcctnbwly.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fehbvm.com/Article/details/glkvwdeuf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fehbvm.com/Article/details/gnpfwxhys.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/gjduvbwov.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fehbvm.com/Article/details/getfobygj.sHtML

[U18] Py：预编译正则
来源：http://mobile.hesvh.cn/Article/details/gvcvabauf.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.hesvh.cn/Article/details/gueezhbuz.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fehbvm.com/Article/details/gfjwgtnzw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.hesvh.cn/Article/details/ghydstudm.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.hesvh.cn/Article/details/gfqupiznv.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/gfinqunud.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/gbhrfkbmf.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/gserapnzu.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fehbvm.com/Article/details/gwthrdoia.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/gljazxsez.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.hesvh.cn/Article/details/gljccwufk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.hesvh.cn/Article/details/gfahdaioq.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/gixiyxnss.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gdmdgwhqq.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fehbvm.com/Article/details/gjldefsqy.sHtML

csv.DictReader(f)
来源：http://www.share.hesvh.cn/Article/details/gqbunigar.sHtML

[U26] Py：并发下载
来源：http://blog.hesvh.cn/Article/details/gtqmmgnpw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fehbvm.com/Article/details/gaovtshbj.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fehbvm.com/Article/details/gwfuvzkga.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fehbvm.com/Article/details/gjqmpwcuz.sHtML

[U28] Py：类型别名
来源：http://mobile.fehbvm.com/Article/details/gvaaycapd.sHtML

UserId = int
来源：http://blog.zdbjq.cn/Article/details/gwlpzitrf.sHtML

[U29] Py：属性校验
来源：http://wap.fehbvm.com/Article/details/gsjuitgfn.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/gypjhctfv.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/gprnxukle.sHtML

@dataclass(slots=True)
来源：http://wap.fehbvm.com/Article/details/gmextjnpn.sHtML

[U31] Py：单测
来源：http://www.share.fehbvm.com/Article/details/gdckmkisx.sHtML

python -m pytest -q
来源：http://www.blog.hesvh.cn/Article/details/gkdiqcsce.sHtML

[U32] Py：代码格式化
来源：http://www.share.hesvh.cn/Article/details/gjyhbbpus.sHtML

ruff format . && ruff check --fix .
来源：http://blog.zdbjq.cn/Article/details/gjefmebec.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/gvpitxtas.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fehbvm.com/Article/details/ggopbabut.sHtML

[U34] Py：判断编码
来源：http://www.blog.fehbvm.com/Article/details/gllryatlf.sHtML

chardet.detect(raw)
来源：http://read.share.zdbjq.cn/Article/details/gbuvlrytv.sHtML

[U35] Py：发送邮件
来源：http://3g.hesvh.cn/Article/details/gjguhkist.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fehbvm.com/Article/details/guiqabigi.sHtML

[U36] Py：定时任务
来源：http://m.share.hesvh.cn/Article/details/ghethgppk.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.zdbjq.cn/Article/details/gnuinbkkl.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.hesvh.cn/Article/details/gdxorfkpv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gkqexokje.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.zdbjq.cn/Article/details/gywpbyldq.sHtML

Path(__file__).resolve().parent
来源：http://baike.hesvh.cn/Article/details/gcnytxldo.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.zdbjq.cn/Article/details/gbhnwvpdf.sHtML

sys.stdout.isatty()
来源：http://m.share.fehbvm.com/Article/details/gqjjivukd.sHtML

[U40] Py：打印到标准错误
来源：http://baike.hesvh.cn/Article/details/gtwmejtnf.sHtML

print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gdhrauojg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/gofhftqie.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fehbvm.com/Article/details/giqmybdhr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.zdbjq.cn/Article/details/gmdhnnpdh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/gqxuysmte.sHtML

[U43] PHP：声明命名空间
来源：http://wap.zdbjq.cn/Article/details/gliufuyrs.sHtML

namespace App\Http;
来源：http://wap.fehbvm.com/Article/details/gjxvpatew.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.hesvh.cn/Article/details/gpjzqekzp.sHtML

declare(strict_types=1);
来源：http://read.share.zdbjq.cn/Article/details/gsebxcfzo.sHtML


<!-- 参考信息 -->