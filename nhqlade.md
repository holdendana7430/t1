代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/gxemkwfuk.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/geauvzjxh.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gieknxqnl.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvtchmvoj.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/gtxqinqmu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnjmfvcsj.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gdjbxxvtn.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/gttvsrgbi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/gizfpdgrl.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/glixkdjec.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gnkwoilye.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gdmncwfry.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/ggrgflgpp.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/gtikvhghl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gshdoknqg.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gvjibavqx.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/ghqpjlbyx.sHtML

[S06] C：字符串比较
来源：http://blog.hesvh.cn/Article/details/gpuauskxd.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gbumaqyol.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/gtmdmffiv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/gqjvfklbk.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gquoxnvfp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gnumwciku.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gmxjkleft.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gpkxvuuvk.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gmvjqykor.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gzfhiwesh.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gieinbori.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gushaeuzc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/gosxxnbyg.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/gzskfuhgy.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gicnjezhn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gklaszail.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gjcdqpxtx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/ghveyjijb.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gtrxefwdy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/gwjhvqkfl.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/gyqovxdms.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gourdhoxh.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/ghafwrmgr.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gaeguxhzo.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/giworuvaa.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/glzeviyci.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gktzqsfnt.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gonsxeavh.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/glaoczunf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gmvvuynca.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/gvevwgsgd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gfjmajtre.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/gnbbinxdn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/glqqxvtfb.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gmmahagvk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gkohnzfzn.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/gthlsrecz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/gbmahrifp.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/goteptmqi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gqpawaiol.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gkefsprmm.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gevhyansp.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/gyizuiwsg.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gslyrtitu.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/gomauijpu.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gttxjyzbi.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/guyfvscxk.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/gvlqqsgsh.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gbqawksfc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/gztzssqhp.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gancfqjeq.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/gdydbsymv.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gadzqytns.sHtML

#endif
来源：http://blog.zdbjq.cn/Article/details/ginzhoazl.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gnkdgorzg.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gugowdlln.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/gdtfskzyj.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gmhsgmqkf.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/gjxsznkxr.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/guymfvort.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gxggbnzaq.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/gspzwqgli.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.zdbjq.cn/Article/details/gzgkgjsah.sHtML

[S35] C++：map
来源：http://blog.hesvh.cn/Article/details/gpmzlilac.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gjupgkzbz.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gtoawhoff.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gbxzmonxg.sHtML

[S37] C++：set
来源：http://www.blog.zdbjq.cn/Article/details/gszomsqon.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gcayjcvtg.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gjtyepmyv.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/gckoizuop.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.hesvh.cn/Article/details/gjtmqivnp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/ghgdquhid.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/gsuukwznl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.hesvh.cn/Article/details/gxzxpeozc.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gdiymtybs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gvqblephg.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/gaeaalicv.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/glaxlxvuy.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gqfrksybw.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/gjeneqhcz.sHtML

[S44] C++：引用传参
来源：http://mobile.hesvh.cn/Article/details/ghnwmjzoz.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/glstuejuh.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gefjipqsh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/ghafoyglb.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/gketxddov.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/gpgktnegz.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gtrtyeics.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gngwabjgc.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gqmzetqif.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/ghzclmayu.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/grsnjtjzt.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/grevcvifh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/gucyoqvhi.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/geakwdsul.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gtdmlmdxg.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/ggkntinxm.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/glbeobdbj.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gwyvcnutx.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/gdkpmegwi.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/gcafmpiaz.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gwfykklfc.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/gtzagjdfe.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gqkwfexoa.sHtML

[S55] C++：结构化绑定
来源：http://m.share.zdbjq.cn/Article/details/gbdzflpyk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gjbxgdmwl.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/gohcftiix.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/gezaomxjx.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/gbyvfnnuo.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/gcnnrkwfb.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/gmqoyrhdx.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gmeaamihp.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/gvhcjudih.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.zdbjq.cn/Article/details/gqzoxgzyy.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/gvirssyxv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/gpmchqvia.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwnhsbqzn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gknyjwfcq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmulizywe.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gtgtvnnfe.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gfpvdanwg.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gjfxegdjt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/gmxpjmpht.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gblyeomvh.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gtempavtv.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/glikfyjyg.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/ghyzbzmay.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/ggnehwdlj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.zdbjq.cn/Article/details/gtntupaaf.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/girljddff.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/grtujegiy.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gxktqhhyu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/ggdlthqyb.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gqzxrivmb.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gbsansisx.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/gjetbewhx.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/gqpelwakd.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/gwgtctlrk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.hesvh.cn/Article/details/gczdiexfl.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gaerufcaj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gfkrqzgjn.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/gfcbqkqyz.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gledmtmby.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/gfymenzkr.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/ggmmgtktw.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gtfipmahp.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/grvrpdlow.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/gvaleldpk.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gqscwqrxv.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gsljkbczf.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gtlkolbhc.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gabwurpul.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/gdizsnosw.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gycnbkehe.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/ghprjnnkh.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/gzftztccx.sHtML

if let n = opt { print(n) }
来源：http://www.share.hesvh.cn/Article/details/gxufcmxjn.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/gwhfeaarw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/gjxuvlvfr.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gqexscjua.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/gqrurqofw.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gzvomiige.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/gvsqbnsaw.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gkremvfcg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/gglosxjsm.sHtML

[T24] Swift：闭包
来源：http://mobile.fehbvm.com/Article/details/gzuxxpqgb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/gbgttxtut.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/gftbjjbzp.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/glbhxwrzv.sHtML

[T26] Swift：类与重写
来源：http://www.blog.zdbjq.cn/Article/details/gqpjalvxd.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/ggtmwtnww.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/grrvqzxbo.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/greudxgtr.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/grkldpemt.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/gbavntwio.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/gmfdsuxtb.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gtwrrsezs.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/gibdakqil.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fehbvm.com/Article/details/gnbgnatqd.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/gbjkdtbwd.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/guuhcwksf.sHtML

[T32] Lua：局部变量
来源：http://wap.fehbvm.com/Article/details/gjrzkdusx.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/gwwyhksrm.sHtML

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/ghjpqbsai.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fehbvm.com/Article/details/gaaklbsji.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gnnjrxfjz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/gmjvanrks.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gfoplurmj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.hesvh.cn/Article/details/gorgsxsgg.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/gzmfxlasf.sHtML

function add(a, b) return a + b end
来源：http://m.share.hesvh.cn/Article/details/goikavhqb.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/glmupvuub.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/gtcnzgqbm.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/giajrlveq.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/ghulbmesu.sHtML

[T39] Lua：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gdqqomopy.sHtML

string.find(s, "%d+")
来源：http://3g.zdbjq.cn/Article/details/gulsrznlf.sHtML

[T40] Lua：元表
来源：http://read.share.fehbvm.com/Article/details/gyhzjllhd.sHtML

setmetatable({}, { __index = base })
来源：http://baike.hesvh.cn/Article/details/gznybwtot.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gkbiujtqa.sHtML

print "Hello\n";
来源：http://baike.hesvh.cn/Article/details/glxrmsbvk.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/gbbxkitjt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gsqccmifl.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gmcfpsvjo.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/gsngoddqq.sHtML

[T44] Perl：条件
来源：http://mobile.hesvh.cn/Article/details/ghmrmfjxk.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/gdghcavzy.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/guvuksixl.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/gitqeeqyg.sHtML

[T46] Perl：哈希操作
来源：http://mobile.zdbjq.cn/Article/details/gabxxgkau.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/gjncbawkh.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/gnbkcjtxo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.zdbjq.cn/Article/details/gotefdkdm.sHtML

[T48] Perl：正则替换
来源：http://www.share.zdbjq.cn/Article/details/gojtcqueq.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/gxhvdmkpl.sHtML

[T49] Perl：函数
来源：http://m.share.zdbjq.cn/Article/details/gunflarhj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/ghhefyqyi.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gdxkomgyg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fehbvm.com/Article/details/gvhlubgtt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fehbvm.com/Article/details/gycjkqlpl.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/giumqekfd.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gjwnamkht.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/gdqkjshun.sHtML

val a = 1;  var b = 2
来源：http://www.share.hesvh.cn/Article/details/gcnleedvt.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gyddvgmdr.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gbsuvahnl.sHtML

[T54] Scala：集合映射
来源：http://m.share.hesvh.cn/Article/details/glsjqslgx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fehbvm.com/Article/details/ghytwvykh.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gvkdoxcqa.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fehbvm.com/Article/details/gmfbewklj.sHtML

[T56] Scala：样例类
来源：http://3g.zdbjq.cn/Article/details/gajfsvpfx.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/gdqwujwdp.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/ggjsritft.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gauvmphpn.sHtML

[T58] Scala：函数定义
来源：http://wap.hesvh.cn/Article/details/gyjriipmn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.hesvh.cn/Article/details/gwafkjkbm.sHtML

[T59] Scala：循环
来源：http://wap.hesvh.cn/Article/details/gygnbtycu.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/ghybjvptw.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/gfiyieteo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/glqnkgsuu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwnhhbzgf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gklrulrbd.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghueplxnz.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/geucjlqjg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.hesvh.cn/Article/details/grzagcvhn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.zdbjq.cn/Article/details/gpsrmfqjq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/gmxxblezd.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/gabcewxcf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.hesvh.cn/Article/details/goaotlgqz.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.hesvh.cn/Article/details/gxvrbjnnm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.zdbjq.cn/Article/details/gqvnmkhpz.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.zdbjq.cn/Article/details/ghbggdafp.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/ghfyezleg.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gfkuqyuiq.sHtML

{**a, **b}
来源：http://baike.zdbjq.cn/Article/details/gyivrakfb.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fehbvm.com/Article/details/gsusfktmk.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.hesvh.cn/Article/details/gzwwqsupk.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/gbgaqmmny.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/gvbdqtsca.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/gjbteghte.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/gydaxpsll.sHtML

[U10] Py：按值排序字典
来源：http://mobile.zdbjq.cn/Article/details/geshzdkoc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/gmfyzuvix.sHtML

[U11] Py：生成器表达式
来源：http://mobile.hesvh.cn/Article/details/gxuhmewbx.sHtML

(x * 2 for x in arr)
来源：http://3g.zdbjq.cn/Article/details/gvvlioxmj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.zdbjq.cn/Article/details/gvbfnksjz.sHtML

Counter(arr).most_common(3)
来源：http://blog.zdbjq.cn/Article/details/gzxannwkf.sHtML

[U13] Py：固定长度队列
来源：http://3g.zdbjq.cn/Article/details/giydviayw.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/gbpguyfft.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.zdbjq.cn/Article/details/gzrhajusl.sHtML

defaultdict(list)
来源：http://m.share.zdbjq.cn/Article/details/ggpqcfwyx.sHtML

[U15] Py：高精度计时
来源：http://wap.hesvh.cn/Article/details/gncjcwmcv.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/gvaxyjfqs.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/gcklhwenk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fehbvm.com/Article/details/ghcbhskso.sHtML

[U17] Py：初始化日志
来源：http://blog.zdbjq.cn/Article/details/gwfddxnhz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fehbvm.com/Article/details/gacxgjdab.sHtML

[U18] Py：预编译正则
来源：http://www.share.hesvh.cn/Article/details/ghbnionmg.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fehbvm.com/Article/details/gklackuys.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.zdbjq.cn/Article/details/gvezejyfs.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fehbvm.com/Article/details/gepifyomj.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fehbvm.com/Article/details/gagqocedz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.hesvh.cn/Article/details/gzbbcidtv.sHtML


<!-- 参考信息 -->