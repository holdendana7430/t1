代发 wailian999

int x; scanf("%d", &x);
来源：http://baike.fehbvm.com/Article/details/gjbntbvaw.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gfsbjhgud.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/gjpdikppa.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gifigelln.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/gceswracd.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gkdlkcwai.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gvkgdieui.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/gjafqbewe.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/ggenlndmm.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/genovnrwp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/gzitozwnr.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/grtcsgmej.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gftfjnghi.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/gmozvqlad.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/gxeypaopl.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gyfazdwsw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/gredgkeow.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/gdrrfgsch.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/ghpfbvnld.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gukkoulhs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/ghlafuxht.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/gxugdejon.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gdnogdgln.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gbeovfngn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/gyadcfmnf.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/glwwnjbag.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gncwsbvji.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/grjfzwweo.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gxkexulbs.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gosvwwfaf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gjxpwyzia.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/gvcyrqkiu.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gbxhrgdfc.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/gpbrohqal.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gowmazejy.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/gtsahwnnk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/grgndylvn.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/gwyycfeqi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gqjcaqnvd.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gnmhoxksp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.hesvh.cn/Article/details/gpygxmaup.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gninaahnv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gvlmjiizn.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/gvhcxyxay.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/grejrkdif.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gbsorakpu.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gyqwxaboi.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/gmjcboshz.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/ggdqxvknp.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gcgbljlvs.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gnesjgzzw.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/gmbabepxg.sHtML

static int counter = 0;
来源：http://read.share.fehbvm.com/Article/details/gjtlfebal.sHtML

[S29] C：变参函数
来源：http://3g.zdbjq.cn/Article/details/gbfptdkgc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/gyjdnfrdj.sHtML

[S30] C：头文件保护
来源：http://blog.zdbjq.cn/Article/details/gofndbbiv.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gchhwfzux.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gzcejqxqw.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gqfmigxzn.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gqtxldobh.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gpaxtazbc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gnwnwtiqy.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/goszhrxka.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gxognsbtj.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gbwpcpbsl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/genhyynrb.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/gcmhsarox.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gguurpknu.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/gdgakdkju.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/geoqsfbfi.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/gzluxjutb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/goopoteds.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gaudajzfl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/gewldgggm.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/gjbzkcnpu.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/ggzizqbut.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/gcstlzkxl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gpkjpugif.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/gogbblhss.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/gniiabpww.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/gtsnlzfoj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.zdbjq.cn/Article/details/gicqgjlfy.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gfbsixxkt.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gchvjmuyh.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/glgagutih.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gaudgebai.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/ggojntrju.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gphhvicok.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gjihyhtgr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/gyouaecyc.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/gfnujomco.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gsvtrjsuc.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gggvkcxop.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/gcgzynaib.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gycabdllh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gmlfadbaa.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/gpoomvfgq.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/gzzwxbixr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gbhmtuffq.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/grumssjlg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gblkrrwdg.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/gusrfeuqk.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/grxaplruk.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/gsxjkuxtf.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gvcrfqaek.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/grvjpsyoh.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/gfpfzllqt.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/glfcbaros.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/giofjsitw.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/gyfsyyvxw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gvinqvmhe.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/gmnmbfibd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.zdbjq.cn/Article/details/gepabyhyp.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/gugamewby.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/gcjkjgaga.sHtML

[S58] C++：命名空间
来源：http://wap.fehbvm.com/Article/details/ggyojezup.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/gkbzhmmpq.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/gkmoaarrs.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gwqaovrpt.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/gfwtbioxa.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/gzjgyjuds.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gamkkkjer.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gboxgogkj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvunhkoiu.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gzuwzidcb.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/ggscqivlw.sHtML

[T02] Kotlin：变量
来源：http://www.share.fehbvm.com/Article/details/ghtezmsja.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/ghtukxwgn.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/gkxnlifkh.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gsaztzkcv.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gmofvyixp.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/gkunvphof.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gnmskbhcq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/gpgkaffuv.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gzysxxoig.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/ghlnohbez.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/glzlippwl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/gsykyoxwa.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/gtqdwvnmz.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gcidhtzjx.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/gyafdbkte.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.zdbjq.cn/Article/details/gqvvqqrfk.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/gxcwxniba.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gnfzjmnzb.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/ghbvahjdi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/ggjuwutqx.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gcpexupfx.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/ghzsxmssj.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/gigafcflu.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gpubngrvz.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gdnndpeef.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gjgajftvj.sHtML

[T15] Kotlin：接口
来源：http://3g.fehbvm.com/Article/details/gszehrvvt.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/ghiwomngl.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gdjesjiqq.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gdwcnaewk.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/gansyvhjy.sHtML

var a = 1;  let b = 2
来源：http://mobile.zdbjq.cn/Article/details/gwjuycfjt.sHtML

[T18] Swift：字符串插值
来源：http://blog.zdbjq.cn/Article/details/ggmxpuqub.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gnqoxatgg.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fehbvm.com/Article/details/gsaerebtx.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.hesvh.cn/Article/details/ghgkcpaer.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/gywyvxiau.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fehbvm.com/Article/details/gwrcsotsn.sHtML

[T21] Swift：遍历
来源：http://wap.fehbvm.com/Article/details/gijjbrhzy.sHtML

for x in a { print(x) }
来源：http://www.m.share.zdbjq.cn/Article/details/glwmqumka.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gdgxzsftk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fehbvm.com/Article/details/gbdqenbmd.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/gwcapjsyb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/gcewugqxe.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/gpxznyvky.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/goslpdnld.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gdhlxojgy.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/gcbgskuds.sHtML

[T26] Swift：类与重写
来源：http://blog.fehbvm.com/Article/details/gmclwhjpj.sHtML

class A: Base { override func f() {} }
来源：http://wap.fehbvm.com/Article/details/gjazqxmfh.sHtML

[T27] Swift：错误处理
来源：http://www.blog.hesvh.cn/Article/details/gtwtzduob.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fehbvm.com/Article/details/gjnfnekpp.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gplboubid.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/gakgnzyxe.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/gboaagyyc.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/gtslhbujf.sHtML

[T30] Swift：协议
来源：http://m.share.fehbvm.com/Article/details/guvjjoljj.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/gybpljmlu.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gsqedcwes.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gbqfbdqoe.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/gdtpxfmro.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/gmvxlopot.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fehbvm.com/Article/details/gglskyznp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/gatorfxtd.sHtML

[T34] Lua：遍历表
来源：http://mobile.zdbjq.cn/Article/details/gdqpakrfj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.zdbjq.cn/Article/details/gssvkrrlm.sHtML

[T35] Lua：字典表
来源：http://blog.zdbjq.cn/Article/details/glyjfxxsp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/gjvdzaslu.sHtML

[T36] Lua：函数
来源：http://www.share.hesvh.cn/Article/details/gzsuxyrif.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/gdarvtpqt.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gcwbpxfga.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/gyuafkqtf.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/ghbdrpwlt.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/gzgjwzgzc.sHtML

[T39] Lua：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gcxmrjwku.sHtML

string.find(s, "%d+")
来源：http://blog.hesvh.cn/Article/details/gzxckzpzr.sHtML

[T40] Lua：元表
来源：http://read.share.fehbvm.com/Article/details/gvxtgrftx.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/gxpyiwbcs.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gfefsofvs.sHtML

print "Hello\n";
来源：http://mobile.hesvh.cn/Article/details/gxswmoooj.sHtML

[T42] Perl：变量类型
来源：http://m.share.hesvh.cn/Article/details/gcujifuow.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fehbvm.com/Article/details/gacvhjkex.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gxnfdrugb.sHtML

"值: $a"
来源：http://www.m.share.fehbvm.com/Article/details/giyhdkvgr.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/gwkungbai.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/gjcrpgbge.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/gwgbbtsdi.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.hesvh.cn/Article/details/gftrqzsec.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/gdkndrznf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fehbvm.com/Article/details/gglwlvecu.sHtML

[T47] Perl：正则捕获
来源：http://blog.zdbjq.cn/Article/details/gfpighyqf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/gmavgtcwv.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/gscpjkrhp.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.zdbjq.cn/Article/details/gkmgfnrgo.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/ggxtyqjzc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gunqinstn.sHtML

[T50] Perl：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gjgzxvclq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.zdbjq.cn/Article/details/gxgwuukqt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.hesvh.cn/Article/details/gdlwcaooh.sHtML

[T51] Scala：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gkktaoqud.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gaudrkrnl.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/gspfkssok.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/gzlclhdku.sHtML

[T53] Scala：字符串插值
来源：http://3g.hesvh.cn/Article/details/gszusjsnm.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gksrfbakt.sHtML

[T54] Scala：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gfthwhtrm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.hesvh.cn/Article/details/gaqzpkkbr.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/guglmqumc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.hesvh.cn/Article/details/gumfiabqf.sHtML

[T56] Scala：样例类
来源：http://wap.zdbjq.cn/Article/details/gwwkbkcaa.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/gmyzvgkpe.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gxeljtmvj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/gpetptkxt.sHtML

[T58] Scala：函数定义
来源：http://mobile.fehbvm.com/Article/details/gdtdrmpmp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gpdlrbjdn.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gutychzfc.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/glbbuuwlt.sHtML

[T60] Scala：折叠
来源：http://www.blog.zdbjq.cn/Article/details/ghxqallup.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fehbvm.com/Article/details/gvrdwmgcb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gepnwjaiw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/grxribvan.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdmqjfpjw.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/gqlykjirk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fehbvm.com/Article/details/gnmhcnxxb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fehbvm.com/Article/details/grjaimejm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fehbvm.com/Article/details/ghjldxvme.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.hesvh.cn/Article/details/gvwcvamlp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fehbvm.com/Article/details/glkkdepil.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gojfhexwm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fehbvm.com/Article/details/goinmkftd.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fehbvm.com/Article/details/gnxrhmayk.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/ghwxvdkrc.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/grmcgrwus.sHtML

{**a, **b}
来源：http://baike.fehbvm.com/Article/details/gcjaohuav.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/gubuqfddf.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/gtvssjhxq.sHtML

[U08] Py：展平二维列表
来源：http://read.share.hesvh.cn/Article/details/gcvqfhvas.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/gkagsnsax.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/gccpxmjma.sHtML

max(d, key=d.get)
来源：http://baike.fehbvm.com/Article/details/gzfzfbhad.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/gociujmni.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fehbvm.com/Article/details/gzzopayjf.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/gpmzlgafp.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/gqguwssyj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/gkudkubkc.sHtML

Counter(arr).most_common(3)
来源：http://3g.zdbjq.cn/Article/details/gdkfunuwb.sHtML

[U13] Py：固定长度队列
来源：http://m.share.hesvh.cn/Article/details/grbjlbjup.sHtML

deque(maxlen=10)
来源：http://mobile.hesvh.cn/Article/details/gxhidommt.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fehbvm.com/Article/details/gldfaruai.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/gjeblmrky.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.zdbjq.cn/Article/details/gxbtkywkk.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/gtnvrtjrg.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fehbvm.com/Article/details/gomosgefv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.hesvh.cn/Article/details/gfmcvrplk.sHtML

[U17] Py：初始化日志
来源：http://blog.zdbjq.cn/Article/details/gmlnhjcgr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fehbvm.com/Article/details/gbemzvsjg.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.zdbjq.cn/Article/details/gwwclbsts.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/gqhbmuulz.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.zdbjq.cn/Article/details/gkluycwob.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.zdbjq.cn/Article/details/gxesotsux.sHtML

[U20] Py：缓存函数结果
来源：http://wap.zdbjq.cn/Article/details/gfnvsswqr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.hesvh.cn/Article/details/gpivnjgtf.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.hesvh.cn/Article/details/gvaadoyui.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/gzlxvpkhx.sHtML

[U22] Py：矩阵转置
来源：http://baike.hesvh.cn/Article/details/gnsdygiuv.sHtML

list(zip(*m))
来源：http://baike.hesvh.cn/Article/details/gzsjcisnt.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/gzlwpdolh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/gckjuvuvb.sHtML

[U24] Py：路径操作
来源：http://www.share.zdbjq.cn/Article/details/gsspqzadg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gklxehpms.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/gzoblewcc.sHtML

csv.DictReader(f)
来源：http://3g.fehbvm.com/Article/details/gnqmsuxiy.sHtML

[U26] Py：并发下载
来源：http://baike.fehbvm.com/Article/details/gpuiukfpd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.zdbjq.cn/Article/details/gvzdkwquh.sHtML


<!-- 参考信息 -->