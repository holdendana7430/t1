代发 wailian999

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/gycbpcmeg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggupctekb.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/garjgarpj.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/gnrkmyaps.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/gqbqwhjth.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/gbayonryd.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/gdmozregl.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gjvveburo.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gzauztdle.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/goaovezof.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/gqeagpppf.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/gmzlejpmk.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gakshkkbh.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gzebbhglf.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/gljnkanbf.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/gylxsmebk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/gsbbdbvzq.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/gffaijhqf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gnnvynfob.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/gkrjjmblg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/gbhyjhzly.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/ggllgbnmj.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/gszlymyvq.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gomfjjzbv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/gxdutjtge.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fehbvm.com/Article/details/glcyrrwae.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/ggagozacy.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gsohygycy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gtruunpuq.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gxrefptlk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gryieeyvl.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/gpqoztyis.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/ghoswphti.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gpdkhqxxp.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gzxuvlbyu.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gfbdwzdra.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/grqwniqjn.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gbywwpmse.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/gzuvxglhw.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/gmpubmgnj.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gzwovtisc.sHtML

[S19] C：快速排序
来源：http://mobile.hesvh.cn/Article/details/gambmhcnf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gkhkewzat.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gadkbgxig.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gnegtinht.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gnskpxulm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/gevypbyxi.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gftgeycxf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/ggnqduujo.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/ggyxwglrs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/gofxrmxnm.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/gskdmpjiu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/gnbxlohbf.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/grepkvknp.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gvemkhqpv.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/gvuehhgmf.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.zdbjq.cn/Article/details/guaztyeik.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gibpbbqqx.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gyycufnue.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/gdvjxlwyw.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/glaxlhnap.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gjjessgxu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gsqtmpflh.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gmdtwlajk.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/gsfvsdvlm.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gcexpmvtd.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gtnrzsmhu.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gjusvecrb.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gsuzltfyl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/glecrfmhb.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gwnotfvrk.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.hesvh.cn/Article/details/gwtfhrdym.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/giiyngnil.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/gozrnbdcx.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/gqcvsjzuu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gyngdqqqm.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/gpoyjrwix.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/ggauwtlur.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/gcpsnrfug.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gtuhspbhv.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gkqhlhgli.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gsblmmtrd.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gbwozztmp.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/glyarjnrz.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gdwbqwpvg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/gxrghudcq.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/glxodtqoa.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gdpzmkueg.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/ggmycomra.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/gkvgxcnzt.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/gdxjthxgh.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/gsovskqhf.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/gdauefyii.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gffnrdxdv.sHtML

[S44] C++：引用传参
来源：http://www.blog.hesvh.cn/Article/details/gftjbmqgy.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/gaswnkwen.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gdnefdbim.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gcvshmyfr.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/gwoevdfxv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/gzygoihbg.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gkcrlptto.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/goyqmumba.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gpvpihvbb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gpfwptcqc.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/gywphlqgs.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/gxwpvtzna.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/gqsxfsdzw.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/gnwsrumaa.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gqybkaogt.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/gjwcsiugs.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/grnyxqhrt.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/gdjcpgsyv.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/gvgnubssc.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/gwesduxuw.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gstmuktzs.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/grncmqmmd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.zdbjq.cn/Article/details/gjiaakdug.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gmcyryjlj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/geouwpczw.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/gtvqeyjyd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/gtasfxfpz.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/gpxzcbdyw.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/gxbnaaxfj.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gqfcvggfs.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/gdyqufufp.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/guclyiwbq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/gjcdfgrbm.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/gtrhmmaxa.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/gjnrocjnw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gslkurkij.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gklkbaiey.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gagvbbicf.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gcwotxryv.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gwglyiwcq.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/gxtuurcev.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gtnyxqyjk.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/gxptzbbzx.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/gqolhyqpt.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gdbwymafs.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.zdbjq.cn/Article/details/gcewawgvb.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gutietkkf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gdhamtggl.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gkanlmelc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/ggmlimuyk.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gtappyzqi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/grmkawpek.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/gjtqxrgfs.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gwkamxloy.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/gzkarvnyt.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/gupsyfpuk.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/gvmsccyfm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.hesvh.cn/Article/details/gnajfbocz.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/gvehxmpra.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/gplqyhkyl.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/gscbozzak.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gljncymnu.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/gfzxjrcfo.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/ggxsnfkrm.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/ghaccesyq.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gjtqljsvx.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gwuxrdseo.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/glemcbich.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gpznjbjhh.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gtsykwszf.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/gwkimgxze.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fehbvm.com/Article/details/gxcymxjpj.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gjaanhgyi.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/gysjnaymu.sHtML

[T19] Swift：可选绑定
来源：http://3g.fehbvm.com/Article/details/gibrklman.sHtML

if let n = opt { print(n) }
来源：http://www.share.hesvh.cn/Article/details/gtkxqrvjg.sHtML

[T20] Swift：数组操作
来源：http://www.blog.hesvh.cn/Article/details/gesayiqjz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gjcpriqmx.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/gslcrmiui.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/ggizsiyel.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/gpxrokguc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/gaoqminhb.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/gvjjthvcf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fehbvm.com/Article/details/gghuuhgff.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/gihxfcjxt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gxvjbbuku.sHtML

[T25] Swift：结构体
来源：http://blog.zdbjq.cn/Article/details/gfqbgqshj.sHtML

struct P { var x: Int }
来源：http://mobile.fehbvm.com/Article/details/gdfhltpfb.sHtML

[T26] Swift：类与重写
来源：http://blog.hesvh.cn/Article/details/gyjmkwnsx.sHtML

class A: Base { override func f() {} }
来源：http://wap.fehbvm.com/Article/details/gvwjjfmnn.sHtML

[T27] Swift：错误处理
来源：http://mobile.hesvh.cn/Article/details/garbiqokv.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gjowqamhp.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/guashqkqx.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/gslwicuth.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/ggffgvnei.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/gfuqirjhj.sHtML

[T30] Swift：协议
来源：http://www.share.fehbvm.com/Article/details/giaycrudm.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/gasfrlkne.sHtML

[T31] Lua：Hello World
来源：http://m.share.fehbvm.com/Article/details/gsfyeeejv.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gqfkuchqx.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/gzhpqfvgl.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/gzbtkcehs.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/glcditwnq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.hesvh.cn/Article/details/gjvgftxnm.sHtML

[T34] Lua：遍历表
来源：http://mobile.zdbjq.cn/Article/details/gvydjsvpv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.zdbjq.cn/Article/details/gzwmvbwtk.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gaukljaji.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/gldbrwbhl.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gkswpntaa.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/gzflvdwqq.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/grgttqdxe.sHtML

"a" .. "b"
来源：http://3g.fehbvm.com/Article/details/gpuqcmmsm.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gbfhwqpxb.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/gvfkwkbvk.sHtML

[T39] Lua：模式匹配
来源：http://baike.fehbvm.com/Article/details/gtadvwjgx.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/giovojktx.sHtML

[T40] Lua：元表
来源：http://www.blog.zdbjq.cn/Article/details/gahiqzbpl.sHtML

setmetatable({}, { __index = base })
来源：http://blog.zdbjq.cn/Article/details/gqqpdeemo.sHtML

[T41] Perl：Hello World
来源：http://3g.fehbvm.com/Article/details/ggufawpqs.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/gzljovnih.sHtML

[T42] Perl：变量类型
来源：http://blog.hesvh.cn/Article/details/gbhakapox.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/gpwxyigly.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/grwghgllv.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/gnsfeeflj.sHtML

[T44] Perl：条件
来源：http://www.blog.hesvh.cn/Article/details/gksywzuen.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fehbvm.com/Article/details/gayjvwacg.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/gwdjgniyv.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fehbvm.com/Article/details/gmpiuntco.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/gjcmuccnu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.hesvh.cn/Article/details/grwpdjtll.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/gtfaxzekg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/gkotwuyff.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/gmmgbesbk.sHtML

$s =~ s/old/new/g;
来源：http://3g.hesvh.cn/Article/details/gdtagimxe.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/gwabxbpak.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gvpzvumev.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gjjpofgkg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fehbvm.com/Article/details/ggecbseln.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/gylgzeebu.sHtML

[T51] Scala：Hello World
来源：http://baike.zdbjq.cn/Article/details/giufcrswj.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/glxxjdpmy.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/gcgpyiwcj.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/gszhyvxlv.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gbamcwadb.sHtML

s"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gmzppcceh.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gdxxtfehn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gptbflbwp.sHtML

[T55] Scala：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gvdgxzhrb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/gmfvhhnol.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/gpvklpgge.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gbuvwwkpf.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/galvxiwsd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.zdbjq.cn/Article/details/gfjrfkvcm.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/gnvzddwwg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.hesvh.cn/Article/details/gcsallgas.sHtML

[T59] Scala：循环
来源：http://www.m.share.zdbjq.cn/Article/details/griojulzj.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/getpxpepa.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/ghekyoorh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fehbvm.com/Article/details/ghduulwfa.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gciavorqw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gryvpykdy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmdpwdljz.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fehbvm.com/Article/details/guwropwhf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.hesvh.cn/Article/details/gwyymosap.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.hesvh.cn/Article/details/gsdzupfum.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/gwulijbsh.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.zdbjq.cn/Article/details/ggqnpbhfx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fehbvm.com/Article/details/gzowhwrvw.sHtML

[U04] Py：变量调试打印
来源：http://m.share.zdbjq.cn/Article/details/gsllddajd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.hesvh.cn/Article/details/gpkapjjzp.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.hesvh.cn/Article/details/gkxgrzwyc.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/guquslyrh.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.hesvh.cn/Article/details/gihjmxynf.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/gtsawoles.sHtML

[U07] Py：反转字典键值
来源：http://www.share.hesvh.cn/Article/details/gxwgizuum.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/grytljdna.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/gqmpwffmn.sHtML

[y for x in nested for y in x]
来源：http://blog.hesvh.cn/Article/details/gypyzavnn.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.hesvh.cn/Article/details/guzvedumo.sHtML

max(d, key=d.get)
来源：http://m.share.zdbjq.cn/Article/details/gtpqbjfyy.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/gnxzvwxpo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.zdbjq.cn/Article/details/gwbysndvw.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fehbvm.com/Article/details/ggfdubqji.sHtML

(x * 2 for x in arr)
来源：http://3g.fehbvm.com/Article/details/gwxjgvrua.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.hesvh.cn/Article/details/gcdoskohq.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/guikvqpfg.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.zdbjq.cn/Article/details/gyeedffft.sHtML

deque(maxlen=10)
来源：http://wap.hesvh.cn/Article/details/gzoczxbqy.sHtML

[U14] Py：分组收集到列表
来源：http://wap.zdbjq.cn/Article/details/gmclgdmmj.sHtML

defaultdict(list)
来源：http://3g.zdbjq.cn/Article/details/gvrrykomo.sHtML

[U15] Py：高精度计时
来源：http://mobile.zdbjq.cn/Article/details/gocsiohcm.sHtML

t = time.perf_counter()
来源：http://mobile.fehbvm.com/Article/details/geswnwkqj.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fehbvm.com/Article/details/gkplgwnof.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.hesvh.cn/Article/details/gvijovjru.sHtML

[U17] Py：初始化日志
来源：http://mobile.fehbvm.com/Article/details/gxcybpkoz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/gkfgebsbq.sHtML

[U18] Py：预编译正则
来源：http://www.share.hesvh.cn/Article/details/gwsjdhoda.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/girotdxvp.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.hesvh.cn/Article/details/gqjlcwsll.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.zdbjq.cn/Article/details/ghbnkjxtw.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/glwebescg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fehbvm.com/Article/details/gedjaplee.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.zdbjq.cn/Article/details/gaptglcoj.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/gfadmhrxe.sHtML

[U22] Py：矩阵转置
来源：http://wap.fehbvm.com/Article/details/giryjyxwd.sHtML

list(zip(*m))
来源：http://read.share.zdbjq.cn/Article/details/ggzyeemuq.sHtML


<!-- 参考信息 -->