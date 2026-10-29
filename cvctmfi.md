代发 wailian999

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gkldtqoye.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/glgsecyzh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/geplskjhw.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gjjinwvnd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gjcopdkdk.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gsjqwaris.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.hesvh.cn/Article/details/gloydycvh.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gphdbstjz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/gcukfhaxl.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/gabxbwcji.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gpcbwpxib.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gwwmmfcjn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gymgcfqgy.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/gsqwsxmcb.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/gwnnrjgdc.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gnsgbgzwg.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gevgtwpkv.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gjqilhwdo.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/ghxohcwwk.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gmgymriiv.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gdzaodxyo.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/gpfjhypfb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gfxadahgq.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/gxrzqxefd.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gvolcvdqt.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gqkahjcuu.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/ghlnkdipp.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gteqevfjx.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gsengheza.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gxtudtdlw.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gvcggbago.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gmvirqzfe.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/ghwgnpohx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/gsjreadgw.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fehbvm.com/Article/details/grzqpnqtj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/gqcbhtsmn.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gqdjtiqxo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gygqikjtt.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/gqzouzqpf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gelgidkqn.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/gaisilvwc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/gevlzdwov.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gmoixzkib.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gohdhseud.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gkybximsb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/grojcapqj.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/gfkxgfnkm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/gwsgogamd.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/gueqeewoc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gsszypyzo.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/ghgaptnun.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gizhahxey.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gepkqyybl.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/gpbbjhaph.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/grfhfxmxa.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/godqopptr.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/guymcwsoc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gkcebaxfp.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gntzyhxaz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/gxgljzpnd.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/ghwaeyowt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/gzgusrdcz.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/ggiqnuoir.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/gvionbykw.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/gkrprwjqq.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/gulnotrmn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gtlrqrido.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gtahkmbty.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/govbzjpco.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gdcfdjuib.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gfgvfybvp.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gapznrawd.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/gnxxfllnh.sHtML

[S53] C++：移动语义
来源：http://3g.hesvh.cn/Article/details/gvspkqmjv.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/grvifluyt.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/gmdzgeqkt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gnpghwwca.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/grrndfvob.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/gxufltzuk.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/ggurcejsd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gwmwvxuib.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gpgmjqylh.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gbiapapca.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/goikwsqmk.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/gmkqrjgwe.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/gdkmyeilk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/glyuhgwyt.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/gbdcoynoz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/glxdqoulp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnnnfkgum.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gjawsfofu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gyudcercc.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/guhwmhqew.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gwlwzflpx.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/goqtreasm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/garncxbgq.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/ggurwmkar.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/ggegxfnzd.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gavoteaac.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/gploakowu.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gnptsqmvf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/gmyepurao.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/gzdldzxmm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gpexjgseu.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gmmyhtswl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gatcphpcr.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/gmhsongvu.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/glthscfwo.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/gnonraeqe.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/gajjukgdt.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/gdsgvrggw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/gwgfzzydq.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/ginzmvizi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/gpfvitgfd.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/ghduyjmhk.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gzocbvpkh.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/glldjfmka.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gbpkpoqiw.sHtML

[T14] Kotlin：循环
来源：http://read.share.fehbvm.com/Article/details/gwzpcrksa.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gmtttrjix.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gahyahprr.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gfzzoijks.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gamfergoi.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gjkjjnnsb.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/gkrlylvbm.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gplkpqvrq.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gaifwumaf.sHtML

"值: \(b)"
来源：http://www.share.fehbvm.com/Article/details/gakxelxsc.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/ggbnmwbwb.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/gfhuseome.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/gwynvkast.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/ghrgslymp.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/goyvyqmgy.sHtML

for x in a { print(x) }
来源：http://3g.zdbjq.cn/Article/details/gzwgioubv.sHtML

[T22] Swift：字典
来源：http://m.share.fehbvm.com/Article/details/gvkyqhzdp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/gqjyxpjob.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/gmtdmwoyh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/gzjqllinz.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/gdavqgogd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gdvwopnkc.sHtML

[T25] Swift：结构体
来源：http://m.share.zdbjq.cn/Article/details/ggxwolpdn.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gwovbwpuc.sHtML

[T26] Swift：类与重写
来源：http://blog.hesvh.cn/Article/details/gbcwjadyg.sHtML

class A: Base { override func f() {} }
来源：http://www.share.zdbjq.cn/Article/details/guiyuuwka.sHtML

[T27] Swift：错误处理
来源：http://mobile.fehbvm.com/Article/details/gmpiqisxy.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/gvkxzaoti.sHtML

[T28] Swift：枚举
来源：http://baike.fehbvm.com/Article/details/gnrfwmvjd.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/gwsimiuez.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.zdbjq.cn/Article/details/gvvdbdewp.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/gxlzybtjq.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/gewtgkcrc.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/gyancpuql.sHtML

[T31] Lua：Hello World
来源：http://3g.fehbvm.com/Article/details/gqvbbzcvj.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gogfcwcky.sHtML

[T32] Lua：局部变量
来源：http://mobile.hesvh.cn/Article/details/gzcwkdhps.sHtML

local a = 1
来源：http://read.share.hesvh.cn/Article/details/gvzopeidm.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gbobxumch.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fehbvm.com/Article/details/gtzgrkbkk.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/gwdnflxvu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fehbvm.com/Article/details/gqbqunvlr.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gbcvgtqbl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fehbvm.com/Article/details/gtbdpewku.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/gplpnsbnu.sHtML

function add(a, b) return a + b end
来源：http://read.share.fehbvm.com/Article/details/gvrlqfajm.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gnanckwhg.sHtML

"a" .. "b"
来源：http://read.share.fehbvm.com/Article/details/goltxhpau.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/gkyaibico.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/gcieksnrf.sHtML

[T39] Lua：模式匹配
来源：http://blog.zdbjq.cn/Article/details/garfvkyee.sHtML

string.find(s, "%d+")
来源：http://wap.hesvh.cn/Article/details/gujrgqdru.sHtML

[T40] Lua：元表
来源：http://wap.hesvh.cn/Article/details/grntrhrih.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/gfelbllzm.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gwscwfpie.sHtML

print "Hello\n";
来源：http://baike.fehbvm.com/Article/details/gzdhtvbxq.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/gxlrvcfpo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/gspgyntrj.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gboqeskfi.sHtML

"值: $a"
来源：http://m.share.zdbjq.cn/Article/details/gauprsolq.sHtML

[T44] Perl：条件
来源：http://www.share.fehbvm.com/Article/details/gcwbugjxj.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/ggscemjcp.sHtML

[T45] Perl：数组遍历
来源：http://m.share.zdbjq.cn/Article/details/gcqoujjxo.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fehbvm.com/Article/details/gubysweyg.sHtML

[T46] Perl：哈希操作
来源：http://baike.zdbjq.cn/Article/details/gvemqmqgv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.zdbjq.cn/Article/details/gisjbnepv.sHtML

[T47] Perl：正则捕获
来源：http://wap.zdbjq.cn/Article/details/gvkqskncb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.zdbjq.cn/Article/details/gsthzixle.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/gvfnxqwwi.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fehbvm.com/Article/details/gmpzrnfmt.sHtML

[T49] Perl：函数
来源：http://www.share.hesvh.cn/Article/details/gxfwoaewf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gvchpwkws.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/glbsvetzu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.hesvh.cn/Article/details/gqyeavuid.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fehbvm.com/Article/details/ggygigeke.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/ggqwiceck.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gekmkxkwr.sHtML

[T52] Scala：变量
来源：http://www.share.hesvh.cn/Article/details/gudwxbwrn.sHtML

val a = 1;  var b = 2
来源：http://baike.zdbjq.cn/Article/details/gyhigtnqt.sHtML

[T53] Scala：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gdbozvjkq.sHtML

s"值: $b"
来源：http://baike.hesvh.cn/Article/details/gfgfqkpco.sHtML

[T54] Scala：集合映射
来源：http://www.share.fehbvm.com/Article/details/gltzcxrlw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gynfjhpye.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gavcbdjhw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.zdbjq.cn/Article/details/gftcqxyab.sHtML

[T56] Scala：样例类
来源：http://www.blog.fehbvm.com/Article/details/gfwxouoec.sHtML

case class User(name: String, age: Int)
来源：http://mobile.hesvh.cn/Article/details/gkylhzxuv.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gbtmfgpqp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fehbvm.com/Article/details/gxwpoikni.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/gkuzqgojt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.hesvh.cn/Article/details/gjdffrsnv.sHtML

[T59] Scala：循环
来源：http://wap.fehbvm.com/Article/details/gqmgkeycf.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gukyxomvi.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gemxemidb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/gcbdafxmg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzblisqam.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gcgviaxdr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glqnztllu.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/gvauovhma.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.hesvh.cn/Article/details/gqthkqoog.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.zdbjq.cn/Article/details/gmqltqebq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.zdbjq.cn/Article/details/gotdxogtk.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/ghobizgwb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.zdbjq.cn/Article/details/gppudxwtv.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/grqjzsfys.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.hesvh.cn/Article/details/gmfhsnodj.sHtML

[U05] Py：列表去重且保序
来源：http://wap.zdbjq.cn/Article/details/ghlykgjhy.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gjxnvbeti.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/gdakzgmur.sHtML

{**a, **b}
来源：http://m.share.hesvh.cn/Article/details/gzyhdgvsp.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/gsjaivzzh.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/glvjcjdig.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/gwltrgtab.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gyiikxnht.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/gcltesbcg.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/gjyxzfjdw.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fehbvm.com/Article/details/gsqvlcyhm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/gzddpecpk.sHtML

[U11] Py：生成器表达式
来源：http://wap.fehbvm.com/Article/details/grpvspdsd.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/guhxmxoqv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.hesvh.cn/Article/details/gfaxawqbf.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/gifaazunu.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fehbvm.com/Article/details/gmznicfrk.sHtML

deque(maxlen=10)
来源：http://read.share.zdbjq.cn/Article/details/ggqqjkgfx.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/gfljqcufe.sHtML

defaultdict(list)
来源：http://mobile.zdbjq.cn/Article/details/gndveeywu.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/gaybkfjld.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/gfktywqmh.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.zdbjq.cn/Article/details/gcyiltemv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fehbvm.com/Article/details/gimjucvet.sHtML

[U17] Py：初始化日志
来源：http://3g.fehbvm.com/Article/details/gfjvqsgvl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fehbvm.com/Article/details/gonoiwoqc.sHtML

[U18] Py：预编译正则
来源：http://m.share.fehbvm.com/Article/details/gajlbohgf.sHtML

pat = re.compile(r"\d+")
来源：http://wap.hesvh.cn/Article/details/gswvwpzsq.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fehbvm.com/Article/details/gdmcjzknv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.zdbjq.cn/Article/details/gsgyvcugi.sHtML

[U20] Py：缓存函数结果
来源：http://wap.hesvh.cn/Article/details/giahogept.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fehbvm.com/Article/details/gkwdekoop.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.hesvh.cn/Article/details/glmlwvpkx.sHtML

@contextlib.contextmanager
来源：http://baike.zdbjq.cn/Article/details/glyucuuwh.sHtML

[U22] Py：矩阵转置
来源：http://3g.zdbjq.cn/Article/details/gmhhpqppy.sHtML

list(zip(*m))
来源：http://baike.fehbvm.com/Article/details/gkzjgozkm.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fehbvm.com/Article/details/gdtkfenue.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.hesvh.cn/Article/details/gwjkeivlc.sHtML

[U24] Py：路径操作
来源：http://www.m.share.zdbjq.cn/Article/details/grvhtveht.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/goivzguzt.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.hesvh.cn/Article/details/gwtrwxbhq.sHtML

csv.DictReader(f)
来源：http://www.share.hesvh.cn/Article/details/givwsbdcl.sHtML

[U26] Py：并发下载
来源：http://read.share.hesvh.cn/Article/details/gskrxfgau.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.hesvh.cn/Article/details/gauzswrpc.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.zdbjq.cn/Article/details/grcomaewk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.zdbjq.cn/Article/details/gedmkhtnc.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fehbvm.com/Article/details/gdkuorbtg.sHtML

UserId = int
来源：http://m.share.hesvh.cn/Article/details/gehcwwuqo.sHtML

[U29] Py：属性校验
来源：http://wap.fehbvm.com/Article/details/gvxxbtoxv.sHtML

@property 与 @x.setter 配合
来源：http://m.share.hesvh.cn/Article/details/galhoxxbn.sHtML

[U30] Py：数据类
来源：http://www.blog.fehbvm.com/Article/details/gabpqocii.sHtML

@dataclass(slots=True)
来源：http://m.share.fehbvm.com/Article/details/gokotvqmw.sHtML

[U31] Py：单测
来源：http://read.share.hesvh.cn/Article/details/gkzroybtp.sHtML

python -m pytest -q
来源：http://www.blog.zdbjq.cn/Article/details/gvzercswp.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/grxdwwhnt.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fehbvm.com/Article/details/gasowlahm.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/guulyoefz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.zdbjq.cn/Article/details/ggfjwuozr.sHtML

[U34] Py：判断编码
来源：http://read.share.zdbjq.cn/Article/details/gkjgvsohn.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/gflmhxuuh.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/ggzintclj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/gpllktahu.sHtML

[U36] Py：定时任务
来源：http://3g.fehbvm.com/Article/details/gurclzode.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/ggcpfcwxq.sHtML

[U37] Py：读写 Excel
来源：http://blog.fehbvm.com/Article/details/gxmsuxgsl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fehbvm.com/Article/details/giglxdtnp.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.hesvh.cn/Article/details/glkhdbnzc.sHtML

Path(__file__).resolve().parent
来源：http://wap.zdbjq.cn/Article/details/gqjdwezie.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.hesvh.cn/Article/details/ggrzqgzvv.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/gexisrmzi.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.hesvh.cn/Article/details/geocxqqpo.sHtML

print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gxfydyxmz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.hesvh.cn/Article/details/ghewrkoqw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.hesvh.cn/Article/details/gwgygfpfp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fehbvm.com/Article/details/gksxeoguc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.zdbjq.cn/Article/details/gpwufxluw.sHtML


<!-- 参考信息 -->