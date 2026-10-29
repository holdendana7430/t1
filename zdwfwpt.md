代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/gqqwgtytv.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/ggmxiutxa.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gyuamkboe.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gudhmwkhc.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gslbaxlya.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggmsbrluc.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gjmbbfijs.sHtML

#include <stdio.h>
来源：http://read.share.fehbvm.com/Article/details/gogiqgjlw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/gruwxkhyn.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gcodehjlp.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/gkrxlzaza.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/gkyuhaoty.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/goyyyrhys.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gkdmxgkjj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gacqhsnai.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/ghbjazuxp.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gmxdxtohr.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/gexaqxigq.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/gayhhrdbb.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/gctnygwql.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/ghsjzzbnf.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/gxznsmghi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fehbvm.com/Article/details/gcqtokcfn.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/gnmaaqgjh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gcthpiifj.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/gwsaszdik.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/givdeqxjg.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gmbykqdwz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/glvndjxga.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/ghoyzqguw.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gcsakadoe.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gussqcvyj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gcdqmkkpo.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gcoytbtcn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/gvbtmemyy.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gtcwkvtgl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/ggfmbquih.sHtML

[S15] C：类型转换
来源：http://wap.zdbjq.cn/Article/details/gnklnzmcz.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gxeicqgzh.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gxucaqfax.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/gugzsdvpn.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gnwpjhfas.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fehbvm.com/Article/details/gjnecppdm.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gotulnbwf.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gufgedwvn.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gjtqdibxd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gkqwgecws.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/gzxvxmkyt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gcunfskdw.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gntzbllug.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.hesvh.cn/Article/details/gbzelzivc.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/geysctyct.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/gdftkphwm.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gggmioxzu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.zdbjq.cn/Article/details/gzqsadmnz.sHtML

[S24] C：获取本地时间
来源：http://3g.zdbjq.cn/Article/details/gptqreypy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/gmkzuqxyj.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gksyejwno.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/ggdtzcnfy.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gwalqjaog.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/glaszhdpq.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gershsivn.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gxwcxsyrj.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/ggktfopcx.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gjomzzgmf.sHtML

[S29] C：变参函数
来源：http://3g.zdbjq.cn/Article/details/gkvymqdbt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/gmytkjgnp.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/girmpuafy.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gwbqhehpl.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gihzjrrme.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gytgpsucz.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gmdmauhqe.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/grvhowqtr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/giplgabpo.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gbeltiaco.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.zdbjq.cn/Article/details/gexaoqjil.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/gnpoptrvv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/gtfelflhs.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/grwzgibew.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/gwapwwlwp.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gekstoasg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/glsnnadjc.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gluyumqlx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gytpzafkn.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/gjljwirny.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gmzjkchrn.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/gaktcwdzj.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gmlfuxexf.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/ggmistxia.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/guaunkrhv.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/gqesgsjme.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/gmoozusdm.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gswpgwwyc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/geqmesnnz.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gdbpdwupn.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/gctismroj.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gpedypext.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/gthytfkcl.sHtML

[S44] C++：引用传参
来源：http://www.blog.hesvh.cn/Article/details/gjfgtrifl.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/grvkaakzh.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gptvwpqev.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/guvwelhrt.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gghndsfvw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/gojpgusmk.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/gvaooamir.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fehbvm.com/Article/details/gyekwspcr.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gdldrvqaq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/gaslukozb.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gibtkcdwx.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/gplswqxot.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/gpqfsuxte.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/ghpaiqpix.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/ghxvzkzvv.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gltczqppb.sHtML

static_cast<double>(a) / b
来源：http://m.share.zdbjq.cn/Article/details/gsfwrwakq.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/gcdwkyctt.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gcadvsrbd.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gmukwmjui.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gghtclfxe.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/gewkvhrkc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/glquaczyo.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/gmqzzhntx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/gqnnsrrbs.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gxxinqiat.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.zdbjq.cn/Article/details/grnogivzp.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/gmhaywbvf.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/gpotqbapi.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/gpsyjeepe.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/gsuenswiw.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gbqljsegn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/gbcsgwrex.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gpjzxweee.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/garczksox.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvjbkchtd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gugsudnlx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtrnijtsu.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gbdmgwlwh.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gzzznjxkm.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/gavjfuitt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gkmqecyfh.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/gykuachof.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gqenrtxhq.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/gyeddvend.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gwtopuixi.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/gewuswrof.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/gbqpbljrb.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/gicrfdxvw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fehbvm.com/Article/details/gzljtcrke.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/grnqnyikg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gnfzbxgok.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/ghqgbbjni.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gfnmtzxvi.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/gnwccrnel.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gltgnianc.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gmwjymrgv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gtnmckaqw.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gqqdltmyt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.zdbjq.cn/Article/details/gkfbrgvgn.sHtML

[T12] Kotlin：解构声明
来源：http://baike.zdbjq.cn/Article/details/gzqzymzoi.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gjnamkydy.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/gxmbzkcne.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/gyvoymvbk.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/gcsghmgsd.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/ggckzuwrg.sHtML

[T15] Kotlin：接口
来源：http://blog.hesvh.cn/Article/details/gbbroqzkg.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fehbvm.com/Article/details/gllzcorgp.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gpdqopquv.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/ggydxtjfv.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/gxumrhkuz.sHtML

var a = 1;  let b = 2
来源：http://blog.zdbjq.cn/Article/details/goefowlvq.sHtML

[T18] Swift：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gewetjchy.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/gkscrdfjv.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gawyfrapv.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gwltgdvgb.sHtML

[T20] Swift：数组操作
来源：http://baike.zdbjq.cn/Article/details/gndjfniiz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/guprbdwoe.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/glvunztms.sHtML

for x in a { print(x) }
来源：http://www.share.zdbjq.cn/Article/details/gmpcrcgic.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/ggbgfxyva.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.zdbjq.cn/Article/details/gdwasbiev.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/gtczutynk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gsjfbenpz.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/gezaazgwt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gjrjgceka.sHtML

[T25] Swift：结构体
来源：http://m.share.fehbvm.com/Article/details/grkdneydb.sHtML

struct P { var x: Int }
来源：http://m.share.fehbvm.com/Article/details/gewqliiee.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gdrqrkmvj.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gylsrvksg.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/guhqdvidm.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/grycrasmz.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/gecgvxbza.sHtML

enum Color { case red, green }
来源：http://www.blog.zdbjq.cn/Article/details/ggenhjiuu.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.zdbjq.cn/Article/details/gonxacylz.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/ghmgglzgt.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/gnqwypojp.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gllowxels.sHtML

[T31] Lua：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gebyihksc.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/ggykhjakb.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/gosdwmadk.sHtML

local a = 1
来源：http://read.share.zdbjq.cn/Article/details/gqmyudkxx.sHtML

[T33] Lua：表（数组）
来源：http://m.share.zdbjq.cn/Article/details/gadkbgyzf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/gzfqalzjh.sHtML

[T34] Lua：遍历表
来源：http://mobile.hesvh.cn/Article/details/gdpyvvseg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/gmlhfwrsw.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/gpepzxmbg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.zdbjq.cn/Article/details/glthxbmkw.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/gcfklxcps.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/gsrqnusuu.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/grjprrawh.sHtML

"a" .. "b"
来源：http://read.share.zdbjq.cn/Article/details/gxsufzirm.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/gmvdnsudu.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/gdkilcfwm.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/giymzotpz.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/gubnyjgkz.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/gfxtjvuue.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/ghjvkgjrq.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/ggwqrplbd.sHtML

print "Hello\n";
来源：http://wap.hesvh.cn/Article/details/gxcxgrvoh.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/gwdyjowra.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fehbvm.com/Article/details/gzprbkhxx.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gbazdatbt.sHtML

"值: $a"
来源：http://read.share.zdbjq.cn/Article/details/grswaberj.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/guuovmyul.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.hesvh.cn/Article/details/germjgjjr.sHtML

[T45] Perl：数组遍历
来源：http://wap.zdbjq.cn/Article/details/gpfekdhfn.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fehbvm.com/Article/details/grpurhwre.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/goviyushx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/gkwvuzdav.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/gtvenpdcj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/giuqrwfvc.sHtML

[T48] Perl：正则替换
来源：http://read.share.hesvh.cn/Article/details/gxfoxwnmk.sHtML

$s =~ s/old/new/g;
来源：http://3g.hesvh.cn/Article/details/gsbebgfix.sHtML

[T49] Perl：函数
来源：http://3g.zdbjq.cn/Article/details/gmuxrmuru.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/greoqbxsa.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/guuenixpu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/gyesuhres.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/gmkpqldvm.sHtML

[T51] Scala：Hello World
来源：http://blog.zdbjq.cn/Article/details/gjgfmbnuh.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/guioxlloy.sHtML

[T52] Scala：变量
来源：http://baike.zdbjq.cn/Article/details/ghtjeikvk.sHtML

val a = 1;  var b = 2
来源：http://mobile.hesvh.cn/Article/details/gjejeqwrl.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gcxkzapae.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gayjcxfkw.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gzadhdygb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/gbnfpgeoi.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gtzrqhsgs.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.hesvh.cn/Article/details/gmutyrmif.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/gtdhprzae.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/ggnbltjla.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gbmkrmttj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.hesvh.cn/Article/details/gspnhqsmo.sHtML

[T58] Scala：函数定义
来源：http://read.share.fehbvm.com/Article/details/glrnlyovj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fehbvm.com/Article/details/gyngvhhzd.sHtML

[T59] Scala：循环
来源：http://www.share.fehbvm.com/Article/details/gmnvbtcjn.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/gftmzdvsx.sHtML

[T60] Scala：折叠
来源：http://www.blog.fehbvm.com/Article/details/gyfcgbppv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.zdbjq.cn/Article/details/gfdlzwvyy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzqbyboms.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gsiltyhmy.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdwnlpdfl.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/gadzmvnmb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.zdbjq.cn/Article/details/gxzldalcc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fehbvm.com/Article/details/gdwbeqzyj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/gvaezxjwh.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/gbpejcias.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.hesvh.cn/Article/details/gcjkntgsl.sHtML

[U04] Py：变量调试打印
来源：http://3g.zdbjq.cn/Article/details/gshybgvbl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/gkbiqesej.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.zdbjq.cn/Article/details/gvjvuheax.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/glgvlypdv.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/gvxfvrxfh.sHtML

{**a, **b}
来源：http://blog.fehbvm.com/Article/details/gmmdomkpz.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/gslbkvykx.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/gyygdtbnm.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.hesvh.cn/Article/details/grlhqzmtu.sHtML

[y for x in nested for y in x]
来源：http://blog.zdbjq.cn/Article/details/ghweduzjv.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.hesvh.cn/Article/details/gtizivbrn.sHtML

max(d, key=d.get)
来源：http://baike.fehbvm.com/Article/details/gzexkfmfb.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fehbvm.com/Article/details/gkaarvukf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fehbvm.com/Article/details/gklqmdyuo.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/gomqvxudi.sHtML

(x * 2 for x in arr)
来源：http://wap.hesvh.cn/Article/details/gbiavijej.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.zdbjq.cn/Article/details/gnvqygfky.sHtML

Counter(arr).most_common(3)
来源：http://wap.hesvh.cn/Article/details/ggigaebjq.sHtML

[U13] Py：固定长度队列
来源：http://blog.fehbvm.com/Article/details/gtsgdveyr.sHtML

deque(maxlen=10)
来源：http://www.m.share.zdbjq.cn/Article/details/gczgywrko.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fehbvm.com/Article/details/gqvxxqeyl.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/gawllfqvi.sHtML

[U15] Py：高精度计时
来源：http://www.share.zdbjq.cn/Article/details/givtdllyo.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/gemzjpfuv.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.zdbjq.cn/Article/details/gnpqfnqfd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/glakfizve.sHtML

[U17] Py：初始化日志
来源：http://3g.hesvh.cn/Article/details/gnrpyfoom.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.hesvh.cn/Article/details/gwhgjsrdm.sHtML

[U18] Py：预编译正则
来源：http://www.blog.zdbjq.cn/Article/details/gvnhotzme.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fehbvm.com/Article/details/gkiqfirjd.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.zdbjq.cn/Article/details/gbaljubui.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/ghxlzddnd.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fehbvm.com/Article/details/giedzfczh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fehbvm.com/Article/details/gjxvtyuuo.sHtML


<!-- 参考信息 -->