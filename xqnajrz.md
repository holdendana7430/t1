代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/gjtnszyoh.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/ghkaxdzos.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gwrnrqfyq.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/goxbyimpf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gdbsfkylo.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gchzpriad.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/gammaofbm.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/guirzwacb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gzudawlcw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/gqtleachv.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gfxtbknbk.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/guvxvqtkv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/gfeyvpfrz.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/gzkbbofgw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gobkshfnb.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/gzzgcjyqg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/gptjhdgao.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/gkbuseprq.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/gqwdymrgc.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gfbmafsrl.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/gncdukthv.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/giqfnjzcp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/gzjtyvxpz.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gezgfagvm.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gouppcmbj.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/ghpvvhnul.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/ghdiqrvdl.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gdfjjlvhs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gdeeisgdq.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/gshoxkbmq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/gllvqyeca.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gzouvnznn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/gpiykheng.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/glxnurmhh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gyuajquak.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/gyytppxrq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gnlegosbm.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gdlyfpbtz.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gsykghgvx.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gzwdrpgvt.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gyvqtcsbn.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gawpcpyvp.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/ggyzkfevf.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gyqwdabry.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gutvkjpep.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/gbybrsbbr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gifyujoep.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/gmkngggix.sHtML

#ifndef X_H
来源：http://3g.hesvh.cn/Article/details/gdjwcbptv.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gqhqcgmkd.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gjpeponyb.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gnmtahgdh.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/gbkzlzzvj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gwkunerak.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/gxivmadxw.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gaarkryhq.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gbitjookx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gglevrnfz.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/ggdqqesja.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvpnuotfb.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gbzkyrtgd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gnlxliccd.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gnvfolnbu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gqvyeepaf.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/gwbmgpqhp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gnkzijskn.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/gxnyhnvxh.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/gvjbiojdu.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/gxicdcwbp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gljqbultq.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gfinuuoii.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gtocbycgi.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/gjwztqdhr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gktxjpyip.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gqivjarjs.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/gmdhzpulg.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/geeewppjz.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gqfqndfhq.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/grhrutnzx.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/gaeodiuyp.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gakitzwwo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/gojsegtff.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gjcoojisv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/grorzsgza.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gkpedgqdq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gxeebtlxx.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gznpkipps.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/glsxvxryo.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/gucvoyuby.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/gehcxhmia.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gmxcqbukr.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gpctogsre.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gemjfphyw.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gbnegocyo.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gjpczuhig.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gqidjirje.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/ghvdlravi.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/gythrlftr.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/geiycefea.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/gewfodmgk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/grnrgfmiy.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/gcmtujtko.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gzurnivgo.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/gqmnwtvjx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/giimlqtaj.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/ggvunaqsi.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gffpfeptn.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/gjqjmeogw.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/glhjrvfuk.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/gkfsabsqb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.zdbjq.cn/Article/details/gbnjcsvko.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/gmprrimur.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/gaffeazcv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcibrwixx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gjrkekecc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/glnzqoibr.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gsmflfyrm.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gussddupz.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gpbcscdvr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/gongidbez.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/gxmyancao.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gjsykpisr.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gskhfbvcz.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/gtbwixiav.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gkxzhzlre.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gbzpqjnkd.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gkzkspwkj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gqxsojimi.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.zdbjq.cn/Article/details/ggrxzhjvt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gjwluvouz.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/girgsfsjw.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gabthjser.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/gkghmaont.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/gdybfmclw.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/gfmouhrtm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/gfffkwsel.sHtML

[T11] Kotlin：协程
来源：http://www.share.hesvh.cn/Article/details/gxamhrrgy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/grdtkrmtg.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/gqawxsiyp.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/grbbaojjw.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gshmhiaxw.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gilnvbyza.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/gbbpobmtw.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gnpfjpvwk.sHtML

[T15] Kotlin：接口
来源：http://wap.hesvh.cn/Article/details/gmzdpsbgm.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/gpkeleqkr.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/ghqstvnus.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gfsdykgyr.sHtML

[T17] Swift：变量与常量
来源：http://read.share.zdbjq.cn/Article/details/gwyrebhxt.sHtML

var a = 1;  let b = 2
来源：http://www.blog.hesvh.cn/Article/details/gerhjfqax.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/gncoqizai.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/gpkarpgjn.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/gurxzgage.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/gskphuryk.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/gkuyiizft.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fehbvm.com/Article/details/gbarhlhyf.sHtML

[T21] Swift：遍历
来源：http://www.blog.fehbvm.com/Article/details/gtidcdipw.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/gngfpqjbd.sHtML

[T22] Swift：字典
来源：http://www.blog.hesvh.cn/Article/details/gmtfjrwww.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.hesvh.cn/Article/details/gqwarsuja.sHtML

[T23] Swift：函数
来源：http://baike.fehbvm.com/Article/details/gvneeoawu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gxxclleaj.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/gtrrvmbmn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gxbcfxlwf.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/ggsnajcer.sHtML

struct P { var x: Int }
来源：http://www.m.share.hesvh.cn/Article/details/ggrcfixyt.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/ggpxgnmxr.sHtML

class A: Base { override func f() {} }
来源：http://www.share.zdbjq.cn/Article/details/gowjbtjnf.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/gbtqhihge.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/gaiskbnil.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/gysyoicfd.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/gilkpmpiq.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fehbvm.com/Article/details/gapbykvjs.sHtML

guard let x = opt else { return }
来源：http://mobile.hesvh.cn/Article/details/gegabbybq.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/gtuvdrazo.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gsavxczti.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gqnujmrar.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gjjbskwnt.sHtML

[T32] Lua：局部变量
来源：http://mobile.hesvh.cn/Article/details/gcoepayta.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/gesiekefk.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/glaekamgf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fehbvm.com/Article/details/gycfmooow.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/gryzeanet.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.hesvh.cn/Article/details/gcvvqufsx.sHtML

[T35] Lua：字典表
来源：http://wap.fehbvm.com/Article/details/grodlxlji.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/ginkxpodm.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/gluygmqfj.sHtML

function add(a, b) return a + b end
来源：http://wap.zdbjq.cn/Article/details/gfekmnirb.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gpyshdpyw.sHtML

"a" .. "b"
来源：http://www.m.share.hesvh.cn/Article/details/gyjpfvyzo.sHtML

[T38] Lua：条件
来源：http://www.share.zdbjq.cn/Article/details/gpltosypp.sHtML

if x > 0 then print("正") end
来源：http://read.share.hesvh.cn/Article/details/gsykqbfnj.sHtML

[T39] Lua：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gnttfmivw.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gsdbspwdb.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/goovyhszs.sHtML

setmetatable({}, { __index = base })
来源：http://wap.zdbjq.cn/Article/details/gsdykscvn.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/glbdmxosh.sHtML

print "Hello\n";
来源：http://wap.zdbjq.cn/Article/details/glccnicbb.sHtML

[T42] Perl：变量类型
来源：http://mobile.hesvh.cn/Article/details/gzlevivhq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.zdbjq.cn/Article/details/ghirhlohl.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gjshleemp.sHtML

"值: $a"
来源：http://m.share.zdbjq.cn/Article/details/gbwshuedw.sHtML

[T44] Perl：条件
来源：http://m.share.hesvh.cn/Article/details/gebnsviaf.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.hesvh.cn/Article/details/gkwtdqbyy.sHtML

[T45] Perl：数组遍历
来源：http://wap.zdbjq.cn/Article/details/gqnulbeec.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/gsbwnpode.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/gnctzowuu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fehbvm.com/Article/details/gyoslcfbj.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fehbvm.com/Article/details/gwrjttqrp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/gctpddrvu.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/gntoxifrx.sHtML

$s =~ s/old/new/g;
来源：http://blog.hesvh.cn/Article/details/glmkchhgq.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/gvlkciqsb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gwzascmtt.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gjsgraxti.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fehbvm.com/Article/details/gikhwdxaa.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fehbvm.com/Article/details/gkvowcxst.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gftjincov.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/ghkzpbrjh.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/gpmceoutz.sHtML

val a = 1;  var b = 2
来源：http://read.share.hesvh.cn/Article/details/glmzhtvus.sHtML

[T53] Scala：字符串插值
来源：http://wap.fehbvm.com/Article/details/gdcwannhn.sHtML

s"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/guroiiogt.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/gjrfkyftm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/gdqkszyyp.sHtML

[T55] Scala：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/glemlmzgq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.zdbjq.cn/Article/details/gjsbndxrs.sHtML

[T56] Scala：样例类
来源：http://read.share.zdbjq.cn/Article/details/gkeunexrr.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gtxukknrx.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/geuxmcagr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gqfdrhicm.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/gbuqkaobk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gsixsaajn.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/glxokdfgl.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gvbupvuan.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/gidsvwnyb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/ggibwnuvy.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwbofwtsv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gxyxequho.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpsjfuogw.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.hesvh.cn/Article/details/gagwlwzmr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.hesvh.cn/Article/details/glfwvkmof.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.hesvh.cn/Article/details/gyurovfkn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/gzldpvdso.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.hesvh.cn/Article/details/gexchdire.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fehbvm.com/Article/details/gyojqjflf.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fehbvm.com/Article/details/gnawttfmj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/glkqlvfiy.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/gyicwbtxr.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gbcdegxsl.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.zdbjq.cn/Article/details/gbbdwdlyl.sHtML

{**a, **b}
来源：http://www.share.hesvh.cn/Article/details/gsctkspsw.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/ghfgcgrlq.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.zdbjq.cn/Article/details/gnapcrkgo.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/gjuzcgffa.sHtML

[y for x in nested for y in x]
来源：http://www.share.hesvh.cn/Article/details/gayrnxqhc.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.hesvh.cn/Article/details/gebuadizm.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gcoxrbova.sHtML

[U10] Py：按值排序字典
来源：http://mobile.zdbjq.cn/Article/details/gyhoabqpr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fehbvm.com/Article/details/ghuetfwem.sHtML

[U11] Py：生成器表达式
来源：http://www.share.zdbjq.cn/Article/details/gbizqnzuh.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/gtsvtgbqk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fehbvm.com/Article/details/gmuatxttj.sHtML

Counter(arr).most_common(3)
来源：http://read.share.hesvh.cn/Article/details/gdjllxlqm.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.hesvh.cn/Article/details/ghyzhpumn.sHtML

deque(maxlen=10)
来源：http://blog.zdbjq.cn/Article/details/gmmddqjkr.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.zdbjq.cn/Article/details/gjrlcriey.sHtML

defaultdict(list)
来源：http://www.m.share.fehbvm.com/Article/details/gdcgbjyie.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.zdbjq.cn/Article/details/gokxkgnua.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/gijsnichd.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.hesvh.cn/Article/details/glyikrwpa.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fehbvm.com/Article/details/gjyzatplg.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.zdbjq.cn/Article/details/gswivuxoo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.hesvh.cn/Article/details/gfyafeovo.sHtML

[U18] Py：预编译正则
来源：http://read.share.fehbvm.com/Article/details/gdmcvjmgz.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fehbvm.com/Article/details/guefifpjf.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.zdbjq.cn/Article/details/gmteexdzq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fehbvm.com/Article/details/gggjsxpma.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.hesvh.cn/Article/details/gtfufvxao.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fehbvm.com/Article/details/gtfhlzihq.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/grdpeswtj.sHtML

@contextlib.contextmanager
来源：http://baike.zdbjq.cn/Article/details/gpucvgfgf.sHtML

[U22] Py：矩阵转置
来源：http://blog.hesvh.cn/Article/details/gnpamzeep.sHtML

list(zip(*m))
来源：http://baike.hesvh.cn/Article/details/gglwpaxck.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/giletnvpf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.hesvh.cn/Article/details/gcwqkggqg.sHtML

[U24] Py：路径操作
来源：http://www.blog.fehbvm.com/Article/details/gvqhyklqw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gkbrnxccz.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fehbvm.com/Article/details/gcoubdikj.sHtML

csv.DictReader(f)
来源：http://baike.fehbvm.com/Article/details/gqhficosv.sHtML

[U26] Py：并发下载
来源：http://www.share.fehbvm.com/Article/details/gwsqdbbeh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.zdbjq.cn/Article/details/gyabjvbkh.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.hesvh.cn/Article/details/gwockjmnx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.hesvh.cn/Article/details/gpivdbitq.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gvcauoygi.sHtML

UserId = int
来源：http://www.share.zdbjq.cn/Article/details/gcpcghnvo.sHtML

[U29] Py：属性校验
来源：http://wap.hesvh.cn/Article/details/gymwhijga.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.zdbjq.cn/Article/details/gnzahmghy.sHtML

[U30] Py：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/ggbkphufn.sHtML

@dataclass(slots=True)
来源：http://baike.zdbjq.cn/Article/details/gkkxwivfm.sHtML


<!-- 参考信息 -->