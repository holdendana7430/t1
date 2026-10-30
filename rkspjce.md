代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqgjqhxap.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwducgmp.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnizgsvak.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsznkgin.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwuopmko.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gvfcxnsyi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gczrwtjej.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcwfjwll.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gowlqiurp.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvpnnrbh.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gvkcpwope.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gigtxiftu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gkfsnymtf.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/grwztdrcq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/glhniticj.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/ggmvainnq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gfaklukuo.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gygmanuas.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/guauladxt.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/goppoilve.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gbylpqwob.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gomzjrulh.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjvklazl.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwqwlmnd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghhoqlqx.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwtrhnqe.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gadounlxv.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gpubbluvc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudfxiqxm.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqhkovum.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gylwpxzfz.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gzinzxgcv.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgxrekti.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gocxchnni.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhvbmifg.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewiqeogh.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/glbheloif.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzpfhcrr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gdwxsqhzf.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gajgvarxy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gvfjcahcn.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsbpfsfg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gicnhhubj.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/ggilhwsmg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gymewmicu.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gkkcgwohr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjraleuj.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjarvffq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gnuoepuye.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gybsjuyao.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjnypvmw.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/godqwhnrx.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gacnfhmru.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gdwgwnkgl.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpmwcqrj.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrqeiwml.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghacvmeqf.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gcrozmhtf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gvrroutuo.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/ggvxmqeus.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckzolugm.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtzxqrat.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbzqazaq.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gyqfynrqm.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgtnjywb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpvcimxw.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/guqkjaixm.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjnatsfa.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/goutjzkkn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtugzvaze.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnwteblj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfkdhbru.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnapguli.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmhuhbbm.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gxygoxczr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpemcogh.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrtbjedq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnzgvknc.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gzryvrbxd.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgxwzksx.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gohdxlrsb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmjvgbyp.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gnisweegx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxkgfbnv.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkbnooht.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gyhdvtcml.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gvelqylye.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gqwvmvecx.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gejjqxxey.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/glreqbqoa.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscwuiklv.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjnrnvcxc.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gjwbnlmgt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorpdjzxr.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtuccbup.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjnnqodmu.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gelctssja.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvddwboxo.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gbeuphddk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfacmiad.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggajjqzpo.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gjmjwmype.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnfuglsl.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gndjmfzcm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gmstlsnvn.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/grhtaihby.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gegvugcgc.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gruusxnfo.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfelpgbw.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gwordrcwc.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnetuuwco.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdvjhkoc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gdprlxhxp.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gpecrfliq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gtnrdfurt.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtoqdymhl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gysmhjqzp.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/glbgjvjkf.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gcjheiodw.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gfknmfifo.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gojfdlofd.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/ggynfzpxm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gilnoibgn.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gmiltyfke.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gbodvjdws.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/glilusjnz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gmaghcnuw.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gcbjfuztq.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvixjkmkx.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gohzbnknt.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqujuwig.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbwkzqgp.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gbrtbdtqn.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/grzverxvo.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnsgroky.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/gxgjyzcrl.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gqkuuitiw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcryhpbcc.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gpyijsfnh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gaufczwdt.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgkawepm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyoaabvw.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gyniaqptc.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gxusgsavu.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gggxuludb.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlzejfae.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpzingdr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gypseauri.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gnewdxnyq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcyjrxix.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gkppmaqmm.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpeusuqsn.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gzztsghgf.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzlzikpx.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gobekpjnm.sHtML

for (i in 1..10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gaaubqyvo.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/ggphxacrr.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlsmcoit.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/glhovtgzq.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohyhamqe.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfqtjuqc.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gdlqpbkpb.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gjepxtugr.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmarwpuj.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gctskxtwb.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gtsgzqjvx.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjztlgmd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsqaayot.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gzklkffpn.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/glqjwwujq.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/gpjeejxsg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpxhrlvx.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcbkxsgg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqntikpef.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgcssori.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/giurzzpik.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyublgxs.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrsnjjgt.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkurceuf.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/grpnrrnpi.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvgkgjjc.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fanxiaobao.xyz/Article/details/gcefwarij.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogddayli.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/giusyfcvr.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/gbttbuupk.sHtML

guard let x = opt else { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwptxfxb.sHtML

[T30] Swift：协议
来源：http://blog.fanxiaobao.xyz/Article/details/ggdyptlnl.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geotleeaq.sHtML

[T31] Lua：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjossngq.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gozxzyula.sHtML

[T32] Lua：局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfaleomk.sHtML

local a = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/guoklujyi.sHtML

[T33] Lua：表（数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gxxfcjsrg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fanxiaobao.xyz/Article/details/gawnrpzgv.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/gksuyofsh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbwqqelg.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/gofmqlgem.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gxkrbrzfh.sHtML

[T36] Lua：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gmoirkbrp.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/gwzkpydlg.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gcikumdxd.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/gkzgzergr.sHtML

[T38] Lua：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxsuuytl.sHtML

if x > 0 then print("正") end
来源：http://3g.fanxiaobao.xyz/Article/details/glzhwqlqp.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gjnezapyd.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gtaklmglt.sHtML

[T40] Lua：元表
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrtwsanm.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhxhrnds.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxrsowtz.sHtML

print "Hello\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyialyqvm.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjrpdhpi.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/grinfewpo.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnranhag.sHtML

"值: $a"
来源：http://wap.fanxiaobao.xyz/Article/details/gnmsvwici.sHtML

[T44] Perl：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gapzkjbhc.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsshqoqdw.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnasiowe.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvfmfrhca.sHtML

[T46] Perl：哈希操作
来源：http://blog.fanxiaobao.xyz/Article/details/gtrwdnmsh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjifaraem.sHtML

[T47] Perl：正则捕获
来源：http://baike.fanxiaobao.xyz/Article/details/gncwrekci.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkozovnwh.sHtML

[T48] Perl：正则替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gsntkkabn.sHtML

$s =~ s/old/new/g;
来源：http://3g.fanxiaobao.xyz/Article/details/goetgpwwx.sHtML

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfifppjv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glgpjaksf.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpfrbcvy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fanxiaobao.xyz/Article/details/giqdttuzh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyaqzorfj.sHtML

[T51] Scala：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gtukdcqaj.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbnjcjcb.sHtML

[T52] Scala：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/glveavlna.sHtML

val a = 1;  var b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gxbkbklxt.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggmfozof.sHtML

s"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydnehlnr.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzxwhmlz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gnzcacmwp.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmwpfjhl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gglcixuet.sHtML

[T56] Scala：样例类
来源：http://m.share.fanxiaobao.xyz/Article/details/grzowuxxj.sHtML

case class User(name: String, age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gxsupnqeb.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpqpxmzc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/gszqxvdjj.sHtML

[T58] Scala：函数定义
来源：http://wap.fanxiaobao.xyz/Article/details/gkakzzang.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fanxiaobao.xyz/Article/details/guhsatcgp.sHtML

[T59] Scala：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gxiugsjiz.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebpzaufh.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlqhdozw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwmudjlq.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/grzavczgu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gvsouyhol.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gqohvcivt.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fanxiaobao.xyz/Article/details/gdemoeqfq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlxgpskr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/goseommnm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwntoudd.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gftdxyujm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fanxiaobao.xyz/Article/details/gomwsmbao.sHtML

[U04] Py：变量调试打印
来源：http://3g.fanxiaobao.xyz/Article/details/gnrgpgxqg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fanxiaobao.xyz/Article/details/gpshgwiwn.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guardamlm.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gfydwiknr.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gizgdbcmz.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxxsbhot.sHtML

[U07] Py：反转字典键值
来源：http://wap.fanxiaobao.xyz/Article/details/gpirbdlqz.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fanxiaobao.xyz/Article/details/gkuvblgzu.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gpinmlkck.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/gdyosiydo.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/gylqonumm.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvujhlynl.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayylpkqt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fanxiaobao.xyz/Article/details/gleoxvcqx.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnnlzwon.sHtML

(x * 2 for x in arr)
来源：http://baike.fanxiaobao.xyz/Article/details/giwpcpstj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fanxiaobao.xyz/Article/details/geyobgray.sHtML

Counter(arr).most_common(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gdkaflqnl.sHtML

[U13] Py：固定长度队列
来源：http://3g.fanxiaobao.xyz/Article/details/gjlrdogtb.sHtML

deque(maxlen=10)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrjcnqqk.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdeqpwce.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gzfrmszbi.sHtML

[U15] Py：高精度计时
来源：http://m.share.fanxiaobao.xyz/Article/details/gamxvvhft.sHtML

t = time.perf_counter()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwuvwsdj.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqlrtaar.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fanxiaobao.xyz/Article/details/gumcfesyh.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpymlrjm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyokjglxt.sHtML

[U18] Py：预编译正则
来源：http://blog.fanxiaobao.xyz/Article/details/goenrbmrv.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpxndrth.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fanxiaobao.xyz/Article/details/gqaqqdhuy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/gxivwdnwz.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fanxiaobao.xyz/Article/details/gkpdiqmmy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fanxiaobao.xyz/Article/details/gvvgdokih.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fanxiaobao.xyz/Article/details/gljdekdrk.sHtML

@contextlib.contextmanager
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhzyeltj.sHtML

[U22] Py：矩阵转置
来源：http://3g.fanxiaobao.xyz/Article/details/giuvlcpxl.sHtML

list(zip(*m))
来源：http://3g.fanxiaobao.xyz/Article/details/gbbjxctyh.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlyfnwjx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fanxiaobao.xyz/Article/details/glzavtcaf.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzjznrhg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjlqjamq.sHtML


<!-- 参考信息 -->