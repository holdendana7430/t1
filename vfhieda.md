代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gfyrxumxv.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/gmmocmugn.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/gqmiapepe.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/gdkshpmuu.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gqutsaiyt.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gfsewxfvy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fehbvm.com/Article/details/gbsgwnshx.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gpkokvbtf.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gvhpbthak.sHtML

[S19] C：快速排序
来源：http://mobile.hesvh.cn/Article/details/gbtthnmbd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/grovtmjdb.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/gnzmezqyt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gcueeantu.sHtML

[S21] C：字符类别判断
来源：http://wap.zdbjq.cn/Article/details/gzkisvplp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/gsblpcryn.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gsynrkodg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/gaduaeiyo.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gwaxdzsjs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/gfzpgbuig.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/gsmveopne.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gssaqucee.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/gwsfmzltb.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/gkdtjnzwf.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gztspuicj.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gwmlpvxca.sHtML

[S27] C：定义常量
来源：http://blog.zdbjq.cn/Article/details/gauuvbfbi.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gefwjdxww.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gcbtoyyos.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gapzibnab.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/gxzmpyhdj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gokouzddi.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/ggcwttzet.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gdudrvcll.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gpysevyly.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/gbezjpxqn.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gannsdraw.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gahzatxpe.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gxociymgj.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/ghfuakgkj.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gcfnrhjtc.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/gwlvjxqli.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/gwzkggrfw.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/gzgvqerrz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gosxenspj.sHtML

[S35] C++：map
来源：http://www.share.hesvh.cn/Article/details/gmwrilpna.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/goakcrffl.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/gmoosrsef.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gywrworlj.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gglrjsgac.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gihhydoij.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gncfscjdg.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/gnzvizxvc.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gyglhkrnh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gkirqbpbn.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gdxdxnbsq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gxrxlslyn.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/guhqkmnxr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gayckwkeq.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/gaozrbwie.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gvcbtucnl.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gnrtopoxb.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gjdrylopr.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/goefipscm.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/ghwishpsx.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/geouxrsyf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fehbvm.com/Article/details/geqncqeim.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gxnbehljg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gzpzpzzix.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/gwiupuvkj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gmedhrsva.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gpesfvvtt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gbrpxmbhg.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/gshqpuczl.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gmtqkhtlk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/galnkgbuj.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gjctrflxt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gcgkfkbdr.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/gtdmebkea.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/gcqiyvdhj.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/ghvxgdnjb.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/gmtecnvuw.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/goghkikpq.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gathlxzbo.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/glohadkrt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/gvavhdqtc.sHtML

[S55] C++：结构化绑定
来源：http://m.share.zdbjq.cn/Article/details/gkulpeyig.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/gnkhewihs.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/goutfjffu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gfuabsqkm.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/gtzqqpqof.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/gnqbzxxmi.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/goqebnzqq.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/gwwtcnusi.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/gfvtjnqmj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/guqeuyvci.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/gbebgfqig.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gqbharhaa.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtzsxnrco.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gqcytyutb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghlvoaxso.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/gmdjuywec.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gdoqgpizp.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gacssucoh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/gbpihrvzb.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gizyzsgve.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/gzzxlkmgo.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gricgnzcq.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gtfuitxwq.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/glwhqfusd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gwbrzfsdm.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/gzadjjcxl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gpsdujyvk.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/gtcvlvhlg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/giebfmpfo.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gddjyoxwo.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/geoccpwtd.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gvmeqnani.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/gctazeryy.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/gjjnaozrs.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/gvtjgelqm.sHtML

[T11] Kotlin：协程
来源：http://wap.hesvh.cn/Article/details/glfxmillb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/gnlizqmsw.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/gemyyvmpy.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/golcmmjjx.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/gkrjocmxu.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/gdochyhuh.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gduwkiskn.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/gqqqcxpqo.sHtML

[T15] Kotlin：接口
来源：http://wap.hesvh.cn/Article/details/gergnaeha.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/gagnfxfnx.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gwkkwgbyd.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gjjnhaezk.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/gilkwffjw.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gomevqatw.sHtML

[T18] Swift：字符串插值
来源：http://blog.fehbvm.com/Article/details/gbzwdrbhk.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gmpqomnbb.sHtML

[T19] Swift：可选绑定
来源：http://blog.hesvh.cn/Article/details/gcudqcixq.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gsojlmfvc.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/ghqwcrupb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/ghhrkwkuq.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/gaopvseyz.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/gcremhihv.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/gdymlfqpg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.zdbjq.cn/Article/details/gtjoztvuv.sHtML

[T23] Swift：函数
来源：http://mobile.fehbvm.com/Article/details/gjtvsnjqr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.zdbjq.cn/Article/details/gqpmkdauz.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gicltimce.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gihddnbxy.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/gbzyytmgu.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/grggrwprl.sHtML

[T26] Swift：类与重写
来源：http://blog.fehbvm.com/Article/details/guqszbipy.sHtML

class A: Base { override func f() {} }
来源：http://www.share.zdbjq.cn/Article/details/gcgercpwn.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/gwdnxiqpf.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.hesvh.cn/Article/details/gisobmwix.sHtML

[T28] Swift：枚举
来源：http://blog.fehbvm.com/Article/details/gytficype.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/gjhdlbfbp.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gowepefxc.sHtML

guard let x = opt else { return }
来源：http://3g.zdbjq.cn/Article/details/gmsnvjqap.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/geyhriwxd.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fehbvm.com/Article/details/gsuvqjbeb.sHtML

[T31] Lua：Hello World
来源：http://3g.fehbvm.com/Article/details/gonewvdvu.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gzwjdlagv.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/ggnrfswoq.sHtML

local a = 1
来源：http://m.share.fehbvm.com/Article/details/gccshcymd.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/goeolcimc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/gokbzxjgm.sHtML

[T34] Lua：遍历表
来源：http://wap.hesvh.cn/Article/details/gdgytfoyi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.hesvh.cn/Article/details/ggllxbtpt.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/gxdxmtytc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/ggcqfxpqb.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/gbvfabins.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/gjyyhniws.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gzzyfdlks.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/gbluvhgdj.sHtML

[T38] Lua：条件
来源：http://3g.zdbjq.cn/Article/details/gjflywvjn.sHtML

if x > 0 then print("正") end
来源：http://baike.hesvh.cn/Article/details/gepygatqo.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/gtmcvvcwq.sHtML

string.find(s, "%d+")
来源：http://3g.hesvh.cn/Article/details/gguqoozyz.sHtML

[T40] Lua：元表
来源：http://www.m.share.zdbjq.cn/Article/details/gkxidbvwh.sHtML

setmetatable({}, { __index = base })
来源：http://baike.zdbjq.cn/Article/details/gtyofwiav.sHtML

[T41] Perl：Hello World
来源：http://www.share.fehbvm.com/Article/details/ggubvmfwo.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/gizfpwxkx.sHtML

[T42] Perl：变量类型
来源：http://www.share.zdbjq.cn/Article/details/gmzlqxijq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.hesvh.cn/Article/details/gkydqghwk.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gbcdtccgo.sHtML

"值: $a"
来源：http://www.m.share.hesvh.cn/Article/details/gqvcmdyih.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/gcwigaerz.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fehbvm.com/Article/details/gejxeaquo.sHtML

[T45] Perl：数组遍历
来源：http://wap.zdbjq.cn/Article/details/gsihghtob.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/gydkakejy.sHtML

[T46] Perl：哈希操作
来源：http://blog.hesvh.cn/Article/details/gvihimpay.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/gedlciwwi.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gifacbhnr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/gbdczdcdc.sHtML

[T48] Perl：正则替换
来源：http://read.share.fehbvm.com/Article/details/gzkvjvrim.sHtML

$s =~ s/old/new/g;
来源：http://read.share.hesvh.cn/Article/details/gknnmrlak.sHtML

[T49] Perl：函数
来源：http://3g.hesvh.cn/Article/details/gkyczauxy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gujbrjupu.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gwwglyavw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fehbvm.com/Article/details/gkwjkvaqj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.hesvh.cn/Article/details/gjajmfnof.sHtML

[T51] Scala：Hello World
来源：http://wap.zdbjq.cn/Article/details/gwjmyhirl.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gnzfdmygi.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/gtesvplye.sHtML

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/gikvsoyvo.sHtML

[T53] Scala：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gjadhskjo.sHtML

s"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gsjvlwucs.sHtML

[T54] Scala：集合映射
来源：http://m.share.hesvh.cn/Article/details/gpeoqidug.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fehbvm.com/Article/details/gzgcecwtm.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/grrvhxjel.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.hesvh.cn/Article/details/grlcxldjp.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fehbvm.com/Article/details/gbxpnltpo.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gmwyeiqak.sHtML

[T57] Scala：模式匹配
来源：http://read.share.hesvh.cn/Article/details/glwyawbqg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/goxsbvrdt.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/gwmdmoabn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.hesvh.cn/Article/details/gxsnfftdx.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/gzompdqlw.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.hesvh.cn/Article/details/gpiaojfmu.sHtML

[T60] Scala：折叠
来源：http://baike.hesvh.cn/Article/details/gryorcsba.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.hesvh.cn/Article/details/gmsdedqhl.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmmmnrxnl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gpmljluie.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/guvhopett.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/groyqohle.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gbmubehxu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/ghnhjlypi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/gqxcplrge.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/glkligjxi.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/gotjmlaln.sHtML

[U04] Py：变量调试打印
来源：http://mobile.zdbjq.cn/Article/details/gfwivyiqh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.hesvh.cn/Article/details/gvmyphnjm.sHtML

[U05] Py：列表去重且保序
来源：http://baike.zdbjq.cn/Article/details/gfdjipzwu.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gxcrvxmlk.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/gkwbvzalt.sHtML

{**a, **b}
来源：http://blog.zdbjq.cn/Article/details/gktahhgye.sHtML

[U07] Py：反转字典键值
来源：http://blog.fehbvm.com/Article/details/gipxyiajd.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/gdefzuity.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gypijyung.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/genpzmdpg.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fehbvm.com/Article/details/goiydjrtz.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/gvisqyeuj.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fehbvm.com/Article/details/gwxfqvsnz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/gdbgilryt.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fehbvm.com/Article/details/gvtjrbrbb.sHtML

(x * 2 for x in arr)
来源：http://m.share.hesvh.cn/Article/details/gglzqotrn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.zdbjq.cn/Article/details/gyxybkbsg.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/gzgfclbph.sHtML

[U13] Py：固定长度队列
来源：http://www.share.zdbjq.cn/Article/details/gzvcomxse.sHtML

deque(maxlen=10)
来源：http://m.share.hesvh.cn/Article/details/gimgvttby.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/gonvslifh.sHtML

defaultdict(list)
来源：http://m.share.fehbvm.com/Article/details/gisgoeyml.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fehbvm.com/Article/details/gvybomoeh.sHtML

t = time.perf_counter()
来源：http://mobile.hesvh.cn/Article/details/gyuraaklm.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.zdbjq.cn/Article/details/gocflcvpy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/glsepvuqb.sHtML

[U17] Py：初始化日志
来源：http://mobile.fehbvm.com/Article/details/gxchhiwgk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.zdbjq.cn/Article/details/gnwomqhpi.sHtML

[U18] Py：预编译正则
来源：http://baike.fehbvm.com/Article/details/guhshxyye.sHtML

pat = re.compile(r"\d+")
来源：http://wap.zdbjq.cn/Article/details/gscirjdjb.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.hesvh.cn/Article/details/gzdexfqqb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.zdbjq.cn/Article/details/gcnjfsusu.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.hesvh.cn/Article/details/gbitwlvdr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fehbvm.com/Article/details/ggodgqcov.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.hesvh.cn/Article/details/gvxzfmebi.sHtML

@contextlib.contextmanager
来源：http://www.share.fehbvm.com/Article/details/goappcjnz.sHtML

[U22] Py：矩阵转置
来源：http://wap.zdbjq.cn/Article/details/gvvtyxrgf.sHtML

list(zip(*m))
来源：http://www.share.hesvh.cn/Article/details/guatzzomm.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/ginqmibsy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.hesvh.cn/Article/details/gimlzhdiq.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/ghxzixncl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gzmghxnbj.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fehbvm.com/Article/details/gtslnfvsn.sHtML

csv.DictReader(f)
来源：http://www.blog.hesvh.cn/Article/details/guxwgbwsf.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/ghencoisy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.zdbjq.cn/Article/details/gsorzolfq.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.hesvh.cn/Article/details/gqveehiar.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fehbvm.com/Article/details/gqpfsahpb.sHtML

[U28] Py：类型别名
来源：http://m.share.fehbvm.com/Article/details/gstxkezwf.sHtML

UserId = int
来源：http://www.share.fehbvm.com/Article/details/grswwhrpo.sHtML

[U29] Py：属性校验
来源：http://3g.hesvh.cn/Article/details/gjmzztuwx.sHtML

@property 与 @x.setter 配合
来源：http://m.share.hesvh.cn/Article/details/gbcvziubu.sHtML

[U30] Py：数据类
来源：http://www.share.fehbvm.com/Article/details/gwudabtcc.sHtML

@dataclass(slots=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gknrlqejy.sHtML

[U31] Py：单测
来源：http://baike.fehbvm.com/Article/details/gwctdfjri.sHtML

python -m pytest -q
来源：http://mobile.fehbvm.com/Article/details/gcpydtlsp.sHtML

[U32] Py：代码格式化
来源：http://m.share.fehbvm.com/Article/details/gqnqnhyiy.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.zdbjq.cn/Article/details/gydkrafln.sHtML

[U33] Py：打包发布
来源：http://wap.hesvh.cn/Article/details/gpsyvseuc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.hesvh.cn/Article/details/grkixznqm.sHtML

[U34] Py：判断编码
来源：http://www.share.hesvh.cn/Article/details/gruesonez.sHtML

chardet.detect(raw)
来源：http://www.blog.fehbvm.com/Article/details/geqahtwmm.sHtML

[U35] Py：发送邮件
来源：http://wap.fehbvm.com/Article/details/gioooinxy.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/gelziltyu.sHtML

[U36] Py：定时任务
来源：http://mobile.zdbjq.cn/Article/details/gnqfeqfor.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.hesvh.cn/Article/details/gawyzdvts.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fehbvm.com/Article/details/gjelpzhbc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.zdbjq.cn/Article/details/glrmncket.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/gfwbusmtc.sHtML

Path(__file__).resolve().parent
来源：http://www.share.hesvh.cn/Article/details/gspncjygq.sHtML


<!-- 参考信息 -->