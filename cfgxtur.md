代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gkhcenhng.sHtML

[S13] C：宏定义
来源：http://www.share.zdbjq.cn/Article/details/gjchcgpen.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gmczxzeum.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/gsecprenj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gnykxhske.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gpwhdsadd.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/gdjkrbklc.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/gmfwmfugq.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gliusqlur.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gdllnputg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gfhofrqsa.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gkvpxakch.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/glijlexqy.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/gluzoizat.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gzrkduzbd.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gvkqnzvzn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gdpisyzvv.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/giqzwdwhd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/gdgbmqhnt.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gyqmxgkyg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gcsjzyngf.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/gzjbbvkim.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/giqpelkis.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/gweoxnjhd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gumeympok.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gspofzxru.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gcqtqydky.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/geettilma.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gwzmiaqlo.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/gslrttqjp.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gnjpesncb.sHtML

[S28] C：静态变量
来源：http://m.share.hesvh.cn/Article/details/goghvhyub.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gweugqcne.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/gygrzqgib.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/gyijyaehp.sHtML

[S30] C：头文件保护
来源：http://www.blog.zdbjq.cn/Article/details/ghnkwnotg.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/gggbbdbtj.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/gxhiyyzwx.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/gflxahwih.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gssgqhute.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/grqvtbztk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fehbvm.com/Article/details/gepdjuujl.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gveqlawwg.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fehbvm.com/Article/details/gklwrreak.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gvtgainmv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fehbvm.com/Article/details/giuaowiax.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gtnkxzuww.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/gqvqtxmdn.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/gsziyblfs.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gtclxubgg.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/gknaavgre.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gymelhizc.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gewrezsdg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gfoadkuts.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gbhzvugtg.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/gbmbknfqv.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gbknxmynr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gncraiapo.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/gajuhddel.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/ghsblydnv.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/gipardwaw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/gbowgfplj.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gkfqsqtkx.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/gkwhkdwvp.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gqyubkcwj.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/gqtqdkjzm.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/goineubdt.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gddugojej.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/gbxlaqrvo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gxqxcfizp.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gzvxhvioj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/gkjcsdnok.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gldewlfxh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gwlvztiar.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gctvdmmtz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/ghfhkrkda.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/gtkptynis.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gopefbmco.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/gatlcjqsn.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/gnnzwhzto.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gljdjiqds.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/gryelaywc.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gkckdaxfb.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/grfxvykpr.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/gqdrizmhi.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gclpbqxmu.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/geffhgdzh.sHtML

[S54] C++：异常处理
来源：http://read.share.fehbvm.com/Article/details/gjoedxmhb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gvukuuuch.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/gcjfygrhr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/gqxmstxlj.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/gymapnmmm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/ghkiubgth.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/gplyxqhim.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gpawbbnuw.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/guibmlcsp.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/geqmzjskl.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/gjjayfxbs.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/gmeejkush.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/gfxzdfixz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gsohuonlk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsqparyqs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gjvgnkzab.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvmyyspal.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gkefmzktu.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gqbioqkof.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/gywvwrufr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/glonmpuqr.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gxbjijldx.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gdivmktax.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/gxtetsbhp.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gkwaswnvv.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gkdruiwon.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/grvbhrkcz.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/gbarzxrug.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gbbhxlqps.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gomcszgdu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gpcotgcfl.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/ghcagxsan.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/ghvkjwkbu.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/gpqpjdand.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gjwfisqgh.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/grjaoedem.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/gyeijoixq.sHtML

[T11] Kotlin：协程
来源：http://wap.hesvh.cn/Article/details/grltbaflh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/gvaipsgbc.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/gckpryegx.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gzlequhaw.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/gwvynrfej.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/gctdcotqw.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/gjepibhlt.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/gpttobsps.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/gvopxdyls.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/gzccavqow.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gswyzxopq.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gnhbqcaag.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.zdbjq.cn/Article/details/ggghszzgy.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gmuizdmkj.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/guymehmcm.sHtML

"值: \(b)"
来源：http://www.blog.hesvh.cn/Article/details/gtrfwbxqx.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/gwgkvdfvg.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gxwsnoelx.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/gilnaejkn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.hesvh.cn/Article/details/gbxaaksgk.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/gtvdyioid.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/gjskmywtz.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/gvdvvhzyr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fehbvm.com/Article/details/ggbabvfgp.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gvnuzldaq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/gdecjbxdw.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/gfpendxls.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/gkyglzxts.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/ghsplzhya.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gblncjtdx.sHtML

[T26] Swift：类与重写
来源：http://www.blog.hesvh.cn/Article/details/glybhxcxe.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/ghqhvzkwn.sHtML

[T27] Swift：错误处理
来源：http://www.blog.zdbjq.cn/Article/details/glxufdzya.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fehbvm.com/Article/details/glvzvxodp.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gcgyqoonq.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/giulfartj.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gtypghepm.sHtML

guard let x = opt else { return }
来源：http://m.share.hesvh.cn/Article/details/gdknvoddt.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/gshiezriq.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fehbvm.com/Article/details/gstuziown.sHtML

[T31] Lua：Hello World
来源：http://3g.zdbjq.cn/Article/details/gjluazago.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gkxciciso.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/gqjtmrjmm.sHtML

local a = 1
来源：http://wap.hesvh.cn/Article/details/gyonsgsnk.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/gyvolzibe.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fehbvm.com/Article/details/gkgrbquhx.sHtML

[T34] Lua：遍历表
来源：http://read.share.fehbvm.com/Article/details/gtyiesnri.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/groywlbsk.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/gugdmxryg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fehbvm.com/Article/details/gbxjlgmkg.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/ghqokdmyz.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/gmikwmsqn.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.hesvh.cn/Article/details/ghwprdufj.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/gdeuskahm.sHtML

[T38] Lua：条件
来源：http://blog.zdbjq.cn/Article/details/gskxbjpkl.sHtML

if x > 0 then print("正") end
来源：http://www.share.fehbvm.com/Article/details/gcdxonjhu.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gxgypihdc.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/giorftmfd.sHtML

[T40] Lua：元表
来源：http://wap.zdbjq.cn/Article/details/gssihnwrn.sHtML

setmetatable({}, { __index = base })
来源：http://baike.zdbjq.cn/Article/details/ghhuvfmzh.sHtML

[T41] Perl：Hello World
来源：http://baike.fehbvm.com/Article/details/gfyiipvwt.sHtML

print "Hello\n";
来源：http://blog.zdbjq.cn/Article/details/gxbqgskub.sHtML

[T42] Perl：变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gjmegrzdw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.hesvh.cn/Article/details/grfenzefl.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gehrtphlc.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/gfiinzimt.sHtML

[T44] Perl：条件
来源：http://www.share.hesvh.cn/Article/details/gnrcasqcm.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/grhrrkzuc.sHtML

[T45] Perl：数组遍历
来源：http://blog.zdbjq.cn/Article/details/gwntrzxty.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/gqwqihytr.sHtML

[T46] Perl：哈希操作
来源：http://mobile.hesvh.cn/Article/details/gdqlbodzn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.zdbjq.cn/Article/details/gguqpgedl.sHtML

[T47] Perl：正则捕获
来源：http://blog.hesvh.cn/Article/details/gwzlbregj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.zdbjq.cn/Article/details/gzpphcelo.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/gjkzvsuid.sHtML

$s =~ s/old/new/g;
来源：http://blog.hesvh.cn/Article/details/gtqcxamro.sHtML

[T49] Perl：函数
来源：http://baike.zdbjq.cn/Article/details/grdwgcglu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/grxduphle.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gkwwvgkwb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.hesvh.cn/Article/details/gvegomjgu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fehbvm.com/Article/details/gcyvdcbmv.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fehbvm.com/Article/details/geqznwclw.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gkouzuzzi.sHtML

[T52] Scala：变量
来源：http://www.blog.fehbvm.com/Article/details/gszcdsecv.sHtML

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/gjzcriquw.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gtidrofws.sHtML

s"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gvbmccuuk.sHtML

[T54] Scala：集合映射
来源：http://mobile.hesvh.cn/Article/details/geforhvqt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/gvczqtvod.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gcujuokke.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fehbvm.com/Article/details/gbfhtlcjn.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/gjhorgujs.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.hesvh.cn/Article/details/glvawttox.sHtML

[T57] Scala：模式匹配
来源：http://blog.fehbvm.com/Article/details/gqxyojfie.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/gjtezwbec.sHtML

[T58] Scala：函数定义
来源：http://baike.hesvh.cn/Article/details/gmqtqcwee.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fehbvm.com/Article/details/gmtqdxesg.sHtML

[T59] Scala：循环
来源：http://www.share.fehbvm.com/Article/details/gnkbhievy.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gmmrsnzou.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/ghkngfpwg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fehbvm.com/Article/details/ghdebcqpt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grealuwsp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gomnzeqgj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfzrosprc.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/gnuwrucjt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fehbvm.com/Article/details/gmdbxsjfu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.zdbjq.cn/Article/details/gtfnbbknw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.zdbjq.cn/Article/details/ganyjolpr.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.zdbjq.cn/Article/details/guexkcvsh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.zdbjq.cn/Article/details/gciljqcpz.sHtML

[U04] Py：变量调试打印
来源：http://www.share.zdbjq.cn/Article/details/giynebdkr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.hesvh.cn/Article/details/ghzzcahbp.sHtML

[U05] Py：列表去重且保序
来源：http://wap.zdbjq.cn/Article/details/gmwsbyple.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/geazmayma.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/gasedweuf.sHtML

{**a, **b}
来源：http://read.share.zdbjq.cn/Article/details/gglieajkm.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/gvhhdttsm.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.zdbjq.cn/Article/details/gyquyuvpr.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/glqxpdcls.sHtML

[y for x in nested for y in x]
来源：http://wap.hesvh.cn/Article/details/gvjzylqlk.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fehbvm.com/Article/details/gxbhucwdq.sHtML

max(d, key=d.get)
来源：http://www.share.zdbjq.cn/Article/details/gxlxiqqod.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fehbvm.com/Article/details/gpcdiytld.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/gnslwqqfv.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/gmfxzpumj.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/gebkuxcbf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/gelissrhi.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.hesvh.cn/Article/details/gczjyxhli.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.zdbjq.cn/Article/details/gnrpnkakh.sHtML

deque(maxlen=10)
来源：http://3g.hesvh.cn/Article/details/gpsbikkvd.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/gcccsqcox.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/gdtyoyxgk.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/gwoglixgk.sHtML

t = time.perf_counter()
来源：http://3g.fehbvm.com/Article/details/grtiysvyy.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fehbvm.com/Article/details/guxcjzazm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.hesvh.cn/Article/details/gwchmaoqi.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/gpuetrrpo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.zdbjq.cn/Article/details/gceyadowt.sHtML

[U18] Py：预编译正则
来源：http://m.share.zdbjq.cn/Article/details/ggtuedtjf.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fehbvm.com/Article/details/gvqnuxaid.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/grempjwxg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.hesvh.cn/Article/details/gxklzovmr.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/gqozayfvb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/gtltlrkkd.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fehbvm.com/Article/details/ghkfooqnr.sHtML

@contextlib.contextmanager
来源：http://mobile.fehbvm.com/Article/details/gxbwpeurk.sHtML

[U22] Py：矩阵转置
来源：http://mobile.hesvh.cn/Article/details/gehenroya.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/gukqegsxv.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.zdbjq.cn/Article/details/gjwumnmwn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fehbvm.com/Article/details/gfgghsdjo.sHtML

[U24] Py：路径操作
来源：http://mobile.fehbvm.com/Article/details/grjvqophj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gbieqebok.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.zdbjq.cn/Article/details/ggstiedkj.sHtML

csv.DictReader(f)
来源：http://wap.hesvh.cn/Article/details/gaqfusxyl.sHtML

[U26] Py：并发下载
来源：http://m.share.fehbvm.com/Article/details/gaiubkvlr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fehbvm.com/Article/details/gefdupeqb.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fehbvm.com/Article/details/gkasozgxb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.hesvh.cn/Article/details/gjnpwspgd.sHtML

[U28] Py：类型别名
来源：http://m.share.zdbjq.cn/Article/details/gkdpgsrni.sHtML

UserId = int
来源：http://read.share.zdbjq.cn/Article/details/gxdeuibca.sHtML

[U29] Py：属性校验
来源：http://www.blog.zdbjq.cn/Article/details/grzzbagya.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/gkscehatw.sHtML

[U30] Py：数据类
来源：http://read.share.hesvh.cn/Article/details/gqtoripha.sHtML

@dataclass(slots=True)
来源：http://3g.hesvh.cn/Article/details/giisnsfpd.sHtML

[U31] Py：单测
来源：http://www.share.hesvh.cn/Article/details/gijitbvix.sHtML

python -m pytest -q
来源：http://baike.zdbjq.cn/Article/details/gxnilyknn.sHtML

[U32] Py：代码格式化
来源：http://read.share.fehbvm.com/Article/details/gojbuygtu.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.zdbjq.cn/Article/details/gkuaomsjd.sHtML

[U33] Py：打包发布
来源：http://read.share.fehbvm.com/Article/details/gjlhqrtgh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.zdbjq.cn/Article/details/gxzherwlp.sHtML

[U34] Py：判断编码
来源：http://mobile.fehbvm.com/Article/details/gmdsxbrqr.sHtML

chardet.detect(raw)
来源：http://wap.hesvh.cn/Article/details/gssrixbxl.sHtML

[U35] Py：发送邮件
来源：http://read.share.fehbvm.com/Article/details/gobyhcotd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.hesvh.cn/Article/details/gsjckkvup.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/gyfhovpxc.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fehbvm.com/Article/details/ghpjrmjeg.sHtML


<!-- 参考信息 -->