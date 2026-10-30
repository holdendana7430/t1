代发 wailian999

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gchfxcbpt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqttjtnvn.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gyndbyscv.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/gieulzits.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/gnrmyjvhm.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/ggxpptrqw.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/glmphjzaz.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gjmbhszpt.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/ghsggknqh.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gmcddupoc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gpzmrcnbr.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/gyfqcvtsp.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/glwvhmhxv.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gyufeuvdq.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/goukmeimk.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gbqwqahav.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/glylwzehu.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gxkmwyzyi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/gryqzstgv.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/gcucitmnc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/gcpplgcxn.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/gatcvewqi.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/glkapbtvb.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gbjdikjyw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/glhrxafkm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gqsyalgui.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/giqihsbus.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/guhaacvaa.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gktclyhlz.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/golzjszky.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gcftidwtq.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gpcxugspg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/guqcuefgl.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/gaumkbenb.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/grhwuuhtt.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gwyuzbltd.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/gugdiassk.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/gtyjbbddn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.zdbjq.cn/Article/details/gzcogdpcw.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/geakeauik.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gztcvgpqu.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/gqostjbuz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gwllazgvy.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/ggtakjngg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gjwfiqzva.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/gpzimtrfg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/gkfhjxbgb.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gqmoqksot.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/gspyiqttg.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gmxjxkaoe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/gdlwbcipf.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/ghnobilcr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gjwsuhzqm.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/gnfhzsjbd.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/guscxpzno.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gwxgaqgyl.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/gxkucmpko.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/ggqgffcce.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gqnpjzrna.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gffmbodaq.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gmhfiwati.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gyfxfwagg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/goqvbbgax.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/ghashktwx.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gbxxjhqqu.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gjgpvogeb.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gvglhbfpt.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gznaoqhqq.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/garikbpum.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.hesvh.cn/Article/details/gdhdmcitb.sHtML

[S32] C++：字符串
来源：http://www.share.fehbvm.com/Article/details/gpvatqbqh.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gofroypvu.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/gzzqsdlbe.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/gdfkjrfuh.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/garapneqd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gsgoezalb.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/glspbohoa.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gmiemdnpd.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gbxkomwhg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gbqelgevq.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gzdqegvjn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gywuzmaae.sHtML

[S38] C++：排序
来源：http://3g.zdbjq.cn/Article/details/goqnrhijb.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/ggdtrxfzr.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/ghvqvaikr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/gutehcezy.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gelkspolh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gclqyjiva.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gpkxmkptr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/ggpvaexhy.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/guvqufxdo.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gprrmxcdj.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/gkzvhxptw.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gwpspilak.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gceposhvu.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/gfmrqowit.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gfwpmgkza.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gyfssfdtd.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gylfnyady.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/ggdzytofj.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gvncbmkyy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gezlbjbbu.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gcrxrqgqs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gcotendme.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gdzabjhmq.sHtML

[S49] C++：写文件
来源：http://m.share.fehbvm.com/Article/details/glrjenawz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/ggfzxghbs.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gkaqpkiui.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gkqqfwcal.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/gsxpavdfx.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gosqkcjdc.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/gcfgvtrng.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gdeeuvamv.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/goyjsqclp.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/gbbhkiona.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gagstycof.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gcfoieenh.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/gloguuotr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gugsiindp.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gqncunpbd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/grwteejoi.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/gskxnyuta.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gjjzkfvqr.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gotjksinp.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.hesvh.cn/Article/details/glimylsuc.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/gxgkwchec.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/glumjlwsd.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gjamkpxur.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gduflryfc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmqlvzpjq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gplfzwwna.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdicikpou.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/gkustqsqh.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gcvzvkdef.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/gsaaqhrch.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gwjyfketn.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/glwatvljj.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gytvfadlh.sHtML

[T04] Kotlin：空安全
来源：http://m.share.hesvh.cn/Article/details/ggkprzzcx.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/gsssubbbj.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/gwxqadnal.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gfdwyiwtc.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gvouhyhhq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gxudbccek.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/glzeyoxqk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/gtdsyhwvd.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/gzgxhjdsc.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gnltsrbyj.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/gsnjhxdio.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/glkzskrui.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gijgsilxz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.zdbjq.cn/Article/details/gwayqfbrj.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/gtzbriwcp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/ggwiurrhs.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/guosecume.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gxyzoldqn.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gjuljowel.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gvggdzsko.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/ggmgytmiu.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/ggtvahefz.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/gwzjgudzm.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.hesvh.cn/Article/details/ggpjaqjtj.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gxpwqjxqp.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gwtuunwqx.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/goznkirws.sHtML

var a = 1;  let b = 2
来源：http://3g.fehbvm.com/Article/details/gcxifihvy.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gbkaqagig.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/gmoeqphgb.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/gxelrasyv.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/gsquxioch.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/gaijfphwz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gndjyeeef.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/gqlkhbufk.sHtML

for x in a { print(x) }
来源：http://m.share.zdbjq.cn/Article/details/gqbhujerx.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/gmjklojxy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.hesvh.cn/Article/details/gsuvnlftv.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/ggibncbgo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.zdbjq.cn/Article/details/ggiqiumtw.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/glcnieues.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gthgdzzeu.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/gprecnbnt.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/gxinzklqt.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gooocvwzv.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/ghfzxiagq.sHtML

[T27] Swift：错误处理
来源：http://mobile.fehbvm.com/Article/details/gwixbmgqb.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/geodlwntt.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gksikgwdi.sHtML

enum Color { case red, green }
来源：http://3g.hesvh.cn/Article/details/gmdyrfidy.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.hesvh.cn/Article/details/gppzlhszb.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/gntvkwbkl.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/gloqdazdt.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fehbvm.com/Article/details/gpyvwzenv.sHtML

[T31] Lua：Hello World
来源：http://3g.fehbvm.com/Article/details/gyfrmjvkd.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gehehnzqj.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/glexvnyew.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/gqrytcaus.sHtML

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/gjxwldihr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/gtumjqhic.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gujlchfdo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.zdbjq.cn/Article/details/gdlyhetwm.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/glfqorezm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/gcujpinga.sHtML

[T36] Lua：函数
来源：http://wap.hesvh.cn/Article/details/gvdhwpems.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/graylorgm.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gektcdtbi.sHtML

"a" .. "b"
来源：http://www.m.share.fehbvm.com/Article/details/gkexxjqsa.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/gipwxvmew.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/gkschfixc.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/geujtynes.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/gofdpcqzx.sHtML

[T40] Lua：元表
来源：http://m.share.hesvh.cn/Article/details/gmllerlii.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.hesvh.cn/Article/details/gepvcuabw.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/gdlguqlpq.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/gexxcthud.sHtML

[T42] Perl：变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gncevcmzc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/gyljxtzif.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gtnrnwbxm.sHtML

"值: $a"
来源：http://blog.hesvh.cn/Article/details/gxjnlmkca.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/gxvpxgeky.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fehbvm.com/Article/details/giwcxwgyl.sHtML

[T45] Perl：数组遍历
来源：http://blog.hesvh.cn/Article/details/gqgfcgskw.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/gmhrbvion.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/guiqnjrbn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.zdbjq.cn/Article/details/gjfhshcpk.sHtML

[T47] Perl：正则捕获
来源：http://blog.hesvh.cn/Article/details/gmtmejfgj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.hesvh.cn/Article/details/gbwdzsgxe.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/gxqrcvtdj.sHtML

$s =~ s/old/new/g;
来源：http://m.share.hesvh.cn/Article/details/guhmcsyut.sHtML

[T49] Perl：函数
来源：http://mobile.fehbvm.com/Article/details/gurgvfkdk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gqlegzabw.sHtML

[T50] Perl：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gjbwtyofl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.hesvh.cn/Article/details/gimmigzqz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/grtnfyoux.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gzmbyxrai.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gzkfkdjlc.sHtML

[T52] Scala：变量
来源：http://www.share.hesvh.cn/Article/details/gotqasnfz.sHtML

val a = 1;  var b = 2
来源：http://read.share.fehbvm.com/Article/details/gimwycncc.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gqzgszjug.sHtML

s"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gsbvwjbxv.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gtlkuwyhd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fehbvm.com/Article/details/geqnnnaxi.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/ghsaihqyi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.hesvh.cn/Article/details/gvxshsbih.sHtML

[T56] Scala：样例类
来源：http://baike.hesvh.cn/Article/details/gwwcalmvw.sHtML

case class User(name: String, age: Int)
来源：http://wap.fehbvm.com/Article/details/gxaqdzvjo.sHtML

[T57] Scala：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gpjczyoxo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fehbvm.com/Article/details/gdyiqzhmj.sHtML

[T58] Scala：函数定义
来源：http://wap.hesvh.cn/Article/details/gllqmshmv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fehbvm.com/Article/details/gfpxfuggy.sHtML

[T59] Scala：循环
来源：http://mobile.fehbvm.com/Article/details/gajjhvzae.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.zdbjq.cn/Article/details/grxhcibsz.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/gvgbphwfj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/gzctuxprc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/geuomfrkj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gmxmiggqf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glhulkhir.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.zdbjq.cn/Article/details/gsimxgmmd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/gbqviyfmj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.hesvh.cn/Article/details/gsqeqeyjt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/gorpgzqbm.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.hesvh.cn/Article/details/ggwkqkcfp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fehbvm.com/Article/details/gqgqyuvsv.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/gmrfiazci.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gqqxgkitt.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gifyyukay.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gtucjcgml.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/gaaxoibts.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/gvnaymqcm.sHtML

[U07] Py：反转字典键值
来源：http://blog.fehbvm.com/Article/details/guwnocwrd.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.zdbjq.cn/Article/details/gbmvomzmz.sHtML

[U08] Py：展平二维列表
来源：http://blog.fehbvm.com/Article/details/gipfoqjaz.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/gjbkuaarr.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.hesvh.cn/Article/details/gwhpdkuwu.sHtML

max(d, key=d.get)
来源：http://www.share.fehbvm.com/Article/details/gfnzrpmme.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gsmqvcmpg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.hesvh.cn/Article/details/gjglgfdpm.sHtML

[U11] Py：生成器表达式
来源：http://www.share.zdbjq.cn/Article/details/gtwgvovpm.sHtML

(x * 2 for x in arr)
来源：http://www.blog.zdbjq.cn/Article/details/ggjnsptmg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fehbvm.com/Article/details/gazptqsxu.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/gvpujdfkb.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fehbvm.com/Article/details/gidohklqj.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/gekdjbvmg.sHtML

[U14] Py：分组收集到列表
来源：http://3g.hesvh.cn/Article/details/gbzemioyr.sHtML

defaultdict(list)
来源：http://3g.hesvh.cn/Article/details/gphoqtfjm.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fehbvm.com/Article/details/grllrepfq.sHtML

t = time.perf_counter()
来源：http://www.m.share.fehbvm.com/Article/details/gogkylifl.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.hesvh.cn/Article/details/gpzxpswuv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fehbvm.com/Article/details/gpxxldtnv.sHtML

[U17] Py：初始化日志
来源：http://m.share.zdbjq.cn/Article/details/gojqxdpaf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.zdbjq.cn/Article/details/gniwodxnp.sHtML

[U18] Py：预编译正则
来源：http://www.blog.hesvh.cn/Article/details/gnsrlimwx.sHtML

pat = re.compile(r"\d+")
来源：http://baike.hesvh.cn/Article/details/gaddehqgk.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.zdbjq.cn/Article/details/gudomviub.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.hesvh.cn/Article/details/ghdnoizli.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fehbvm.com/Article/details/glxmwsepq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gwhyfdgzq.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.hesvh.cn/Article/details/gapiswydg.sHtML

@contextlib.contextmanager
来源：http://www.blog.hesvh.cn/Article/details/grayxepsd.sHtML

[U22] Py：矩阵转置
来源：http://wap.hesvh.cn/Article/details/gdenuhoon.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/gswuzieww.sHtML


<!-- 参考信息 -->