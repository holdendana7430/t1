代发 wailian999

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3netjhffa.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3zjnxmyvs.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3dyeeoyvf.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3dhcscyoj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3puegytnf.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3dumptfac.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3qwvbogbq.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3znnoccng.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ygiexciu.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3bphuojhx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3nekwmwcd.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3xfrvxgjz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3xxwtoowa.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3ryjtbdbb.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3pntdpjzj.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3zksoxuxq.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3fuxddwxl.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3syrjxbxr.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dftophtm.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3cfhpdixg.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3mkabgbuw.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3inkftvvc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3aazwiecq.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3wjupxhlz.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3pzojuipz.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3cirlzpct.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3zexikaqf.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nvmwzimc.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3klbqyqpb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3amsgucoa.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3ciwwfviw.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3uqhfyxsu.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3tzrraiza.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fvwoaxwp.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3xpxxmyrs.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fatwckmw.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3hisqqtnf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hpnrrodg.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3uvoxpmut.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3weiasfog.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3vnusfmdq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jefgipof.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3xzmpllop.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3velwevcj.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3lkbeajek.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3nkpiaqrq.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3jaburxdp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3xaojbcla.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3xxewjjkn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ppjdkyqk.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3sbgurhmz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3qqigcscc.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3qnxsmxde.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ldenxjkh.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3voddrbjn.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3owhvqtfq.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ulmwdhmn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3iujjazzx.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3zqqjmlfi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zgdhkolw.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3viogawav.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3polwuchh.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dchhakge.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3idzirsrz.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lsanoxhm.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3jakcgulo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3sqbubqsd.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3jflxnrcm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wvmfshgw.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3xmnheloq.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3zvwdttfe.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3jwvqmbzz.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3iiikhfmm.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3oohkhjtn.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3ldcyozlo.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ozldmijk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3hquslokr.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3fozimhht.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3rzwwnwvx.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3mwlmpfej.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ocxqzrab.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3byfxtoro.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pybjajsy.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3paqxwwoi.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fshcgskp.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3jvqvorgo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ajhcxkcf.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3xzavysth.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3addtljub.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wagdcpzk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ucbxghml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qgxshoch.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gwudzfmn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3panqkbzr.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3dvjzefzy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3jvohyogg.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3bvlgivbm.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3lywholoe.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3gsmhmnnr.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3cmqiootq.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qcouztkb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3yzrmnjll.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3txygtxrv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xgwcvmwo.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3tddubdvb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3cieqsinw.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3kbofnzzk.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3mgbjzokt.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3qiocumxo.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3mutuzjrk.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3wkkrlela.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3xnorxvim.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3jlbjzhlk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3theubxtw.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3ljjymhrg.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rcrijgum.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3qqeloqgx.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ztmiccrj.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3kilywkiv.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3wswkxguj.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3mympzmli.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3effufxsf.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uehhljro.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hsijtehg.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3xnzcepuo.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3mrtiqato.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ybuepdwm.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3jqhamucz.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3mxsjksec.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3ahxbuxyi.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3kpzghjyk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3kbsgsdtr.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3twwevhua.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3muwairpp.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3bgdnjrqz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mmgfeyry.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zxibtqsc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3dpdvbwhm.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3bsokleoq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ywmmcexx.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3yuemkume.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3rgbmsiok.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3lpbfrwkk.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3iilxqiwt.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3chtuazfb.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3fqugbfik.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3kdoxbyuv.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3aqfnlcfm.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ufhzgkbc.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3nbdlwlyh.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3rgayuolu.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3vdqhmoge.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3aloatozq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jyhzqkgi.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ncgxktur.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3xdfsnnon.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ulznqvoe.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3mqxcmtoa.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3xoqfzhvu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3sjtifwfq.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3lxczhmdd.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3edidiukx.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3irbeiekf.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3riwfhiqq.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3caaxnwij.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3cvuthqaf.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ltcsjtci.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3zesvblin.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fovjxshn.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ejzjnvdb.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3aklbketg.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3gfvdlooh.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jemoyqaz.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3fknhoegq.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3oaikwalf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ekpaljag.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3dyawkctp.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3tboosbpx.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3khimhieu.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3yzhtmipp.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3xtnmwyds.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ibwxvnbu.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3cffbkzkz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3frwsyhor.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3zvmshxjz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3ufqhlkoj.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3jtkmgmfm.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3ctwsdbjv.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3zuwnzuxp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nycifwmi.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mhutwcwh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3ltlsqjua.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3yaakvtcv.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ayfcfmur.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3duvvowvt.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3miwkdlvd.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tuavbsbs.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3baantdro.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3kuoykmiy.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3paogigqk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3ooikdvpu.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3pnorxqrj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tpwttfjf.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3bjzncdau.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3sqbnuzna.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3hxortnva.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3uyhjhelt.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3ktioigbf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3ipwmjehv.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3czktxnjj.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ltcwwsab.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3evjkvfdl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3mgekvyup.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yioyqvoe.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3uuaqwijy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eoqemzvw.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3gktkrlaj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3ujrznhgh.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3zxyxnkjo.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3wpczfntk.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3hcnsmwvj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3ptcxesvh.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3fueseing.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3kpbeprxk.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3mfexaojj.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3jqunucnv.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3kbjrgzob.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3dsmsggrw.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3dkvblvwn.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3glcqxupf.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3updkmdan.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3pxvhexdd.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3sjmxanfm.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3uevkqdjt.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3flhcwwcz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3chrukgbt.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ycxfhimv.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3klsedyxm.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3pexnvick.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3qifmfmll.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3mgxagvls.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3wanpdrtj.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3dovurswc.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3orckqufx.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3ejtomhgq.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3vsdoduac.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ikpvszbs.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3uruisivx.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3prxurjuf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3gxjapuyc.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3gojoaolu.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3luozgdsr.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3lyuwmdex.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3juzgfnbd.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3maqivoae.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3zicceybt.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3janwfugx.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3zkldjfyq.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3bljwnytk.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3cixjxxbq.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3mwtcizcg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3stajefgc.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3bkdnobil.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3sqmvoouu.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3umyucfng.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3iaxjvcvi.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3cncpizuv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3jsloibro.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3sdywxoov.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3wdswtqfx.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3mvimpyiy.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3pfrspmmq.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3ugyuoeck.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3cgbvszmw.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3igwsszve.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3phjjboxr.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3nogsfjla.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3idohtalb.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qnepojdz.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3vubkhzvl.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3fecuvbev.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3rtjahxqa.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3wbvlyjtm.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3wcyfkmsf.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3nbiqomov.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3qaxxlexa.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3qhlkplst.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3fdqmtjqg.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3szoipnva.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3wawikuie.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3gvacorkw.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3sapyabhd.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3icckkqhf.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3aweppibt.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3tmccjdvg.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3xxboviyf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3nnjzzmlt.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3lpmvldwj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3yjaeehpr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3vjzdiwzm.html


<!-- 参考信息 -->