代发 wailian999

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/giwvxxepq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbwcpwfpe.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gkjgsthev.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/gousquinj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/giqrtqmoq.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/gnfxieobl.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/gjuvtcezo.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gnrjzffum.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/gygwhkjmq.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gbjuamfad.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gzqgodvyw.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/ggukshezb.sHtML

strlen(s)
来源：http://www.blog.zdbjq.cn/Article/details/gviuitenl.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gumoayzem.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/gxbiazrwt.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/giuxehizm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.zdbjq.cn/Article/details/gzjotztlc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/goxhoxexe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/gvsrorskl.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/gtgunwnwb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gcypvzuuq.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/griqgpiap.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gshbcgmax.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/guiqrwfaw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/ggrblfutm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/gkjoijkwf.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/gmvdhungh.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/goxcxtafw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/gmxwtecme.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/grruzmgqz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gngvyglzp.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/grkvtpxox.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gpfkhauys.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/grquhmvqh.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gycogivop.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/gavqtugxf.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gjboftpyc.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gzkipftuk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gqqixrijd.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gviclltbx.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/gtqzidvkz.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/gcfaqueiy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gaohbksww.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/gtwjrneem.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gypydnbpd.sHtML

[S21] C：字符类别判断
来源：http://www.blog.hesvh.cn/Article/details/gxjhjcyyw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gsxbrigmk.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/goamwktwz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/gfetijmds.sHtML

[S23] C：随机数
来源：http://mobile.fehbvm.com/Article/details/gkyrnseje.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.zdbjq.cn/Article/details/gtwrlnwxc.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gonedioxq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gilzvifvc.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gyavfwczw.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gohewgvxb.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gaprbihbn.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gkcvytyzl.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/glcgsgjtr.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gjbefpxqv.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gqocrglix.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gftsaljop.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gqjzokehs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gadonffvc.sHtML

[S30] C：头文件保护
来源：http://blog.zdbjq.cn/Article/details/gptwvqbex.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gjfbvnjaf.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gqdeqakma.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/geovgdxyb.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gmmmrrxvf.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/gtwpxtkgq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.hesvh.cn/Article/details/gaqmwedxe.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gqwglkhix.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gnrueqbvz.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/glfioovxh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/gofcictcw.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/gxsemtftv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gppnzvozi.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gklfplcfp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gquuuytbi.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gkthpjeae.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gxmaxyqds.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gnuojcxms.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/glkuagerf.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gvvwmimou.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gaufsvxid.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/ggxboogny.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gkuldsqub.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gacqcrijz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gdzlymvay.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/giwxkqmcb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gpzoweann.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/gbtvuwimu.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/gwbfpwiul.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gtwmjfbyk.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gbpebzxhj.sHtML

[S44] C++：引用传参
来源：http://mobile.hesvh.cn/Article/details/gzvtsdttp.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/gxrgolxys.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/gfqdhgezt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/gixhpdczz.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/ghuefcnnv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gqgutzqsy.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gyotithpx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/gbxpyyvpg.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gljljvuey.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/gudeprlon.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/glursjhiv.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gstyukwsa.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gzqjnrpxl.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/gajspbdsf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gsrjhoklm.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gtdpyxywg.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gixpkwigw.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gzagxhmsz.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gftegcwse.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/ghitkybmc.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gedtejdna.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/geyertyet.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gbgvdmbdh.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/ghmsbadln.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/gxsgaaonp.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/gsuavnymr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/gosravmty.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/gnbtsadke.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/gjpbgccpx.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/ghxuwyxyd.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/ggewbktuw.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/gbttofhuf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/geyfnbhed.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gzvqubuhq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/goqkdtqwd.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gujttsknf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gijzkcaoq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqzpeeqee.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gmohhmhmj.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/ghpthnfht.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gblryzvsr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.zdbjq.cn/Article/details/giozqyvsm.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gsvnwmxwb.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/glymqjjph.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gjwmctmha.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/gapfhtfzv.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/ggglxsssz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/grpwhkftk.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/gakhalgoa.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/gpjyhxypr.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/grnvnyqku.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/gqdcckvww.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/gzagadocc.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/gdyckwwdl.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/gfsxmkhkc.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gsrxhwrmj.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/ghzigmhjl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/gelesjnlm.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gvsbvuyqq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fehbvm.com/Article/details/gyprzfwad.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/gdibigvhe.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fehbvm.com/Article/details/gkfgmeggo.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.hesvh.cn/Article/details/gucguchos.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/gdswmecfj.sHtML

[T14] Kotlin：循环
来源：http://www.share.hesvh.cn/Article/details/gooizuuac.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gmtmzjyta.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/gjaoafypa.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/ggfxywfiz.sHtML

[T16] Swift：Hello World
来源：http://wap.fehbvm.com/Article/details/geedtnobm.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gmzrxntmz.sHtML

[T17] Swift：变量与常量
来源：http://read.share.zdbjq.cn/Article/details/gfqpepcsq.sHtML

var a = 1;  let b = 2
来源：http://3g.hesvh.cn/Article/details/ggugeiubp.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gdstxqtyv.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gxxyuvtnw.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/gbstkjwra.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/gwmshqlpa.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/gnpabtief.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fehbvm.com/Article/details/gxcnehlsl.sHtML

[T21] Swift：遍历
来源：http://mobile.fehbvm.com/Article/details/gkqkojdno.sHtML

for x in a { print(x) }
来源：http://m.share.fehbvm.com/Article/details/gvdmxyidi.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/ggpxuqyso.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.zdbjq.cn/Article/details/gylezvstt.sHtML

[T23] Swift：函数
来源：http://baike.zdbjq.cn/Article/details/ghuuqhsle.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gswqbasim.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/gtxeyiarr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gscczubgw.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/gutjueesl.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/gabibcaaz.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/gdfpnmukq.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/goqhufjdf.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/gsuwfavqq.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.hesvh.cn/Article/details/gxoevhsid.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/goapowaxu.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/gvwsxndza.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gogkigced.sHtML

guard let x = opt else { return }
来源：http://www.share.zdbjq.cn/Article/details/gttortamd.sHtML

[T30] Swift：协议
来源：http://3g.hesvh.cn/Article/details/guuzdytbi.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/guvocexjl.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/gblvqkdhc.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gsahxbhms.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/gvemqexmg.sHtML

local a = 1
来源：http://3g.fehbvm.com/Article/details/gqmsjcbtj.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fehbvm.com/Article/details/gxhubkrfx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.hesvh.cn/Article/details/grwuyfnbt.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/gosnltijr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/gzlpqwsos.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/glxywtvwc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.zdbjq.cn/Article/details/gmsngysag.sHtML

[T36] Lua：函数
来源：http://www.share.fehbvm.com/Article/details/gzvvvyzcv.sHtML

function add(a, b) return a + b end
来源：http://mobile.fehbvm.com/Article/details/gplizyerb.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gujzpxoco.sHtML

"a" .. "b"
来源：http://wap.fehbvm.com/Article/details/gsalrbqld.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/gsptznqjx.sHtML

if x > 0 then print("正") end
来源：http://mobile.zdbjq.cn/Article/details/gzmugforu.sHtML

[T39] Lua：模式匹配
来源：http://baike.hesvh.cn/Article/details/gdlrazsvc.sHtML

string.find(s, "%d+")
来源：http://mobile.fehbvm.com/Article/details/gibkhtubl.sHtML

[T40] Lua：元表
来源：http://wap.hesvh.cn/Article/details/gxqxxiocq.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/grupiperh.sHtML

[T41] Perl：Hello World
来源：http://baike.fehbvm.com/Article/details/gprokkqtt.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/ghwxijiee.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/glfczuaae.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.hesvh.cn/Article/details/gjgsizlbx.sHtML

[T43] Perl：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gofwuxvno.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/gqfdttdwr.sHtML

[T44] Perl：条件
来源：http://mobile.zdbjq.cn/Article/details/gjlukffws.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.hesvh.cn/Article/details/guwswgbdr.sHtML

[T45] Perl：数组遍历
来源：http://3g.hesvh.cn/Article/details/gvydmrzrv.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gsclhcdtk.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/gtnrnuora.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/gzjqxrcaz.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/gjnazqobe.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.zdbjq.cn/Article/details/glolsqmai.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/gjemrzqdv.sHtML

$s =~ s/old/new/g;
来源：http://3g.hesvh.cn/Article/details/gmurfsbtu.sHtML

[T49] Perl：函数
来源：http://www.m.share.hesvh.cn/Article/details/gxiotwdgf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gqdopocis.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gdqptxdbj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fehbvm.com/Article/details/gahfegzln.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fehbvm.com/Article/details/gjvjxczth.sHtML

[T51] Scala：Hello World
来源：http://baike.zdbjq.cn/Article/details/gnzxjgmxa.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/guvetlftq.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/gwqcryjfc.sHtML

val a = 1;  var b = 2
来源：http://blog.zdbjq.cn/Article/details/gbbeaqbcp.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gzmipdqfg.sHtML

s"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gweywevlu.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/gqjlamaup.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/godnjjtkg.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gbvphsjky.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fehbvm.com/Article/details/gnwzqzcmr.sHtML

[T56] Scala：样例类
来源：http://baike.hesvh.cn/Article/details/grwhqhlbp.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/gfwjpifrz.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gudeexhwh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fehbvm.com/Article/details/grxuqiram.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/gbrigcayu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/gcuwtsglv.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/gghpxwlwu.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gxcgxbxuc.sHtML

[T60] Scala：折叠
来源：http://www.blog.zdbjq.cn/Article/details/ghruwmhed.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/glnwriiln.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grvzuqeiu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/gpodtaczt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glvstihbx.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/gkdtumeok.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.hesvh.cn/Article/details/gbvbpjbre.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.hesvh.cn/Article/details/ghvhueplw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.zdbjq.cn/Article/details/gndmnkmjv.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/gsgtlfjyh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/gnslaiddy.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gpeihwqdq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/gnljumjww.sHtML

[U05] Py：列表去重且保序
来源：http://baike.zdbjq.cn/Article/details/gbmmzbaca.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/ggeekyyht.sHtML

[U06] Py：合并两个字典
来源：http://baike.zdbjq.cn/Article/details/grgjgwndb.sHtML

{**a, **b}
来源：http://www.m.share.fehbvm.com/Article/details/gqqfyzpye.sHtML

[U07] Py：反转字典键值
来源：http://www.share.hesvh.cn/Article/details/gujcxibxs.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fehbvm.com/Article/details/gqjfxszyj.sHtML

[U08] Py：展平二维列表
来源：http://blog.fehbvm.com/Article/details/gezwfyfgv.sHtML

[y for x in nested for y in x]
来源：http://wap.hesvh.cn/Article/details/gqzxdesrc.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.hesvh.cn/Article/details/guuinqyqp.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gaqbdbesq.sHtML

[U10] Py：按值排序字典
来源：http://wap.fehbvm.com/Article/details/ghyttnhfo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fehbvm.com/Article/details/gjgfpqhly.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/gzqnmtvdv.sHtML

(x * 2 for x in arr)
来源：http://3g.hesvh.cn/Article/details/gubyeobhw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.hesvh.cn/Article/details/gtrwcnjdu.sHtML

Counter(arr).most_common(3)
来源：http://blog.fehbvm.com/Article/details/giuezcnrr.sHtML

[U13] Py：固定长度队列
来源：http://blog.hesvh.cn/Article/details/gtjtavwwe.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/gzinhbvcs.sHtML

[U14] Py：分组收集到列表
来源：http://baike.zdbjq.cn/Article/details/gksoxfxax.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/gxvcnueyn.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/gjwufbbxb.sHtML

t = time.perf_counter()
来源：http://www.share.zdbjq.cn/Article/details/grmhlmpvm.sHtML

[U16] Py：命令行参数解析
来源：http://baike.zdbjq.cn/Article/details/geoqomspo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/goyymfxfa.sHtML

[U17] Py：初始化日志
来源：http://m.share.fehbvm.com/Article/details/gqlhghjxn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/gikybbrzp.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/grdkyxihj.sHtML

pat = re.compile(r"\d+")
来源：http://blog.hesvh.cn/Article/details/gitmokrmt.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/ganbncreh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/gtnrmgxki.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.hesvh.cn/Article/details/gwzdhrcgp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.zdbjq.cn/Article/details/gcagbgknd.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.hesvh.cn/Article/details/gxdxrlpki.sHtML

@contextlib.contextmanager
来源：http://wap.fehbvm.com/Article/details/gsytzajht.sHtML

[U22] Py：矩阵转置
来源：http://www.share.hesvh.cn/Article/details/gpxluzpml.sHtML

list(zip(*m))
来源：http://m.share.fehbvm.com/Article/details/gieeiggxi.sHtML


<!-- 参考信息 -->