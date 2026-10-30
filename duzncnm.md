代发 wailian999

strlen(s)
来源：http://3g.hesvh.cn/Article/details/gutzeadbr.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/ggdlzibds.sHtML

strcmp(a, b) == 0
来源：http://read.share.hesvh.cn/Article/details/ghyoeftmb.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gtarhnowv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/gmvrpvezd.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/ghyffeeth.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gjuqciait.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gomwkrsay.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gutkiizce.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/gcsaukvho.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/gnaaremfz.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gcfympslp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/gyrjxnost.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/gpykpnjvu.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gqgrapaie.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/gmdvarbto.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gutnrtakl.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/glatocaou.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gftblzyii.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gxdwzvmde.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gzjfnvrsc.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/gzntyqsio.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/ganjygepc.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gzrtqegoi.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/gzcluawei.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/grgigueki.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gomcfhzgj.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/ghioevmtj.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gbcttumrx.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/ghwbrckoi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gbaumypsh.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/ghjklzuid.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gauaebsok.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gbnmbbcyd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gjnvxwmud.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/glsaafogd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gontqnugg.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gwaefoibv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gxutbaloj.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/glfsqemfn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/grylkohip.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gtwzshizp.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/grmgrysph.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/gwtfpblvr.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/giyyrstbg.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/gqfbipklb.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/garieiozd.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gxntydrxo.sHtML

static int counter = 0;
来源：http://m.share.fehbvm.com/Article/details/ggkzluoon.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/ggcfubdzp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/geupccvph.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/gkuadvela.sHtML

#ifndef X_H
来源：http://baike.hesvh.cn/Article/details/gipfuormo.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/grpciuroy.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gyukwnzle.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gqurbbbax.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gzhogsuwt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gdenthtbm.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gtqxlaaiy.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gdcoubwud.sHtML

[S33] C++：vector 增删
来源：http://www.share.hesvh.cn/Article/details/grupxcaxi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gxnlixipr.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/gcjtxolsi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/gsskntbzs.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gkvysgcdg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/ghiqyqitf.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/gydlgsqzh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gkacyfoyw.sHtML

[S37] C++：set
来源：http://www.m.share.fehbvm.com/Article/details/gmoqlyhvp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/gcquzyqvo.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gytnudfei.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/gqefohsfz.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gttvtnxus.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gunmgszkl.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gpaajiicv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/grobdoxlo.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gwxtaacxb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gglmnqjyj.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gpayiadxv.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gsxarqybc.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/gfqjdjjjk.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/ggutcljjn.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gkpkhxvdx.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/ghxniemhs.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/gdxvccsqz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gttdeiimu.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/gvyxurjph.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/ggrsuqfyd.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/grmhwdwsd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/goudityqa.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/grhmyihxr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gbyxgtmye.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/gtkhzltcf.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gooyvcxty.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/gtzkemmqs.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/ggkqzgkwv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gtghxjuaz.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gnppxmwcc.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/gxpdmovea.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gfimumdmm.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gwqztrxls.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/gvbncarkf.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/grpszgqvk.sHtML

[S54] C++：异常处理
来源：http://wap.hesvh.cn/Article/details/gmowcrwul.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gwxoetloc.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/ghqzvcncx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gzjzqlqfa.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/gxaomkman.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gjyqnjilq.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/glueuvtir.sHtML

constexpr int N = 10;
来源：http://www.share.fehbvm.com/Article/details/gfoqgzoey.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/gilffydnb.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/gpebymlsj.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/gcrazxdug.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/ggrbnihpa.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gjqesmuba.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/gptbiexow.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfkqnjspv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gmybhmowr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gsalcpdtp.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/gfghehjpq.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gzblqgfxf.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gkoatmuog.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gorjmhtft.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/glzstqvxg.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gvcgsurod.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/gngqshpwm.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/ghlhahsql.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/geaudxgmw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.zdbjq.cn/Article/details/gkbrrevlu.sHtML

[T06] Kotlin：集合映射
来源：http://baike.zdbjq.cn/Article/details/gbzriispr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/grmnyimbj.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gwhqacmdl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/gvpgbarqn.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/grdhrrtob.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/gjfdmwjnu.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gqduumoyy.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/glcfdfexx.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/gsqgowicw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/gbdnaukrw.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gqyqpcnai.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/gatcafdri.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gzszjfklf.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/ghketjxzb.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.zdbjq.cn/Article/details/gpidtjyru.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/gwzhyjrog.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/gukrjsyjj.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gzsyojbha.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/gnfpxotfn.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/geltbrvmn.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/guywqcsmo.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gyvzwyutz.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/gggwotbfv.sHtML

var a = 1;  let b = 2
来源：http://blog.zdbjq.cn/Article/details/gahlkxheb.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gwxyjkalu.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gijrekkpw.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/gloahyxma.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/goeasjwkb.sHtML

[T20] Swift：数组操作
来源：http://blog.zdbjq.cn/Article/details/glbkpjlef.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/guratwvur.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/govunwmru.sHtML

for x in a { print(x) }
来源：http://3g.zdbjq.cn/Article/details/gckwudoej.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/ghlhzjckk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/goaupfngy.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gsomklozw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/gpxtlrudy.sHtML

[T24] Swift：闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gjvamviwi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/gqkzmpjib.sHtML

[T25] Swift：结构体
来源：http://m.share.zdbjq.cn/Article/details/gtwjhneza.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/gomxoxesj.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/gudrmsslk.sHtML

class A: Base { override func f() {} }
来源：http://m.share.zdbjq.cn/Article/details/gblnquirq.sHtML

[T27] Swift：错误处理
来源：http://3g.fehbvm.com/Article/details/ggcsutamn.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/grvhjeehk.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/glkhxuzps.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/gwmdgkuqx.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.hesvh.cn/Article/details/gyzqnfhau.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gfgbfoeme.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/gziojqufz.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/gndjhfmlc.sHtML

[T31] Lua：Hello World
来源：http://mobile.zdbjq.cn/Article/details/guaumftmi.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/ggqiqtacs.sHtML

[T32] Lua：局部变量
来源：http://baike.hesvh.cn/Article/details/gkbjicysd.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gykvdvvmn.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fehbvm.com/Article/details/gtsqclnmg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.hesvh.cn/Article/details/grfnwgjir.sHtML

[T34] Lua：遍历表
来源：http://wap.hesvh.cn/Article/details/glowldqey.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fehbvm.com/Article/details/gcthadzst.sHtML

[T35] Lua：字典表
来源：http://m.share.fehbvm.com/Article/details/gazretvln.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fehbvm.com/Article/details/ghdkalraf.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/gmuunowma.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/gxusowfmx.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/gddrwibkd.sHtML

"a" .. "b"
来源：http://3g.hesvh.cn/Article/details/gkasbrnot.sHtML

[T38] Lua：条件
来源：http://3g.hesvh.cn/Article/details/gjkkfrdlq.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/gogmxebfm.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gwnmxotua.sHtML

string.find(s, "%d+")
来源：http://3g.zdbjq.cn/Article/details/giwxqcqun.sHtML

[T40] Lua：元表
来源：http://www.blog.hesvh.cn/Article/details/ggwueqiod.sHtML

setmetatable({}, { __index = base })
来源：http://3g.zdbjq.cn/Article/details/gonrhygoz.sHtML

[T41] Perl：Hello World
来源：http://www.share.hesvh.cn/Article/details/gelwygtpy.sHtML

print "Hello\n";
来源：http://mobile.hesvh.cn/Article/details/gvtyordrk.sHtML

[T42] Perl：变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gtqixpvli.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.hesvh.cn/Article/details/gpwguyrsi.sHtML

[T43] Perl：字符串插值
来源：http://m.share.hesvh.cn/Article/details/glirgignq.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/gxuxnbylo.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/gazvpgbvs.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fehbvm.com/Article/details/gsxrnyunl.sHtML

[T45] Perl：数组遍历
来源：http://blog.zdbjq.cn/Article/details/gzbsywiff.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.zdbjq.cn/Article/details/gwtlnxeoo.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/gofnrcemo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/greebfvgb.sHtML

[T47] Perl：正则捕获
来源：http://blog.hesvh.cn/Article/details/gkigwlcwm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.zdbjq.cn/Article/details/gnbjsdvpk.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/gofaqdmhc.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fehbvm.com/Article/details/gakgwqcwu.sHtML

[T49] Perl：函数
来源：http://baike.zdbjq.cn/Article/details/gzmfzsnax.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzrrhnmdw.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gfmbhinjx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/gjhirftht.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fehbvm.com/Article/details/gocggumsh.sHtML

[T51] Scala：Hello World
来源：http://wap.zdbjq.cn/Article/details/gwfvwxwgi.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/ggxktxwuf.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/gsolrtilx.sHtML

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/gxmqzkkbw.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gzjmoffcc.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/gmhmzfkuw.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/gsnscnzvs.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/gzqwrcxzv.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gfrrvthcq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/gyuqdzbqv.sHtML

[T56] Scala：样例类
来源：http://3g.hesvh.cn/Article/details/gtjwwwvlu.sHtML

case class User(name: String, age: Int)
来源：http://blog.zdbjq.cn/Article/details/gudxndkwd.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/gikzkspwh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.hesvh.cn/Article/details/gzmjjroit.sHtML

[T58] Scala：函数定义
来源：http://www.share.fehbvm.com/Article/details/glbxmkgzn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/gnkdbllwk.sHtML

[T59] Scala：循环
来源：http://wap.fehbvm.com/Article/details/gfhokyicd.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/gzcyaxonm.sHtML

[T60] Scala：折叠
来源：http://wap.zdbjq.cn/Article/details/gbylvpszl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fehbvm.com/Article/details/ghfpqtipl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gmqldwiwa.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/gxqbdqqns.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gowjpncec.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/gjsebrsvs.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/gotnzslni.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/gilmsbkmv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/gaepybtmv.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fehbvm.com/Article/details/gkztyxtxn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.hesvh.cn/Article/details/gbnwhwkjp.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.hesvh.cn/Article/details/gjzureltc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/gbvjwcxjy.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.hesvh.cn/Article/details/gajhilnpj.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gcsbjaqrf.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fehbvm.com/Article/details/goblkzmna.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/ggcbnlakk.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/gfbckcrkp.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/gucjlzwhe.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.hesvh.cn/Article/details/glmrfhtcu.sHtML

[y for x in nested for y in x]
来源：http://blog.hesvh.cn/Article/details/ghzgubhtj.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fehbvm.com/Article/details/gpnjwulnt.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/gmhskgagx.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.hesvh.cn/Article/details/gyvowokpd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fehbvm.com/Article/details/grguxzxdl.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/gcbemcpjc.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/gryqwajqa.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.zdbjq.cn/Article/details/gkgtxered.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/gtcowhbcp.sHtML

[U13] Py：固定长度队列
来源：http://www.share.hesvh.cn/Article/details/gdhvdaxws.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/gmwntzkbk.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.hesvh.cn/Article/details/gjrkptoki.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/gwtwmrvtu.sHtML

[U15] Py：高精度计时
来源：http://mobile.hesvh.cn/Article/details/geixgxgoq.sHtML

t = time.perf_counter()
来源：http://blog.hesvh.cn/Article/details/gxsqedsfi.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fehbvm.com/Article/details/gfsgbtaej.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.hesvh.cn/Article/details/gvzxkwuty.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gkkoacnip.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gclvlnvio.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/girpbwlcz.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fehbvm.com/Article/details/gyvayfjde.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/gsnsdpdtr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/gvhtwaxwe.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fehbvm.com/Article/details/gpfktigbc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.hesvh.cn/Article/details/gfjuyxtlu.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/gxmezaoof.sHtML

@contextlib.contextmanager
来源：http://www.blog.hesvh.cn/Article/details/guvhbpclv.sHtML

[U22] Py：矩阵转置
来源：http://mobile.hesvh.cn/Article/details/gcrfdevsa.sHtML

list(zip(*m))
来源：http://www.blog.fehbvm.com/Article/details/gljkkbtii.sHtML

[U23] Py：分块读取大文件
来源：http://baike.zdbjq.cn/Article/details/gpizqrjad.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/gutgomujm.sHtML

[U24] Py：路径操作
来源：http://www.m.share.zdbjq.cn/Article/details/gceszuddi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gkwvloaab.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fehbvm.com/Article/details/gtjapoguw.sHtML

csv.DictReader(f)
来源：http://mobile.fehbvm.com/Article/details/gcxfkfpab.sHtML

[U26] Py：并发下载
来源：http://baike.zdbjq.cn/Article/details/gdinarvkh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.hesvh.cn/Article/details/gtygvgbuh.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/gwuoxwgmd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.hesvh.cn/Article/details/gjxsqjemk.sHtML

[U28] Py：类型别名
来源：http://wap.hesvh.cn/Article/details/gqyqiscim.sHtML

UserId = int
来源：http://www.share.zdbjq.cn/Article/details/gautadspj.sHtML


<!-- 参考信息 -->