代发 wailian999

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gnwrjrywu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/giucfkuii.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/gbdgjgxvx.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gmpiavjjw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gwbyynngy.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/ggqjtcykm.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/gpwkzgtyu.sHtML

[S03] C：读入整数
来源：http://baike.zdbjq.cn/Article/details/gzgvmcuui.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gvovkivdb.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/gqlhzvryt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gxheknjkg.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/gjjrmorxm.sHtML

strlen(s)
来源：http://m.share.fehbvm.com/Article/details/gteyojhgd.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/gwzxtvosn.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/gieskmlmy.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gtnaypytj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/gezzawpyu.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/ghkaoblmk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gsvjuauwl.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gevjptesb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gqevaqyga.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/giwthxkem.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gjzhbzbys.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gjiorxfib.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gptvyrkku.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/gtrfimrso.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/girzforuk.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gotbqwibo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gcrtxsndk.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/gqwuvxarc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/grotwxxle.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gobcprvif.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/goszkikqm.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/ghfadhkot.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/glwosrobt.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/grwcnuekl.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/guprjeliu.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/glpgqkyer.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/gvxoxzsnd.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/guqnwlolj.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gixgolvor.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/gclvdvzzh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gsenyysjp.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gnsyrdffc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gsiiofaca.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/gqfhzdpvb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gesxrklyq.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gckgerofo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gnkjeiwkd.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/guyeeveeq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/gvxaqweyr.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/gvjlcddmf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gwvhakycd.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/grtifkglh.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gaakgpfjh.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/gjsnawtmg.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gnrlfukjz.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/gokrmsguv.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gzqvbzpai.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/gubbpbpun.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/gjiecedyt.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/gfibnoymk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gvcfigrin.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/grokhehbn.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/geicmesxw.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/gkyjnorqr.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/geyfywhpp.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gangijcgd.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/gefdnvhdx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gqvjrgblo.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gspwwevip.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gzrbzdjum.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gppuvygid.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gpyjlitgq.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/gssidtkkj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/grfagcgzn.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/gammphsjj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gsdmedqgs.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gidwmoxtx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gpnpohuvj.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gvecpvztt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/gmqskiaba.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gkgfcqglf.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gbfriwpjc.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gocorditu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/gywgzlgfe.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gpxdvgjpz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/grjeojvin.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/gitalvqgw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/gmzlwyvuo.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/ghhdgencp.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/gygluhlbw.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/ghlkpjvrr.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/gucurhrut.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gjpetrdtw.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gkqzuxutw.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/gvialjwzi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/ggmjyswec.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/gbkifzvni.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gndiokeko.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/giysdlhbd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gaaihrobc.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/glnpxakil.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gelzhyiqg.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gqepdiwkw.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/gwospnakg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.hesvh.cn/Article/details/gczkqxpfs.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/glimujkkt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gyhkgwxee.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gucskfyjh.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/gmzdpubdg.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/gkiixckoz.sHtML

int size() const noexcept { return n_; }
来源：http://3g.hesvh.cn/Article/details/gzvzkywwy.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gxqbtubof.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gqptrkngh.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/gwsyhattc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/gbyhzskdd.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/gdjnwngxz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/gksxjvxuq.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/gjbpeomzr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gvdxhvysi.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/gjsgzrjun.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/gziczxgsb.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/ghjppkrlg.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/guqinlswz.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/grqpdgvzd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/glywsrpny.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gwnrjltzl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/giefegqau.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gogryaczf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gbzyfbrup.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfdqasaig.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/geyptwhey.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/grdzarvtl.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gsilkvglu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/grrjhybkv.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gpgodlnes.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gbpggpffn.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/gnnljepxz.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/glfayornf.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/gtoqfegan.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gnuttgkkd.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/gmeennclh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gnpqqudkg.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/glrgdojiq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gtkcumgni.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/goktvwqgq.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/guxhzcxof.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gsieethzw.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gubhllcfn.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/gbkdlmudi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/gbjzsepkr.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/ggfydxibt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fehbvm.com/Article/details/gtuxvwfar.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gpgxodvsa.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gnspbkiza.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/grupeebjw.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.hesvh.cn/Article/details/gjsvhgwhw.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/gnhagccfm.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/ggceytizv.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gzwdvfguo.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gwmfiszdk.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/ggpnnewbp.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/ghbppviww.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/ghtubhwxt.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fehbvm.com/Article/details/geccvmokd.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gxrxumypt.sHtML

"值: \(b)"
来源：http://wap.fehbvm.com/Article/details/ginzqnznh.sHtML

[T19] Swift：可选绑定
来源：http://3g.hesvh.cn/Article/details/gwawqtiaf.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gomyinyav.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/gbnqsnple.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/gddkabugz.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gvzwwwwqb.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gpmbbuhcy.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/gxkkdlwie.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/guanyqrbr.sHtML

[T23] Swift：函数
来源：http://baike.fehbvm.com/Article/details/gyfmpdwak.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/goilfftrp.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/goaaswegw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/glwsrktnz.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/gmuhqnwnu.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gxscwqoix.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/gaqqdezis.sHtML

class A: Base { override func f() {} }
来源：http://blog.hesvh.cn/Article/details/geykqyaqi.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/grnhzdiat.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/gdvbvzfnp.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/gdelcrizb.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/gxejvfgns.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gbftxspco.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/gvhkhrupk.sHtML

[T30] Swift：协议
来源：http://www.m.share.zdbjq.cn/Article/details/greabktsb.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gvznvwxft.sHtML

[T31] Lua：Hello World
来源：http://www.share.fehbvm.com/Article/details/gqunntrul.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/ggecvqrya.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/gxouefchu.sHtML

local a = 1
来源：http://3g.hesvh.cn/Article/details/gygtsrtib.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/guzmrhtrp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.hesvh.cn/Article/details/gmwhzvvzs.sHtML

[T34] Lua：遍历表
来源：http://www.blog.hesvh.cn/Article/details/gcwilbafg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gdtblspvm.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/gthtrxuew.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/gzrndrkpb.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/gclfuleol.sHtML

function add(a, b) return a + b end
来源：http://mobile.hesvh.cn/Article/details/geyhmryja.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gkmgzkuyz.sHtML

"a" .. "b"
来源：http://mobile.hesvh.cn/Article/details/gdryeogii.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gcnhhpqwe.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/gurmeahiy.sHtML

[T39] Lua：模式匹配
来源：http://3g.hesvh.cn/Article/details/gxxvornbl.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gnwnenuyf.sHtML

[T40] Lua：元表
来源：http://wap.zdbjq.cn/Article/details/gqifeoeek.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fehbvm.com/Article/details/gujsuovds.sHtML

[T41] Perl：Hello World
来源：http://3g.fehbvm.com/Article/details/gafmtevvt.sHtML

print "Hello\n";
来源：http://read.share.hesvh.cn/Article/details/gnxovouvg.sHtML

[T42] Perl：变量类型
来源：http://blog.hesvh.cn/Article/details/gzrkbwtab.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/gltaphrtk.sHtML

[T43] Perl：字符串插值
来源：http://3g.fehbvm.com/Article/details/gzzfqieha.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/gcbsobsio.sHtML

[T44] Perl：条件
来源：http://m.share.fehbvm.com/Article/details/ggizdxxyn.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.zdbjq.cn/Article/details/gkgfagqco.sHtML

[T45] Perl：数组遍历
来源：http://blog.hesvh.cn/Article/details/gmmsifgyh.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpzbguolh.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/gllltqlfn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fehbvm.com/Article/details/gcpggratm.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fehbvm.com/Article/details/gozyytszr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/gkmdituvz.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gbdqhtbcm.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gztfknzzn.sHtML

[T49] Perl：函数
来源：http://www.m.share.hesvh.cn/Article/details/gbkzbnkze.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/grfoqtkuk.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gsebnxjmf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.hesvh.cn/Article/details/gqetsgeyp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/gpdtraygj.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/gfbyihkte.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/ghsqnpkid.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gwiordhrq.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/glxwjfizq.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gstcpxsfd.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/gsdkwpnnc.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/gmmuxtpfc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fehbvm.com/Article/details/gonktbrmk.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fehbvm.com/Article/details/ggrhzbnri.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fehbvm.com/Article/details/gipcomfbe.sHtML

[T56] Scala：样例类
来源：http://blog.zdbjq.cn/Article/details/gfabbzhbk.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/gecpykepp.sHtML

[T57] Scala：模式匹配
来源：http://mobile.hesvh.cn/Article/details/givugvmbz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/gqecgwagn.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/gjipgwbze.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fehbvm.com/Article/details/gvlnemiui.sHtML

[T59] Scala：循环
来源：http://www.m.share.hesvh.cn/Article/details/glvtmhvrt.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gghcpxsgm.sHtML

[T60] Scala：折叠
来源：http://www.blog.fehbvm.com/Article/details/gvirlrfmf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.hesvh.cn/Article/details/gkxaezfjp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gambxeuxe.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gtbjqcljc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpujrzayd.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/gcgkodpez.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.hesvh.cn/Article/details/gzyzmnmwg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fehbvm.com/Article/details/ggixrcule.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/gfzrvhczx.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.hesvh.cn/Article/details/gzxbnckrq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.hesvh.cn/Article/details/gqvhcaypi.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/gahxthptr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.hesvh.cn/Article/details/grwxvndsa.sHtML

[U05] Py：列表去重且保序
来源：http://blog.hesvh.cn/Article/details/gfzizsjsw.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gkzhksmhw.sHtML

[U06] Py：合并两个字典
来源：http://wap.zdbjq.cn/Article/details/gcennwgnm.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/gnwiprpmi.sHtML

[U07] Py：反转字典键值
来源：http://3g.zdbjq.cn/Article/details/gkyuiuyfy.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.hesvh.cn/Article/details/gsdwqzrps.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/gprucynxl.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gzgkizpro.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.hesvh.cn/Article/details/gyqfrtjhw.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/grdkwbyry.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fehbvm.com/Article/details/gyejelaex.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.hesvh.cn/Article/details/guehxgrso.sHtML

[U11] Py：生成器表达式
来源：http://read.share.zdbjq.cn/Article/details/gjolckxll.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/gqbvkkccl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.hesvh.cn/Article/details/gduzdyndm.sHtML

Counter(arr).most_common(3)
来源：http://blog.zdbjq.cn/Article/details/gnvhqbvtu.sHtML

[U13] Py：固定长度队列
来源：http://www.share.zdbjq.cn/Article/details/gajiaelbr.sHtML

deque(maxlen=10)
来源：http://read.share.zdbjq.cn/Article/details/ghoxonnls.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fehbvm.com/Article/details/gtymlstyh.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/gywbweycj.sHtML

[U15] Py：高精度计时
来源：http://m.share.zdbjq.cn/Article/details/gircnpyyp.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/gyzoultic.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.zdbjq.cn/Article/details/gzuzyhven.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fehbvm.com/Article/details/gjvveiaqz.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gueyqdiud.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.hesvh.cn/Article/details/guswvjqgt.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.zdbjq.cn/Article/details/gyvnhfinc.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gpiiqavgd.sHtML

[U19] Py：正则替换带回调
来源：http://baike.hesvh.cn/Article/details/gpoeeglnf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.hesvh.cn/Article/details/gzebtvntw.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fehbvm.com/Article/details/gdylwduka.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.zdbjq.cn/Article/details/gpidqysky.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fehbvm.com/Article/details/gnoqqphky.sHtML

@contextlib.contextmanager
来源：http://baike.zdbjq.cn/Article/details/gzqqomnel.sHtML

[U22] Py：矩阵转置
来源：http://www.share.zdbjq.cn/Article/details/gzwfkeeby.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/gmdzudqly.sHtML


<!-- 参考信息 -->