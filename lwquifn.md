代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/glzqfkxxo.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/ggpazeths.sHtML

time ./run.sh
来源：http://3g.zdbjq.cn/Article/details/ghvrnqkwt.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkyynvjuc.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gnoyaztma.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gezhbhamu.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/gygrachpq.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/gavszpdxy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/gnndigruy.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.zdbjq.cn/Article/details/gzupuzcbc.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gdktyspjc.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gpkjhaqtc.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gamdndveu.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/ghrfzzyrf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gasqgltbd.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/guqrgrrab.sHtML

strlen(s)
来源：http://www.blog.zdbjq.cn/Article/details/gkcietwsr.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gfxvtobjh.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/gvlvbeqbs.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/grpmcoagb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.hesvh.cn/Article/details/gkvqiwiyf.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gtbyfpghj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/gheoskjte.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/gkqnqijrt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gbjhydeey.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gtsytlayq.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gevwgsepu.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gxmzyjpzu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gddrhudnu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gdudsmynr.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gestmzujj.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gdygukhmn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gcijcntlo.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gsaevqwuk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/ghrzjhuif.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gdbonaviy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/gnxetczva.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gngtubsqc.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/gnjgrnpgv.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gguizfmvy.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gqkditvpw.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gragjvgve.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gshmycbny.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gvvvkgkkw.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gqqcnarzh.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/gbvhlapes.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gyqyzultv.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/gtodzfbzh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/ghnnmmtbt.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gyrkqphil.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/gdhudyqwi.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gbzftsvnj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/gzbnkosad.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/ghsablfco.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/gldhaulql.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/grjasyigd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/gdfacjezm.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gaygxcvds.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gxrtlgwof.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/gxtipqsqq.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gdnqkaidi.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gvktoviep.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gdidrrliv.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gycmbtwdf.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gjtggymaw.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/guoezyszs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fehbvm.com/Article/details/gksskhltc.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gvzhzobwk.sHtML

#ifndef X_H
来源：http://blog.hesvh.cn/Article/details/gdhoyzdoj.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/gyowwvpxs.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gcfeyzvsy.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/grziefwav.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/giosxqfal.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/gyhlmjmma.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/gqvnriqot.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/gnsbcwhjd.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/gbiwovlch.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gccpezexw.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/ggsdchzcj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/gaphpetav.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gsdbshjxt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gogoubtqn.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gymdsixdm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gohiwwhcu.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gzxbrqhlh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gsoekeifm.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/gmmkwnnkl.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gjkoftdxv.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/giumnrpxp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gjhfllwti.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gkbaqgvdp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/gsksyaeej.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gruoyuioq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gcarjwcfe.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gkevkixbs.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/gazrwoymd.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/gepwtpcof.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/gnmseumkw.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gpcxagoyz.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/gkhajyfwo.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gdfrsbgcg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/ghjiradcd.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gtbcailsm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/gkmiuopbf.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/gallisixu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gzhuvyphm.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gbaukodll.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gpaqajjkp.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/gxfktizlh.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gknzimlkr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/goespqiqa.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/gmiivkxns.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gnpezfzjt.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/giqxflzeg.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/ggzsdknrf.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/gfpmnvxcc.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/gutsvguce.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/glvfrryjb.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gbxexemao.sHtML

[S54] C++：异常处理
来源：http://wap.hesvh.cn/Article/details/gdogfgemm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/gblyrchxr.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/gkzkssqnv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gtaibxirv.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gkaewckez.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzxcucrao.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/gnyvhvjxp.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gtwvktnjb.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/gsefsttoz.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fehbvm.com/Article/details/gcwaavnnj.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gjpqtwbum.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fehbvm.com/Article/details/gtoebmqor.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/gcjpjwced.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fehbvm.com/Article/details/gtkbsnuwe.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/goxjdppon.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gngxmuqbf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvilnlvdy.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gwwraiwnh.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gvsupbbob.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/gtokvsqpe.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/ggjcldudo.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gbqqsgrln.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gfuucspwr.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/guagvpxhx.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.zdbjq.cn/Article/details/gkhydhduw.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/gafgeumpc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.zdbjq.cn/Article/details/gagrkdtjk.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/gtsqpizuv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/gyxwwzmcl.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gclpmqsaj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gkyvnbpev.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/gkyfzsthc.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gegiqpdjj.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/gkwuxeymj.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/guzhbuiso.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gzilnqkcv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/gzpacyecv.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gvqbgvwni.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/gepbyrglj.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/gqsfninrw.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gmbphbsuv.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/gkvuqaofw.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gcmxkirxw.sHtML

[T14] Kotlin：循环
来源：http://read.share.zdbjq.cn/Article/details/gccxgaksu.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gxhokczqx.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/geugowvmi.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/grbjwbgaw.sHtML

[T16] Swift：Hello World
来源：http://mobile.hesvh.cn/Article/details/ghkoajtpq.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gwygbwfwt.sHtML

[T17] Swift：变量与常量
来源：http://baike.hesvh.cn/Article/details/gseoiorjt.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/gsytpclyp.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gkckxhjtw.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/gtljmrzso.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/gzcpwcjsg.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/gofnifrqt.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/gpoxoxfoo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/glksfpsto.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/ggxtvuxhz.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/ghjlaspyb.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/gnsxrmpvo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.zdbjq.cn/Article/details/gbsvaffnz.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/goqlxnoxl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/gexskomeh.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/gjdiwhcxn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fehbvm.com/Article/details/ggxvzvejj.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/gwksgjwjr.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gjcxqywsd.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/gkfzgkpcq.sHtML

class A: Base { override func f() {} }
来源：http://read.share.hesvh.cn/Article/details/gkqqmpkme.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/ghibrmwkr.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/gkouqjxhd.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/gyrzzpmeq.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/gijxydwzq.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gwsgvkcsa.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fehbvm.com/Article/details/gcieswypj.sHtML

[T30] Swift：协议
来源：http://m.share.fehbvm.com/Article/details/gaxqevlit.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/gcnazicsg.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/gjavrtjas.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gebwzvnfv.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/guowfoizv.sHtML

local a = 1
来源：http://blog.zdbjq.cn/Article/details/gpgfdjnpk.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fehbvm.com/Article/details/gfinaalve.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/gzhmgdsmq.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/gdegitkrx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/gbzrgyarm.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/gfbbwmrfp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/ggzokztyq.sHtML

[T36] Lua：函数
来源：http://read.share.hesvh.cn/Article/details/gmobgggfa.sHtML

function add(a, b) return a + b end
来源：http://baike.hesvh.cn/Article/details/gkzitdabk.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gwgdimukc.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/gfhluwicj.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/geixchbzq.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/gzytnowoc.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/gsodwuxle.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/gkpmnorwk.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/gcjhqtpbw.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/gvgkxiqdj.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gcibcqxjz.sHtML

print "Hello\n";
来源：http://mobile.fehbvm.com/Article/details/gzbbrzrmj.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/gbowofjmx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/gypnvbpvl.sHtML

[T43] Perl：字符串插值
来源：http://3g.hesvh.cn/Article/details/ggbzluwbs.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/gssjfxmuz.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/gdczbjhrq.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.zdbjq.cn/Article/details/gbzxhnfuy.sHtML

[T45] Perl：数组遍历
来源：http://wap.fehbvm.com/Article/details/ghxsqtjjm.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.zdbjq.cn/Article/details/gfplaortc.sHtML

[T46] Perl：哈希操作
来源：http://baike.hesvh.cn/Article/details/gbylhozaq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/gfrldnzmj.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/ghmwhxxau.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/ggarvqqcu.sHtML

[T48] Perl：正则替换
来源：http://baike.zdbjq.cn/Article/details/gvnpcalgt.sHtML

$s =~ s/old/new/g;
来源：http://www.share.hesvh.cn/Article/details/gpueoattg.sHtML

[T49] Perl：函数
来源：http://read.share.hesvh.cn/Article/details/gddjpvnre.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gxvvondrg.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gvaigpdpc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/grojcpylu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fehbvm.com/Article/details/guotrfasz.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gmrtchpzw.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gwvuimosw.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/gweichltf.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/gwdehvyee.sHtML

[T53] Scala：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gnywsbajp.sHtML

s"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gpkdiiykq.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/gnkohuerq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fehbvm.com/Article/details/gfznckjlk.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/ghzasjmau.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.hesvh.cn/Article/details/gwyicfzcm.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gnzmgrixt.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/gaqrobhde.sHtML

[T57] Scala：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gasyortoi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gwniwtnls.sHtML

[T58] Scala：函数定义
来源：http://www.blog.zdbjq.cn/Article/details/gebhlhujp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fehbvm.com/Article/details/gaiprkezu.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gzscdjgse.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gnjsoczza.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/gvxfpcvuy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/gxlcwchwz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gaoidmywz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gfaidsbac.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxmvvxhos.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/gtfxwtiks.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/guimelmpo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.zdbjq.cn/Article/details/gdeekshdp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fehbvm.com/Article/details/ghqezplvr.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fehbvm.com/Article/details/gvlyfxcme.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fehbvm.com/Article/details/gsobwyzjz.sHtML

[U04] Py：变量调试打印
来源：http://mobile.zdbjq.cn/Article/details/grtrrtwre.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fehbvm.com/Article/details/ggkiwydda.sHtML

[U05] Py：列表去重且保序
来源：http://blog.zdbjq.cn/Article/details/gqscomyop.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/giaepulme.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/gsthnwsla.sHtML

{**a, **b}
来源：http://mobile.zdbjq.cn/Article/details/gngjbecuh.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fehbvm.com/Article/details/ghwcjprpw.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/ghmyhpikx.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/gvnsxibkz.sHtML

[y for x in nested for y in x]
来源：http://3g.hesvh.cn/Article/details/gfgsnwbdu.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.hesvh.cn/Article/details/glkbxlnug.sHtML

max(d, key=d.get)
来源：http://www.m.share.zdbjq.cn/Article/details/gcaxaxjkm.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/grlmmalxk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.hesvh.cn/Article/details/gnfpyggqt.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/gzizhlylu.sHtML

(x * 2 for x in arr)
来源：http://baike.fehbvm.com/Article/details/gcmwqusix.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fehbvm.com/Article/details/gjwuhsiyq.sHtML

Counter(arr).most_common(3)
来源：http://blog.fehbvm.com/Article/details/gbllnjktu.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fehbvm.com/Article/details/gmycynkjx.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gslogutbg.sHtML

[U14] Py：分组收集到列表
来源：http://baike.hesvh.cn/Article/details/gqcfmupst.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/ghiyukgpu.sHtML

[U15] Py：高精度计时
来源：http://blog.hesvh.cn/Article/details/gvvrxglxn.sHtML

t = time.perf_counter()
来源：http://blog.hesvh.cn/Article/details/gxunkwmnd.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.zdbjq.cn/Article/details/glnzapabw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.zdbjq.cn/Article/details/gouxgdgut.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/gtnmgrpkc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.hesvh.cn/Article/details/gmcpjifaj.sHtML

[U18] Py：预编译正则
来源：http://m.share.zdbjq.cn/Article/details/gahgpdkuq.sHtML

pat = re.compile(r"\d+")
来源：http://3g.zdbjq.cn/Article/details/gdbzlfgpw.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/gqusaqccr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.hesvh.cn/Article/details/gpvaaxjlb.sHtML

[U20] Py：缓存函数结果
来源：http://wap.hesvh.cn/Article/details/gqozttiws.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.zdbjq.cn/Article/details/gvlpooauk.sHtML


<!-- 参考信息 -->