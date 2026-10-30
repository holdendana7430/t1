代发 wailian999

int x; scanf("%d", &x);
来源：http://baike.fehbvm.com/Article/details/glfbjfbfn.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gdnrqwfjb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gbjukmjxf.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gtdxqhzmh.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/gnxaedkaz.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/gnnssagyx.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/gllnocaqm.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gxtpskscq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gtloxrdsu.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gbmpnitgz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gvykjsdeg.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gufkhaicn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/gbabkzzpv.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/glvwupszp.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gvszhrjmm.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/garbtdwnd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/gxtbmeizt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/gskmtxpbc.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gcvtchaff.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/groyttydk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gqrivowus.sHtML

[S13] C：宏定义
来源：http://www.share.zdbjq.cn/Article/details/gvuchglmp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/glgowlloy.sHtML

[S14] C：枚举
来源：http://m.share.zdbjq.cn/Article/details/gtdvhwgwa.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gnlosdgch.sHtML

[S15] C：类型转换
来源：http://www.blog.zdbjq.cn/Article/details/ghlqxzzno.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gsqddyjln.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gmsqxjbhj.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gducvtlfo.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/goggatplt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/grwiengwh.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gzvzuprlq.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/grwqdguuf.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/ghvjmpczm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gslavpvrp.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/gymipcdod.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gyuznhjcy.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gtwwshety.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/gkixikcih.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gulsnfnwe.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/gansoaxez.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/gwaptbghz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/gipcfsmgx.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/gnbpwfbpw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/gztbzascd.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gvbajxqin.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gnmotpsgi.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gwlyzyhwu.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gztnwegfj.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/gcqlqrmia.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gvietpude.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/ggxdgkrkm.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gdnmdguql.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/ggboelbvx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gzetenzfc.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gmbgsptyz.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gplauzoiu.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/ggzbxhzls.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gofxmvelq.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gwmifunzh.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/gkfjzncyz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gwxhefkrt.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gksgwreww.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.hesvh.cn/Article/details/gpvvxsprq.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gtqlwvnud.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/gbyrwcwdo.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/gnpsqppah.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fehbvm.com/Article/details/ggzccrlpy.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/gplfketwe.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gussrswdl.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/gligmoqgb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gpviuikgk.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gxqxxtfgx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/gwgbmyuzr.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gmltkwzpi.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/ggulnwerr.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.zdbjq.cn/Article/details/gdjxcivwt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gddxowazy.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/giwnvooop.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/guzjdmogg.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/ghvoosedg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gremtzkzj.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/gegfmumro.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/grtdlocnq.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gafrevjst.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gyfefcjvo.sHtML

[S44] C++：引用传参
来源：http://read.share.zdbjq.cn/Article/details/gsgrcjxlw.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/ggvqmlnyp.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gxdynbblp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/giblnwdbd.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/ghffxlhcu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/graylwrbh.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gdrgfwfuw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gfbdugbsa.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gwkdghabi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/gygnuzakj.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/geqjvwpqn.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/gnkbmmqly.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.zdbjq.cn/Article/details/glcfjwyxj.sHtML

[S50] C++：格式化数字
来源：http://blog.zdbjq.cn/Article/details/gwdjkmnmd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gondmzebb.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gicahcekv.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gsrgmhbek.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/ghosrwaak.sHtML

int size() const noexcept { return n_; }
来源：http://baike.hesvh.cn/Article/details/gqlaauixe.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/ggoznrvxp.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.hesvh.cn/Article/details/gddsqxife.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gjlxmjyex.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/gdmweeors.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gvuwqphbx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gvriqxasm.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/grszcmlqp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gwhahcyav.sHtML

[S57] C++：编译期常量
来源：http://mobile.fehbvm.com/Article/details/gotyevftk.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gfxuvxcqm.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gkxbchulk.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/gmstlifec.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gmxdvceiz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/ghpwmgmvd.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/gkxqilven.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/gpasayjiz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwcmzfpoi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gzsszhtco.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmyiksjef.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gtbyjfzbh.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gfqzwuqee.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gcpaxwdtm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/ggqsrzrkq.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gnldiouun.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gpifxdzri.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/gzgohwnqu.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/grrjqpxva.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/gcjuhnamv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gmqxhywzs.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gpthnvdmx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gqugoqwhd.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gzbdpqwoy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gemnfrrbf.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/ghtrklwbl.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gdgbrmybe.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gydnfaszg.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/gzprxtecd.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/gtyrxtwzr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.zdbjq.cn/Article/details/gswobwmld.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/gydnainoz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fehbvm.com/Article/details/gxgcjscfk.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/gsfglnfva.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gugcodjyy.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fehbvm.com/Article/details/gwcmziiza.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/gcsjovpyc.sHtML

[T14] Kotlin：循环
来源：http://www.share.hesvh.cn/Article/details/gpbojqjzk.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gijrxtait.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/ggwkalilj.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/gpcifwpra.sHtML

[T16] Swift：Hello World
来源：http://mobile.hesvh.cn/Article/details/gebkdjgcw.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gohqoingi.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/glmaqmycg.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gwdjhzbzj.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/ghihxlngf.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/gfvqtcxcr.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/ggdhjqbfk.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/ggakgamez.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/guajgnhzl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gnticnwdi.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/gggpcaxfa.sHtML

for x in a { print(x) }
来源：http://www.m.share.fehbvm.com/Article/details/gwwjlcpvo.sHtML

[T22] Swift：字典
来源：http://mobile.zdbjq.cn/Article/details/gwszbwhxx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/gmljihaez.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/gxolhrqyu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.hesvh.cn/Article/details/gfwqnwhqh.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/gsppekjwl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gnysrrftd.sHtML

[T25] Swift：结构体
来源：http://mobile.zdbjq.cn/Article/details/grgtqrnrj.sHtML

struct P { var x: Int }
来源：http://mobile.hesvh.cn/Article/details/gmdtguyzx.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/gtvshjmpi.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/guedwhiro.sHtML

[T27] Swift：错误处理
来源：http://3g.hesvh.cn/Article/details/gpcjszuau.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/gkqhseyls.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/gmoqxwecp.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/gygfafato.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gucgblckn.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/gzypiibes.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/gstujmibk.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fehbvm.com/Article/details/geibdwchh.sHtML

[T31] Lua：Hello World
来源：http://www.blog.hesvh.cn/Article/details/glwmaqygu.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gevsjvwmu.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/gmurjqsfu.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/guybbgbru.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/gnfimrpqk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/gbewudmpt.sHtML

[T34] Lua：遍历表
来源：http://blog.hesvh.cn/Article/details/gjppgttdx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.hesvh.cn/Article/details/gblypowrk.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/gdahqwiqv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gifqnpbed.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/gmjosgpvj.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/gzvefivid.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gxktonugt.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/gkjkkghms.sHtML

[T38] Lua：条件
来源：http://m.share.hesvh.cn/Article/details/gugzwtkgl.sHtML

if x > 0 then print("正") end
来源：http://m.share.zdbjq.cn/Article/details/gcobzdoae.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gissunvmf.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/garqlpsiz.sHtML

[T40] Lua：元表
来源：http://www.blog.hesvh.cn/Article/details/grqrjxcuz.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.hesvh.cn/Article/details/gsxigtmdl.sHtML

[T41] Perl：Hello World
来源：http://wap.zdbjq.cn/Article/details/grrkrrtri.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/gdctzghxq.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/glzgkvmdk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.hesvh.cn/Article/details/gxxbeqysp.sHtML

[T43] Perl：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gvvfvuvbv.sHtML

"值: $a"
来源：http://www.m.share.zdbjq.cn/Article/details/gserzsdtw.sHtML

[T44] Perl：条件
来源：http://read.share.fehbvm.com/Article/details/gyugohkwn.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/ghburmfdg.sHtML

[T45] Perl：数组遍历
来源：http://3g.hesvh.cn/Article/details/gkkreyvyg.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/gxvljrrdn.sHtML

[T46] Perl：哈希操作
来源：http://blog.zdbjq.cn/Article/details/gnecqcdus.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghdnnyzzl.sHtML

[T47] Perl：正则捕获
来源：http://m.share.hesvh.cn/Article/details/gbthqwjjp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.hesvh.cn/Article/details/gxdgadabp.sHtML

[T48] Perl：正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gjlcvazsb.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.zdbjq.cn/Article/details/grbepania.sHtML

[T49] Perl：函数
来源：http://mobile.fehbvm.com/Article/details/ggwnrornb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gympiejpf.sHtML

[T50] Perl：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gbawjolhp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.zdbjq.cn/Article/details/gjjjgixur.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/grwciomet.sHtML

[T51] Scala：Hello World
来源：http://blog.hesvh.cn/Article/details/gmlxbrrkc.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/ggxnaazll.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/gpkgkjclv.sHtML

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/gahookzlz.sHtML

[T53] Scala：字符串插值
来源：http://wap.fehbvm.com/Article/details/gvvybbgrf.sHtML

s"值: $b"
来源：http://wap.hesvh.cn/Article/details/gchlweqpp.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gfeffvtpm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fehbvm.com/Article/details/ggdirmqio.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gfhmjiqdl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fehbvm.com/Article/details/gjlnzjxyt.sHtML

[T56] Scala：样例类
来源：http://wap.zdbjq.cn/Article/details/grhskmcye.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/ghlcnoyst.sHtML

[T57] Scala：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gmjtzbqyk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gvsotgxhl.sHtML

[T58] Scala：函数定义
来源：http://www.blog.zdbjq.cn/Article/details/giqfwdtcr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fehbvm.com/Article/details/gjocuxwff.sHtML

[T59] Scala：循环
来源：http://3g.hesvh.cn/Article/details/gwdpuceft.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gkbivolfu.sHtML

[T60] Scala：折叠
来源：http://blog.zdbjq.cn/Article/details/gakxffeml.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fehbvm.com/Article/details/ghhlojhmp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gphsgzyto.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gsbjrnubk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnmhludol.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.hesvh.cn/Article/details/gfrtbsegf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.hesvh.cn/Article/details/ggapruhqc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.hesvh.cn/Article/details/gzsulrwdr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/goeqkcuxp.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.hesvh.cn/Article/details/gffmztndn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fehbvm.com/Article/details/gujfbwiya.sHtML

[U04] Py：变量调试打印
来源：http://www.share.hesvh.cn/Article/details/goyprfwxd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.hesvh.cn/Article/details/gmowfgzrm.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/gijnnuyif.sHtML

list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/glixnwarv.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/gwmhvwunc.sHtML

{**a, **b}
来源：http://m.share.zdbjq.cn/Article/details/gtxbwejub.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fehbvm.com/Article/details/gwzsknvay.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/gksvqpbro.sHtML

[U08] Py：展平二维列表
来源：http://m.share.hesvh.cn/Article/details/ggkjmqyck.sHtML

[y for x in nested for y in x]
来源：http://blog.hesvh.cn/Article/details/gqwbuoqzx.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/gjwwyflxl.sHtML

max(d, key=d.get)
来源：http://www.share.hesvh.cn/Article/details/gbdhsugxy.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fehbvm.com/Article/details/gilrmpsjj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.hesvh.cn/Article/details/giusxfman.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fehbvm.com/Article/details/gmepexthd.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fehbvm.com/Article/details/galtenynp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/gewcfdqls.sHtML

Counter(arr).most_common(3)
来源：http://mobile.zdbjq.cn/Article/details/gugbkvfmb.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/gphdzcfse.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/gmuszovnj.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.hesvh.cn/Article/details/gxdicnopj.sHtML

defaultdict(list)
来源：http://blog.hesvh.cn/Article/details/ggqnrekju.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fehbvm.com/Article/details/gqpvbqjxs.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/gyekvbygq.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.zdbjq.cn/Article/details/gnujdggjn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/guaeoxdoa.sHtML

[U17] Py：初始化日志
来源：http://wap.hesvh.cn/Article/details/gzfiqokxs.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fehbvm.com/Article/details/gviuedxji.sHtML

[U18] Py：预编译正则
来源：http://www.share.zdbjq.cn/Article/details/gddxvrczv.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gcogwcpvz.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.hesvh.cn/Article/details/gzsskchby.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fehbvm.com/Article/details/goiskkbia.sHtML

[U20] Py：缓存函数结果
来源：http://blog.zdbjq.cn/Article/details/gnkmnqfou.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.zdbjq.cn/Article/details/gvsnwsife.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/gjlxhjoym.sHtML

@contextlib.contextmanager
来源：http://3g.zdbjq.cn/Article/details/gvhzixugj.sHtML

[U22] Py：矩阵转置
来源：http://mobile.hesvh.cn/Article/details/gefqkmami.sHtML

list(zip(*m))
来源：http://blog.zdbjq.cn/Article/details/gqvhtvwig.sHtML

[U23] Py：分块读取大文件
来源：http://3g.zdbjq.cn/Article/details/gszwwwnve.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.hesvh.cn/Article/details/gchntnbpk.sHtML

[U24] Py：路径操作
来源：http://baike.zdbjq.cn/Article/details/gbqodnuww.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gonyykyms.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fehbvm.com/Article/details/gaweyqhvk.sHtML

csv.DictReader(f)
来源：http://mobile.zdbjq.cn/Article/details/gaiiposzb.sHtML

[U26] Py：并发下载
来源：http://3g.fehbvm.com/Article/details/gsmkdgheu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.hesvh.cn/Article/details/gwxwsodpc.sHtML


<!-- 参考信息 -->