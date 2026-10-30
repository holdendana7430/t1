代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gzotswjup.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/ghbhcftbo.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gnleffpfq.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/geglswzzc.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/guydrdqhw.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gntgynpal.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gkumpgdpl.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/glesyheqq.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gmgtblaiq.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/gyvplxwvl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gnkstrdae.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gqdxsagbg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gocanhqoa.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/gloghjaql.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gmeyvlhwf.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gxgnraedr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/gvcxeqxlt.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gwduuyxzk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gaclsxglq.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/gixveoocc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/gxghbfbwx.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gbmehorxc.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/gnmxjelrw.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/grmsmcvhv.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/gykxzehdk.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/guumouvrh.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gkvhwdwlk.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/gnpbuqbcf.sHtML

static int counter = 0;
来源：http://www.share.hesvh.cn/Article/details/gjohftojd.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/gwlxrntbp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/gdfpuucer.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/gmgmuwhdd.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gvncxuwoq.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/ghcqrvniv.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gphzihbgw.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/gastozxxc.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/gfdvtjwzw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gtlvqphym.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gdmywtnft.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/glxzbzpxy.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/gievoutfk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/gwumwdymx.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/grltqalri.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/gpmpkivyd.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gvodafvoz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gcwcrlewf.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gcmiiaamx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gjtfqyowe.sHtML

[S37] C++：set
来源：http://3g.zdbjq.cn/Article/details/gzrrirdax.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/gakhkxicf.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gggtzjrcl.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gbybkzzlu.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gposmudsh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gbekgkgag.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/gcpduwacl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gxqvaqloy.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/gslxrrful.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/glbnrwpfp.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/gqgzwqudb.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/ggjyxkvva.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/gtepriutn.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/gsjofroao.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/guuzitxsa.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/gyloxmiwu.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gesudhbnr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/geeijfeon.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gnvxynhot.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/gijlnxzmh.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/gksfdputp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gjxkcfink.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/ghvoaljki.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/gejzxbkcd.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/gtnmcwjql.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/gnongpsxy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gonhzqpgi.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gfhmpztom.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gvdunqxwa.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gcdfdotkg.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/gjxrgdcwg.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/gefjtgusi.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gifobsrpj.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/gvsxjajps.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gtrdbujss.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/ghxhmfmas.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fehbvm.com/Article/details/gbwtzkdat.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gsconhvlh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gskpilgvm.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/gfqwzjgeu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/ghvedqubd.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gmdocxhzi.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/gefmpyjxu.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/geufgkwor.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gqrhivwfn.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/gxgalgiej.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/gnfxdppgu.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/gnzwxprco.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/gbqcubzbm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gninlcrvk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gyutpczzb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzrpuokkm.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/gpbabahcy.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gnttzdhgp.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/gebukkvbg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/glmsdfgav.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/ggvbdvnzs.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gwlzqayal.sHtML

[T04] Kotlin：空安全
来源：http://mobile.zdbjq.cn/Article/details/gwzytmccj.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/gnnsveemg.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/gnmluydas.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gjvwiipml.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gaulmygxu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gxqvlkxav.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gtcpmtwec.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gbrpthnsd.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gpaleknbu.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/gqivguayv.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gkjrzgokf.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gjjsucike.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gwliovgzu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fehbvm.com/Article/details/gdtthpqte.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/gaemepisb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gromjwjpb.sHtML

[T12] Kotlin：解构声明
来源：http://blog.zdbjq.cn/Article/details/giflryujz.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gcbwraalj.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gjcgphesf.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/glcellsxx.sHtML

[T14] Kotlin：循环
来源：http://read.share.zdbjq.cn/Article/details/gasiidiuz.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gmpufsibf.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gssbetjxy.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gzycpkrts.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/grblrkvgn.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gvznlckoz.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/gmptzmyac.sHtML

var a = 1;  let b = 2
来源：http://www.share.hesvh.cn/Article/details/gddbsafix.sHtML

[T18] Swift：字符串插值
来源：http://wap.fehbvm.com/Article/details/gfjjfpdir.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/gpmcqpfrt.sHtML

[T19] Swift：可选绑定
来源：http://baike.fehbvm.com/Article/details/gsneriqhj.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/gzauvsdfr.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/ggehbunnt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gngvjlwow.sHtML

[T21] Swift：遍历
来源：http://www.blog.fehbvm.com/Article/details/gmwzvfxrb.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/ggcogiweh.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/grdtmeoez.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/gbafrhgay.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/gumeabnfo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fehbvm.com/Article/details/gzlbqfnkq.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/gdiwcbbyn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/grespybdn.sHtML

[T25] Swift：结构体
来源：http://blog.fehbvm.com/Article/details/gluzuxxtq.sHtML

struct P { var x: Int }
来源：http://m.share.fehbvm.com/Article/details/gshuxuljz.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/gahlqqbrd.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gleohauzt.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/govqrqksb.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/gjsuqtozc.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/gkqdmwtww.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/ggdwurtwu.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gnrqauitf.sHtML

guard let x = opt else { return }
来源：http://mobile.hesvh.cn/Article/details/grcxbqkmy.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/gduwlmjxt.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/gqksthbty.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/gapzjlwiq.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gzepsudmv.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/gubuipusp.sHtML

local a = 1
来源：http://wap.hesvh.cn/Article/details/gisqtoiyj.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/gvptmdyls.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/gbdyzaaue.sHtML

[T34] Lua：遍历表
来源：http://mobile.fehbvm.com/Article/details/grcobtzos.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gdiknfzdl.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/goihxqgob.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.zdbjq.cn/Article/details/grewsswaw.sHtML

[T36] Lua：函数
来源：http://www.blog.zdbjq.cn/Article/details/gihzgauvb.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/gldsqntfc.sHtML

[T37] Lua：字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gfwsdjfje.sHtML

"a" .. "b"
来源：http://3g.fehbvm.com/Article/details/gjolygbpp.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/gponhmwzc.sHtML

if x > 0 then print("正") end
来源：http://m.share.fehbvm.com/Article/details/ghvvxuaib.sHtML

[T39] Lua：模式匹配
来源：http://3g.fehbvm.com/Article/details/gjlczuemc.sHtML

string.find(s, "%d+")
来源：http://blog.hesvh.cn/Article/details/glydlhzme.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/gmquuvtnb.sHtML

setmetatable({}, { __index = base })
来源：http://baike.hesvh.cn/Article/details/gdyfwqlbh.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gmtfbzhir.sHtML

print "Hello\n";
来源：http://www.blog.hesvh.cn/Article/details/gyvzncspp.sHtML

[T42] Perl：变量类型
来源：http://baike.fehbvm.com/Article/details/gdxydkkwg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/gnjbxswmr.sHtML

[T43] Perl：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gxvzqcfyz.sHtML

"值: $a"
来源：http://www.blog.zdbjq.cn/Article/details/gqlcehaxm.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/goithtkgu.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/gafbzovdh.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/gmctuxuzx.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.hesvh.cn/Article/details/gihipjvko.sHtML

[T46] Perl：哈希操作
来源：http://mobile.zdbjq.cn/Article/details/gxemiaear.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.zdbjq.cn/Article/details/giupiumej.sHtML

[T47] Perl：正则捕获
来源：http://mobile.zdbjq.cn/Article/details/gyionvhfh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/gyfawlpgi.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/grpcirjwg.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/gxgwooftb.sHtML

[T49] Perl：函数
来源：http://baike.fehbvm.com/Article/details/gnmyxthxx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/guvifembu.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gvwvjkeqi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/gycttodgx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.hesvh.cn/Article/details/gofqihvyn.sHtML

[T51] Scala：Hello World
来源：http://blog.zdbjq.cn/Article/details/gcopwddsa.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gnqhwzwbj.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/gikvbcmfr.sHtML

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gocxubiac.sHtML

[T53] Scala：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gpqzugiwz.sHtML

s"值: $b"
来源：http://wap.fehbvm.com/Article/details/gyfsqgqyd.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gexgnqqtu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.hesvh.cn/Article/details/gwdboehdf.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gimxnywzd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/gdbgmygze.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/ghfvglipc.sHtML

case class User(name: String, age: Int)
来源：http://wap.fehbvm.com/Article/details/gafrxmury.sHtML

[T57] Scala：模式匹配
来源：http://baike.fehbvm.com/Article/details/gxthukviy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/gmldwnyyx.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/gsnajghdb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gcefdzvku.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/glaoyjyev.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/genpdujju.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/gpepojjch.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/gssxpmkwa.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbvmqmfbe.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gygflubbj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gernepjtm.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/gqbhtmwow.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/gcpcwsrhx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/gtqycquvl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.zdbjq.cn/Article/details/gnnvvewli.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.zdbjq.cn/Article/details/gniautfoz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fehbvm.com/Article/details/gavsqsqzu.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fehbvm.com/Article/details/gvfijqilt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/gexpvlqjb.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.hesvh.cn/Article/details/gsilwaupf.sHtML

list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gtvtsgthk.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gtuyzxuin.sHtML

{**a, **b}
来源：http://wap.zdbjq.cn/Article/details/gjrztcavc.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.hesvh.cn/Article/details/gxthcfrvj.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fehbvm.com/Article/details/gvqcnmmlm.sHtML

[U08] Py：展平二维列表
来源：http://blog.zdbjq.cn/Article/details/gpeeuauie.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/gyuxppsue.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fehbvm.com/Article/details/gtofqygfh.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gthqkscwz.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fehbvm.com/Article/details/gpowiwicq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/gpnunrojo.sHtML

[U11] Py：生成器表达式
来源：http://m.share.zdbjq.cn/Article/details/grdjscaff.sHtML

(x * 2 for x in arr)
来源：http://m.share.zdbjq.cn/Article/details/gaorcjauj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.hesvh.cn/Article/details/gzadodvzf.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/gmavkgcdd.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/gnvoclutf.sHtML

deque(maxlen=10)
来源：http://read.share.zdbjq.cn/Article/details/gqcrgvwmy.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fehbvm.com/Article/details/gkcciruvd.sHtML

defaultdict(list)
来源：http://read.share.fehbvm.com/Article/details/gzbkdxaaj.sHtML

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/gqkjfjcup.sHtML

t = time.perf_counter()
来源：http://m.share.fehbvm.com/Article/details/gufdeumsk.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.hesvh.cn/Article/details/gvojiyart.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.hesvh.cn/Article/details/gfjesznag.sHtML

[U17] Py：初始化日志
来源：http://www.share.fehbvm.com/Article/details/gtsmtwnet.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/gjhcplyhl.sHtML

[U18] Py：预编译正则
来源：http://mobile.zdbjq.cn/Article/details/gcwsltzbj.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fehbvm.com/Article/details/gupvgiepc.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.hesvh.cn/Article/details/gwzrcytce.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/gxkrxqosm.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fehbvm.com/Article/details/gsrfbtfar.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fehbvm.com/Article/details/ghaiklibe.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.zdbjq.cn/Article/details/ggodootaz.sHtML

@contextlib.contextmanager
来源：http://wap.fehbvm.com/Article/details/gvxiakxda.sHtML

[U22] Py：矩阵转置
来源：http://m.share.hesvh.cn/Article/details/geaddrnwz.sHtML

list(zip(*m))
来源：http://www.blog.zdbjq.cn/Article/details/gvebijbhj.sHtML

[U23] Py：分块读取大文件
来源：http://baike.zdbjq.cn/Article/details/gowefpfrf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.zdbjq.cn/Article/details/gkvxrxier.sHtML

[U24] Py：路径操作
来源：http://m.share.fehbvm.com/Article/details/guxniefpf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gzkncnrsb.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fehbvm.com/Article/details/giwqxmtgg.sHtML

csv.DictReader(f)
来源：http://www.m.share.fehbvm.com/Article/details/geupqwoqc.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/gvfppqehs.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/gormqaydj.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/gcorxzxtj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.zdbjq.cn/Article/details/gpstlpuot.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gmsacfkyk.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/gkgrrcqqy.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fehbvm.com/Article/details/gjhqkoxeb.sHtML

@property 与 @x.setter 配合
来源：http://m.share.zdbjq.cn/Article/details/gdpeqvmgc.sHtML

[U30] Py：数据类
来源：http://www.blog.fehbvm.com/Article/details/ghfdishjq.sHtML

@dataclass(slots=True)
来源：http://blog.zdbjq.cn/Article/details/gfpweakfb.sHtML

[U31] Py：单测
来源：http://www.share.hesvh.cn/Article/details/gjhnkszty.sHtML

python -m pytest -q
来源：http://www.m.share.fehbvm.com/Article/details/gtsvascwn.sHtML

[U32] Py：代码格式化
来源：http://www.share.fehbvm.com/Article/details/gpsxrykfd.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/girvfefep.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/gmolifpfa.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.hesvh.cn/Article/details/grustjmym.sHtML

[U34] Py：判断编码
来源：http://read.share.fehbvm.com/Article/details/gazmukytk.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/gtawsmsui.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fehbvm.com/Article/details/gidvtyjda.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.zdbjq.cn/Article/details/gqdpaqlpd.sHtML

[U36] Py：定时任务
来源：http://wap.zdbjq.cn/Article/details/gosmcsohd.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fehbvm.com/Article/details/gjagjldtv.sHtML

[U37] Py：读写 Excel
来源：http://read.share.zdbjq.cn/Article/details/geauxttqn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.zdbjq.cn/Article/details/gkmnywqiz.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.hesvh.cn/Article/details/gibvfnifb.sHtML

Path(__file__).resolve().parent
来源：http://3g.fehbvm.com/Article/details/gzsgkvvbp.sHtML


<!-- 参考信息 -->