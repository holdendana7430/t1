代发 wailian999

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gepdqdrko.sHtML

[S04] C：字符串复制
来源：http://www.m.share.hesvh.cn/Article/details/gimktcaox.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gucfsscdj.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/gohhxhigp.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gsiuazsec.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/gaodksefy.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/ggreuhmkh.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gxpqqwgwm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gombhksrn.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/gwizvwwgp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/gltctdlzu.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/gqfnovopr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gjfaxxsoy.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gkxeeoxsl.sHtML

int *p = &a;  *p = 5;
来源：http://baike.zdbjq.cn/Article/details/ghhrwsqqg.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gchvpkeic.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/gcqzsisth.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/gwqobdepl.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gpxvmraww.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gctsmepcb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/gfkvpxqga.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/getztyble.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/gtgmtywvd.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gurkisjya.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/gxffyfqkj.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gzlfbbeyh.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gopygyvwg.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/gbwrakodg.sHtML

x |= (1 << 3);
来源：http://blog.fehbvm.com/Article/details/gxuwqjfpv.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gfsiamyum.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gawdsxjdf.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gfytnlfds.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/gxjxcvmsg.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gsilmtbym.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gnsqjvdvk.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gmibbnrqy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gqcjrrxcz.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/gzfybnpfz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/ggosefzxk.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gvtbiacui.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gxhthriaf.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gtkzxmzgw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/goylqdmlm.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/ghhhpyabi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/gaomluglv.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gdbmauiht.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gljvugksr.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gdhaexbil.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gskdeqdfv.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gepspzdim.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gbimhhwkf.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/guqzesohz.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/grrseiwxj.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/ghvatatgd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/ggtcsnxmf.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/gynardujs.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gpdodyxim.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gkqkvqaxk.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gjhkccayc.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/gccynjsvl.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/gmpmoyyhp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gnfcoocwe.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gouoqezta.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gpzawiasd.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/gwfajovuj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gprffwstw.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gjydzqgfh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.hesvh.cn/Article/details/gkmaqdikk.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/glzgvyeap.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gxcfwndbx.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/ghqnixizk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/grfbavcmr.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/ggvbbxfxq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/guxzjdryv.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/gsnlounwn.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/gqsjnmqqf.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/grezigyks.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/gscugkchi.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gyrzxcdqb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gsywcfdiw.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gbxzlftxt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/gdvvvuggg.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/gltqhxzrp.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gkwxzwjjn.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/gfvyyijsv.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/gvdokxgub.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gysmuecez.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gnudwxtoc.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/gyntaxnzn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.hesvh.cn/Article/details/gcgcywfec.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/gjtbbzojl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gzqyjtigh.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/gpuuozinl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/goldtagfs.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gievvhwml.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/ghokqnoxj.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/gdmiprxzq.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/gwuqorlwd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gbovjfuxl.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/gtmdhayby.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/gyceddchd.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gjrptvsbr.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/gjsrneqdu.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gmaaqeafu.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/gboaapxwr.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gdolwadha.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/grkbgpwue.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/gfsehmtce.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gpyywczgb.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/grfhrqsap.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/gidebgskm.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gkyhwwnxt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fehbvm.com/Article/details/gojdubgkb.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/ghqzwqplg.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/gtdwgeyuz.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/gcdockwip.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/gsujkonxk.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/gylhimbpy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/gmwvxycox.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fehbvm.com/Article/details/gntridmmy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/gesbbggui.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gisoktpnn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gkqvuymgr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gyqszrvzh.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gnlwwxwrz.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gyobytqxe.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/gsylmuvkp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/guxhmfnwc.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/gutcgnvcg.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gelnnbxyq.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/gvjhxnsdt.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/gjivgspcd.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/ghahomvpc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/gkiftbeud.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gxvfuxqqi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/gyjyditqv.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gsbijkjgg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/gbxjkbsid.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/gikflrwtp.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/guukmoukw.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gksjxamjm.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gwcydhdwj.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/gbltfddlk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gcphemrcd.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/gypkufard.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/gsfezmrcv.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/gxiovncgw.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gjbsixxna.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/ghuultdhc.sHtML

val m = mapOf("a" to 1)
来源：http://wap.hesvh.cn/Article/details/gumpqzdvp.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/gbvygrtov.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/grxodbdzl.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gnbeofvpm.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.hesvh.cn/Article/details/gvvxqwihv.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gavjokhgx.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/glopxreoz.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/goasnnpcc.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gdnfvplos.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/gcjwtentf.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gvipxqksq.sHtML

[T19] Swift：可选绑定
来源：http://www.share.hesvh.cn/Article/details/gcymhyhgk.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/grhlaofjj.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/gqwjwsmgq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gnvcrsmzj.sHtML

[T21] Swift：遍历
来源：http://wap.hesvh.cn/Article/details/gpinyulon.sHtML

for x in a { print(x) }
来源：http://m.share.zdbjq.cn/Article/details/ghpfqvbas.sHtML

[T22] Swift：字典
来源：http://mobile.zdbjq.cn/Article/details/glgeyouwe.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/ghqfbotuw.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/gqxcvpnsm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gldjkcpkg.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/gvcwijcrj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/gappkseyo.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/gbrpafbom.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gqjjxgyor.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/gjmcwrywf.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/gpooatazy.sHtML

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/gxedpsupg.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.hesvh.cn/Article/details/gihdaplbi.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gotkifmgg.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gbdbquepk.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fehbvm.com/Article/details/ggclienlo.sHtML

guard let x = opt else { return }
来源：http://3g.zdbjq.cn/Article/details/glwylndaq.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/glthppbkc.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fehbvm.com/Article/details/grzgjfbah.sHtML

[T31] Lua：Hello World
来源：http://www.share.fehbvm.com/Article/details/gxtrcuqdm.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gdwrmhsyc.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/gosnjlznt.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/gddglmpoc.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/gmokzpnca.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fehbvm.com/Article/details/gvpabpofw.sHtML

[T34] Lua：遍历表
来源：http://read.share.fehbvm.com/Article/details/glrnfhlub.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gdgirhehk.sHtML

[T35] Lua：字典表
来源：http://m.share.hesvh.cn/Article/details/goirdinug.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/gyhqnsvpd.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/gqvamagqx.sHtML

function add(a, b) return a + b end
来源：http://read.share.fehbvm.com/Article/details/ghcgragov.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gmzuoaagr.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/goxgjptjy.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/gegjrdtcp.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/gbxlfpnde.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gykedygel.sHtML

string.find(s, "%d+")
来源：http://read.share.hesvh.cn/Article/details/gxavsdcxr.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/gyugzqapo.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/gcwghbute.sHtML

[T41] Perl：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gwowjuzgd.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/ggutginvd.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gfiofpdpr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/gdcvefyti.sHtML

[T43] Perl：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/ggtfxkuyq.sHtML

"值: $a"
来源：http://wap.fehbvm.com/Article/details/gsobiygli.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/gnucekuoq.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.zdbjq.cn/Article/details/gyeuhzhjv.sHtML

[T45] Perl：数组遍历
来源：http://m.share.zdbjq.cn/Article/details/ggupoxipn.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fehbvm.com/Article/details/gvzbjxvum.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/gbsynydpj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fehbvm.com/Article/details/ghhgedvdh.sHtML

[T47] Perl：正则捕获
来源：http://blog.hesvh.cn/Article/details/gxjdjipjk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/gasnfjhhw.sHtML

[T48] Perl：正则替换
来源：http://3g.fehbvm.com/Article/details/gvcnwyybr.sHtML

$s =~ s/old/new/g;
来源：http://3g.fehbvm.com/Article/details/ggmovpplv.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/gqiuvtsrl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gffkunnxp.sHtML

[T50] Perl：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gkvcpevue.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.hesvh.cn/Article/details/gcqlwdkch.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/gcyndnghm.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/grnxqvmpx.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/grbbhahvg.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/gescrisau.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/gxxnsvpju.sHtML

[T53] Scala：字符串插值
来源：http://m.share.hesvh.cn/Article/details/guxjqqdcz.sHtML

s"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gpmpqyyik.sHtML

[T54] Scala：集合映射
来源：http://read.share.fehbvm.com/Article/details/gocuohput.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/gcikamnzz.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fehbvm.com/Article/details/grofyxflu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/gojgkqnfq.sHtML

[T56] Scala：样例类
来源：http://mobile.hesvh.cn/Article/details/gwkqbyvej.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gecgsqxus.sHtML

[T57] Scala：模式匹配
来源：http://blog.fehbvm.com/Article/details/grvzwqane.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fehbvm.com/Article/details/giigpepyg.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/gfwdgkqan.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.zdbjq.cn/Article/details/glhiqeiay.sHtML

[T59] Scala：循环
来源：http://m.share.hesvh.cn/Article/details/gbuzkcakn.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gmgxtaszs.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fehbvm.com/Article/details/gzittrejd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/gvrlpavih.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/guogsxems.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gdjmkxqlu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gycatkhrc.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.zdbjq.cn/Article/details/gorgjhcio.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.hesvh.cn/Article/details/gdxsapwjg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fehbvm.com/Article/details/gwpdqwusb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/gvivqlhmi.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gwzndjnyx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fehbvm.com/Article/details/gmhkcokto.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.hesvh.cn/Article/details/gmpvhkacj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/gmpghuyud.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.hesvh.cn/Article/details/gaawtsude.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gbxjumyvk.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/gsuswuytp.sHtML

{**a, **b}
来源：http://wap.zdbjq.cn/Article/details/ggdxsmtuq.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/gwvjlfirg.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.hesvh.cn/Article/details/gebdccual.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fehbvm.com/Article/details/ghfptnzan.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/giowxkstu.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fehbvm.com/Article/details/grgnfciux.sHtML

max(d, key=d.get)
来源：http://3g.fehbvm.com/Article/details/ggfpcmasj.sHtML

[U10] Py：按值排序字典
来源：http://read.share.zdbjq.cn/Article/details/geljnzmrq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/gqqvcxprc.sHtML

[U11] Py：生成器表达式
来源：http://3g.fehbvm.com/Article/details/gklshrhvt.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gfzrbzkzn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.hesvh.cn/Article/details/givcsowxf.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/gaszbmkfu.sHtML

[U13] Py：固定长度队列
来源：http://baike.hesvh.cn/Article/details/gjdjqrqrf.sHtML

deque(maxlen=10)
来源：http://wap.fehbvm.com/Article/details/gjskondnp.sHtML

[U14] Py：分组收集到列表
来源：http://baike.hesvh.cn/Article/details/glwnkgltq.sHtML

defaultdict(list)
来源：http://wap.hesvh.cn/Article/details/gzvrfenix.sHtML

[U15] Py：高精度计时
来源：http://baike.hesvh.cn/Article/details/gkbaevoft.sHtML

t = time.perf_counter()
来源：http://blog.fehbvm.com/Article/details/gngpremwo.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.hesvh.cn/Article/details/gurirfcpr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.hesvh.cn/Article/details/gpjkwbdmo.sHtML

[U17] Py：初始化日志
来源：http://3g.fehbvm.com/Article/details/gwxkmqenf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fehbvm.com/Article/details/gevgtjphd.sHtML

[U18] Py：预编译正则
来源：http://wap.hesvh.cn/Article/details/gfbxsgkqi.sHtML

pat = re.compile(r"\d+")
来源：http://3g.zdbjq.cn/Article/details/gyzcvwacv.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/gyjshcmib.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.hesvh.cn/Article/details/gbdqtbqea.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/gsvsnkqhe.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.zdbjq.cn/Article/details/gfbpxqtmc.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.zdbjq.cn/Article/details/gljiuwfyg.sHtML

@contextlib.contextmanager
来源：http://mobile.fehbvm.com/Article/details/gvzupovzh.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/gakrmgelr.sHtML

list(zip(*m))
来源：http://wap.fehbvm.com/Article/details/gbsxuiwsk.sHtML

[U23] Py：分块读取大文件
来源：http://blog.zdbjq.cn/Article/details/gtauoqnra.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.zdbjq.cn/Article/details/gygmppqco.sHtML

[U24] Py：路径操作
来源：http://www.m.share.hesvh.cn/Article/details/gvxnabwib.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/giqaealen.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.hesvh.cn/Article/details/ggdplfzqu.sHtML

csv.DictReader(f)
来源：http://blog.zdbjq.cn/Article/details/gwcqgifha.sHtML

[U26] Py：并发下载
来源：http://m.share.hesvh.cn/Article/details/gmfxscavv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.hesvh.cn/Article/details/ghnkjafyu.sHtML


<!-- 参考信息 -->