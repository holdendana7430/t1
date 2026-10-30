代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gygknhwbf.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gtjadlcco.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/gehuvypcz.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/gqboepjwi.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gaudwkzah.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/gjhrhpwth.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/gxqgivdlw.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/gjfnessjf.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/gayndjbwh.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/ghfxpqnzt.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/gahlnimnu.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/gsutpcoay.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/grswzmqku.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gndhsjgmk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gmgaxkrqq.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gdqisascg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/ggocerijp.sHtML

[S10] C：指针与解引用
来源：http://www.share.hesvh.cn/Article/details/gxemwujjx.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/geqicnobk.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gzbtafwqk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gmrkxtind.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/gabuoweqv.sHtML

fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/ggmpphdzg.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/guphjmcvl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/gyobuzlsl.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/gtcpwoufw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.zdbjq.cn/Article/details/gnbguybiq.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gqtcyqpmy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gusleyujz.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gtmzjhyjr.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/ginfwuveg.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/glfbwzuwr.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/gdbjrnpph.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gsytpnfvw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/gmqzeqlxn.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gdblygokj.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/gkyogrvsm.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/gvutnulvl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/ghhgfdnpx.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/gasnrajsh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gcildtvxo.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/guvtdnurc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/gmtiarroh.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/grjkndykv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/gqfkxbvzp.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gmaedvtrw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/gmmrirfbw.sHtML

[S24] C：获取本地时间
来源：http://3g.zdbjq.cn/Article/details/gjvwwqzdo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gljeamdwm.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/goqzxhjnd.sHtML

memcpy(dst, src, n);
来源：http://baike.fehbvm.com/Article/details/gvchzozdl.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gknxqmrzy.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/gsmrymaet.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/gqnroncrd.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gecokcyft.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/gohovluna.sHtML

static int counter = 0;
来源：http://read.share.fehbvm.com/Article/details/ggadmkhee.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gsdaprvss.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gfycfmaqh.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/gdvoittam.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gewuvbmrq.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/geofjazdf.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/gumjcjcrz.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gcditsakh.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/gsaplzqoy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gfvdedanv.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/giysctgyp.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/ggieckutm.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/gmdytjrju.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/gzufhkldl.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/gpqrxnvmz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/gxnisuwfy.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/gscimuqmm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/glxbrspss.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gxmyffmye.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gxasnxgkn.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/gnaurrrxc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gxyaqkrke.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/gfgrrwlfj.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gwttzmiay.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/gnxlvepff.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/grtvrqfuf.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/gqhpygyow.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gynmkypzl.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/gepfrwovp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/gapslpyae.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/glodvfmre.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gbwmicupq.sHtML

[S43] C++：智能指针
来源：http://blog.fehbvm.com/Article/details/gbejzhtft.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/gifmvgjns.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gxmjbbeec.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gmacbkktm.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/gebdxaomt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/gtdkcdjdh.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/gukugriiw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gsotuatdx.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/gxwjwdqid.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gxkgiopzv.sHtML

[S48] C++：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gmefdftpd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/gywjpytgl.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/gpugompiv.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gwsypwbhf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gdustxgrh.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/gunkvjsig.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gobqnefza.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/govkozlxx.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/grxjlriog.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gtywqwepe.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvomddhsx.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/gaifhyigs.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/gzqbbfytg.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/gixebivkx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/gqytwciza.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/grdfduocz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gxjcsmgeb.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/gybhivslo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/gcyouytkp.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gkwmhrcpo.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/glsvjzlgw.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gvlydmukx.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/gqvusfvnz.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/gmbuhznqe.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.zdbjq.cn/Article/details/gcaaxwcxw.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/gpvkjdedr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gyevtuklf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbdmrhsxq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gxzrnpaxg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtlkwxcdr.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/gvdiwlxaq.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gwbnourvt.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/giuhshodk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/ggcpyphse.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/gffxibujq.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gffzwmwrd.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/griarozew.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/gfwayqoxx.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gldhecndz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/gozkllxtx.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.zdbjq.cn/Article/details/galqmiqaj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gtjqxvman.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gchjusxjt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/ghahunxaa.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/gudcohfrl.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gcdgmqpyx.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/gpwpirdhq.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/gsxlinlxx.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gaaluoeav.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.hesvh.cn/Article/details/genqgzsts.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/glgzdnghm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gfftfzgfh.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/gnmcxlfws.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/glcmnlyby.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/ggenmzppg.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/gqscotljn.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/gcjxzsbmh.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/ggdnnfrkt.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/geivxcicn.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/ggtvhrast.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/gtdzcpcii.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/goradeotz.sHtML

[T17] Swift：变量与常量
来源：http://read.share.zdbjq.cn/Article/details/gfqhokgdy.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/gqcrbjbhu.sHtML

[T18] Swift：字符串插值
来源：http://wap.fehbvm.com/Article/details/gtasryuix.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/gzrnbnidd.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/gnozfpxmy.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/gwtxeulrt.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/ggzadllpk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gdqsgvvxv.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/gzyrdadhg.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/gemzezgog.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/grklsrqxc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/glhoujdib.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/glsqtfnrv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/gnhnnxiva.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/gfsyetwhg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gsktfdais.sHtML

[T25] Swift：结构体
来源：http://mobile.fehbvm.com/Article/details/grljzgzyq.sHtML

struct P { var x: Int }
来源：http://m.share.fehbvm.com/Article/details/gisljiadz.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/gynetrepm.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gfgdkqeen.sHtML

[T27] Swift：错误处理
来源：http://mobile.fehbvm.com/Article/details/ghzniqghz.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.hesvh.cn/Article/details/gyecgvnzf.sHtML

[T28] Swift：枚举
来源：http://www.blog.fehbvm.com/Article/details/gkochhqwd.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/gamzpeyws.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/gtdjqqgnm.sHtML

guard let x = opt else { return }
来源：http://www.blog.fehbvm.com/Article/details/gxcbgmadr.sHtML

[T30] Swift：协议
来源：http://mobile.zdbjq.cn/Article/details/gjfylvzwc.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/giuqiquln.sHtML

[T31] Lua：Hello World
来源：http://mobile.zdbjq.cn/Article/details/goyxpnapo.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gwqqthwsm.sHtML

[T32] Lua：局部变量
来源：http://baike.zdbjq.cn/Article/details/genyspcqj.sHtML

local a = 1
来源：http://blog.zdbjq.cn/Article/details/gbiabouci.sHtML

[T33] Lua：表（数组）
来源：http://m.share.hesvh.cn/Article/details/gtsucagfw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/ghmmiyvhq.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/gfzjhflsa.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/ggwthqvrc.sHtML

[T35] Lua：字典表
来源：http://m.share.zdbjq.cn/Article/details/gvzpzwedx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.zdbjq.cn/Article/details/gbmiyngjn.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/ghuttggvb.sHtML

function add(a, b) return a + b end
来源：http://read.share.zdbjq.cn/Article/details/gibaahmfj.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gymdtstke.sHtML

"a" .. "b"
来源：http://www.blog.zdbjq.cn/Article/details/gdzedhoqm.sHtML

[T38] Lua：条件
来源：http://read.share.zdbjq.cn/Article/details/gpxzenhjz.sHtML

if x > 0 then print("正") end
来源：http://mobile.hesvh.cn/Article/details/ggvlevviz.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/ggkeoivpv.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gmilhzdgc.sHtML

[T40] Lua：元表
来源：http://m.share.hesvh.cn/Article/details/gzzhrwlft.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/gxlzulwnf.sHtML

[T41] Perl：Hello World
来源：http://read.share.fehbvm.com/Article/details/gbcbknhuc.sHtML

print "Hello\n";
来源：http://www.blog.fehbvm.com/Article/details/guctfcznf.sHtML

[T42] Perl：变量类型
来源：http://m.share.fehbvm.com/Article/details/gfgaozraf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.hesvh.cn/Article/details/gcggftysv.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/gyhujwdrj.sHtML

"值: $a"
来源：http://www.blog.zdbjq.cn/Article/details/gvxgkrytt.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/ghufclenc.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/gbcltoiae.sHtML

[T45] Perl：数组遍历
来源：http://blog.hesvh.cn/Article/details/gorayygtv.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/gmpzvevyv.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/geshjcktp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.zdbjq.cn/Article/details/gvojqrlhv.sHtML

[T47] Perl：正则捕获
来源：http://mobile.zdbjq.cn/Article/details/gqiqrzvgv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.zdbjq.cn/Article/details/gejqiyufi.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/grhbcpqvw.sHtML

$s =~ s/old/new/g;
来源：http://read.share.hesvh.cn/Article/details/giyhjuxhg.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/gadpkxgll.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gdxqhbdib.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/geldsckcc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/gimbjnskg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvibhcwfy.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/glpdzpdty.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gnygzqddn.sHtML

[T52] Scala：变量
来源：http://mobile.zdbjq.cn/Article/details/gdbgaupwo.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/gliytvgaj.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gserobutq.sHtML

s"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gscjymxgt.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gtetklzlz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/gxtrapjge.sHtML

[T55] Scala：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gafcdofxi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/gwaspwemy.sHtML

[T56] Scala：样例类
来源：http://www.m.share.hesvh.cn/Article/details/gudboojdw.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gmpxrzeko.sHtML

[T57] Scala：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gaxxpjlru.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/gkrcwrllq.sHtML

[T58] Scala：函数定义
来源：http://3g.hesvh.cn/Article/details/gauhvbpsb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fehbvm.com/Article/details/gjffdidza.sHtML

[T59] Scala：循环
来源：http://www.share.hesvh.cn/Article/details/gfbbeixvz.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gurloxrns.sHtML

[T60] Scala：折叠
来源：http://www.share.zdbjq.cn/Article/details/gsrpuymtm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/gtkxghfzq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/geicnhnrs.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gypkucgsk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcnmlvhme.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fehbvm.com/Article/details/gtacfpzzi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/gzmnflomd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/gvudngkzf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.hesvh.cn/Article/details/gnvyawiiu.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gjzlljfiq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fehbvm.com/Article/details/gixrixkla.sHtML

[U04] Py：变量调试打印
来源：http://m.share.hesvh.cn/Article/details/grdriyhhy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/gcvvevbrd.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fehbvm.com/Article/details/gvkigkiel.sHtML

list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gbbxgtuaj.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/gappqwwfv.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/gxhalfdeb.sHtML

[U07] Py：反转字典键值
来源：http://m.share.zdbjq.cn/Article/details/gohzkqott.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.zdbjq.cn/Article/details/gyyaxjrqx.sHtML

[U08] Py：展平二维列表
来源：http://wap.zdbjq.cn/Article/details/gouosnhjq.sHtML

[y for x in nested for y in x]
来源：http://m.share.hesvh.cn/Article/details/gbtjponeg.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/gmfyuzemt.sHtML

max(d, key=d.get)
来源：http://wap.fehbvm.com/Article/details/gyanxdqka.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gvxomraaz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.hesvh.cn/Article/details/gzbhqrbnd.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/gylzkddtq.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/gqlfbrlxp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/gdrmjpuhb.sHtML

Counter(arr).most_common(3)
来源：http://www.share.zdbjq.cn/Article/details/gcmptjfta.sHtML

[U13] Py：固定长度队列
来源：http://3g.zdbjq.cn/Article/details/gocxayudu.sHtML

deque(maxlen=10)
来源：http://www.m.share.hesvh.cn/Article/details/gypfxalku.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/gacgjxjco.sHtML

defaultdict(list)
来源：http://www.m.share.fehbvm.com/Article/details/ghfrxhqns.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/gkpdhxsvw.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/gqjqjbqbj.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.zdbjq.cn/Article/details/gtvwuphys.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.hesvh.cn/Article/details/gkigjibzf.sHtML

[U17] Py：初始化日志
来源：http://wap.hesvh.cn/Article/details/gaffoppcy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.zdbjq.cn/Article/details/gguhdygpb.sHtML

[U18] Py：预编译正则
来源：http://read.share.zdbjq.cn/Article/details/gxxofleif.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gxetvxmhi.sHtML

[U19] Py：正则替换带回调
来源：http://wap.hesvh.cn/Article/details/gqimokqis.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fehbvm.com/Article/details/gibmybixd.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fehbvm.com/Article/details/gjlvpfdyw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/godihuatu.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.zdbjq.cn/Article/details/gskmzqhgy.sHtML

@contextlib.contextmanager
来源：http://wap.fehbvm.com/Article/details/gdgirenrq.sHtML

[U22] Py：矩阵转置
来源：http://www.share.zdbjq.cn/Article/details/gmeiwotzl.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/gjrwksozr.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.zdbjq.cn/Article/details/ghirjnzbp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.hesvh.cn/Article/details/gaxpgtnnf.sHtML

[U24] Py：路径操作
来源：http://www.blog.hesvh.cn/Article/details/gsdfxsyrf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gcizjropl.sHtML


<!-- 参考信息 -->