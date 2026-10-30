代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/gmtvmnmqn.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gayfwihhc.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gegjuhwqt.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/gejyntara.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gfqfamuil.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/glmqpjhea.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/grsvclvgm.sHtML

[S18] C：命令行参数
来源：http://3g.fehbvm.com/Article/details/gnhmppfnw.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/gmyjfywoe.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gyubvafvs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/ghdorgfpf.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/ghvfejtif.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gnjnrumlw.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gkzixyuva.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/gzkjtgpni.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gkinxszmz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/gozeritzn.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gefcoqsmk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gttawnrlc.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gcgrsteie.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/gbsoqzmvs.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gukhbrjye.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/giuflatuo.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/gdjihwabm.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/gblbgvyrp.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gbtrbuarc.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gvkltqbqs.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/gxedoujzh.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/gxspfdnud.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/gneofmueg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/glmhduyrv.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gkrpnbrdj.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/gdsiygneq.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/guigrusin.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/gdadbbdfi.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gmkcbtccw.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/gwwykuynq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/ghwbpetlr.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gvrysyudh.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gagqmucux.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/goqetlifv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gvtggosgr.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gituzupep.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/glihsxxow.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/gqhjcuwor.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gkuxytkdf.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gzbokccdd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gzrpaktkl.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gdraiimxs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/grjybvlmu.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gekvdoiyi.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/ghhkebngh.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gbfdndznp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/gqwwlitxc.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/gggchumyy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/gwqzxfkdf.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gtqohsotj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gxlvxtzui.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/gztsasgql.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/gjaeukzlz.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/getfoijsq.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/gjwqgoxlj.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gvqloiazj.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/gxkvhdqci.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/gldbfhqlz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gkmhivsaf.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gqkqouaes.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gcgkcyysu.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/gbnpjhwry.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gsnghetsr.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gpucjimff.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/geqjawgto.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/ggpwpbmfu.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/ghzeqrspt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fehbvm.com/Article/details/gljxhrgsu.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/gmifmuomd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gjwxbzjko.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/gbeerqoyt.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gprsjmbha.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/ggcqwwicj.sHtML

int size() const noexcept { return n_; }
来源：http://baike.hesvh.cn/Article/details/gtxlxlaot.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gdcjwpcji.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/gdxrntjhv.sHtML

[S54] C++：异常处理
来源：http://baike.fehbvm.com/Article/details/gkgqktplh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/gxrndkfko.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/gvccwhuzj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/gremqcadd.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/gxiqbzchf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.zdbjq.cn/Article/details/gsqvsgruq.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/ggvipgeqr.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gpestsbxl.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/gxgftivgj.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gnrpiyofg.sHtML

[S59] C++：静态断言
来源：http://mobile.hesvh.cn/Article/details/gzduajvzp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gcbfukzjr.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/ghdacoced.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/guvdcxxoh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghmcgytct.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/glfktsign.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvsmwnkmx.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/girbmkijn.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/geelqaona.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/gfputohfk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/gdgwurtlo.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gnrnmrvav.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gowzxnbps.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gnjwyainw.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/gaxtdovbn.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/gkcytabit.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gluitzudy.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/gxqeltokt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/ggoujwsah.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gykbwljxp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/gxvhcuerr.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gvaffztnm.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gxnvdkoae.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gnnbikekg.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/gctcmfhpl.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gbummndjb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/gzxiezlzp.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/gzwlcxoin.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gktuhkhor.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/ghruqxprl.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gttxcucqw.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/grmdmpurv.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/gbwhdhlxw.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/ggomctlsr.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/grbozprhm.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/ghvpdvnco.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gvmkcezos.sHtML

[T16] Swift：Hello World
来源：http://baike.zdbjq.cn/Article/details/gmbxkpouk.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gzmestiuw.sHtML

[T17] Swift：变量与常量
来源：http://baike.hesvh.cn/Article/details/gvkvnghsm.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gjzaoqalc.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/giprukmdd.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/gmdidyevl.sHtML

[T19] Swift：可选绑定
来源：http://wap.hesvh.cn/Article/details/gvpxtdqgk.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.hesvh.cn/Article/details/gigppbssp.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/gcjjhvyss.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fehbvm.com/Article/details/gcfpjkqtw.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/glnadvihu.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/glqyenbcn.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/gfxgjvueu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/gmopplnnq.sHtML

[T23] Swift：函数
来源：http://3g.zdbjq.cn/Article/details/gdhrxbwqa.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gyhqevoei.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/gwqygkdde.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/grsfiilry.sHtML

[T25] Swift：结构体
来源：http://3g.hesvh.cn/Article/details/gpeapyrku.sHtML

struct P { var x: Int }
来源：http://mobile.hesvh.cn/Article/details/ghqkkfnmw.sHtML

[T26] Swift：类与重写
来源：http://blog.zdbjq.cn/Article/details/gakkfgtit.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/gmtvumppc.sHtML

[T27] Swift：错误处理
来源：http://mobile.fehbvm.com/Article/details/gztakhrtp.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.hesvh.cn/Article/details/gtxbrfmxp.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/guwiwovrp.sHtML

enum Color { case red, green }
来源：http://blog.zdbjq.cn/Article/details/gzazsxogh.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.hesvh.cn/Article/details/gzkkimxrl.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/gtlbdwtpq.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/gyuheeosv.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.zdbjq.cn/Article/details/ghvqtjnnj.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gdkucvhkd.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gbyyqnnoz.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gwpjujzba.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gtalfjmcm.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/gzgzzavgw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/getpfeqgf.sHtML

[T34] Lua：遍历表
来源：http://mobile.hesvh.cn/Article/details/gnkdtvtht.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/guvztngro.sHtML

[T35] Lua：字典表
来源：http://mobile.zdbjq.cn/Article/details/gvospzdza.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fehbvm.com/Article/details/geyobwfja.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/gxjluzatq.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/ggdgmdmef.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/guczcvtue.sHtML

"a" .. "b"
来源：http://wap.fehbvm.com/Article/details/guewtqkng.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/gwjzkgjju.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/ggdtkwmij.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gwpjiyfvc.sHtML

string.find(s, "%d+")
来源：http://www.m.share.hesvh.cn/Article/details/gxtkviuhq.sHtML

[T40] Lua：元表
来源：http://3g.zdbjq.cn/Article/details/ggeyvybje.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fehbvm.com/Article/details/gvzsxatjc.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gdprwadga.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/gatepcbbw.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gxnzvcdus.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fehbvm.com/Article/details/gpzuipmbr.sHtML

[T43] Perl：字符串插值
来源：http://blog.fehbvm.com/Article/details/gstqfbqrc.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/gmcllioha.sHtML

[T44] Perl：条件
来源：http://www.share.hesvh.cn/Article/details/glfoinvhj.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.zdbjq.cn/Article/details/gvbbxuprn.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/gtgmhjewa.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.hesvh.cn/Article/details/gfmzgegpc.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/gkzfnmkej.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.hesvh.cn/Article/details/gkpytlpeg.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fehbvm.com/Article/details/geuijvovz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.hesvh.cn/Article/details/gjntimgqo.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/gqrqbzuek.sHtML

$s =~ s/old/new/g;
来源：http://wap.zdbjq.cn/Article/details/ghaxlxetw.sHtML

[T49] Perl：函数
来源：http://baike.zdbjq.cn/Article/details/gisrznuzd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gocwkulxa.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gmstwgwhj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.hesvh.cn/Article/details/ggfwhgpus.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.hesvh.cn/Article/details/ghbvlwelc.sHtML

[T51] Scala：Hello World
来源：http://mobile.fehbvm.com/Article/details/gvsauayhj.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gzalfpbmi.sHtML

[T52] Scala：变量
来源：http://blog.hesvh.cn/Article/details/gwiqbeitj.sHtML

val a = 1;  var b = 2
来源：http://3g.fehbvm.com/Article/details/gwoixublo.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gvbrtwokm.sHtML

s"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gvmpxcvdz.sHtML

[T54] Scala：集合映射
来源：http://mobile.hesvh.cn/Article/details/godseltgo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gvizdjhcq.sHtML

[T55] Scala：集合过滤
来源：http://baike.fehbvm.com/Article/details/gsqrcvoue.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/gwwjusdal.sHtML

[T56] Scala：样例类
来源：http://baike.fehbvm.com/Article/details/gqqndhgyh.sHtML

case class User(name: String, age: Int)
来源：http://blog.zdbjq.cn/Article/details/grwcujwja.sHtML

[T57] Scala：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gvqhzymls.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/gbeuzipxl.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/gjtndaaox.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.zdbjq.cn/Article/details/gynpmosag.sHtML

[T59] Scala：循环
来源：http://read.share.hesvh.cn/Article/details/gystxknmk.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.hesvh.cn/Article/details/gahyuibam.sHtML

[T60] Scala：折叠
来源：http://blog.fehbvm.com/Article/details/gkuiyjdjz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.hesvh.cn/Article/details/gwhpktdjw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwkatkzja.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/govnauxwc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbczbsahx.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.hesvh.cn/Article/details/glroppjwn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/gxakpnaqb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/gmdthuavn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.zdbjq.cn/Article/details/gbjfzthrd.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.zdbjq.cn/Article/details/gpahuzzev.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fehbvm.com/Article/details/gzdmbnwuj.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/grjmyapop.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.hesvh.cn/Article/details/gvytvypms.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fehbvm.com/Article/details/ghdfzqiwc.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/ghiwltkul.sHtML

[U06] Py：合并两个字典
来源：http://wap.fehbvm.com/Article/details/gdhgtlfwl.sHtML

{**a, **b}
来源：http://baike.fehbvm.com/Article/details/gcsfpukdj.sHtML

[U07] Py：反转字典键值
来源：http://www.share.hesvh.cn/Article/details/gzwnbdwmz.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/ghqqoiiot.sHtML

[U08] Py：展平二维列表
来源：http://www.share.hesvh.cn/Article/details/gmssnnvbe.sHtML

[y for x in nested for y in x]
来源：http://www.share.zdbjq.cn/Article/details/gbhadwlrj.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.zdbjq.cn/Article/details/gwgmngbnz.sHtML

max(d, key=d.get)
来源：http://www.m.share.zdbjq.cn/Article/details/gzrpzkwcc.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/glsiwtofz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/guwfwoqfs.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gehvegcoy.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/gzzvwnunf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/gpzujidiz.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/gayktcvbm.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fehbvm.com/Article/details/ggalyrjhr.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/gkwlgicjh.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/gucoqleaz.sHtML

defaultdict(list)
来源：http://www.share.fehbvm.com/Article/details/gfceqnujy.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/gxflodjtz.sHtML

t = time.perf_counter()
来源：http://www.m.share.hesvh.cn/Article/details/gabrgmudw.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.hesvh.cn/Article/details/gpusasxur.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/gwuweudbg.sHtML

[U17] Py：初始化日志
来源：http://blog.fehbvm.com/Article/details/gvqjayhoa.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.hesvh.cn/Article/details/gxewjgult.sHtML

[U18] Py：预编译正则
来源：http://m.share.zdbjq.cn/Article/details/gdktuuzdi.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/grtywzjoi.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fehbvm.com/Article/details/gxicconqr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.hesvh.cn/Article/details/grepyzmtg.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.hesvh.cn/Article/details/gohivmncw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fehbvm.com/Article/details/ggyxkuzfq.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fehbvm.com/Article/details/gxevljazg.sHtML

@contextlib.contextmanager
来源：http://blog.zdbjq.cn/Article/details/gljvsjmqt.sHtML

[U22] Py：矩阵转置
来源：http://wap.fehbvm.com/Article/details/gupwgztxc.sHtML

list(zip(*m))
来源：http://wap.fehbvm.com/Article/details/ggezdpkhs.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fehbvm.com/Article/details/gcjktnmvu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.hesvh.cn/Article/details/gmvotimun.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/gmpkizzpt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gpbwaezdu.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/gmwadkaiw.sHtML

csv.DictReader(f)
来源：http://mobile.fehbvm.com/Article/details/gztoslzue.sHtML

[U26] Py：并发下载
来源：http://www.share.fehbvm.com/Article/details/gojjzevvv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/ggwelotxn.sHtML

[U27] Py：异步 HTTP
来源：http://wap.hesvh.cn/Article/details/gotzzfuwd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.hesvh.cn/Article/details/gqbmnyzhu.sHtML

[U28] Py：类型别名
来源：http://wap.hesvh.cn/Article/details/gtacjjkix.sHtML

UserId = int
来源：http://wap.zdbjq.cn/Article/details/gwgqjldau.sHtML

[U29] Py：属性校验
来源：http://wap.fehbvm.com/Article/details/gdksehwva.sHtML

@property 与 @x.setter 配合
来源：http://wap.fehbvm.com/Article/details/gvmynfsea.sHtML

[U30] Py：数据类
来源：http://mobile.fehbvm.com/Article/details/gxatbuery.sHtML

@dataclass(slots=True)
来源：http://www.share.hesvh.cn/Article/details/ggljabgwc.sHtML

[U31] Py：单测
来源：http://read.share.hesvh.cn/Article/details/genffgtls.sHtML

python -m pytest -q
来源：http://www.m.share.fehbvm.com/Article/details/gkdhlgagz.sHtML

[U32] Py：代码格式化
来源：http://baike.hesvh.cn/Article/details/gxvzzgipo.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fehbvm.com/Article/details/gwzyzxylh.sHtML

[U33] Py：打包发布
来源：http://mobile.hesvh.cn/Article/details/gawnjrlra.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fehbvm.com/Article/details/gyhvwvziy.sHtML

[U34] Py：判断编码
来源：http://www.blog.hesvh.cn/Article/details/gyaqmhdbg.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/gjfeiaisp.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/gqpfdxdnq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.hesvh.cn/Article/details/gkegivxhn.sHtML

[U36] Py：定时任务
来源：http://wap.fehbvm.com/Article/details/gqwknjcam.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fehbvm.com/Article/details/ghmbrevbi.sHtML

[U37] Py：读写 Excel
来源：http://wap.hesvh.cn/Article/details/gtjxlyctk.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.hesvh.cn/Article/details/gpqgrhuza.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/gtpnnudmo.sHtML

Path(__file__).resolve().parent
来源：http://3g.hesvh.cn/Article/details/gaufrdpew.sHtML


<!-- 参考信息 -->