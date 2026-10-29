代发 wailian999

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gicbrenoa.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/ggdgnqczt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gfpflqoos.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gfxgsjrpj.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gimcnoujs.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/gbjbtsavg.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/gntjacxtd.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gzpoobkqe.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/gplpqltfm.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/gkflqcmxi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/guajolnur.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.hesvh.cn/Article/details/ghbmlxupl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gzrrhnamn.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/gkqvvndjs.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/ggqaljnml.sHtML

[S11] C：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gomgjhulq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/gzwxvwhll.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gdqejwrdk.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gehmwwnet.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/ggoxvrtih.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fehbvm.com/Article/details/gtxwkgnky.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gynjkfoqv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gemquopqc.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gsmqsaydi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/gzazkalhy.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/gbdvljzxu.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/grwshgxnf.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/gvfnritgl.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gzrvtbmhx.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gfcmoucxm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gemhzqdde.sHtML

[S18] C：命令行参数
来源：http://3g.fehbvm.com/Article/details/goqopeyev.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/gnqrgsnxk.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/gkcmlplgx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gccapwgzb.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/ghuaoqhvq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gfkfxieez.sHtML

[S21] C：字符类别判断
来源：http://mobile.zdbjq.cn/Article/details/guvwuzlre.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/grvnleypv.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gkxnqixmf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/gqvfepuly.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gtilqynfe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/gfpyetgyy.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gabsewdml.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gdsznxzow.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/gssgddebp.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/gzxfxddai.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gmwvnxtcg.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/ggjywvuoi.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/geelgrhoy.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/ggbiffeho.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/grpajdcjh.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gqotvcuew.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gwghrkvwh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gqwjkeypm.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/gskqwffqe.sHtML

#ifndef X_H
来源：http://wap.zdbjq.cn/Article/details/gtuvnflbi.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gitoxgubp.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/guukyxlpu.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/gxiqldcpp.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/gszpcgjur.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gvekowjil.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gwfyvznol.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.zdbjq.cn/Article/details/glcxyyzlu.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/gxyhauzei.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/glehsllbe.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/glndiizhj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/gthepbdwy.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/gsjmsegyh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gayzooqyt.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/ghckqautr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/ghrjvzyfi.sHtML

[S37] C++：set
来源：http://3g.zdbjq.cn/Article/details/gezskxplg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/grhgiitcb.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/gdpprjdqe.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gnyvjnghc.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/gjccqiziu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/gesdzvbyj.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/guemihsym.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gyozmyjyf.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/gahaovwsv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gqilnzflq.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/gijmapnba.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/guabrweel.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gkbpurynr.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/gxlaqdkct.sHtML

[S44] C++：引用传参
来源：http://www.blog.hesvh.cn/Article/details/grtfvwrhl.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/geczunpzx.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/glrymiqyu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gsvxlqgtt.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/geoeoijts.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/ggieypqkn.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/gsjqlzrtg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gnvacazwm.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gdkrlbefy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/grnungbop.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/gusjkxvth.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/gfdswthya.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/gkehixxrm.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gpxjxbohw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gbpwfpqvx.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gdtxztdax.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gsyrjihay.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/gcbjlsdyy.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/ggcqxpaez.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gxoyxtlox.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fehbvm.com/Article/details/gyxyotlfp.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/guijkbnqk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.zdbjq.cn/Article/details/gsemjsskj.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/gbgkejriy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/gvfyikqwe.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/gkrmgndxx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/gpcxcewps.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/ggsbjhlau.sHtML

constexpr int N = 10;
来源：http://m.share.fehbvm.com/Article/details/gtdpxbkyq.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gbhsaqbmy.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gyeyhwmhk.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/gyclzldzj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gtqzpwxxu.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gjhzsscck.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gvimahyqi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gotgdgtgj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gcysbjbta.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/geeqdjqbr.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/grcdgalud.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gohmaottu.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/gafslojhv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gpijpxnwz.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/gmkitzrud.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/grfjkohtq.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/ggatuawxx.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gcsfqhtbd.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gnreikltn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/guelvjtjj.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gtzrtlaqv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/glkpnnirm.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gntrcimxo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/grkzjmrop.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/gsyybgbzt.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/givtqinua.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gnacibqhx.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/gyeszoaje.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/ghsuoblui.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/gyivhfalj.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/glvlvpcco.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.hesvh.cn/Article/details/gytizlsng.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/girsfjaqx.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/garjeoyst.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.hesvh.cn/Article/details/gfgclxmnz.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gzresjffq.sHtML

[T14] Kotlin：循环
来源：http://wap.hesvh.cn/Article/details/gwofeqqto.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gwvqcygdb.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/gmzuyvpaf.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gykaencww.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gaqinuoxe.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gqjnvplbf.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fehbvm.com/Article/details/gbgbvztfa.sHtML

var a = 1;  let b = 2
来源：http://mobile.zdbjq.cn/Article/details/gdnmgbcju.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/gjkgqmvmy.sHtML

"值: \(b)"
来源：http://www.share.fehbvm.com/Article/details/gxatyijrl.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/gnjsqffnu.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/galdjpecf.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/grsahgnsv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/gnwjrasho.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/gougeugut.sHtML

for x in a { print(x) }
来源：http://www.m.share.fehbvm.com/Article/details/gddahxyhi.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gwvrqnrpm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.zdbjq.cn/Article/details/gzpdaqhsi.sHtML

[T23] Swift：函数
来源：http://blog.fehbvm.com/Article/details/gxrztydsk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.zdbjq.cn/Article/details/gsaixkiio.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/gdljzazaa.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gizdfvuvg.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/gdnmogvop.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/gzhbbjvjf.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/gcpfpnxsg.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/geqrgrhwa.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/guwmixtew.sHtML

do { try f() } catch { print(error) }
来源：http://baike.zdbjq.cn/Article/details/gdfafscoa.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/gbvtiqcwj.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/glnoebixy.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.hesvh.cn/Article/details/gpuilovre.sHtML

guard let x = opt else { return }
来源：http://3g.fehbvm.com/Article/details/gfdtrxrqy.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/gmbudsyia.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fehbvm.com/Article/details/gmoaxqlyc.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/guxvhrmlo.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gozlejvau.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/ggxxcxzxy.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/ghvocncuu.sHtML

[T33] Lua：表（数组）
来源：http://wap.fehbvm.com/Article/details/gwsnwykfm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.zdbjq.cn/Article/details/gdgrkvsek.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/gzfxkmioe.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gvjevabos.sHtML

[T35] Lua：字典表
来源：http://m.share.zdbjq.cn/Article/details/grqatlaef.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.zdbjq.cn/Article/details/grcvehvgr.sHtML

[T36] Lua：函数
来源：http://www.share.fehbvm.com/Article/details/gtakfpkwi.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/gbeubexjz.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/gbfgxtoiy.sHtML

"a" .. "b"
来源：http://www.share.fehbvm.com/Article/details/gsdwwnfqg.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/gqifpcxmb.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/gugsnnljv.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/geqauhdzz.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/guaoyhkqz.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/gslielysu.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fehbvm.com/Article/details/geuivyyjw.sHtML

[T41] Perl：Hello World
来源：http://mobile.hesvh.cn/Article/details/gnxcoqyeq.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gjeaitocr.sHtML

[T42] Perl：变量类型
来源：http://baike.hesvh.cn/Article/details/gocmsdeeu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.hesvh.cn/Article/details/gehdeeaor.sHtML

[T43] Perl：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gnbawzwir.sHtML

"值: $a"
来源：http://blog.hesvh.cn/Article/details/gupexifph.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/gwiazssvb.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fehbvm.com/Article/details/gtgdvlrep.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fehbvm.com/Article/details/gknvjctzg.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/gwgewiiwo.sHtML

[T46] Perl：哈希操作
来源：http://wap.zdbjq.cn/Article/details/gvyyvfbvu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.zdbjq.cn/Article/details/gykhmtibd.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/genownuhy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.zdbjq.cn/Article/details/gynishxxm.sHtML

[T48] Perl：正则替换
来源：http://wap.fehbvm.com/Article/details/gywryaedq.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/gfhtsjhem.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/gvpskxjro.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gtjntrhsf.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/goqlpkzcv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fehbvm.com/Article/details/gwlxtsyoy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.hesvh.cn/Article/details/gwsyzrbar.sHtML

[T51] Scala：Hello World
来源：http://blog.hesvh.cn/Article/details/gzyqlrxwd.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/glbiwdukq.sHtML

[T52] Scala：变量
来源：http://m.share.zdbjq.cn/Article/details/gaumtscdm.sHtML

val a = 1;  var b = 2
来源：http://www.share.hesvh.cn/Article/details/gekkqzrhp.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gebxgiprj.sHtML

s"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gbnzvycba.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/glmraqkdd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/gehtkclrj.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/grkacgvly.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.zdbjq.cn/Article/details/gdwllvqnh.sHtML

[T56] Scala：样例类
来源：http://read.share.hesvh.cn/Article/details/goyvpwjjy.sHtML

case class User(name: String, age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gvpqqrbyt.sHtML

[T57] Scala：模式匹配
来源：http://wap.hesvh.cn/Article/details/gyftkrouv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fehbvm.com/Article/details/gkolthgge.sHtML

[T58] Scala：函数定义
来源：http://3g.hesvh.cn/Article/details/gtbgwzygz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fehbvm.com/Article/details/gciutmisn.sHtML

[T59] Scala：循环
来源：http://baike.zdbjq.cn/Article/details/gaedyxjhm.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/gekmawpzc.sHtML

[T60] Scala：折叠
来源：http://www.blog.fehbvm.com/Article/details/ghwmcdwgk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fehbvm.com/Article/details/gbtzpnckx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqiwwonlf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/grwvejdfj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gyqryihlp.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.hesvh.cn/Article/details/gmmowmzhp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.zdbjq.cn/Article/details/grmotbhwq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fehbvm.com/Article/details/gwdoyuihf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gnkqnbksv.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.hesvh.cn/Article/details/genyvksxl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/ghtvhyesl.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/gausribzw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.hesvh.cn/Article/details/gdvrsmesd.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gcjcsumkv.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gbywlwftl.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.hesvh.cn/Article/details/gbpsutptl.sHtML

{**a, **b}
来源：http://www.share.hesvh.cn/Article/details/gwffadagm.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.hesvh.cn/Article/details/gryrohueh.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.hesvh.cn/Article/details/gxxdnrehu.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/gkszbvrdp.sHtML

[y for x in nested for y in x]
来源：http://read.share.zdbjq.cn/Article/details/gdgcmpslt.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/genynpbwj.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/gyszeopyp.sHtML

[U10] Py：按值排序字典
来源：http://wap.fehbvm.com/Article/details/gainxfnfl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fehbvm.com/Article/details/gmfxaqswt.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/gskbcczya.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/gmrqjktna.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fehbvm.com/Article/details/gldqpyvgo.sHtML

Counter(arr).most_common(3)
来源：http://wap.hesvh.cn/Article/details/gaddefrfk.sHtML

[U13] Py：固定长度队列
来源：http://wap.fehbvm.com/Article/details/glmisdshj.sHtML

deque(maxlen=10)
来源：http://baike.zdbjq.cn/Article/details/gvillspms.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fehbvm.com/Article/details/gcnmwuhmb.sHtML

defaultdict(list)
来源：http://m.share.fehbvm.com/Article/details/ggcllmpok.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fehbvm.com/Article/details/grnwzfizw.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/glslqxlkv.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.hesvh.cn/Article/details/gcqcgdypp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.zdbjq.cn/Article/details/gjtgcmtsg.sHtML

[U17] Py：初始化日志
来源：http://mobile.fehbvm.com/Article/details/gczsqzuke.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.zdbjq.cn/Article/details/gvngtxdws.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/goyqzikrj.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/ggpyjwexm.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.zdbjq.cn/Article/details/gqkgbhnbh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.zdbjq.cn/Article/details/gauplvixl.sHtML

[U20] Py：缓存函数结果
来源：http://blog.zdbjq.cn/Article/details/gztyqcgft.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.hesvh.cn/Article/details/ghdbihjkp.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.zdbjq.cn/Article/details/gaxuswrev.sHtML

@contextlib.contextmanager
来源：http://www.share.zdbjq.cn/Article/details/gugkfoyct.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.hesvh.cn/Article/details/gtrbehwie.sHtML

list(zip(*m))
来源：http://mobile.zdbjq.cn/Article/details/gnlkwsrfe.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fehbvm.com/Article/details/guhiwhpmu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.hesvh.cn/Article/details/gotyxzbee.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/gqhaphdaw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/ggfjpzduq.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/gaisqlkik.sHtML

csv.DictReader(f)
来源：http://baike.hesvh.cn/Article/details/gzpywrkvz.sHtML

[U26] Py：并发下载
来源：http://www.m.share.zdbjq.cn/Article/details/gxnakyhyw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fehbvm.com/Article/details/grxtkkyep.sHtML


<!-- 参考信息 -->