代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gebcaxakc.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.zdbjq.cn/Article/details/gsimhizdp.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/gkvfgycwy.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gufbxkbgq.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gsksszkkk.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/gtbufqhxv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.hesvh.cn/Article/details/gwbzyrjet.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/gzojuspvn.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/ghhlfuswd.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gllxmbckk.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/gbkzkdoly.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/ghqoeuusb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/gvqkgmzxf.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gaahafoze.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/ghqwqdttc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gkrvlpaof.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gvqfdeisj.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gtdrezkix.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gilijxfhx.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/ghjqgtlwa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/gttkyrdrl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gwufzdbah.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gmpnmxkle.sHtML

[S12] C：写文件
来源：http://blog.hesvh.cn/Article/details/gfkhnihwg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gmxbhhukr.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gxujsotss.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/ghwstzlrh.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/gftggsxvs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gvtlmaicd.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/gqpjxqxud.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gwdcyiqsd.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/gtlyafisw.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gepgzarrv.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gyinppqwb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/golbawqbw.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/gttgtxnbk.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gbupwmfzg.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/giemcdudb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gfjcedxhb.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gpxcgzzkg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gnillvfwo.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gogfnhbqe.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/gupbpknaj.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gdtvstciv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/gxdhmuvto.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gbwphbeys.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gymzevbof.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/gwhprrtzr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/geljdssur.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gqrwsdbgu.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gibuuiflg.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gyyenkoho.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gqpamvwuw.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gvjmoyhbe.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/geuwafvti.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gbiqimkmn.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/gmwqbfxxm.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/genbwdtul.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gtsjmjrgy.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gepinykit.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/gqikyadbh.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/gghdyzcsa.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/ghsfxysqo.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/gflshrrha.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gdkqesrkn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcspojkrm.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/giymilzbu.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/gfrzvemfc.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/gmwizqrra.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/giuikphjv.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gfgppdjre.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/gnbrseift.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/guwouhxlw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/glqalwndp.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/gxehognos.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/ghjwgbhwu.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/golfqgscq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/ghohtvdgm.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gdbzjzsly.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/guhcoebwn.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gabrxjoau.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gogtifmgl.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/ghjudbknc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/gkrtqoabv.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/gpeywarca.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/gtsheorcy.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/gfnzzgawc.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/gkimfmnlu.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/gjxrvgwuf.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/gubxukyre.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/gquypngsv.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gdqjpszlo.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gvcbxjrxy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.hesvh.cn/Article/details/gihwnktcf.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gjbhstrmv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gbopektno.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gvgkwqtub.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/ghuapamno.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/glzthroqy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fehbvm.com/Article/details/gycnpatus.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gltuxelxf.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/goyawdhoc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gahzopvgw.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/ggcutohvv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gxqazjsxs.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gdtoivbai.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/gotbcmmaa.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gbkhlnhky.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/gjhdgemme.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/ghiczkoqn.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/geuuqwzyx.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/gptnrkrvy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/giqnknolu.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gbteykmln.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/gcdearzcf.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/gygvlgrkg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/goshmbkel.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/geamuipjw.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gqciatcyn.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gipjeiqeu.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/gquknswoh.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/gihqhfgnk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.zdbjq.cn/Article/details/grvwukslh.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/gsotfxhni.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/gafsfpnig.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfztyrxet.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gcaoncdlg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gghgpwhal.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gfdpfqcto.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gpwpqmkaz.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/guezsadan.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gmnxkqowm.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/gwseebrbu.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gswvoezot.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gjqabyvwx.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gksinreym.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gnrghlmro.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.hesvh.cn/Article/details/ggyfxvkzn.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/goxpahcat.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/gaptrgcvq.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gyqckzfcc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gahcutzmd.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gydtylqjk.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/gbtrnuikt.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.zdbjq.cn/Article/details/gzdvqjqgd.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gcgzswuxv.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gmqsplwwy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/ghcvxdxoy.sHtML

[T11] Kotlin：协程
来源：http://wap.hesvh.cn/Article/details/gmqgsijbh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fehbvm.com/Article/details/gjxwkqrpy.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/gujxipnls.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gvhxvqths.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fehbvm.com/Article/details/guzdibnwf.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/gdheghyxv.sHtML

[T14] Kotlin：循环
来源：http://wap.hesvh.cn/Article/details/gxaemmlnv.sHtML

for (i in 1..10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gghjtaevm.sHtML

[T15] Kotlin：接口
来源：http://baike.zdbjq.cn/Article/details/gewbgbgof.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/ggynvbdhi.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gpmoyvtjl.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gvibcpvve.sHtML

[T17] Swift：变量与常量
来源：http://read.share.zdbjq.cn/Article/details/ggjxuptsj.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fehbvm.com/Article/details/gfzsxtsxs.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/giglrondm.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/ggfpayexw.sHtML

[T19] Swift：可选绑定
来源：http://m.share.zdbjq.cn/Article/details/gtpqqtamx.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/ghbumyrtf.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/gekuclupq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/giaijevsp.sHtML

[T21] Swift：遍历
来源：http://mobile.zdbjq.cn/Article/details/grpegcqxw.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/ggruzugku.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/grjflwigq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fehbvm.com/Article/details/gasfztgxl.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/gkwfafgza.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gyrjpmdud.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/grfhpbcpd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gpgqcxcva.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/gqbiubrpa.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/giuottzot.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/gwmkxclow.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/ghrvykdcn.sHtML

[T27] Swift：错误处理
来源：http://blog.zdbjq.cn/Article/details/gqdaoqkme.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/ghtbwxnwu.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/gooebmfgs.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/glwhqzrmo.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/ghgmzdctp.sHtML

guard let x = opt else { return }
来源：http://read.share.zdbjq.cn/Article/details/gxlcxtgxs.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gsvqemfzt.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/gmedqouxk.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gtotbqakc.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/ghptqowwx.sHtML

[T32] Lua：局部变量
来源：http://read.share.fehbvm.com/Article/details/gsdkfwhmv.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/gbehlajcx.sHtML

[T33] Lua：表（数组）
来源：http://blog.fehbvm.com/Article/details/gsbtptpyt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fehbvm.com/Article/details/gbqkuxqmm.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/gkmrhuxci.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/gzmbpwzft.sHtML

[T35] Lua：字典表
来源：http://www.share.fehbvm.com/Article/details/gjuoqfaff.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gtarzhocl.sHtML

[T36] Lua：函数
来源：http://m.share.zdbjq.cn/Article/details/giosasraa.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/gmogvvavy.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gyngfkjfi.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/gpomvdsre.sHtML

[T38] Lua：条件
来源：http://www.blog.fehbvm.com/Article/details/gsasdusoq.sHtML

if x > 0 then print("正") end
来源：http://read.share.hesvh.cn/Article/details/gvbxdqsdz.sHtML

[T39] Lua：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gjeujfpyh.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/gzxwmyeus.sHtML

[T40] Lua：元表
来源：http://www.m.share.fehbvm.com/Article/details/gshcnevnx.sHtML

setmetatable({}, { __index = base })
来源：http://baike.hesvh.cn/Article/details/gjifsciiu.sHtML

[T41] Perl：Hello World
来源：http://www.share.hesvh.cn/Article/details/gitqfchch.sHtML

print "Hello\n";
来源：http://read.share.hesvh.cn/Article/details/gbennpfkp.sHtML

[T42] Perl：变量类型
来源：http://blog.fehbvm.com/Article/details/grutfjfgn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.hesvh.cn/Article/details/gloyxlbfy.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gmjdhwbjo.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/gqerkyysn.sHtML

[T44] Perl：条件
来源：http://baike.hesvh.cn/Article/details/gpwtsovmx.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fehbvm.com/Article/details/gwajjriqo.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/glnbzjmpw.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/gmknjbzfi.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/gctimiclq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/gftcayhog.sHtML

[T47] Perl：正则捕获
来源：http://blog.fehbvm.com/Article/details/gdqbfwieq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.zdbjq.cn/Article/details/gacrgutyq.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/gvexdsfom.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fehbvm.com/Article/details/gnlzsjdut.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/gninzuhym.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gvizbaatj.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gbaoqixeu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fehbvm.com/Article/details/gyfarodmn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/ghsnpqszu.sHtML

[T51] Scala：Hello World
来源：http://blog.fehbvm.com/Article/details/goinhjwdg.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gsctabdrg.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/gmftmathv.sHtML

val a = 1;  var b = 2
来源：http://blog.hesvh.cn/Article/details/gisfczltl.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gosvqjwad.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/gqxjszkgn.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gczyhlwjg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/gbveqgvox.sHtML

[T55] Scala：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gterckuch.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.hesvh.cn/Article/details/gpzcrbecz.sHtML

[T56] Scala：样例类
来源：http://3g.zdbjq.cn/Article/details/gllvuzeia.sHtML

case class User(name: String, age: Int)
来源：http://www.share.hesvh.cn/Article/details/gddhmrnmz.sHtML

[T57] Scala：模式匹配
来源：http://baike.fehbvm.com/Article/details/gwktzeasg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fehbvm.com/Article/details/gidnggjol.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/gdsmdnoip.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/gtxposdht.sHtML

[T59] Scala：循环
来源：http://www.m.share.hesvh.cn/Article/details/gxzbyycyg.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fehbvm.com/Article/details/gmqejyaus.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/gfqguaefz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.zdbjq.cn/Article/details/ghyqnegij.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfcslqiei.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gtlaaqtsf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggxivpqfk.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/gydoyjbza.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/gdsewisoq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.zdbjq.cn/Article/details/gyaidrifm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.zdbjq.cn/Article/details/gwiguzmrl.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.zdbjq.cn/Article/details/gxyxyhjgn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.hesvh.cn/Article/details/ggfxdqfjx.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/gmngasrvi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.zdbjq.cn/Article/details/gwgqoxgvx.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/gfxbwkdtm.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gcdlnydqq.sHtML

[U06] Py：合并两个字典
来源：http://3g.zdbjq.cn/Article/details/glrvrhsjp.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gqvsdrvmj.sHtML

[U07] Py：反转字典键值
来源：http://m.share.hesvh.cn/Article/details/gsyfkrntl.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/gzrnqpdez.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.hesvh.cn/Article/details/gjbiaiqnh.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/gvpuuerfz.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fehbvm.com/Article/details/goetheutq.sHtML

max(d, key=d.get)
来源：http://www.share.hesvh.cn/Article/details/gmjjeaxlv.sHtML

[U10] Py：按值排序字典
来源：http://baike.zdbjq.cn/Article/details/gxlpvcgyl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/gucuvilkm.sHtML

[U11] Py：生成器表达式
来源：http://www.share.hesvh.cn/Article/details/gydguwcic.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/gqmfshbsp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fehbvm.com/Article/details/grcdrwlgz.sHtML

Counter(arr).most_common(3)
来源：http://baike.hesvh.cn/Article/details/ghucezyer.sHtML

[U13] Py：固定长度队列
来源：http://baike.zdbjq.cn/Article/details/gavhfxsrw.sHtML

deque(maxlen=10)
来源：http://read.share.fehbvm.com/Article/details/gcdmtepus.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.hesvh.cn/Article/details/guiogvdff.sHtML

defaultdict(list)
来源：http://blog.fehbvm.com/Article/details/gnzouxila.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fehbvm.com/Article/details/grcftrofx.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/grokcheax.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fehbvm.com/Article/details/gcxvhxooi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gnvjekmlz.sHtML

[U17] Py：初始化日志
来源：http://read.share.zdbjq.cn/Article/details/gpzejnmwa.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.zdbjq.cn/Article/details/gktmfcotw.sHtML

[U18] Py：预编译正则
来源：http://m.share.zdbjq.cn/Article/details/gzefotdsz.sHtML

pat = re.compile(r"\d+")
来源：http://baike.zdbjq.cn/Article/details/gtqiwjzue.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.zdbjq.cn/Article/details/ggqhnfjee.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fehbvm.com/Article/details/guqnvfrbo.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.hesvh.cn/Article/details/gfvwugcxe.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fehbvm.com/Article/details/gnokboxci.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.zdbjq.cn/Article/details/gzexmsahx.sHtML

@contextlib.contextmanager
来源：http://www.blog.zdbjq.cn/Article/details/godlzuoso.sHtML

[U22] Py：矩阵转置
来源：http://www.share.zdbjq.cn/Article/details/ghockuttd.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/gjzneinth.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.hesvh.cn/Article/details/ghtjkoepb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.zdbjq.cn/Article/details/gevhbcbhm.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/goxdiqtnk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gopqcnuma.sHtML


<!-- 参考信息 -->