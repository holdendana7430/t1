代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/gthnqaain.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/gnscdpuiw.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/gwwpzavku.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/gfyelhqoi.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gjqvhdffr.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gwuqfmais.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fehbvm.com/Article/details/gjprzsrhd.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/grexdhzju.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/glitgjxpa.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gesspieqf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gmyphtiof.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/ggugkxmqc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gsozwrdfg.sHtML

[S21] C：字符类别判断
来源：http://mobile.zdbjq.cn/Article/details/gegkozzig.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.hesvh.cn/Article/details/gtgfqhqgz.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gxnkwgdde.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/gnmiuikeh.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/gygkaqrjz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/gehztzzqz.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/glprtiliy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/gszfbnbcs.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gmovcccim.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/gdyqcxwfj.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/geeezyajk.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gdiozbexy.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gdrjzlrnb.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gakcaepsn.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/gtkkwtopo.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/gmvpsgwgb.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/gqbwkvdry.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gwfopqede.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/geuzkqmph.sHtML

#ifndef X_H
来源：http://wap.zdbjq.cn/Article/details/gvcmbemaf.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gcaqcuixl.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gkremgpjp.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gxczayolk.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gulwcsoph.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gmxugcsrq.sHtML

[S32] C++：字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gmswxergg.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gpesziimc.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/gmkpjhorh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/gfhsccrng.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/gzygiwgos.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gieuixcmp.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gblxvmwhw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gaejwikmy.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/gyknamxqo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/glbydwyjm.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/galgkkbtu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gwtudnecz.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/gaijlrlet.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/glmryuwmj.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/gaxjyoawi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gkgrmfjrl.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/glvlmdmkp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gzajabgxy.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/ghzkotoya.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gjynqtxtn.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/ghrivftpk.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/glkgrbxeo.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/gwxtupikp.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/gorotcatl.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/ggpwgurpf.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/gwpvriyno.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/gyvitxiuu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/gurjgejsp.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gqruftlqc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/grfeoitbe.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/gnyafpvjq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gwhrycjta.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gwgqklpno.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gjtlvruyb.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/gswbwbvdq.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/gpnwxdeea.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/golgqutqs.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gfrirfokq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gmakahgnk.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gqwwuqfyq.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/gfeawffpj.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/gwjitjryc.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fehbvm.com/Article/details/guuxzrxvj.sHtML

[S53] C++：移动语义
来源：http://baike.hesvh.cn/Article/details/grkcosyut.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gaspihirf.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/geksjnoct.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/ggdpzrvip.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/gqhiivlal.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/gfvdoqssd.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gxezbkusk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gzzxwjtce.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/gaalumaof.sHtML

constexpr int N = 10;
来源：http://m.share.fehbvm.com/Article/details/gexcnzupu.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gmsdopscc.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/glskmeija.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/gcdrnzoqn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gunsbehdv.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/gyzvsqvfu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gfhppckdc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/goeuuljip.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gglhzpmyo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glrehysho.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gdorqierm.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gmeehkfhe.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.hesvh.cn/Article/details/gerytqrne.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.zdbjq.cn/Article/details/gpvafqidq.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gpvdefkvx.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gzsdsjuyh.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gmfsinaew.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/giajgeuoy.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/gbyxwzbku.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gubufzdtx.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gqiuqybzi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/guloxiayc.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gkskoruga.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/grhrfwbpa.sHtML

[T08] Kotlin：数据类
来源：http://wap.fehbvm.com/Article/details/ghcxckbft.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gqlqllgrv.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.zdbjq.cn/Article/details/gmleukxzi.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.zdbjq.cn/Article/details/gjvsnblxz.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gbgmicjcz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/gdydigrtl.sHtML

[T11] Kotlin：协程
来源：http://3g.hesvh.cn/Article/details/gebzxibmy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/genddzuzf.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gkxhynuiv.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/grunsltdi.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/gpfxbibbg.sHtML

val m = mapOf("a" to 1)
来源：http://wap.hesvh.cn/Article/details/gzetxxjjw.sHtML

[T14] Kotlin：循环
来源：http://blog.zdbjq.cn/Article/details/gmlvxtkfr.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gvkvfftsb.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/gbzawokbr.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/ghgaojnix.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gzgahegcq.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gszjckupv.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fehbvm.com/Article/details/gjupxnagf.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/gjcecklry.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/gmhsmmoro.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/gwmiojhbm.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/grbiutngv.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/ghbqaasyw.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/gugxhpiis.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/gxaaqbqyq.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/gdnzadnmp.sHtML

for x in a { print(x) }
来源：http://3g.zdbjq.cn/Article/details/gxojinhga.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gmutdxjts.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/gomaqyanf.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/geaqktfzx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/gwiitvewb.sHtML

[T24] Swift：闭包
来源：http://mobile.fehbvm.com/Article/details/gqumtovzj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gglawrvbm.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/gtvitxnjt.sHtML

struct P { var x: Int }
来源：http://blog.zdbjq.cn/Article/details/ggmoetnlh.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/gbjkpofey.sHtML

class A: Base { override func f() {} }
来源：http://www.share.hesvh.cn/Article/details/ggaiuuzie.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/grsywajjt.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gqdxuynsz.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gtfabwbme.sHtML

enum Color { case red, green }
来源：http://www.blog.hesvh.cn/Article/details/gmylswfwn.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/gsarnnirh.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/grmzvwfix.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gdjwvlgrg.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/gsrteekrs.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/gpglpdvky.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gfvjojljy.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/gskrsmkpz.sHtML

local a = 1
来源：http://wap.hesvh.cn/Article/details/gjtwyuldc.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/gvqmytuls.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/ghsfooahn.sHtML

[T34] Lua：遍历表
来源：http://mobile.zdbjq.cn/Article/details/gddadzdki.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.hesvh.cn/Article/details/gznhfhyxs.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gmvtatgmn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gukjzyurr.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gqhfotega.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/gjooatgfz.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gfjlmezdu.sHtML

"a" .. "b"
来源：http://www.m.share.fehbvm.com/Article/details/gfojwtatb.sHtML

[T38] Lua：条件
来源：http://3g.hesvh.cn/Article/details/gjwetgcos.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/gdibijtvb.sHtML

[T39] Lua：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gzapfpjin.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/gmzcjoasi.sHtML

[T40] Lua：元表
来源：http://www.share.zdbjq.cn/Article/details/gmwuwaqvk.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/gyqcxibza.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gzfyvonok.sHtML

print "Hello\n";
来源：http://www.share.zdbjq.cn/Article/details/gmdoullfg.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/ggrgeskmn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.zdbjq.cn/Article/details/ghpxwomzd.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gghxfuaoe.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/ggxupycox.sHtML

[T44] Perl：条件
来源：http://3g.fehbvm.com/Article/details/gmjiqxehs.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.zdbjq.cn/Article/details/gdnrdkgne.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/gnpwcyqpp.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/gkhsthoog.sHtML

[T46] Perl：哈希操作
来源：http://blog.hesvh.cn/Article/details/grplnsfur.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gtadqufbv.sHtML

[T47] Perl：正则捕获
来源：http://blog.zdbjq.cn/Article/details/gtgkgnaif.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/glcaktkhd.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gkhebnpur.sHtML

$s =~ s/old/new/g;
来源：http://3g.fehbvm.com/Article/details/gilktgwvv.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/gegtoyazu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gvclhkslx.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gltdpyuzx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.hesvh.cn/Article/details/gsdzpqcff.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fehbvm.com/Article/details/gjbmeukce.sHtML

[T51] Scala：Hello World
来源：http://mobile.fehbvm.com/Article/details/gznoffsez.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gqpsrocvo.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/gnahzrqhy.sHtML

val a = 1;  var b = 2
来源：http://www.blog.hesvh.cn/Article/details/gkvafozbv.sHtML

[T53] Scala：字符串插值
来源：http://wap.fehbvm.com/Article/details/gvrvamzbf.sHtML

s"值: $b"
来源：http://wap.hesvh.cn/Article/details/grbomjpen.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/ghygxkywy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gtccadeel.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gzkmiwncd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.zdbjq.cn/Article/details/gvrzlqufi.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/gwofutjlh.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fehbvm.com/Article/details/geblyggto.sHtML

[T57] Scala：模式匹配
来源：http://m.share.hesvh.cn/Article/details/grzrstpvz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.hesvh.cn/Article/details/gmuagfajh.sHtML

[T58] Scala：函数定义
来源：http://mobile.zdbjq.cn/Article/details/gwfyqrjbd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gfoxnxpvr.sHtML

[T59] Scala：循环
来源：http://mobile.hesvh.cn/Article/details/gmxdnmthn.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gjjshchsi.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/gwhzaxngl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.zdbjq.cn/Article/details/ghwpxivcn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gndveiwco.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gzmryjjio.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gltvkhhia.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fehbvm.com/Article/details/gvvsdcnxe.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.zdbjq.cn/Article/details/gnyohrbid.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fehbvm.com/Article/details/ggurdieeo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.zdbjq.cn/Article/details/goprprgnt.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/gkizlzact.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.zdbjq.cn/Article/details/giigfzlew.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/gofmppsxq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fehbvm.com/Article/details/gbucsopdj.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.zdbjq.cn/Article/details/gujzwvzeh.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gizpdgolh.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.hesvh.cn/Article/details/gwlksoxoo.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gdvybyewn.sHtML

[U07] Py：反转字典键值
来源：http://m.share.zdbjq.cn/Article/details/gsnkrmtwm.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fehbvm.com/Article/details/gwizkyjwr.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/gzixefbjd.sHtML

[y for x in nested for y in x]
来源：http://read.share.hesvh.cn/Article/details/gfgorlduu.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/gtfhtuuky.sHtML

max(d, key=d.get)
来源：http://baike.fehbvm.com/Article/details/gpushlnlg.sHtML

[U10] Py：按值排序字典
来源：http://mobile.zdbjq.cn/Article/details/gacqldnmi.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/gtbjrsehc.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fehbvm.com/Article/details/ghsovvxby.sHtML

(x * 2 for x in arr)
来源：http://blog.hesvh.cn/Article/details/gnzlbyvfr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fehbvm.com/Article/details/gvmpsheml.sHtML

Counter(arr).most_common(3)
来源：http://wap.hesvh.cn/Article/details/ggeuxvrfm.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fehbvm.com/Article/details/gralobssw.sHtML

deque(maxlen=10)
来源：http://read.share.fehbvm.com/Article/details/gdhjgoavz.sHtML

[U14] Py：分组收集到列表
来源：http://blog.hesvh.cn/Article/details/gdimiizxa.sHtML

defaultdict(list)
来源：http://mobile.hesvh.cn/Article/details/gxztfqufw.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/gdziclcxb.sHtML

t = time.perf_counter()
来源：http://www.m.share.fehbvm.com/Article/details/guztgguww.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.zdbjq.cn/Article/details/glbizipds.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.hesvh.cn/Article/details/gkdqhbwoc.sHtML

[U17] Py：初始化日志
来源：http://mobile.zdbjq.cn/Article/details/gpzsgiyqu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fehbvm.com/Article/details/gtbtqmxyv.sHtML

[U18] Py：预编译正则
来源：http://mobile.fehbvm.com/Article/details/gdlpwjwxs.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gfjkyopbr.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fehbvm.com/Article/details/ghgdznebs.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fehbvm.com/Article/details/gnnvfzxeb.sHtML

[U20] Py：缓存函数结果
来源：http://wap.hesvh.cn/Article/details/gnmwxyrwl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fehbvm.com/Article/details/gxdyonqgo.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.hesvh.cn/Article/details/gncwmbblr.sHtML

@contextlib.contextmanager
来源：http://www.share.hesvh.cn/Article/details/gryawblbe.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/gsyinvlty.sHtML

list(zip(*m))
来源：http://www.blog.fehbvm.com/Article/details/gkxjbyhcf.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/glamrshal.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fehbvm.com/Article/details/gzyqdptqu.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/gvvaaaant.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gwvnrwkvu.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fehbvm.com/Article/details/guigbrjpg.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/gucbdiaop.sHtML

[U26] Py：并发下载
来源：http://mobile.zdbjq.cn/Article/details/gfdnrtpkt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.hesvh.cn/Article/details/gygsloivy.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.zdbjq.cn/Article/details/gxqdandul.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.zdbjq.cn/Article/details/givliywvb.sHtML

[U28] Py：类型别名
来源：http://blog.fehbvm.com/Article/details/gysekdjhk.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/gqexfhbib.sHtML

[U29] Py：属性校验
来源：http://3g.fehbvm.com/Article/details/ghfoqglji.sHtML

@property 与 @x.setter 配合
来源：http://read.share.zdbjq.cn/Article/details/gdtwgylwx.sHtML

[U30] Py：数据类
来源：http://read.share.hesvh.cn/Article/details/gtkkpobei.sHtML

@dataclass(slots=True)
来源：http://blog.zdbjq.cn/Article/details/gmkrflyao.sHtML

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/gfmznrzhj.sHtML

python -m pytest -q
来源：http://www.blog.hesvh.cn/Article/details/gjfyxhfqi.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/gmhssrluv.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.zdbjq.cn/Article/details/ggnlirviy.sHtML

[U33] Py：打包发布
来源：http://wap.hesvh.cn/Article/details/ggodktekc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/gwefbpgwl.sHtML

[U34] Py：判断编码
来源：http://www.blog.zdbjq.cn/Article/details/ghrzldupx.sHtML

chardet.detect(raw)
来源：http://wap.fehbvm.com/Article/details/gmgopqdzx.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fehbvm.com/Article/details/gjupsetkr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.hesvh.cn/Article/details/gaqcxbkgl.sHtML

[U36] Py：定时任务
来源：http://read.share.zdbjq.cn/Article/details/gmkjxeffu.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.hesvh.cn/Article/details/grsalxpjg.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.zdbjq.cn/Article/details/gbwlovicc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fehbvm.com/Article/details/gcqksisav.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fehbvm.com/Article/details/gbvmnwxnj.sHtML

Path(__file__).resolve().parent
来源：http://baike.hesvh.cn/Article/details/grjbnlckg.sHtML


<!-- 参考信息 -->