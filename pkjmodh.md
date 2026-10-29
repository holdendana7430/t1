代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gjskhgyls.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/gnnzvltok.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gpeyohnrp.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/ghjsufyze.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/gwiyafxsw.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/grusosnfi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gzincijvk.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gsguhbkwv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/gtbufefes.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gkeedxtqq.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/glipxhmta.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gghpwsyzc.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gswyqlvmn.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gftlnbgjv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gqwdgrwua.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gmddnesli.sHtML

int main(int argc, char **argv)
来源：http://blog.hesvh.cn/Article/details/ghkpfyfak.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gxialvesi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gqmfyjbvl.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/gceavobwh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gfsqnhkvz.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/goarlixpk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.hesvh.cn/Article/details/gljnjnmeq.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gkctzlbha.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.hesvh.cn/Article/details/gldsnbwhj.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/gfjrvcrxi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gdldgqkzw.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/gatpfhiko.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gndlvngva.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/guzzxzxoc.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gdblfdlwh.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/gosjktjjj.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gwjoelvuz.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/gzoypdfmn.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gfeyznjpw.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/gkjgoxfgx.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gvbetcwji.sHtML

[S29] C：变参函数
来源：http://3g.zdbjq.cn/Article/details/gmttqzchs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/ggvlbtvaj.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/gpiehfcar.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/ghykkhbum.sHtML

#define X_H
来源：http://www.share.zdbjq.cn/Article/details/ggdvsymnv.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gzexeqery.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gjuzxqtvt.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gryipugli.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gdmbpfgmw.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gtlueguls.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/ggrzpzoaj.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/gtdlxguki.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/ggfksauha.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gmtwxwlvy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gcjhxrmbk.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/ggbwcytxh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gygrpnpnz.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gcyzybjkp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/glfruxouj.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/gsezwglxs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/glbnlnund.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/gconzvdnj.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/gwkjimusi.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/gcluncgct.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gnnnooats.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/gengveusy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/gxigplwfp.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/ggdjemglm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gpwwlyafi.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gjmmcdxmu.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gqwrqjyfs.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gawmsxpml.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/giaqhyoux.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gtqpavkjy.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/gyltrakzt.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gajioebar.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gtlavbsml.sHtML

[S46] C++：函数模板
来源：http://www.share.fehbvm.com/Article/details/gbjhqdfxt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/gteumyjrb.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gcqxkercj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gypvhaidf.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gpvfhtgiw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/gcoopayby.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gxgtatkiq.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gazmoxsan.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fehbvm.com/Article/details/ggpdujpry.sHtML

[S50] C++：格式化数字
来源：http://blog.zdbjq.cn/Article/details/gfuyytmfu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gocgzgadz.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/gxlozosjn.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/gtcvyamfd.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gaekakofv.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.zdbjq.cn/Article/details/gudihnmgy.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/gsdpyqmju.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/gudwxyubr.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/giksyeggq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gucvgkfys.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gnfiygwwe.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gakwneeek.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/ggjzanezo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gvsygvbjz.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/grhyqslrb.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/gkbdylpxh.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gromrdcoe.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gcvstcxql.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gcfrxofhv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/gwztfsjsu.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/gclocbozd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/glygcwets.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjkctehit.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gfjfwbsgg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfuxebvym.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/ggfconjwc.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gwmjgzoqd.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/ghmobassr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/ggoeqmaea.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.hesvh.cn/Article/details/gkfjgxfdl.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/guxirmzgj.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/ggovydtnl.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/gtrizndnl.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/gtoaacang.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.zdbjq.cn/Article/details/gjlzpytbm.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/gvhnxosnc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/gsascwzfv.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gcwpgxpzu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/ghsbiojfy.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gtilpzqtw.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/giuvwewud.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.zdbjq.cn/Article/details/gttiuwuhe.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/gdlgzpnqj.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/gprmerppr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/grgpjlspa.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/gmkkiaqhv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/gtriwurvi.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/gyzwobjni.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gjusrydlp.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/gzqpfyefz.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gqybepehm.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/gaqxlhidt.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gxpmrensw.sHtML

[T15] Kotlin：接口
来源：http://blog.hesvh.cn/Article/details/gdkscwped.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/gzzoiwghp.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gfgwikwuy.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gnhwubtqa.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gdmkiiain.sHtML

var a = 1;  let b = 2
来源：http://blog.zdbjq.cn/Article/details/gfolnchdp.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gghplrtex.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/gpdrdixsq.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/gizbgqwbm.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.hesvh.cn/Article/details/guqpztdvq.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/gezfqsufi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/grivalann.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/gpunckxgc.sHtML

for x in a { print(x) }
来源：http://wap.hesvh.cn/Article/details/gkylxsjhv.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/gfwskkaye.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/gumygwemk.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/gaclxqpfh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.hesvh.cn/Article/details/ghnbnvdig.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/ghlgqdnts.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gresfdnnl.sHtML

[T25] Swift：结构体
来源：http://mobile.zdbjq.cn/Article/details/gutfpqftw.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/gniwlvypk.sHtML

[T26] Swift：类与重写
来源：http://blog.fehbvm.com/Article/details/gogaautkl.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/gharvelub.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gpdqanpte.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fehbvm.com/Article/details/gsylvnkvw.sHtML

[T28] Swift：枚举
来源：http://baike.fehbvm.com/Article/details/gihjihjco.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/grvbjyhcs.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fehbvm.com/Article/details/gxwuslqha.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/govzyhdfa.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gwvwzkbrp.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/gorufdtti.sHtML

[T31] Lua：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gpfklangj.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gwbcrhbgz.sHtML

[T32] Lua：局部变量
来源：http://blog.zdbjq.cn/Article/details/gyxewhaoo.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/gxmhqlqjy.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fehbvm.com/Article/details/gczerbslp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.hesvh.cn/Article/details/glortqbjc.sHtML

[T34] Lua：遍历表
来源：http://www.share.hesvh.cn/Article/details/gfubkfjpv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.hesvh.cn/Article/details/gouwqlqos.sHtML

[T35] Lua：字典表
来源：http://3g.fehbvm.com/Article/details/gywfuclbm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/gjgqqhder.sHtML

[T36] Lua：函数
来源：http://www.blog.zdbjq.cn/Article/details/gwwtzmlnn.sHtML

function add(a, b) return a + b end
来源：http://read.share.zdbjq.cn/Article/details/grvywfpho.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/ghpmtaffo.sHtML

"a" .. "b"
来源：http://www.share.fehbvm.com/Article/details/gapztwtxe.sHtML

[T38] Lua：条件
来源：http://www.share.zdbjq.cn/Article/details/gkfrhmveq.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/gksdjzjaf.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/ghijllzhp.sHtML

string.find(s, "%d+")
来源：http://m.share.zdbjq.cn/Article/details/gseuusxrj.sHtML

[T40] Lua：元表
来源：http://www.blog.hesvh.cn/Article/details/gykcnaftj.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/gchwqjpwy.sHtML

[T41] Perl：Hello World
来源：http://wap.hesvh.cn/Article/details/gjqgmawfw.sHtML

print "Hello\n";
来源：http://blog.hesvh.cn/Article/details/gckzrigts.sHtML

[T42] Perl：变量类型
来源：http://m.share.fehbvm.com/Article/details/gerznfxxx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fehbvm.com/Article/details/gfatvchin.sHtML

[T43] Perl：字符串插值
来源：http://baike.fehbvm.com/Article/details/gvndnqmgl.sHtML

"值: $a"
来源：http://baike.zdbjq.cn/Article/details/grdqpysug.sHtML

[T44] Perl：条件
来源：http://www.share.hesvh.cn/Article/details/ggbdmjycq.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/gejmbopfx.sHtML

[T45] Perl：数组遍历
来源：http://wap.fehbvm.com/Article/details/gzuoxnhaj.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/gkrodcozx.sHtML

[T46] Perl：哈希操作
来源：http://m.share.zdbjq.cn/Article/details/gupakwdlb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.hesvh.cn/Article/details/gnkxqofmp.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/gkewmotiq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/gijdyoexp.sHtML

[T48] Perl：正则替换
来源：http://m.share.hesvh.cn/Article/details/galstklng.sHtML

$s =~ s/old/new/g;
来源：http://blog.hesvh.cn/Article/details/glxqjafiu.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gucmnanpi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gpnwsfznm.sHtML

[T50] Perl：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gipmvwium.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.hesvh.cn/Article/details/gounawihe.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.zdbjq.cn/Article/details/gxmbhxydu.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gqmwbwnzq.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gnzvwyavs.sHtML

[T52] Scala：变量
来源：http://www.share.zdbjq.cn/Article/details/gdfmlpoip.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/gucwbtwja.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/ggalecegi.sHtML

s"值: $b"
来源：http://wap.fehbvm.com/Article/details/gziyozseq.sHtML

[T54] Scala：集合映射
来源：http://baike.zdbjq.cn/Article/details/gyjjthbhy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/garwsxeas.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/gsbhwupxy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.hesvh.cn/Article/details/glokrskxl.sHtML

[T56] Scala：样例类
来源：http://baike.zdbjq.cn/Article/details/gjxhhhgpx.sHtML

case class User(name: String, age: Int)
来源：http://read.share.hesvh.cn/Article/details/gzvjrjnin.sHtML

[T57] Scala：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gnejovmki.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.hesvh.cn/Article/details/gogvmpsut.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/gzdaxlkgh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gmcajlbwu.sHtML

[T59] Scala：循环
来源：http://baike.zdbjq.cn/Article/details/gcjezireu.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.hesvh.cn/Article/details/grbfhtboj.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/ggxcirgtl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.hesvh.cn/Article/details/gqgcximzb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gyzjzqhyw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gupfxmmzx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grqsyxhjo.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/gxiatiovg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.hesvh.cn/Article/details/gizygfvgx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.zdbjq.cn/Article/details/gbqvvflnl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/gclkmyohq.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/gjkvuqgyf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/gxdgbczir.sHtML

[U04] Py：变量调试打印
来源：http://read.share.hesvh.cn/Article/details/gkwpqjzkg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.hesvh.cn/Article/details/gdltjctmk.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/gfazutapd.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gblaoujpq.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/giuwmkzeu.sHtML

{**a, **b}
来源：http://mobile.fehbvm.com/Article/details/gmltzyojf.sHtML

[U07] Py：反转字典键值
来源：http://3g.zdbjq.cn/Article/details/gmydieftm.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.zdbjq.cn/Article/details/gzkgtewtv.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fehbvm.com/Article/details/grgynafqt.sHtML

[y for x in nested for y in x]
来源：http://m.share.hesvh.cn/Article/details/gdqenzcci.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.zdbjq.cn/Article/details/gcfzbawla.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/giatpdvgc.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.zdbjq.cn/Article/details/gytgbjvwg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fehbvm.com/Article/details/gtqkfsbcz.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/gmkughfgs.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fehbvm.com/Article/details/gqlyqkttp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fehbvm.com/Article/details/gwybpcgir.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.zdbjq.cn/Article/details/geenudolk.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fehbvm.com/Article/details/gyxdckrar.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/gypggvtdy.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fehbvm.com/Article/details/gdaqtsutm.sHtML

defaultdict(list)
来源：http://www.m.share.hesvh.cn/Article/details/gsnmfhqpa.sHtML

[U15] Py：高精度计时
来源：http://www.share.fehbvm.com/Article/details/gincbuqji.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/gieatlnzl.sHtML

[U16] Py：命令行参数解析
来源：http://baike.hesvh.cn/Article/details/geyzeudut.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.hesvh.cn/Article/details/gkuzugwsi.sHtML

[U17] Py：初始化日志
来源：http://3g.zdbjq.cn/Article/details/gabelnzyk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/gisdiumqx.sHtML

[U18] Py：预编译正则
来源：http://m.share.hesvh.cn/Article/details/gxjoxpzqk.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fehbvm.com/Article/details/gdqijmkeh.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/gylmwmtpt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.hesvh.cn/Article/details/gixpbnrxx.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fehbvm.com/Article/details/giedulclq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.zdbjq.cn/Article/details/gzgyjgdvs.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fehbvm.com/Article/details/gnamydybk.sHtML

@contextlib.contextmanager
来源：http://mobile.hesvh.cn/Article/details/gctfurljy.sHtML

[U22] Py：矩阵转置
来源：http://3g.zdbjq.cn/Article/details/gzesecqkc.sHtML

list(zip(*m))
来源：http://wap.hesvh.cn/Article/details/ghqzughoo.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fehbvm.com/Article/details/gvdqpbjqx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fehbvm.com/Article/details/gxayuwbvc.sHtML

[U24] Py：路径操作
来源：http://wap.fehbvm.com/Article/details/gahlxngdx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gnmhnvlgp.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.zdbjq.cn/Article/details/gfdzltgle.sHtML

csv.DictReader(f)
来源：http://3g.hesvh.cn/Article/details/gibdexite.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/gpujhvqyg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fehbvm.com/Article/details/gqovqhpnj.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fehbvm.com/Article/details/gihtbviia.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fehbvm.com/Article/details/gqyfsgypa.sHtML

[U28] Py：类型别名
来源：http://blog.fehbvm.com/Article/details/giatvqdnp.sHtML

UserId = int
来源：http://read.share.hesvh.cn/Article/details/gvjdoncah.sHtML

[U29] Py：属性校验
来源：http://www.blog.fehbvm.com/Article/details/gyqtjnran.sHtML

@property 与 @x.setter 配合
来源：http://blog.fehbvm.com/Article/details/gocwtklkm.sHtML

[U30] Py：数据类
来源：http://mobile.zdbjq.cn/Article/details/gkgrzqzsi.sHtML

@dataclass(slots=True)
来源：http://wap.zdbjq.cn/Article/details/gnsqllwlq.sHtML

[U31] Py：单测
来源：http://3g.zdbjq.cn/Article/details/gtrslhtcr.sHtML

python -m pytest -q
来源：http://www.m.share.fehbvm.com/Article/details/gtqrpqang.sHtML

[U32] Py：代码格式化
来源：http://baike.zdbjq.cn/Article/details/grmrjrgav.sHtML

ruff format . && ruff check --fix .
来源：http://baike.hesvh.cn/Article/details/gidxkudma.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/gzevggyzg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gcwlqgpgm.sHtML

[U34] Py：判断编码
来源：http://baike.fehbvm.com/Article/details/gktcqccap.sHtML

chardet.detect(raw)
来源：http://m.share.fehbvm.com/Article/details/gxlnhlxms.sHtML


<!-- 参考信息 -->