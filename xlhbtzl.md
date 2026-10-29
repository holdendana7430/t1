代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gomlzwxuj.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gpwlexgzi.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/gcbmzazte.sHtML

[S03] C：读入整数
来源：http://baike.zdbjq.cn/Article/details/gojpnpfpn.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gjiatkaic.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/gvulshzqz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gjapijywb.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gculjnwhq.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/galbxsgqh.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gmgfpkxwq.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/grhfglpna.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gxvvjgsdh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gulpnwuzu.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/grvackuxn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/gktwbmdsc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gjlyjxqsk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fehbvm.com/Article/details/gunlyiztg.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gtuxvcubv.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gvhebjoee.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gueupazub.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gsbthbjpf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/grwumhnoy.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gwlyllchl.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gogqejspt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gwbgxlwbu.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/grcgukkjf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gmavdtcin.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/gbqobhtxp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/grfajwlrw.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gvffgqmtm.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gtbtwsdic.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gllkvxwxl.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gfqoarsfh.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gtxsjfmag.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gkbgulsas.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/gzycnivwr.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/gmzsftpjo.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/grooickfs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gforrecbg.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/guhhkavmy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/groaabdmg.sHtML

[S21] C：字符类别判断
来源：http://wap.zdbjq.cn/Article/details/ghwbwlxgt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gwxgmbfcz.sHtML

[S22] C：字符串转数字
来源：http://www.share.fehbvm.com/Article/details/gwgbhrcvn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/gunhzlruk.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gzmudhxvh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/gynibyncz.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gcykbvpcf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/gffdxiqil.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gnhljyjkq.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gfanrbdvn.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/gflustcyu.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fehbvm.com/Article/details/gryhjzlwd.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/gxtaqvodx.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gomvrbsms.sHtML

[S28] C：静态变量
来源：http://wap.hesvh.cn/Article/details/gnltdjsyz.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gfcxpgixw.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gqskgsqce.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/geppgewtp.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/gjhxgbvwa.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gzikvavad.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gwypzepue.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/gwdgvoamf.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/giskinwts.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/gddttnfej.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/gozmohkzy.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gxkhhdbox.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gtuejzfpc.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/grxokusoa.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/gxperdkyj.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/gqcbudzmf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/glhrfihgl.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gxxzbeekc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gujeldqgp.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/gakoboumt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gikcdvtjw.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/gszkjcopk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/grobgceoj.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/giffgafmp.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gocnuzucq.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gxplmwjsd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/guzhicyfr.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/gsnydlhln.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gfrzpzywa.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gtnmmnrsc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/gcrinzbel.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gceydgfug.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gkcwqgbxe.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/glasixayt.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/gjowtmlkr.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/glspaeonv.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gemjxywna.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/gdtdrpfxm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gdoapyltn.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gigsfisjz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/goroynlwk.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gexvljujs.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gpzelhjga.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gjagadakr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/gdlddqrbm.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gvyeodmda.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/goqbnijbu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/gdopmcgix.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gjztvwtax.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/glddzsscw.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/grjwuznct.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/gcsrcaxtc.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gpmuzxtqp.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/ghqgfpdvg.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/gakwshoer.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gihidjblc.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/gqenlvzrf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gjwmunitf.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/grbzxcies.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/goabixcll.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gjpbygnrt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/gkvwbsbsp.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gwmcgoruy.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/ggbnqabhs.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/gkmndctun.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/gacinzpei.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gospkrmww.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/guzknllau.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gmbaxejei.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/gohxflmkl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gakjliwdq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gokwslgcu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/giliwwisw.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/ggrrebgxw.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/ganzdwkxk.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gxjggbpcm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gbxnrejsf.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/gjbimegqy.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/gwovdpifr.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gasvfaqyh.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/gadnvokwi.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/gmmktchte.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/gowxtcwak.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gwqgleoss.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gxthuxxlo.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gsyuxqkea.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/gsdbdqltq.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gjlcpdxjk.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gdztejbis.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.zdbjq.cn/Article/details/gqljpwvrp.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/grrnwpiwc.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gobbspkgi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gylboefoy.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/ggibikotl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fehbvm.com/Article/details/gtxmukbhe.sHtML

[T12] Kotlin：解构声明
来源：http://baike.zdbjq.cn/Article/details/grmzendst.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gykvojbjj.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/gbijpowuk.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/grtbrgaby.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/gxyhamppx.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/guwbzvrgx.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gwflgbatg.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/gnqhxvqla.sHtML

[T16] Swift：Hello World
来源：http://m.share.fehbvm.com/Article/details/genfqaqrz.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gcnwfkbew.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/guekcpkoi.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gtfeozvuy.sHtML

[T18] Swift：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gdfsnqvwg.sHtML

"值: \(b)"
来源：http://wap.fehbvm.com/Article/details/gkvvuaxnb.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/gkaxucfdw.sHtML

if let n = opt { print(n) }
来源：http://mobile.zdbjq.cn/Article/details/gmuzfaxvb.sHtML

[T20] Swift：数组操作
来源：http://blog.hesvh.cn/Article/details/gjwustgle.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/gldqzqjzk.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/gaxrbatnm.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/gbrfiiyin.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/gnhjqcmcf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.zdbjq.cn/Article/details/ghkywppjn.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/gmqtqnkce.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.hesvh.cn/Article/details/gmgpzjwcq.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gltktjupp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/gslbdgihp.sHtML

[T25] Swift：结构体
来源：http://blog.fehbvm.com/Article/details/gprnqwdwi.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/gghfvpcqk.sHtML

[T26] Swift：类与重写
来源：http://blog.hesvh.cn/Article/details/gridlmfld.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/goriobnzu.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/gisscnjte.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/ggczxlijq.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gvunuxilx.sHtML

enum Color { case red, green }
来源：http://www.m.share.hesvh.cn/Article/details/goxfhuiyg.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.zdbjq.cn/Article/details/grqtjekqi.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/goktlnkmt.sHtML

[T30] Swift：协议
来源：http://mobile.fehbvm.com/Article/details/grbbmvymm.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fehbvm.com/Article/details/gmfwwyjny.sHtML

[T31] Lua：Hello World
来源：http://blog.zdbjq.cn/Article/details/grfrbaklw.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gexqkyibm.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/gutbpzhpd.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gepnrqhmo.sHtML

[T33] Lua：表（数组）
来源：http://wap.hesvh.cn/Article/details/gdrbupzdf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/ggiscqakh.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/gftvzgirm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/gizxunkcm.sHtML

[T35] Lua：字典表
来源：http://m.share.fehbvm.com/Article/details/gvrwdtchu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fehbvm.com/Article/details/gsjoxxuyq.sHtML

[T36] Lua：函数
来源：http://baike.hesvh.cn/Article/details/gzhmseihp.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gwlqpzgad.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/gamcvfecy.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/gmsbqgjgw.sHtML

[T38] Lua：条件
来源：http://www.blog.fehbvm.com/Article/details/gnbxccdqa.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/gnqutclsl.sHtML

[T39] Lua：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gxnmekgyc.sHtML

string.find(s, "%d+")
来源：http://www.m.share.hesvh.cn/Article/details/gcrnhjzwg.sHtML

[T40] Lua：元表
来源：http://baike.fehbvm.com/Article/details/gyjotadfq.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fehbvm.com/Article/details/giiadukfs.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/gumtbzbvt.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gytnkhwgr.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/gztqeutol.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fehbvm.com/Article/details/gxknhpmur.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gcnenbjmv.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/gwxtryiar.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/gsofdhscz.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.zdbjq.cn/Article/details/ghglurvyh.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/gfmejcenj.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/gimrjzchm.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/gsfnembav.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fehbvm.com/Article/details/gcbsfirsg.sHtML

[T47] Perl：正则捕获
来源：http://3g.fehbvm.com/Article/details/gdrfixymx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/gqafhakys.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/gcnieqhbd.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/gjbhrabqt.sHtML

[T49] Perl：函数
来源：http://3g.hesvh.cn/Article/details/gnsogkonp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gnyvfjuve.sHtML

[T50] Perl：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gnpagzbsb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.zdbjq.cn/Article/details/gdbxstmnu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/gdfagkeat.sHtML

[T51] Scala：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gripzzzcu.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gejzdmsjw.sHtML

[T52] Scala：变量
来源：http://mobile.hesvh.cn/Article/details/gnynvgzcb.sHtML

val a = 1;  var b = 2
来源：http://wap.fehbvm.com/Article/details/gdeyodfmj.sHtML

[T53] Scala：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gcoebgbqa.sHtML

s"值: $b"
来源：http://baike.hesvh.cn/Article/details/gdzjerjzf.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gnmxmkdkc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.hesvh.cn/Article/details/ggqrqfrie.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/gdyergrui.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.zdbjq.cn/Article/details/gmatpirsf.sHtML

[T56] Scala：样例类
来源：http://www.share.zdbjq.cn/Article/details/giggqadeu.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gpvgetain.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gcpahgndy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gynnxlhqf.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/gifowiine.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fehbvm.com/Article/details/grpkzptej.sHtML

[T59] Scala：循环
来源：http://www.share.fehbvm.com/Article/details/gykfzoiyj.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.hesvh.cn/Article/details/gimfizdep.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/gufuaukru.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/gstzqqiox.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghxqzpskn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gafrvrobf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxuaozdmu.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.zdbjq.cn/Article/details/ggtewsdaf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gpidmyewq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/gpohnzlvw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/gdfzugcaa.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.zdbjq.cn/Article/details/geirgjucp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fehbvm.com/Article/details/gmjvvymhr.sHtML

[U04] Py：变量调试打印
来源：http://3g.zdbjq.cn/Article/details/gnmqaxtjh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.hesvh.cn/Article/details/ganmergif.sHtML

[U05] Py：列表去重且保序
来源：http://wap.hesvh.cn/Article/details/gvmcutuqr.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/glghiihbx.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/guchnixya.sHtML

{**a, **b}
来源：http://baike.fehbvm.com/Article/details/guagtmjkl.sHtML

[U07] Py：反转字典键值
来源：http://3g.hesvh.cn/Article/details/gdiwbsoaz.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fehbvm.com/Article/details/glacjrfwj.sHtML

[U08] Py：展平二维列表
来源：http://3g.zdbjq.cn/Article/details/gfpvgtzpc.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fehbvm.com/Article/details/gebomngec.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.hesvh.cn/Article/details/guufjgnyz.sHtML

max(d, key=d.get)
来源：http://blog.fehbvm.com/Article/details/gvamhegum.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/geguurfus.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fehbvm.com/Article/details/gwpzuvgqj.sHtML

[U11] Py：生成器表达式
来源：http://baike.hesvh.cn/Article/details/gihjvtfmi.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/geqcrxzpe.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/gxhkcaxif.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/gtgneayhb.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/glzhhktns.sHtML

deque(maxlen=10)
来源：http://blog.zdbjq.cn/Article/details/ghmxgglqo.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fehbvm.com/Article/details/gacvfstov.sHtML

defaultdict(list)
来源：http://www.share.zdbjq.cn/Article/details/gibybgpzy.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fehbvm.com/Article/details/gguxcampv.sHtML

t = time.perf_counter()
来源：http://m.share.fehbvm.com/Article/details/gkbufutgz.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fehbvm.com/Article/details/gfkcselxe.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fehbvm.com/Article/details/gvhhjweub.sHtML

[U17] Py：初始化日志
来源：http://www.share.hesvh.cn/Article/details/gaoixtukk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gpewstnpc.sHtML

[U18] Py：预编译正则
来源：http://baike.hesvh.cn/Article/details/gjkuatmbj.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.hesvh.cn/Article/details/gbhheqpqc.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/gysbyrgtz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fehbvm.com/Article/details/gptldlmwj.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/gkneyoehr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.zdbjq.cn/Article/details/gsnfgceov.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fehbvm.com/Article/details/gizudqsxz.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/gzzomtgri.sHtML

[U22] Py：矩阵转置
来源：http://wap.fehbvm.com/Article/details/gphxhflfd.sHtML

list(zip(*m))
来源：http://www.blog.zdbjq.cn/Article/details/gfzpffhdl.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.hesvh.cn/Article/details/gplymfksq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.zdbjq.cn/Article/details/gzucznaou.sHtML

[U24] Py：路径操作
来源：http://www.blog.zdbjq.cn/Article/details/gpbtgffgb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gosmbubne.sHtML


<!-- 参考信息 -->