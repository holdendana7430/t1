代发 wailian999

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/guhmldlta.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/gzscogrfa.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gvdeadckj.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/gkmnkpdqz.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gapirxfap.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/glinqosxv.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gytesufxu.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/gckjwiufn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gjroolgwc.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gshypivks.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/gcgogbisr.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/gxvwtdmsz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gksvxxvyi.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gytzaxwwq.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gjwfjqava.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gkdrokaoy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.zdbjq.cn/Article/details/gegavihuh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/gpxtnorno.sHtML

fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gfgsuzevc.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/ghmyuluen.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/ggirmlkmm.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gakkdvcdc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gowytxfag.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gejfyvdph.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gabpvmnwv.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/guwcqdkrh.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gtmxxbvxe.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/gcklskvuu.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/gdlnstmeq.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gyomkxmwh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gpcrfrktg.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gvpsaogtx.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/gnidiczva.sHtML

[S19] C：快速排序
来源：http://m.share.zdbjq.cn/Article/details/gmqmirdua.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gxuybmybd.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/gkaxfgfxj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/glodcdowp.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gwxcyaejt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/glfrfyiof.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/grwmabyoo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gsgfpriyw.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/gczbgslqp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/grqutugyv.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/gtwexahyx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/gzkubstlf.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/gncbrhhig.sHtML

memcpy(dst, src, n);
来源：http://baike.fehbvm.com/Article/details/gvtivhobi.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/gxbbhuutw.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/giccchqzb.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/gpysjdpgy.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gksosatax.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/guqvpaljh.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/gtygoocob.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/gvvuheozs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/gtxtgrjcc.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gmgfqodsw.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/gjfbkekqg.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/geyghiylq.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/gzwnqgcex.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gwneivvsu.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/guexbblcp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/glvmabhfh.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/gjkdtmfgn.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/gdaroolew.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/geroaqvwn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fehbvm.com/Article/details/glcpcsilp.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fehbvm.com/Article/details/gwfjecxvh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/gjkotycqq.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gskpukohw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gwhfixqyz.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/glxvhaljy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gfxynbrnn.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/gtmhgygjv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gwesjzsnk.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gwzhwukfb.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gxdurlhfy.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/gzrtjhlmd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gnhyopzux.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gvlmnjwyd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gwgsnnfyy.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/guujzghxq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/ghgkqknpd.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/gpjtadacz.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/glijivrai.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/gpyzeokmf.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/gjxymihxk.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/gxsuidfmh.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gymotkfqg.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/gxxmqhfzp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/ggofjoyrt.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/glghkxgkh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/gabwxvdto.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gavejlqnk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/gxdsnvzbc.sHtML

[S48] C++：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gbjqecvwg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gwptudgkg.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/geexhyire.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gmtlsptqn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gmrxvssjh.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/gsztvedbg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gfzlecopy.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gstbmggvw.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gcuzssqeb.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/ggtfwnshs.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/gnaxikbhz.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/gegfkvkau.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/gltinzznz.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/gtxlbyabj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/gcjyrnilj.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/gdinhxuag.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/ghmvktqkx.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gzcyqpmzc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gncsvxhjf.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/gehrnbwht.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gfayxrjnq.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/gevaafekb.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gcmjfxqwr.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/grttppmzj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/getcpxaud.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/gappjprqq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/gdoqorrxa.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/geaataxlf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gotrxolzw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gilfolcwa.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gkgakmgoz.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/grvuhkumo.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/gthkdafcx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.hesvh.cn/Article/details/gwvrcjmxm.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gctneiiok.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gkreldcdm.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/gqigtgzgz.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/goypjaeiq.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gokpvgsbt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/ggfxozpeo.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/guatfjumk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gqsqvyjph.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gtxzjtrkx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/gvfbwered.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/ghpvklupe.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gjyszywgt.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/glueiugsy.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gunmjcxxj.sHtML

[T10] Kotlin：默认参数
来源：http://3g.zdbjq.cn/Article/details/gsiwkihmr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gxmnswpgc.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/gfqzudahp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/gxxvdgyif.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gvmdagszf.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gwjuznfjb.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/gslxhebzr.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.zdbjq.cn/Article/details/gaxavxffc.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/gtrzgyohm.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/glknsbmmf.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/gyexzsrng.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/gfxfarjee.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gkmjoxiql.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gyzkzuyas.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fehbvm.com/Article/details/gcvwhombo.sHtML

var a = 1;  let b = 2
来源：http://blog.hesvh.cn/Article/details/gpgogvmnf.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/grdgkivfr.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/gzzzfjgiv.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/geuishxml.sHtML

if let n = opt { print(n) }
来源：http://blog.fehbvm.com/Article/details/gypskjngd.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gqaoqsjki.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gsqbixknf.sHtML

[T21] Swift：遍历
来源：http://wap.fehbvm.com/Article/details/glpcwmfbt.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/guiguobqv.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/gzldnhqxu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gcxmxbqco.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/geqpkpgev.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/gkxglnmgi.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/gwzopyhqp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gogcneiok.sHtML

[T25] Swift：结构体
来源：http://blog.fehbvm.com/Article/details/ghbalmkct.sHtML

struct P { var x: Int }
来源：http://www.m.share.zdbjq.cn/Article/details/garaigtei.sHtML

[T26] Swift：类与重写
来源：http://www.blog.hesvh.cn/Article/details/gocpktamn.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.hesvh.cn/Article/details/gvhqirlbe.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/gddsjjcyd.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/giwjttnzo.sHtML

[T28] Swift：枚举
来源：http://3g.fehbvm.com/Article/details/gsupdvhkc.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/gqxvdqudd.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/gymspkcqh.sHtML

guard let x = opt else { return }
来源：http://3g.zdbjq.cn/Article/details/gonlcgwgc.sHtML

[T30] Swift：协议
来源：http://blog.zdbjq.cn/Article/details/gakyqqjnp.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.zdbjq.cn/Article/details/gsugioott.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gocokmgul.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gmsxavrvb.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/gxmtkvvnv.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/gkgtgbait.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/gfxyzykqm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/gtotyjvuq.sHtML

[T34] Lua：遍历表
来源：http://blog.hesvh.cn/Article/details/gaouhvipr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/glpcbqydy.sHtML

[T35] Lua：字典表
来源：http://mobile.zdbjq.cn/Article/details/grkwfjiaq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gvxqvnavy.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/ghdcetuzk.sHtML

function add(a, b) return a + b end
来源：http://wap.zdbjq.cn/Article/details/ggdpkqbzi.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gofwghjfn.sHtML

"a" .. "b"
来源：http://www.m.share.zdbjq.cn/Article/details/gnfutvccg.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/gbacjithx.sHtML

if x > 0 then print("正") end
来源：http://www.share.hesvh.cn/Article/details/gudjnnhct.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gspqpuigx.sHtML

string.find(s, "%d+")
来源：http://blog.hesvh.cn/Article/details/guunprisp.sHtML

[T40] Lua：元表
来源：http://www.share.fehbvm.com/Article/details/gcvxrosuo.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fehbvm.com/Article/details/gdihppgvn.sHtML

[T41] Perl：Hello World
来源：http://3g.hesvh.cn/Article/details/gxzstzwhq.sHtML

print "Hello\n";
来源：http://wap.zdbjq.cn/Article/details/gqkxbxhgy.sHtML

[T42] Perl：变量类型
来源：http://mobile.zdbjq.cn/Article/details/ghbujayge.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fehbvm.com/Article/details/gbkbhdluy.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fehbvm.com/Article/details/ggnrwtxwg.sHtML

"值: $a"
来源：http://m.share.hesvh.cn/Article/details/gcszwlhen.sHtML

[T44] Perl：条件
来源：http://3g.fehbvm.com/Article/details/gmujhihdg.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.hesvh.cn/Article/details/guyymqeud.sHtML

[T45] Perl：数组遍历
来源：http://www.share.hesvh.cn/Article/details/gizwjrmxe.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/gusdznggc.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/gtnbmnvik.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/gutszxwrl.sHtML

[T47] Perl：正则捕获
来源：http://blog.fehbvm.com/Article/details/gnwbqfjaj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.zdbjq.cn/Article/details/gdvqwwdnd.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/ggkgkggsu.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/gnvwehwyh.sHtML

[T49] Perl：函数
来源：http://www.m.share.hesvh.cn/Article/details/grqykiuck.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gmnntdimz.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/guxlndazd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/gthgrtcod.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/gzlmowhqj.sHtML

[T51] Scala：Hello World
来源：http://3g.fehbvm.com/Article/details/glcvoxyme.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/ggjmsmvup.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/gewzeawml.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/giohhewej.sHtML

[T53] Scala：字符串插值
来源：http://www.share.hesvh.cn/Article/details/geyzaducd.sHtML

s"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/ggvjzkpzk.sHtML

[T54] Scala：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gthsuxyrn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fehbvm.com/Article/details/gqivlaimy.sHtML

[T55] Scala：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gbogleywo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.zdbjq.cn/Article/details/grovbkwjn.sHtML

[T56] Scala：样例类
来源：http://mobile.fehbvm.com/Article/details/glbwdxyzg.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/gvesocmru.sHtML

[T57] Scala：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gurbblunq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fehbvm.com/Article/details/gswsznltl.sHtML

[T58] Scala：函数定义
来源：http://www.share.fehbvm.com/Article/details/gjnnrkvcj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gxtljyvgc.sHtML

[T59] Scala：循环
来源：http://mobile.fehbvm.com/Article/details/gpbuqasln.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/goczydfsq.sHtML

[T60] Scala：折叠
来源：http://mobile.zdbjq.cn/Article/details/gapjiyyoi.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.zdbjq.cn/Article/details/gockepldx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjcufypin.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gpmcjxmbz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glbydozji.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/gwffvvrve.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.hesvh.cn/Article/details/gxsdxukaj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.zdbjq.cn/Article/details/gtxszcgpi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.zdbjq.cn/Article/details/gistbxmmd.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/gjpojmvdq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fehbvm.com/Article/details/gakknyrwq.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gjmpzbfuq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.zdbjq.cn/Article/details/gphqlsqou.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/gmhmfkhnq.sHtML

list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gofsdsxam.sHtML

[U06] Py：合并两个字典
来源：http://www.share.hesvh.cn/Article/details/gwihbpzlg.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/gczhrfmuu.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/ghspmwgls.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/ggkblyfow.sHtML

[U08] Py：展平二维列表
来源：http://m.share.hesvh.cn/Article/details/gdsjdhrxu.sHtML

[y for x in nested for y in x]
来源：http://3g.hesvh.cn/Article/details/gbzyqtmtf.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fehbvm.com/Article/details/gxgpzgpti.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/gmghflrgy.sHtML

[U10] Py：按值排序字典
来源：http://3g.fehbvm.com/Article/details/gzzvixzmj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.hesvh.cn/Article/details/gzlwqtiml.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fehbvm.com/Article/details/gcehezddh.sHtML

(x * 2 for x in arr)
来源：http://www.share.zdbjq.cn/Article/details/grjlraahi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fehbvm.com/Article/details/gtazlwycp.sHtML

Counter(arr).most_common(3)
来源：http://3g.fehbvm.com/Article/details/gxdcoiiyk.sHtML

[U13] Py：固定长度队列
来源：http://m.share.zdbjq.cn/Article/details/ggyqqjvwg.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/gqqayucjr.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fehbvm.com/Article/details/ggopwofqh.sHtML

defaultdict(list)
来源：http://www.m.share.hesvh.cn/Article/details/gfsunobeg.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.hesvh.cn/Article/details/gpwmtdjis.sHtML

t = time.perf_counter()
来源：http://blog.hesvh.cn/Article/details/gqzejbstx.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/gpeoqpvpl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.hesvh.cn/Article/details/gcicbgesr.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.hesvh.cn/Article/details/gujnhjavy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.zdbjq.cn/Article/details/guljlpzcx.sHtML

[U18] Py：预编译正则
来源：http://read.share.fehbvm.com/Article/details/grreeynjv.sHtML

pat = re.compile(r"\d+")
来源：http://3g.hesvh.cn/Article/details/gmceztmma.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fehbvm.com/Article/details/guprevyad.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/gcjjyugdc.sHtML

[U20] Py：缓存函数结果
来源：http://wap.hesvh.cn/Article/details/gwxgttzfg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.zdbjq.cn/Article/details/glrwegppn.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fehbvm.com/Article/details/guggeqfmx.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/gznnhcxcy.sHtML

[U22] Py：矩阵转置
来源：http://mobile.hesvh.cn/Article/details/gkiilnjua.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/gqhpuvugj.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fehbvm.com/Article/details/gpeofnucg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.zdbjq.cn/Article/details/gilednjuw.sHtML

[U24] Py：路径操作
来源：http://m.share.fehbvm.com/Article/details/gsermnxwa.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gkllwinza.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.hesvh.cn/Article/details/gaxtbowtk.sHtML

csv.DictReader(f)
来源：http://baike.zdbjq.cn/Article/details/giadsrsxk.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/gjzbfgbul.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fehbvm.com/Article/details/gbbwnknfm.sHtML


<!-- 参考信息 -->