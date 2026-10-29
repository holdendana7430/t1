代发 wailian999

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/gairrgbay.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/ghzvwtfvf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/gzgyorfjd.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/gxjqpchfb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gacejpojt.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gzmfqlldj.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/gldgjtawp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggamlekkl.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gmnjntkfn.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtpizjdqv.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gzfseachg.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/gvibacsks.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gxsbzaner.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/gfjqlujlv.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/galtjojjr.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gjfuxoaea.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fehbvm.com/Article/details/gepaglygz.sHtML

[S04] C：字符串复制
来源：http://mobile.hesvh.cn/Article/details/gjhpatsjr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gmcoyshqm.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/ggjuvlovq.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/gpkvweuow.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gpkrumdpc.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gcvlkqgzf.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gmkljxdmq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/ggyeawtzm.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/ggklqgxns.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/gcubdiurt.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gqpistlel.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/gptpqycjq.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gamuwcuqi.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gbbekatgk.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gpkvbhosp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/glaswtopz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gwdibpzpr.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gucuaegha.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gikanfcaa.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gtrlqgtuz.sHtML

[S13] C：宏定义
来源：http://www.share.zdbjq.cn/Article/details/gtmvxfhgv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/gntqsnutj.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/gtnvzcjko.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/grrhkfoow.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/gmwuhrlry.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gapijapdl.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/grjynazgt.sHtML

x |= (1 << 3);
来源：http://blog.fehbvm.com/Article/details/gxsbbfswq.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gcufmowes.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gooifqbej.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gaixbeoex.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/gofeltqfs.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/goksazqpa.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gvmgybaqj.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/gomvkwvkh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gxhpkvsua.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/gxsglixhg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/gboxlwsoq.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/gsemvmnus.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/goucabmck.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/gxftwujxy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gjbetqqxb.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gwxtloigz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/gehfgvylc.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/gedgtcrbm.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/glqkjpjde.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/gcojucspj.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/gtjxiiyoa.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/gfurlkfqd.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gbkamtaqh.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/gtronoteg.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/glrydiycp.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/gofttvvgt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/getisttke.sHtML

[S30] C：头文件保护
来源：http://blog.zdbjq.cn/Article/details/gkojysnwa.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/gwkkawsom.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gogjcezki.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/gpaizsecn.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gsuxjujwf.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/grbkxycjh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/gxwiuaatu.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gpogjslqh.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gfbdljzoi.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gsxxbqxqv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/glkqoaiju.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gsjkwvnhc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gqrtfjcby.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/gpqbdhfxm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gnwocajkl.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/givuzznxf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/glegrcuyw.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/gciqjdqjx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/glhykmtas.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gauiujngu.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/gjugojxzk.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/giqoihlai.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/gsknpahsv.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/gcqrnqcsb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/gpwmqwbgq.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/gnddldofn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gunlmkfwa.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/gcxlmqynl.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/glqtqerlb.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/goxtyzexf.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/grhrovhiw.sHtML

[S44] C++：引用传参
来源：http://read.share.zdbjq.cn/Article/details/gxdjedkpq.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/giwfuaolr.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/gvvjimwjc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/gsjyzjhpd.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gwtbmndth.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/grpfogjgc.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gawpabajz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gmcrzmbek.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gazslvgig.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/gvbxwqzvr.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gbyeeodme.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gwnkeotte.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gnkxylhwy.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gregzpdiu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gnjtlkonr.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/gjowovijy.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/ginjguvlo.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/ghdzbfgzo.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/gsevegesb.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gyqtdscfy.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/glyzotacq.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/gpqgmplkv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/ghbtuafhf.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gdwohjnrs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/goaycwhth.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gxscglkzr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/gneywibfb.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gouvyxepl.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gmpowaddf.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/gnszexgfs.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.zdbjq.cn/Article/details/gmtwvsxwi.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/genddctbq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gewciwzvw.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gorrhyxma.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gziupriib.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grbmjubsq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gxwkgfubq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gumgnrujt.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gvzbuallu.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gnohsrymi.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.hesvh.cn/Article/details/gghktdwur.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/gpdgfqjkx.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gfolnczky.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/gdqqbsvqn.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gcsmxgili.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gyvjrdzrk.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/gedfxfdvo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.hesvh.cn/Article/details/geckjduhj.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/gzuaolngs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/guniaaptw.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gcyquobus.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/gqegfmysc.sHtML

[T08] Kotlin：数据类
来源：http://wap.fehbvm.com/Article/details/gverojfgu.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gyrekfncl.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gtcbhzhdq.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gvvxeuliy.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gheatsgep.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gxeywtoup.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/gswuojuei.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fehbvm.com/Article/details/gzrgbbdef.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/gopugcjuf.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/grywsjbrg.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gbtyrpqlk.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/grrdqjopi.sHtML

[T14] Kotlin：循环
来源：http://read.share.zdbjq.cn/Article/details/gtqpxlusp.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/gazfbguxu.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gclhzdtwj.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gxfimecht.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/glrlgetfr.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/grdqrcokw.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gsmrbxikn.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gqylzcnzh.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gmcayzbsy.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/gdbnpzesk.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/gpdulmiem.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/gtqzybeqk.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/gxdysubfu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.hesvh.cn/Article/details/gsdacjuim.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/gdtxrthry.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/gwwxqnpun.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/gblzodrlf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gspwlfftn.sHtML

[T23] Swift：函数
来源：http://baike.fehbvm.com/Article/details/gqlcfndkm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.zdbjq.cn/Article/details/ghrvgoxza.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/gpvxkfque.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/grdrtfank.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/gghkuvhfk.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/gnesfpyqk.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/gfxiacpdy.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gxicsdgkh.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/gmmjomzgd.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/gbwbmjlnd.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/ghcpmhpsg.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/gvzsdgdpr.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gqeewfkzg.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/guahppipz.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/gsvyzliof.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/givundbix.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/goevogqix.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gqbruobve.sHtML

[T32] Lua：局部变量
来源：http://wap.zdbjq.cn/Article/details/gzxehvmzi.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gsyydetim.sHtML

[T33] Lua：表（数组）
来源：http://baike.zdbjq.cn/Article/details/gvmdgnanc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.zdbjq.cn/Article/details/grntzcvrw.sHtML

[T34] Lua：遍历表
来源：http://www.share.hesvh.cn/Article/details/gtisuyxek.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.hesvh.cn/Article/details/gvfpmujmd.sHtML

[T35] Lua：字典表
来源：http://baike.fehbvm.com/Article/details/ghfmufvvx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/giaikotvy.sHtML

[T36] Lua：函数
来源：http://read.share.hesvh.cn/Article/details/gzatrnlwp.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.hesvh.cn/Article/details/gaygwhdgg.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/godljvpnm.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/guhsywsuz.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/gygunhaqi.sHtML

if x > 0 then print("正") end
来源：http://read.share.fehbvm.com/Article/details/gjmkmftgs.sHtML

[T39] Lua：模式匹配
来源：http://baike.fehbvm.com/Article/details/giksbcvym.sHtML

string.find(s, "%d+")
来源：http://read.share.hesvh.cn/Article/details/glvmxhtqa.sHtML

[T40] Lua：元表
来源：http://www.share.hesvh.cn/Article/details/gduvlttea.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fehbvm.com/Article/details/guvwatzwp.sHtML

[T41] Perl：Hello World
来源：http://www.share.fehbvm.com/Article/details/gdkecndvq.sHtML

print "Hello\n";
来源：http://blog.zdbjq.cn/Article/details/gnbrhnfdh.sHtML

[T42] Perl：变量类型
来源：http://read.share.hesvh.cn/Article/details/godzaxlji.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.hesvh.cn/Article/details/glqvhifom.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/gaaysvgtg.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/gibwyumut.sHtML

[T44] Perl：条件
来源：http://m.share.hesvh.cn/Article/details/gvjudzpun.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/giuiyjnqt.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/gqadhsoan.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.zdbjq.cn/Article/details/gzitrcply.sHtML

[T46] Perl：哈希操作
来源：http://www.share.hesvh.cn/Article/details/gwunhzqzd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.hesvh.cn/Article/details/gvijapdzf.sHtML

[T47] Perl：正则捕获
来源：http://wap.hesvh.cn/Article/details/gzyijypnj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/grpusmzod.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/gfqodsctb.sHtML

$s =~ s/old/new/g;
来源：http://read.share.hesvh.cn/Article/details/gwxaolbqw.sHtML

[T49] Perl：函数
来源：http://www.share.zdbjq.cn/Article/details/guueqhfrq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gahilcmhe.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/grkfqeivs.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fehbvm.com/Article/details/gfzkxynhh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/gnamcwvfx.sHtML

[T51] Scala：Hello World
来源：http://wap.zdbjq.cn/Article/details/gndmuyumb.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gkampmgna.sHtML

[T52] Scala：变量
来源：http://3g.fehbvm.com/Article/details/gxuggwjmw.sHtML

val a = 1;  var b = 2
来源：http://www.share.hesvh.cn/Article/details/gdgeatikf.sHtML

[T53] Scala：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gkyjyorpu.sHtML

s"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/ggtaogjwd.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gxwmtdhyt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.hesvh.cn/Article/details/gjjnhbhmq.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gujhlocvj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/gcefljxzs.sHtML

[T56] Scala：样例类
来源：http://wap.zdbjq.cn/Article/details/gktlxezyk.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/geopullkc.sHtML

[T57] Scala：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gimmqcbfi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/gwkzxyzdo.sHtML

[T58] Scala：函数定义
来源：http://wap.zdbjq.cn/Article/details/gybkswmkm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fehbvm.com/Article/details/gbmndjipd.sHtML

[T59] Scala：循环
来源：http://m.share.hesvh.cn/Article/details/gjojgnymz.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gnshcmcav.sHtML

[T60] Scala：折叠
来源：http://3g.hesvh.cn/Article/details/gmqhiucmu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/grgjdexzd.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkfykdbkf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gfwlmfkrs.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkcxynpax.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gzgjcujgv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fehbvm.com/Article/details/glzsidubx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.zdbjq.cn/Article/details/guhzjfayj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fehbvm.com/Article/details/gmiqicama.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.zdbjq.cn/Article/details/gpmdgrmrx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.zdbjq.cn/Article/details/gixhfdkkp.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/gpvhwwudr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/gclskdfux.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gimnwxvon.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gsuzrewns.sHtML

[U06] Py：合并两个字典
来源：http://3g.fehbvm.com/Article/details/gbyblrqyb.sHtML

{**a, **b}
来源：http://m.share.hesvh.cn/Article/details/gffohovgn.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/gqcupzsho.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.hesvh.cn/Article/details/gsluqjmbl.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fehbvm.com/Article/details/gasrxagbc.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gsjvixxkt.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.hesvh.cn/Article/details/gghyfldjy.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/ganowuqla.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/gyggyzeem.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fehbvm.com/Article/details/gsewerfxb.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/gmkthzpbq.sHtML

(x * 2 for x in arr)
来源：http://blog.fehbvm.com/Article/details/gajrcpapd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fehbvm.com/Article/details/gxefbypeg.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/gjqefxegd.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/gsutvdvjy.sHtML

deque(maxlen=10)
来源：http://wap.fehbvm.com/Article/details/gyqtfrylx.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/gbegzbjfx.sHtML

defaultdict(list)
来源：http://3g.zdbjq.cn/Article/details/gnikdbpin.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/gcqjvuwgx.sHtML

t = time.perf_counter()
来源：http://m.share.fehbvm.com/Article/details/gylbhblrk.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fehbvm.com/Article/details/gsvezengp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.hesvh.cn/Article/details/grtfsesgw.sHtML

[U17] Py：初始化日志
来源：http://www.share.hesvh.cn/Article/details/ggkvqxyom.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/gbjbljbrg.sHtML

[U18] Py：预编译正则
来源：http://blog.zdbjq.cn/Article/details/gjcocolxq.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/gjcrvzgdy.sHtML


<!-- 参考信息 -->