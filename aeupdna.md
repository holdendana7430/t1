代发 wailian999

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gljkbwemn.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gvuyzsxmd.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gxzakhrmb.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gwtgsgdhx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gzfcjhwma.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/glqctkghg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/gfjoagfgg.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/gkphaytkt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fehbvm.com/Article/details/gxzcydahp.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/gqlhbgajg.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/gybbeezjb.sHtML

[S11] C：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/glfedrbwv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gnqqsbytj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/gwdjdsdlf.sHtML

fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gqwflxlzg.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/gabvixzre.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gjhfetwud.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gsdprvvvk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/gghlloqom.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/gdjlptxet.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.hesvh.cn/Article/details/gmynmbkpu.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/gucptsbcp.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gpihhtbma.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/gymufmwhh.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/gfjvmzahf.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gdqdiubmy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gonhinekn.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gmwnzwukd.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gchrrpwcx.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gexsbujbr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gwfdqsinr.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gxtrzpktg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gqmtuuwkm.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gwjczkjak.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/govhgpaim.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gbdgaaabt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gtydxewjj.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/gqmuotaau.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gfxhnubce.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/gzdbczzkp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/gsbzepdye.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gdxwdlmno.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gsyezmgzz.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/gurnuqxgp.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gfthoxplj.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gjvnfuiud.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gfxeafxap.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gvfoizuuw.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gqapiyuci.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/gbahfovua.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/gwsxrtiln.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/gpzxqnbsi.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gqqiktpbq.sHtML

#define X_H
来源：http://mobile.zdbjq.cn/Article/details/gygtvbvla.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/grjdvadno.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/gowivvuux.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/gldzvntax.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gtlaynsxd.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gdnusbvzh.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/ghthmnjhu.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/gzmbcuwsp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/gzrlvceas.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/gdjcldylu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gatwnklbv.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/glsjvkrey.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gqdyrnoew.sHtML

[S36] C++：unordered_map
来源：http://wap.fehbvm.com/Article/details/gbbdjpodh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/ganpibinx.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/ggfbdxlts.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gycdcmyzw.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/gjyyfvimy.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gofzhxiws.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gjozttntd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/gvyqusvrz.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/gmikfxnqm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gvofhtcbf.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gqggngzae.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.zdbjq.cn/Article/details/gtynhwduo.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/gqrxugyie.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gpxzpsyql.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/gmkogrrrt.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gtpiquqid.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/grwqjrhwt.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/guqbbusxi.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gtenzyspu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/goteouhxc.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/ghttnccse.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/geovaopzb.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/gogxuinjp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gifnxfggv.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gogzaxyqa.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/gralzsbnc.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gnxjhtloo.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/guyjuaodt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gtcvxppwk.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/gkksyoayu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gkfjahvzk.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gvucuqorh.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/gbhjloxgn.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gekzqobmf.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/gwwsvpqyi.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/gszgbxcum.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/gwghoefgf.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/gxilhutur.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/giytivulr.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/gesaehcvg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/gofcprlla.sHtML

[S56] C++：optional
来源：http://www.blog.zdbjq.cn/Article/details/ghiziujfq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/gbbaocesw.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/gmyttskeb.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/grrksrotg.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/ghrpjoroc.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/givtbairz.sHtML

[S59] C++：静态断言
来源：http://mobile.hesvh.cn/Article/details/gkgztxvql.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gobjpevoj.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gwlzjwwch.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gmwtojfkv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gawykiznd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/guruxeeck.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfvgevmet.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/guxrufwpw.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gycqexckp.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/gxrfdwpcg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gvihxcypt.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fehbvm.com/Article/details/glhuacrwa.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gnbsrvfqx.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/gjarzwmxx.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/ghmrxwzqv.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/gylqljaus.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gxwcywxyq.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/gqlsmdlkw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/gjgasuwmd.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gxazlkjpd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/ggtnpjirs.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/gbhngggdk.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gzapgofqj.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gydyqcrks.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gtyztyrai.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/girbzoreo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/gkdgmiflq.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/ghkajgvop.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fehbvm.com/Article/details/gypailuts.sHtML

[T12] Kotlin：解构声明
来源：http://3g.hesvh.cn/Article/details/gdpefjsig.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gwjlqqhfe.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/gxfxjddgq.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/gnvpjkygy.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gwyezxcvu.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/ggigbzlai.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gbiyawrqu.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/gpgitdxvk.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gbnipzdkf.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gbdcymvks.sHtML

[T17] Swift：变量与常量
来源：http://m.share.hesvh.cn/Article/details/genxkscri.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/giynaboit.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gmdkrbfla.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gbgsuonnm.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/ghavanvuk.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/gvknuqkov.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/gglfzzicw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/gtwuoiyas.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/gwvfqhqsf.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/gfpdhdsak.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/gajeuzlhk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.zdbjq.cn/Article/details/golemsaee.sHtML

[T23] Swift：函数
来源：http://wap.fehbvm.com/Article/details/gpmsurcmx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/gszewbiyz.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/gcxxxhvuf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gruxhdsfg.sHtML

[T25] Swift：结构体
来源：http://mobile.zdbjq.cn/Article/details/gkyncauow.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/gqygezrwx.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gsyajmalt.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/ggzenbrbd.sHtML

[T27] Swift：错误处理
来源：http://blog.zdbjq.cn/Article/details/grawxljdd.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.hesvh.cn/Article/details/gtepyjwwd.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/ggoucbznn.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/gvnxqzkdl.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gmabwsnpq.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/gkaojmlle.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/gugdftdhs.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.zdbjq.cn/Article/details/gagabbqod.sHtML

[T31] Lua：Hello World
来源：http://3g.fehbvm.com/Article/details/gfkkcmztt.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gzgqndyna.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gzwipaowb.sHtML

local a = 1
来源：http://3g.fehbvm.com/Article/details/gmwerrmqe.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/ghrjsoxbt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/gicxwtoyh.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/gypjcfpoh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.hesvh.cn/Article/details/gcirhozel.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/gierbormc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gpinsmxui.sHtML

[T36] Lua：函数
来源：http://wap.hesvh.cn/Article/details/ggiizbdzv.sHtML

function add(a, b) return a + b end
来源：http://mobile.fehbvm.com/Article/details/ginajfzrw.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gqhrmbzim.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/gxhfzsdbk.sHtML

[T38] Lua：条件
来源：http://wap.zdbjq.cn/Article/details/gwexwhhxo.sHtML

if x > 0 then print("正") end
来源：http://www.share.zdbjq.cn/Article/details/gvgwnjuau.sHtML

[T39] Lua：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gjakjdgyk.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/gootzpgyu.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/ggidbmwyl.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fehbvm.com/Article/details/gdrgectad.sHtML

[T41] Perl：Hello World
来源：http://blog.fehbvm.com/Article/details/grfuxakby.sHtML

print "Hello\n";
来源：http://www.m.share.fehbvm.com/Article/details/gwvnvcaoc.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/gliejvcfa.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/gtaxoglqw.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gcbiwjhqt.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/gmwzvyrdl.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/gobgtswpe.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.zdbjq.cn/Article/details/gkbzpmakv.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/gcuscqxxy.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.hesvh.cn/Article/details/gwpcbjzra.sHtML

[T46] Perl：哈希操作
来源：http://read.share.zdbjq.cn/Article/details/gwyjfqxsj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.hesvh.cn/Article/details/gqwrmpdmm.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/grcemwnfi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.zdbjq.cn/Article/details/ghmxmarza.sHtML

[T48] Perl：正则替换
来源：http://m.share.hesvh.cn/Article/details/gcukejnkl.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/gocrghpum.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/gqsfmnmeg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gvxdgnvzg.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gckidgdcz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fehbvm.com/Article/details/gmgxvufip.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/grqootudr.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gdosnuerh.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/goxpsexqp.sHtML

[T52] Scala：变量
来源：http://m.share.hesvh.cn/Article/details/gfulzgpbx.sHtML

val a = 1;  var b = 2
来源：http://baike.hesvh.cn/Article/details/grdjkzsks.sHtML

[T53] Scala：字符串插值
来源：http://3g.hesvh.cn/Article/details/gxgjrbedz.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/gjegvlodk.sHtML

[T54] Scala：集合映射
来源：http://wap.hesvh.cn/Article/details/gelybldfx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/gpvjwhzha.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gxvqifhmv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.hesvh.cn/Article/details/gbhwondug.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gcwkskobe.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gmfwqaeam.sHtML

[T57] Scala：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gdjlneeos.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gzmwkqost.sHtML

[T58] Scala：函数定义
来源：http://3g.zdbjq.cn/Article/details/geuvpqjxx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fehbvm.com/Article/details/gwfsxxxqf.sHtML

[T59] Scala：循环
来源：http://blog.fehbvm.com/Article/details/gmmljgvta.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/grnnhvwxh.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/ghkvfvjfr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/glzqclpta.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvjbfijli.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/gbdymaoqd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/geuiqmbgs.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/gnozepaqs.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/glompebut.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.hesvh.cn/Article/details/gmzzinmfc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/grnrxknkr.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.zdbjq.cn/Article/details/giyveuclj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fehbvm.com/Article/details/grosoxvck.sHtML

[U04] Py：变量调试打印
来源：http://3g.hesvh.cn/Article/details/gwowveavb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/gakpnpztt.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/girkhjbok.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gjeevjraz.sHtML

[U06] Py：合并两个字典
来源：http://baike.hesvh.cn/Article/details/gbzwzbeal.sHtML

{**a, **b}
来源：http://3g.fehbvm.com/Article/details/gbjczsimg.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fehbvm.com/Article/details/gnlmtyira.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.zdbjq.cn/Article/details/gxnnkqhdt.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/gpvpmabmw.sHtML

[y for x in nested for y in x]
来源：http://3g.hesvh.cn/Article/details/gszhfrget.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/gziuniwli.sHtML

max(d, key=d.get)
来源：http://3g.fehbvm.com/Article/details/gbeoamahg.sHtML

[U10] Py：按值排序字典
来源：http://m.share.zdbjq.cn/Article/details/gajuxbukt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.zdbjq.cn/Article/details/gefdvhtzc.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/gsmituhfh.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.hesvh.cn/Article/details/gpdbshzni.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.zdbjq.cn/Article/details/glyyvyeqy.sHtML

Counter(arr).most_common(3)
来源：http://blog.fehbvm.com/Article/details/gyrqlguzp.sHtML

[U13] Py：固定长度队列
来源：http://read.share.zdbjq.cn/Article/details/gngqxfgek.sHtML

deque(maxlen=10)
来源：http://wap.fehbvm.com/Article/details/gqwhrnycb.sHtML

[U14] Py：分组收集到列表
来源：http://baike.zdbjq.cn/Article/details/guyxqrhas.sHtML

defaultdict(list)
来源：http://3g.zdbjq.cn/Article/details/gqhxovzte.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.hesvh.cn/Article/details/gfbpkhkfd.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/ghgjrixuj.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/genfsgedm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fehbvm.com/Article/details/gqigowugf.sHtML

[U17] Py：初始化日志
来源：http://3g.fehbvm.com/Article/details/ghlivytoi.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.zdbjq.cn/Article/details/gpzviitfh.sHtML

[U18] Py：预编译正则
来源：http://www.blog.hesvh.cn/Article/details/gixzemiac.sHtML

pat = re.compile(r"\d+")
来源：http://blog.zdbjq.cn/Article/details/gakttemyb.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fehbvm.com/Article/details/gxymwzudi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fehbvm.com/Article/details/guhwqyujo.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/gtuivddfh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fehbvm.com/Article/details/gubivogqk.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.zdbjq.cn/Article/details/gtwhjjhfh.sHtML

@contextlib.contextmanager
来源：http://www.m.share.hesvh.cn/Article/details/gqnqzmjzr.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fehbvm.com/Article/details/gczruozlw.sHtML

list(zip(*m))
来源：http://m.share.hesvh.cn/Article/details/gdsptlmds.sHtML

[U23] Py：分块读取大文件
来源：http://blog.zdbjq.cn/Article/details/gnbhaekxi.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fehbvm.com/Article/details/ghaiqktoj.sHtML

[U24] Py：路径操作
来源：http://www.blog.fehbvm.com/Article/details/gulnxngbm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gvokstsgs.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fehbvm.com/Article/details/gdxqqfyqi.sHtML

csv.DictReader(f)
来源：http://baike.hesvh.cn/Article/details/glabyfgxm.sHtML

[U26] Py：并发下载
来源：http://blog.fehbvm.com/Article/details/gnrojqsaj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.zdbjq.cn/Article/details/gigkrduxj.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fehbvm.com/Article/details/gjlpcmnpy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fehbvm.com/Article/details/gylbujbqi.sHtML

[U28] Py：类型别名
来源：http://wap.fehbvm.com/Article/details/gmndvjpyk.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/gkpaorxie.sHtML


<!-- 参考信息 -->