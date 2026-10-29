代发 wailian999

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gkcdrvmpr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqpoaqgqh.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gcnteitmo.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/gojlcawaw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gfscawhnj.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/ghaknovxy.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gkpissxum.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/gjletclbv.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/guvknnxvy.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/giljnnkea.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gkdriudgs.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gjpuktsou.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gjnpcepea.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gjuwumptu.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/ghvzvtwcw.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/gjbzjgqtu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gmounfwfz.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/grzlzbflv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gvfkxioon.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/govlhsxne.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gmezqzkft.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/gwvimuhdh.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gwsepkbln.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gbbzvchfl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/ggxctsgaa.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fehbvm.com/Article/details/gsyvitgqh.sHtML

fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/giuzumvzl.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/ggenfkirn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gqphuexcx.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gilishsyw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/ghrffscoq.sHtML

[S14] C：枚举
来源：http://3g.fehbvm.com/Article/details/gptkltcpi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gbsghheys.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/gruqydvjg.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/glcsivvik.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gcmbbrxus.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gzjavxiso.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gysltflfw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/ghnbkdimw.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gwjoztekp.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/ggfrokbeq.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gcmlfdoni.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gkqezjtxs.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/glvprowlo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gwgzkxhdm.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gbngagrzb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/gqzwiyvyx.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gilxmqbia.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/gexliswgi.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gonjpmgog.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gjguudxyn.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/ggvbpnbmk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/grrereueh.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gayveinsh.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/gvqcdzjkv.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/ggmwkuvlc.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gvbpcmiab.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gwwhycpjq.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/grzzqhgjd.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gkmwhcixh.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gubcrvbah.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/gvceprisr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/gfbqjjatn.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/geqmicazk.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gqfmxlgsl.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/gryaxrfeq.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gliblnatf.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gwrurhvei.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gutbyejdc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/grfrqsqpq.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gvmofygfg.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/glxtmdhri.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/gbyllbrmk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gighvbvmv.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gswzztlxf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.zdbjq.cn/Article/details/gzunhnbwz.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/ggpbkzspj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gmgwlclez.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gkeknepzl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gapnvcrnp.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/glqiulwau.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/gnkmtlmay.sHtML

[S38] C++：排序
来源：http://www.blog.zdbjq.cn/Article/details/gyrqeiyhe.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gvojfmynr.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/gszprgjly.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.zdbjq.cn/Article/details/gaklyprwz.sHtML

[S40] C++：查找元素
来源：http://m.share.zdbjq.cn/Article/details/gzgvprurh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/ghehzjlvj.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gxfvwsmfz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/ghpywqlok.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/gjpqsyhfg.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/gqfnblfka.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gsgkbqlkw.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/gzunntxqb.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gtyenmadm.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/gqignjlqf.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gqoqkxpmg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/gytiscbxi.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/gbofbadrx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gekjolcvl.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gnnqecfqk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.zdbjq.cn/Article/details/gdvqmmtmq.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gpzemtpam.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/gnkkiauhj.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gcgwouqhf.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/ggrhchylz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gsmxpvfna.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/gdllqgkot.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.hesvh.cn/Article/details/gmihhznzl.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gcqugaxbz.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/grdapdqbj.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gcnfvvvxx.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/grepobrzb.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/gkvpzkzqk.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gvvoqijvl.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gtkzxtsuy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gmqscecef.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fehbvm.com/Article/details/gkiqhjjdv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/glfbawkvm.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/ggevzljrk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/gbevucsua.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/gkrovcdxb.sHtML

constexpr int N = 10;
来源：http://www.share.fehbvm.com/Article/details/gwacrentx.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/ghftcqehj.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/gxgjzudzh.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/gepmrrxow.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gybmfdpsg.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gmpuvxiyo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/gfhtnfehz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjobhmgob.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/graqpjoqj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxpjzlvbu.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/gtgcjimpg.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gvwqjodaf.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gaaxlhyti.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/gmgncelzi.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gzluwfxcv.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/gjmkjxnfl.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gipurxybd.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gbglxlmmm.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gmqsawjxr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gjiwgzwvl.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gquwuwbok.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/gsdeorgno.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gxzresjxa.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/gqnitgcov.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/gcsolcxhd.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/ggvpenscq.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/gcrkmzghq.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gtoppdllg.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gercukqfw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.hesvh.cn/Article/details/ghdovbpkn.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/gsoshmeay.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fehbvm.com/Article/details/gttuegmhi.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/gjrvdzjkp.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gkjktujwu.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/gxhmgimgf.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gqnljwhzl.sHtML

[T14] Kotlin：循环
来源：http://blog.hesvh.cn/Article/details/gxcxiipqc.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gjmlpoeov.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/gecqchmyi.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gzykzfcrt.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gjklykhii.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gxshoeuck.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/gjngcwsnm.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/gwrklvwys.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gppdrwkqv.sHtML

"值: \(b)"
来源：http://baike.hesvh.cn/Article/details/gimqgltdt.sHtML

[T19] Swift：可选绑定
来源：http://3g.fehbvm.com/Article/details/gdmjevsrq.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gvhjkazkh.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/glynlqoge.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/ghhbsgfuo.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/glxpcrmmo.sHtML

for x in a { print(x) }
来源：http://m.share.zdbjq.cn/Article/details/gwadpoccf.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/gnlpkbluw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/gpnbupsop.sHtML

[T23] Swift：函数
来源：http://www.blog.hesvh.cn/Article/details/gibmvqotl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/gsiylxxxy.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/gzmwoxhgo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gezogsumr.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/gksqzqabp.sHtML

struct P { var x: Int }
来源：http://mobile.hesvh.cn/Article/details/gfmgkjbph.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/gvkhsxpou.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gjscrnzzi.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gvtozcjkl.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/gzdbeusiu.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gtedkpobv.sHtML

enum Color { case red, green }
来源：http://www.m.share.hesvh.cn/Article/details/groziwidy.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/gsprtjcsk.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/gnymcwdij.sHtML

[T30] Swift：协议
来源：http://blog.zdbjq.cn/Article/details/ghyigossb.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fehbvm.com/Article/details/gchdedwut.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gaqkdimnz.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gmpvkevxd.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/gnwhidylc.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/gjrqrhehj.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fehbvm.com/Article/details/gcezsymfx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/gldvnigvf.sHtML

[T34] Lua：遍历表
来源：http://read.share.fehbvm.com/Article/details/gqhxjhnlh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.hesvh.cn/Article/details/gtmjplrvg.sHtML

[T35] Lua：字典表
来源：http://wap.fehbvm.com/Article/details/gylhgbfsn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gkiuqnvuw.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/gaejanuud.sHtML

function add(a, b) return a + b end
来源：http://read.share.zdbjq.cn/Article/details/gzpifhngz.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gfdilvdsq.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/ggctuflgp.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/gralpjtey.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/gntybvdfp.sHtML

[T39] Lua：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gvistzcnt.sHtML

string.find(s, "%d+")
来源：http://wap.zdbjq.cn/Article/details/gacogmotp.sHtML

[T40] Lua：元表
来源：http://www.m.share.fehbvm.com/Article/details/goutqsosq.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/gletcliqo.sHtML

[T41] Perl：Hello World
来源：http://blog.fehbvm.com/Article/details/gpycrfrwa.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/gdtilociv.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/ghunqixbn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/gnadcbpmx.sHtML

[T43] Perl：字符串插值
来源：http://wap.hesvh.cn/Article/details/ghshptrvo.sHtML

"值: $a"
来源：http://baike.fehbvm.com/Article/details/gjzenrxrr.sHtML

[T44] Perl：条件
来源：http://read.share.zdbjq.cn/Article/details/gkcbercec.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.zdbjq.cn/Article/details/gttprwale.sHtML

[T45] Perl：数组遍历
来源：http://wap.fehbvm.com/Article/details/gormfqhdk.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdfpytdck.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/gufzvivgr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gbzyhyjbe.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/gnstpuuzv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fehbvm.com/Article/details/gbmgoddem.sHtML

[T48] Perl：正则替换
来源：http://mobile.fehbvm.com/Article/details/gmvobshnx.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/ghvxmayba.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/gxmwsmacq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gdtxyibur.sHtML

[T50] Perl：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gidgxtgtp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.zdbjq.cn/Article/details/gkkulolss.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/gcjpjhgag.sHtML

[T51] Scala：Hello World
来源：http://mobile.hesvh.cn/Article/details/gygyphtvt.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gigpoddnp.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/gxwylfmdk.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/goyqeoreo.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gyblkeogu.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/gfijnbqbe.sHtML

[T54] Scala：集合映射
来源：http://baike.zdbjq.cn/Article/details/geptmemhn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/gndjrqool.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gtohnadyz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/gccuzjvqj.sHtML

[T56] Scala：样例类
来源：http://wap.hesvh.cn/Article/details/gjgxptqfj.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fehbvm.com/Article/details/gjojtearg.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/gplasxgjc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.hesvh.cn/Article/details/gmgnjnilc.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/gxengfjgr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.zdbjq.cn/Article/details/grujuztwh.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/gnciuvlzk.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/ghvksdjnv.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/gqzmeeuio.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/ggduadykv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggxjwagam.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gbynhqsoe.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjvgaxjbx.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.hesvh.cn/Article/details/ggwahomds.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gxzsznbgd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fehbvm.com/Article/details/gjmtsvnbn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.zdbjq.cn/Article/details/gyvncghrd.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/gahcmpaue.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/geizwxtmz.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gtucjhasr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.hesvh.cn/Article/details/gyrbotpwa.sHtML

[U05] Py：列表去重且保序
来源：http://wap.hesvh.cn/Article/details/gjjsbzdqu.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gwczofbfz.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/gyffutczt.sHtML

{**a, **b}
来源：http://blog.fehbvm.com/Article/details/gysryhyde.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/gwcdlsoss.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/gviofosxk.sHtML

[U08] Py：展平二维列表
来源：http://3g.zdbjq.cn/Article/details/giinkygdc.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/gnjbvlmua.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.zdbjq.cn/Article/details/gmklshdgd.sHtML

max(d, key=d.get)
来源：http://blog.fehbvm.com/Article/details/gmszalopz.sHtML

[U10] Py：按值排序字典
来源：http://mobile.zdbjq.cn/Article/details/gqcsbgsik.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fehbvm.com/Article/details/gtmyzmvmw.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.zdbjq.cn/Article/details/gczjjkgbl.sHtML

(x * 2 for x in arr)
来源：http://read.share.zdbjq.cn/Article/details/gbwziwgua.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/gcddksdsc.sHtML

Counter(arr).most_common(3)
来源：http://baike.hesvh.cn/Article/details/ggzqbaycy.sHtML

[U13] Py：固定长度队列
来源：http://blog.hesvh.cn/Article/details/gtqqsgyrr.sHtML

deque(maxlen=10)
来源：http://www.m.share.zdbjq.cn/Article/details/gaphrtkex.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.zdbjq.cn/Article/details/geyqehfon.sHtML

defaultdict(list)
来源：http://www.share.hesvh.cn/Article/details/gebbrztoy.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/gxzvdmppz.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/gmpdblzzl.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.zdbjq.cn/Article/details/gcwqsqcio.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.hesvh.cn/Article/details/getlbshwk.sHtML

[U17] Py：初始化日志
来源：http://baike.hesvh.cn/Article/details/grbncgxow.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/gxkyebzun.sHtML

[U18] Py：预编译正则
来源：http://3g.hesvh.cn/Article/details/gyjchvild.sHtML

pat = re.compile(r"\d+")
来源：http://3g.hesvh.cn/Article/details/ggbqjxzca.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.hesvh.cn/Article/details/gmjlkdprq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.hesvh.cn/Article/details/gfhcclgno.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/guntyvrwm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fehbvm.com/Article/details/ghhksxcpg.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.hesvh.cn/Article/details/grukeiyla.sHtML

@contextlib.contextmanager
来源：http://baike.zdbjq.cn/Article/details/gisdtaxhm.sHtML

[U22] Py：矩阵转置
来源：http://3g.zdbjq.cn/Article/details/gywdiredh.sHtML

list(zip(*m))
来源：http://read.share.fehbvm.com/Article/details/gszufdnvq.sHtML


<!-- 参考信息 -->