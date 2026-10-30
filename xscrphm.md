代发 wailian999

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvdqttbw.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gztbdcugc.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gwcyyqwkw.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcdbuyns.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkggkwbs.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/ganrvjkvx.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gjtdoldmy.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gfevgzsmm.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmasmipyi.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtzmrjhu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gngdmxojc.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/garznjzuv.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmicotoo.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gobrsnulc.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gflwbytvb.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givulajms.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjdnqopx.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdnthugn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgzrkexi.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbqicjbr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdtswdqi.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gakacovzy.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/glzpvwvgh.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/goivxlwhm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gmysfltip.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshdehryp.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvcqhvxu.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gfphmpsan.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjlxuauo.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gugrqbxsk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gcmeinwhl.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmyseznx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gakratjxv.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gbmkzrxiy.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/glpzwabvw.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmlxcksx.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyphmzpxm.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/ghoadstjx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gikympbiz.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gkmmpjvzn.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwonesro.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/ggglmqoto.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geldkbbem.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gyeflavem.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynsquhaf.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gazhyksmn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gwolvsrvx.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gusdbobxo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gkhaobdsr.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gcnfzkiql.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gtgpxwezl.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnenustkd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gceedqczh.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gdpyzjcyv.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gzaxajmoy.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gyjlonxrh.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gnlroxwel.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwydgplw.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwguuamo.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmtlesno.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnozyikx.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/goewuiajt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gklbgmptr.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/ganxbccat.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gabqffosi.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gekjmnbok.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjxuthje.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/greumersp.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfabfzzyk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcgzxhntg.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gymrthpee.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfzgomsr.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifbahuxp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwejwmbi.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrpmacai.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/goxnyvuhl.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gkcpzsqyw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvxhoybv.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/girgrzgyt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyrybqtr.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gaesvzcsx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gznzrcyoh.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gvwyelpmp.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/glejltugg.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmsvuyskq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gymzfshpl.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gsxvzbmhc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gdljcwnks.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaujrlvml.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gskmebnfw.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gijoyglyt.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gvbpvdgdh.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gjgtmjyys.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfkipjhe.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/ggevnzyjt.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqizvngp.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnlbpwcx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/gbfyomhbm.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gvcprvnmv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjlvdoufg.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gtrcapltt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvgzhpnbu.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghnkdurjg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/ggtkwmphb.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqzuqevf.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gghmirmhi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmnsvqvz.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gcvnrfses.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmwudzpq.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gaadjatxi.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvayhdjf.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/gruoxfubs.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guoxxgifn.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gypggdunq.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcisebnu.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gstfgbbdj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gtxrgwplb.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gtpedoyms.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/glhzufras.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapzedzsx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gowhhoicv.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/gudctmqdi.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyitexyal.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsqtcmdr.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqfoizqi.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gowseuzii.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gtizwdegw.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gcfbrfmhy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/ggvavcosw.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/giujxfcic.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxrxyafw.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gpykfsyac.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwdzvnim.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkqlwbrx.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwsccrix.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gcarszeut.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gaxhvdzle.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzscgfqj.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpealilu.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gzfztmzpu.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/giephlhni.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltvdahwo.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzhcmfjx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhtbpjbf.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gbocdqbct.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwemcasft.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gsaehusgu.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gzafabldl.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gyihsojkn.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqibsdeal.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpommqob.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gxztcikvs.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/gteqmwbpe.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/gyqwbvgkr.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcuvlrsj.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gnygfjqgq.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gmobqtxrq.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gtoebkvlr.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gigwjbdlr.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/grluwpiyg.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmfydivn.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gjaxhuxgb.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gaagbkzla.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gxigusefh.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/gwdrmrntl.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gzuaafrnx.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gzbcqfbpn.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcghumyp.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacctoooi.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gufxerntv.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gfujqhsmx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gwrjhzkyn.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gtimowjjb.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmvulfsf.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/gklnlmefx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/glfvlvnzy.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gwhzjrgsx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/goyaktfnu.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/guynrefdw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gatcnwtuk.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/gcpbmfmgu.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/glzhwradd.sHtML

[T26] Swift：类与重写
来源：http://blog.fanxiaobao.xyz/Article/details/glckkrcjb.sHtML

class A: Base { override func f() {} }
来源：http://blog.fanxiaobao.xyz/Article/details/ghvrxhrle.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/glaqtshkt.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/gnoubpzpq.sHtML

[T28] Swift：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmlzzwzy.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbrggdtd.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/grypnofjp.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjoeemlb.sHtML

[T30] Swift：协议
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfvmhhjc.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkflatwkl.sHtML

[T31] Lua：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/guazbmcsl.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbgibjii.sHtML

[T32] Lua：局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/grffsbsly.sHtML

local a = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gkypqigol.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/glohtukeh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxhswngv.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdvcurfw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjkadmsl.sHtML

[T35] Lua：字典表
来源：http://baike.fanxiaobao.xyz/Article/details/gowvdnduw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/grkbgtlek.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gfoanoxyh.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gqufsxola.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gudsqggba.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqobpujk.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gwmzesimq.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgqxocfd.sHtML

[T39] Lua：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/ghhmxsqnk.sHtML

string.find(s, "%d+")
来源：http://wap.fanxiaobao.xyz/Article/details/ghmfargxm.sHtML

[T40] Lua：元表
来源：http://3g.fanxiaobao.xyz/Article/details/guujsajxf.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fanxiaobao.xyz/Article/details/gjfqcenzq.sHtML

[T41] Perl：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gmijtveyh.sHtML

print "Hello\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gsqnpmvqt.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgrjejfl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gfzlskiwl.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuqdwbff.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdsbpwiv.sHtML

[T44] Perl：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gclxqzndk.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gezwkwagw.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gezjmwgba.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmsubxnq.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fanxiaobao.xyz/Article/details/geozhftqi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlxxtyja.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjfwetnl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqxawsyzi.sHtML

[T48] Perl：正则替换
来源：http://baike.fanxiaobao.xyz/Article/details/gcphgyjoq.sHtML

$s =~ s/old/new/g;
来源：http://blog.fanxiaobao.xyz/Article/details/gawzjqsug.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gcbdbovdm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpvspowx.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/ghjrybjdr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fanxiaobao.xyz/Article/details/gbcyotjwx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfcedpwd.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxrwqsmi.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqmpcrya.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gotwkoijs.sHtML

val a = 1;  var b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gskzmpvpu.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpqousgx.sHtML

s"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqnvpafr.sHtML

[T54] Scala：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmnnrbnp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gvfppphuz.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlhmqdjq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmmyiajf.sHtML

[T56] Scala：样例类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknqiehwk.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/glausyaon.sHtML

[T57] Scala：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gzcuuihpn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/ghzkxixfk.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztiyfljf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fanxiaobao.xyz/Article/details/grdtaawex.sHtML

[T59] Scala：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gvibsptzd.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwccpxlun.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgqvdens.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvjmedui.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvflljrf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxtdypmp.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/guugvdprv.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhuubuts.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fanxiaobao.xyz/Article/details/grnmkfdoi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gvirmcrfu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwadexjl.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyoajwqp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdxiiezo.sHtML

[U04] Py：变量调试打印
来源：http://blog.fanxiaobao.xyz/Article/details/gtvsihhxl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplnpmtzs.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fanxiaobao.xyz/Article/details/gpfrhacii.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gmgexyxtu.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gayhooude.sHtML

{**a, **b}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytbczgqh.sHtML

[U07] Py：反转字典键值
来源：http://blog.fanxiaobao.xyz/Article/details/gcmcwialh.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbewjtvyv.sHtML

[U08] Py：展平二维列表
来源：http://blog.fanxiaobao.xyz/Article/details/gxvsgrgra.sHtML

[y for x in nested for y in x]
来源：http://wap.fanxiaobao.xyz/Article/details/gzchoznhu.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqsxcrpc.sHtML

max(d, key=d.get)
来源：http://blog.fanxiaobao.xyz/Article/details/gwtvtjmrg.sHtML

[U10] Py：按值排序字典
来源：http://wap.fanxiaobao.xyz/Article/details/geesztsbu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fanxiaobao.xyz/Article/details/gnlymdifi.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gyivduxfc.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldhmrenh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybkptwbg.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/guoydmwkw.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrghtzuf.sHtML

deque(maxlen=10)
来源：http://m.share.fanxiaobao.xyz/Article/details/goascxwqy.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjofxzrur.sHtML

defaultdict(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkfbikfh.sHtML

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/glppkzuqy.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/gilkozjrp.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/gjqjqpunu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/gjwfvnvdd.sHtML

[U17] Py：初始化日志
来源：http://baike.fanxiaobao.xyz/Article/details/gviqqtlom.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fanxiaobao.xyz/Article/details/gctpttbjh.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/guznuniiq.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsumntlqp.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fanxiaobao.xyz/Article/details/gmihertnp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fanxiaobao.xyz/Article/details/grgqwcrfx.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/gbgrectpg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fanxiaobao.xyz/Article/details/gigshesvp.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvdpdhwd.sHtML

@contextlib.contextmanager
来源：http://blog.fanxiaobao.xyz/Article/details/gfowseraf.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fanxiaobao.xyz/Article/details/gkniazslx.sHtML

list(zip(*m))
来源：http://3g.fanxiaobao.xyz/Article/details/guglfzbae.sHtML


<!-- 参考信息 -->