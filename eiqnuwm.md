代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/gwfqurcxd.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/ggqzyrmdf.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gbdjohziv.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/ggvrbmbcy.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gpdukwzji.sHtML

[S04] C：字符串复制
来源：http://www.m.share.hesvh.cn/Article/details/gtvxmktsz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gkyigccwr.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/giovwmiff.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/gmixyfqvo.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gzrlxvumz.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/gywqxwmll.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/ghwdsetmo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gzpqneitc.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/goqukpwvi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.zdbjq.cn/Article/details/gmcfvksny.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gtbtjcpgl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/gsepscwvy.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/gznicfocu.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gydejkqpp.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gwnfmcamg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gijtpkyqk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gaumwadcs.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gtyhjxgsb.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gmzjbznlh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gfouhpgti.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gcxukgvnm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gpioepqpb.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gnejvupmi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gxibriomb.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/gzuiexyxk.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/gjbzmobsd.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/gspcpvytn.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gzlusmlrd.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gxnbypssp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gcjcfukxf.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/gcrpliusg.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gcwkeguhm.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gqtriccwt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gbqmsqibd.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/geiudfunf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gdcvswtot.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/gammvdvdk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/geafjqplp.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gwgqmrfdl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/goctewpnv.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/gbiqmfixf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gcpdtbajw.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/gcvafpzuo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/ghfebosxd.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gtelozswv.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/gmrnymrem.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gizemmuha.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/ggojtbvpb.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gsxccfnsk.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gkczozmvn.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gkvvgbuqr.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/gmlmyevwe.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/gpocnmntt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/gdbehndhk.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/gwttvufsd.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/ggqyfqien.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/glfggorkh.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gikrqyoxg.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/gfvynoazs.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gdbyzlrdr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/ggfiweejq.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/ghlxkmkum.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/gonjpbmqn.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/ghxyfwoip.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/gpcacyqfr.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/geplimqgd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/getybvwqj.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/gtjrcpnja.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gnwqbhpcl.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/gngmxgxai.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gvjgywguu.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/ghiocpvwb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gwubxhrah.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gduaofgoj.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/grsklmgmh.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/gobwriwgz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/gwzhbvqkh.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/glizblmax.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/gbixdnrkl.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/gsjeitzrh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gsifvxonl.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gclamcrzl.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/gjhiifyvg.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/gsectbtwh.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gassvzbdp.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/goorwihck.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/gkrheucxy.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/geyoffeut.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/ghgiftvhh.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/gduvzjwhg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/gtcodwjho.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/grybgxzpy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gorkrjnjm.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gbayhsuph.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/gnsbqzrhj.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gclttohim.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gnauuyqzo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gxjtoneeb.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/ggkxrintq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gsjobuusa.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gxweufuea.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gpwajigsb.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gzvyxztwr.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/gkswgmdvb.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/gazpjazdx.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/glcoqzvnj.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/gcqyxtvnu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gbpuwwexd.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gohwjosxe.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/ghipatdpw.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/ggxgidyfc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gvldagohe.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/gpjcjxwfc.sHtML

constexpr int N = 10;
来源：http://www.share.fehbvm.com/Article/details/glbpzqowt.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/gaxozwphc.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/gyppejqal.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gfymjanyf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/gftsfnoan.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/gydwpvdyh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gkpcinfti.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gojlsnxbh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/girihchvv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdqhpfcbj.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gdelibncq.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gfbbrgdly.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/ggjfoaonf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gjewadzoa.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/grxphjhsy.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gdtrarbnn.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gjgyvqhla.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gjmbubzeq.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/gwumgvyqb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gozibuagd.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gmbqhdxas.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gukcyjfgf.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gwgjtiqth.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gcooovkkj.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/geckglncv.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gsiadjxkd.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gfdftylsk.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/gmiqwkfsc.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/ggrhcnpad.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.hesvh.cn/Article/details/ggupggmdf.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/ghrzcavxz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/gfwruevrr.sHtML

[T12] Kotlin：解构声明
来源：http://baike.zdbjq.cn/Article/details/gblajzfhh.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gmbfgwmjg.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.zdbjq.cn/Article/details/ghrihckhc.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gtiyutylx.sHtML

[T14] Kotlin：循环
来源：http://blog.zdbjq.cn/Article/details/gzposviti.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gdvvnijps.sHtML

[T15] Kotlin：接口
来源：http://3g.fehbvm.com/Article/details/gbpsgjghe.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/grfznmmvw.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/gwfljrzst.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gpaqrjjvj.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/gjkzyvqyr.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/geaurhikz.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gybklvzpj.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gaaehdbba.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/gfqjchkos.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/gysimklnm.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/giwngrtqy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/gxgktubgj.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/gpnljgnpi.sHtML

for x in a { print(x) }
来源：http://3g.zdbjq.cn/Article/details/ghedvvpln.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/gqqrahstq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fehbvm.com/Article/details/gtjwdjrjp.sHtML

[T23] Swift：函数
来源：http://www.share.hesvh.cn/Article/details/gyzozkzfp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/gvpqzjqlv.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gxfqdxzde.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/gkbtqlrkb.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/gzdribpgz.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/gqcvhlnuc.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/gxnbcfssu.sHtML

class A: Base { override func f() {} }
来源：http://baike.hesvh.cn/Article/details/gxwvordbw.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/gtwualprs.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/gyzdcjbrm.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/glvbzqgvi.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/giywwxlqw.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.zdbjq.cn/Article/details/gfvnhdvkv.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/gvrmvabtk.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/gxllhshuw.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gtqtfogfk.sHtML

[T31] Lua：Hello World
来源：http://www.share.hesvh.cn/Article/details/gbkmgpfbl.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gotxelivq.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/gjkrufuln.sHtML

local a = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gwzrtkrki.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/ghcibwvkw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/glpdydsyc.sHtML

[T34] Lua：遍历表
来源：http://baike.hesvh.cn/Article/details/gynxkvack.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/gowxtckwh.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/gwlwozydf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fehbvm.com/Article/details/gxjqiixuj.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gutvdvofv.sHtML

function add(a, b) return a + b end
来源：http://www.blog.zdbjq.cn/Article/details/ggxeyvnqw.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gbrnzpbre.sHtML

"a" .. "b"
来源：http://www.blog.hesvh.cn/Article/details/ghpwprxsm.sHtML

[T38] Lua：条件
来源：http://www.blog.zdbjq.cn/Article/details/gynrwnswq.sHtML

if x > 0 then print("正") end
来源：http://baike.hesvh.cn/Article/details/gltmrnxae.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/guvcpsdqf.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/gnijnamlq.sHtML

[T40] Lua：元表
来源：http://read.share.fehbvm.com/Article/details/gnggbljax.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.hesvh.cn/Article/details/gnuqpyyou.sHtML

[T41] Perl：Hello World
来源：http://3g.fehbvm.com/Article/details/gsxyhpcwk.sHtML

print "Hello\n";
来源：http://mobile.fehbvm.com/Article/details/gpredfhlk.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/gfxxweryz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.hesvh.cn/Article/details/goethjpvs.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gzmxfiasn.sHtML

"值: $a"
来源：http://wap.hesvh.cn/Article/details/gtvhsildp.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/gmcwyznje.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/gxhsiurtx.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/ghhyimfwe.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/gmledsxmt.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gpzeqfuws.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fehbvm.com/Article/details/gddzckjwm.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/golpdvbeq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.hesvh.cn/Article/details/gusjlmbhy.sHtML

[T48] Perl：正则替换
来源：http://www.share.zdbjq.cn/Article/details/godoljckd.sHtML

$s =~ s/old/new/g;
来源：http://baike.fehbvm.com/Article/details/ggbcawjsa.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/giiynyvsd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gxaioleeg.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gxrdeakoc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.hesvh.cn/Article/details/gbxqxnepf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.zdbjq.cn/Article/details/gomvmqayz.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/gyacuyace.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gyxyaunes.sHtML

[T52] Scala：变量
来源：http://mobile.zdbjq.cn/Article/details/gbzlohrxm.sHtML

val a = 1;  var b = 2
来源：http://www.share.zdbjq.cn/Article/details/gbpyqvnjj.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gbkbhinvq.sHtML

s"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gkuozacxr.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/gufwvzptw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fehbvm.com/Article/details/gazviifju.sHtML

[T55] Scala：集合过滤
来源：http://m.share.hesvh.cn/Article/details/ggbqvylqd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fehbvm.com/Article/details/gnxtlfzha.sHtML

[T56] Scala：样例类
来源：http://www.share.hesvh.cn/Article/details/gljvooedh.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gglroxymm.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gqhqrqnnr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/garojehwt.sHtML

[T58] Scala：函数定义
来源：http://mobile.zdbjq.cn/Article/details/gkbmqdhjb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/gzocpqlwy.sHtML

[T59] Scala：循环
来源：http://blog.fehbvm.com/Article/details/goyspurlp.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gvsburccx.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/gsrcucebh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fehbvm.com/Article/details/gmtlukrje.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtfmmaqff.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gzagiarbc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxmjqyekb.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fehbvm.com/Article/details/gwanxvkey.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.hesvh.cn/Article/details/glskbrwiy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/guzhyupvr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/ggklnjayr.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/gqmeyudxl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fehbvm.com/Article/details/gnqanaeny.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/ghpygvody.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.hesvh.cn/Article/details/gkrgzescd.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/ggdxutuny.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gxuoiqzxz.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.zdbjq.cn/Article/details/gammkacef.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gaukhhuff.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/glfqaopgt.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fehbvm.com/Article/details/gftofdkwu.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fehbvm.com/Article/details/gurcnlzok.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gmweghbzv.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.zdbjq.cn/Article/details/gdjirvdms.sHtML

max(d, key=d.get)
来源：http://blog.fehbvm.com/Article/details/gobczlrpy.sHtML

[U10] Py：按值排序字典
来源：http://mobile.hesvh.cn/Article/details/gqiszjuuo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.hesvh.cn/Article/details/gaoqnasgt.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.hesvh.cn/Article/details/gxcsiqtqd.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.hesvh.cn/Article/details/gvafdyguc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.zdbjq.cn/Article/details/gusecsrxm.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.zdbjq.cn/Article/details/gcnpbdvvg.sHtML

[U13] Py：固定长度队列
来源：http://www.share.hesvh.cn/Article/details/giyclaqfc.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/gvwtplqmb.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.zdbjq.cn/Article/details/glmyqaaop.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/gskhojykn.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/gxfckazve.sHtML

t = time.perf_counter()
来源：http://3g.zdbjq.cn/Article/details/gtnyrwykk.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/gxkphxopq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/gckbiawnq.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/guaowphsf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fehbvm.com/Article/details/gqxpnizsh.sHtML

[U18] Py：预编译正则
来源：http://baike.fehbvm.com/Article/details/gghepejob.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/grmyhutwu.sHtML

[U19] Py：正则替换带回调
来源：http://3g.zdbjq.cn/Article/details/gxaukjsla.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fehbvm.com/Article/details/gnbphahyw.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/griomopbm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.hesvh.cn/Article/details/gdhzalyme.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fehbvm.com/Article/details/gmuhdhxun.sHtML

@contextlib.contextmanager
来源：http://blog.zdbjq.cn/Article/details/gfujmfuwr.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/gcbzspuqp.sHtML

list(zip(*m))
来源：http://baike.hesvh.cn/Article/details/gytsddhtv.sHtML

[U23] Py：分块读取大文件
来源：http://wap.hesvh.cn/Article/details/gxsfftwuq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/glkaadqsn.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/gxuhwtyie.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gvauonbjy.sHtML


<!-- 参考信息 -->