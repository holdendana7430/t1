代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gtdhzgrrt.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gmwivrpid.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/gsqajxzpy.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gazviornp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.zdbjq.cn/Article/details/gkijtbkni.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/grbevelzx.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gtixqhixv.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/gulgihsgt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gkduyjele.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/ghebyfchr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gxvxkybtw.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/ggqrfuayc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gtfaqcoyc.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/gwtyaunbc.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gdgxyqktv.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gcmepqeyi.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gupszlqbr.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gfcpefepk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/gfxbywklf.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gtvfqhggj.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gvxpedvdc.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gxkwbifsy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gikizmigx.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/gqecyqzcf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gqchczmsj.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/gxfsbahjl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/grlfrnuld.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gbluquadv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gurytqhuy.sHtML

[S23] C：随机数
来源：http://mobile.fehbvm.com/Article/details/gfwhvobai.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gxvqvkgyx.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gbmttbbsf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/gvokhyifo.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/gxeezfwrf.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/ggizwpvrw.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/gajtzuukb.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/gqsgbsadm.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/glzkseqsg.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gpxzektwg.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gujocavcy.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gxzriglfe.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gpljyhmgf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/gycbokwdu.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/gzduetjuf.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/ghatsqazp.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gjpldfwoe.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gmlabniea.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gyklgchji.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gevbukifi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/gjlechtdc.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gstduuyqs.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gtopiscvl.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/ghtqmzzas.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/golbsxwph.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/gohozymct.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/gycbxykpo.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/ghstjzgez.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gzbzkrdnj.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/giwcvdgra.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gkofvcprr.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/gwlzuhkqt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/gvhiyytrc.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/gbzhfhkil.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gywaausrw.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gklhtfwfo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gsowjqddn.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gxscigkoa.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/gyevhlbcy.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/ggejtusdi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gdjlmaaep.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gscbtzpvg.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gkgkgpujv.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gkqgreauv.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/gzswzkena.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gpzjgulzf.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/gdhhcyyog.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/gchtginru.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.hesvh.cn/Article/details/gjeglkrqo.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/gwhmpdonq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gjqdtoril.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/gmuknarey.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/gsbvrjjub.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gmwawskbt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/gmzdzoezo.sHtML

while (std::getline(in, line)) { }
来源：http://baike.hesvh.cn/Article/details/gtojqsskn.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gvwzutrjq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/gwwbxcbfh.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gnyhxvufu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gwouswkir.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gxbabbmag.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/gcpeganjx.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/grehohtur.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gttnnsyvh.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gaambbagh.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/gubgrfsla.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/gnmofjory.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.zdbjq.cn/Article/details/grktdldiq.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/gctsefooj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/gttxrvdza.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gbweponsv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gjmceytzj.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/gvvvqswxk.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gcnuvtrqf.sHtML

[S58] C++：命名空间
来源：http://wap.fehbvm.com/Article/details/gacdzinkw.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/gmzxwsfma.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gwjeyypab.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/gmueegnps.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gbhevvabg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/gdlbqqspq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gunuzpzzb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gkedwssny.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ginjvzhsj.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.hesvh.cn/Article/details/gybizbbni.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/grgqcncrf.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gjzetxapl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gpnsivyio.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/gfgxandwt.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gbafrkknf.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/gppdzquvu.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gielniqxu.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.zdbjq.cn/Article/details/genzutusw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/gjbxsiasb.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gvuibregg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/geulpqsoy.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gpfaehzdv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/gskuzpsax.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gqmphqorh.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gwueujowo.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.hesvh.cn/Article/details/gfhexpuxl.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/gywgevbkt.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gebpojxuv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/gobvjvyqn.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/gucaenebk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/gjmvldgdk.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/gfwiyisqc.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gbjycifsl.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/gdcvqyrzh.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gjnilrucc.sHtML

[T14] Kotlin：循环
来源：http://wap.hesvh.cn/Article/details/gjctnntrv.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gpunwieqq.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/gfuivrhle.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/gqgunkmms.sHtML

[T16] Swift：Hello World
来源：http://m.share.fehbvm.com/Article/details/gtfsepcba.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gqkowdhky.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/glxpqhpxd.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gmunuhnim.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/ghkkqfwpl.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/gssgjvfxp.sHtML

[T19] Swift：可选绑定
来源：http://wap.fehbvm.com/Article/details/gohnweqdo.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gbuugqqvi.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/gtlwotvaq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gevodbcti.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/gapwepgjh.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gleacyqey.sHtML

[T22] Swift：字典
来源：http://wap.zdbjq.cn/Article/details/goqetmhem.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/gsvgbjzio.sHtML

[T23] Swift：函数
来源：http://3g.hesvh.cn/Article/details/gpnbvlrug.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gdzxiosyo.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/gosdvejyu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/ggwjvdzwp.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gaocwanac.sHtML

struct P { var x: Int }
来源：http://www.m.share.zdbjq.cn/Article/details/gkziqhtyt.sHtML

[T26] Swift：类与重写
来源：http://read.share.fehbvm.com/Article/details/gxzrzdmac.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.hesvh.cn/Article/details/gbmdibgde.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/gbuydpyhk.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fehbvm.com/Article/details/gsjpgmyed.sHtML

[T28] Swift：枚举
来源：http://www.blog.fehbvm.com/Article/details/grbcnssss.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gbddccpqw.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.hesvh.cn/Article/details/gubshrudz.sHtML

guard let x = opt else { return }
来源：http://m.share.hesvh.cn/Article/details/gnrysybcy.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/gnvsjautn.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fehbvm.com/Article/details/gxnxpippk.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gcufvbuwi.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gzfneozkv.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gjqqnpggi.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/gnovixfzh.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/gysyosrng.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/gtrzwshvr.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/gkkbnvbvu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/gqfljebzh.sHtML

[T35] Lua：字典表
来源：http://blog.fehbvm.com/Article/details/gzsmjdmel.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/gledfrpey.sHtML

[T36] Lua：函数
来源：http://baike.hesvh.cn/Article/details/gfjlgqjtg.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/grpnaunjg.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gnsjdjlbf.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/givrmnvlc.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/gcryuwlpe.sHtML

if x > 0 then print("正") end
来源：http://read.share.zdbjq.cn/Article/details/gvfnpzxrs.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gcfekutdr.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/gdydoqxwh.sHtML

[T40] Lua：元表
来源：http://wap.hesvh.cn/Article/details/gdwlsofdt.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/gilkuugvb.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gteeqlegy.sHtML

print "Hello\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gfkkkiarh.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/ggedpoksg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fehbvm.com/Article/details/gtmsrmdly.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/guhbtliha.sHtML

"值: $a"
来源：http://read.share.hesvh.cn/Article/details/gkcoesrpm.sHtML

[T44] Perl：条件
来源：http://wap.fehbvm.com/Article/details/grsnpvxyr.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/gtswcholw.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gchavmbsu.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.zdbjq.cn/Article/details/gknizcohc.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.zdbjq.cn/Article/details/gumbshevd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.zdbjq.cn/Article/details/gahoxufze.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/geoooutkc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/gcevbbxck.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/geukesesf.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fehbvm.com/Article/details/gpsgkbmmo.sHtML

[T49] Perl：函数
来源：http://read.share.hesvh.cn/Article/details/gdjvcvzkr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gfjiinhoe.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gnnuczazu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fehbvm.com/Article/details/ghymfzadn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/gonchpqzb.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gmokcknbx.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/glhjplurr.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gchkoienu.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/gdvcoykes.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gtrfjiuav.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/grvqnhgnb.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/gguzysyso.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gpsjpwnce.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gbosnwhhy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fehbvm.com/Article/details/gllpjflrb.sHtML

[T56] Scala：样例类
来源：http://blog.zdbjq.cn/Article/details/gfhyhlglo.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gdjzidpqt.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gkizvmthm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/ggjjtopkh.sHtML

[T58] Scala：函数定义
来源：http://read.share.fehbvm.com/Article/details/gxzrqlvsi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fehbvm.com/Article/details/grdbbiowv.sHtML

[T59] Scala：循环
来源：http://read.share.zdbjq.cn/Article/details/gmbfzqrgv.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gfwsqwfar.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/gilcchfgk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.zdbjq.cn/Article/details/gnjlhwdhy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzywboykz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gngvjyzmx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvnasaolz.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.zdbjq.cn/Article/details/gbzcqjqpv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fehbvm.com/Article/details/gymihghan.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.zdbjq.cn/Article/details/glrhnieqr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/gjwvhgpxw.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/gerftfgij.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/gkeqxprjb.sHtML

[U04] Py：变量调试打印
来源：http://baike.zdbjq.cn/Article/details/gmkwfcluk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/gyacijdlg.sHtML

[U05] Py：列表去重且保序
来源：http://3g.hesvh.cn/Article/details/gxbhripni.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gjeobnazt.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/gjngfhxcl.sHtML

{**a, **b}
来源：http://read.share.zdbjq.cn/Article/details/glvkhslki.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/gpyzejqux.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.hesvh.cn/Article/details/ghvdmofyu.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/grjvqbhgf.sHtML

[y for x in nested for y in x]
来源：http://www.share.fehbvm.com/Article/details/gpybafhcd.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.zdbjq.cn/Article/details/gkhhnhrae.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/gnvkbamcx.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/gtnvqhctd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.zdbjq.cn/Article/details/gpjspudts.sHtML

[U11] Py：生成器表达式
来源：http://read.share.zdbjq.cn/Article/details/gmznmmugl.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/gopjgchca.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.zdbjq.cn/Article/details/gxivtcxec.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fehbvm.com/Article/details/gerfveroo.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fehbvm.com/Article/details/gztzjrqjq.sHtML

deque(maxlen=10)
来源：http://www.m.share.zdbjq.cn/Article/details/gorwhpwwe.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fehbvm.com/Article/details/gmwyqigmb.sHtML

defaultdict(list)
来源：http://www.share.zdbjq.cn/Article/details/gqkfrhtih.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/gxrzwadle.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/glqqfdysc.sHtML

[U16] Py：命令行参数解析
来源：http://blog.hesvh.cn/Article/details/ggzvsgrus.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gepovzglg.sHtML

[U17] Py：初始化日志
来源：http://mobile.zdbjq.cn/Article/details/gooorfgbo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.zdbjq.cn/Article/details/ggfeiegjz.sHtML

[U18] Py：预编译正则
来源：http://m.share.hesvh.cn/Article/details/ghxbhxakx.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fehbvm.com/Article/details/glgldotcl.sHtML

[U19] Py：正则替换带回调
来源：http://baike.hesvh.cn/Article/details/gkednygvk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.zdbjq.cn/Article/details/giwyewcoo.sHtML

[U20] Py：缓存函数结果
来源：http://baike.zdbjq.cn/Article/details/ggyehrmtk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/gdsrqzmbg.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.hesvh.cn/Article/details/gwkydomtc.sHtML

@contextlib.contextmanager
来源：http://wap.hesvh.cn/Article/details/givdnvvna.sHtML

[U22] Py：矩阵转置
来源：http://blog.hesvh.cn/Article/details/gtdqujkzp.sHtML

list(zip(*m))
来源：http://www.share.fehbvm.com/Article/details/gaxystumb.sHtML

[U23] Py：分块读取大文件
来源：http://blog.hesvh.cn/Article/details/gpdgnuhhn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/gllvlfbom.sHtML

[U24] Py：路径操作
来源：http://m.share.fehbvm.com/Article/details/ghxkcklxa.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gfjezvwzx.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.hesvh.cn/Article/details/gubwitier.sHtML

csv.DictReader(f)
来源：http://www.share.fehbvm.com/Article/details/gmphpjjnm.sHtML

[U26] Py：并发下载
来源：http://read.share.hesvh.cn/Article/details/gdxuqiqqr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/gtxjsfzep.sHtML

[U27] Py：异步 HTTP
来源：http://baike.zdbjq.cn/Article/details/gdytedgsz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.zdbjq.cn/Article/details/gwjvqdkzj.sHtML

[U28] Py：类型别名
来源：http://www.blog.hesvh.cn/Article/details/gkzprwdoy.sHtML

UserId = int
来源：http://wap.zdbjq.cn/Article/details/gezwgbyru.sHtML

[U29] Py：属性校验
来源：http://read.share.fehbvm.com/Article/details/gishzuhbr.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fehbvm.com/Article/details/ggqaumrmp.sHtML

[U30] Py：数据类
来源：http://read.share.hesvh.cn/Article/details/gpaqyroig.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fehbvm.com/Article/details/gudhsdpte.sHtML

[U31] Py：单测
来源：http://www.blog.zdbjq.cn/Article/details/ghfaleuik.sHtML

python -m pytest -q
来源：http://mobile.fehbvm.com/Article/details/gtspwalkh.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/gqcijygqh.sHtML

ruff format . && ruff check --fix .
来源：http://baike.hesvh.cn/Article/details/gwbaptyfy.sHtML


<!-- 参考信息 -->