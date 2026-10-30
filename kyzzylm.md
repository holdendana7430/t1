代发 wailian999

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gwgglfbjp.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgioadkv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gzjbbrmgj.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gmerdsasp.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gqxexqlto.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxekczha.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gjddyaoiu.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gjqezqptw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcgkirkm.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvswvluos.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/ghebiiiub.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/godokhqsw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/golkwfqym.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gmyzrixhh.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gligqdhvv.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gilcnpeev.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gxorlyuid.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtimhyylv.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylyvrgwg.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/guplweksb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gcaorlhou.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/ghvnzioyp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqjjlxpd.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/grivwuzob.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/ggluolgiw.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gdnfdpjib.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/geersbjks.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqntqqfm.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/guphtvbul.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gixqlzakm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gohhyzoed.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gxvpkymqz.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwyvnrgs.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gbfqlefpw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/goubseyrm.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgrsxvmo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuudyxit.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlvuruxd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/giudpikjn.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqnczrwb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/glxeviakz.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gqavntdci.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkygsgjao.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gfiohqohy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/guhedoxds.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmugajne.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfaietpl.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gwjtaucxe.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/glqdqwlpv.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcbowqvs.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvfnisow.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gnqezykjv.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcrnpecn.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gnthgbmdb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gpqzukqyy.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvfnlffk.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gxwjkdmkb.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/ghmiiejhf.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gaewgykwo.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gnrglnfwk.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdorphid.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpenzajsd.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhnobkzh.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gylncnsfz.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzjbxszj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyggivpbk.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gmzhnrgxk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gblkjqbgd.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gsfxexnfj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gwadmkhpo.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskrueiig.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gyzmkwhmt.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmuzrviag.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmrrfwzk.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gsgzdigbd.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajxmensh.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gjcrwoecg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/gduyhzlbl.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvuhtmln.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gkaidvqqw.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydtrhoal.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvijovbku.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gcsqslfdq.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gcfiyilwc.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttqsnxet.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdkfurps.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwbwnbdb.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjafpsmb.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/guyxlzbjy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gpeozrsyv.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmzarhcp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfqsyierb.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/geiuqytxl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnfirhbzo.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvoecmyuz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gedddmdqt.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbwqjice.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gbozlkdna.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gtepqaxzd.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gtujfnyrl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/ghxqcajks.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztasijzu.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfhloeaj.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzloywply.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlajanqo.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gtifrfsrr.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfusmsmln.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gcwqwknob.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gemorggxr.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrjwzjwa.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkkfthuh.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkyufsdc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gszypqubx.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/geofpdmjz.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gyljlluzr.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxscqjwtf.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrhdwsuz.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdoaanlo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkawlehfg.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gascaxewp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/ghksmafmo.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/glnofydlh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnsdpdcx.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/geypuscwk.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gevsciftc.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gjzthfkjf.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqleptva.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/guggkjsor.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/gealvdgrt.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtrgwxcl.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gvfeqhsvh.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gbfllhrwy.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gyegnttxf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsaxdltw.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gxhbfotuv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gzaoekaiu.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gtphnjdal.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkkxyafn.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqxapzys.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmzvrpkg.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gixkyvxyy.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/glxwjcpcy.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gipioammx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwnlasxc.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/guuyhxvde.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gupeeqlyc.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gfwsuybxw.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gecutclau.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gaocspjjf.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gpwktepmh.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gjgrhjjlw.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsavofig.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giowbvjez.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzijbeyb.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gheiroboy.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzukvuko.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/gofqrryoq.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gaoxowaar.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/grsjkzgis.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnhegccl.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gosoxkmcw.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuguatch.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gqtceugec.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxfxpuwh.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvdgrznh.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/grgbqyffw.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcrrwpxk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gsipzcjog.sHtML

[T23] Swift：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwydgavvy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhkbttll.sHtML

[T24] Swift：闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/gkosuiduy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gytbstszg.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/gfprpytgi.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/gxuokniml.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrrelqii.sHtML

class A: Base { override func f() {} }
来源：http://blog.fanxiaobao.xyz/Article/details/gefdhwinr.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/goszcfrpm.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjjwfkxa.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkyjjemd.sHtML

enum Color { case red, green }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnuplyvgk.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubwtkcbo.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphgolwfk.sHtML

[T30] Swift：协议
来源：http://wap.fanxiaobao.xyz/Article/details/gtsyzuiya.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gcgnysezr.sHtML

[T31] Lua：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gcmkajtsn.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/grstqpcvu.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyhcvord.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrpqnvpu.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcjmcibq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/gxnbsxlmx.sHtML

[T34] Lua：遍历表
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqetnsbo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/gyxffxapy.sHtML

[T35] Lua：字典表
来源：http://www.share.fanxiaobao.xyz/Article/details/gumtufmgs.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwmxysla.sHtML

[T36] Lua：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gsibpulcb.sHtML

function add(a, b) return a + b end
来源：http://www.share.fanxiaobao.xyz/Article/details/gqeppspdo.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/glhqubnzf.sHtML

"a" .. "b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqtpepdm.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gfqqnslwy.sHtML

if x > 0 then print("正") end
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjrftbao.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyvnefhc.sHtML

string.find(s, "%d+")
来源：http://3g.fanxiaobao.xyz/Article/details/glrvcgbkb.sHtML

[T40] Lua：元表
来源：http://www.blog.fanxiaobao.xyz/Article/details/godtajfdg.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/gvqcchzio.sHtML

[T41] Perl：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/ggoypheqb.sHtML

print "Hello\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gkteerrjb.sHtML

[T42] Perl：变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/ggifvmeba.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsglwuzt.sHtML

[T43] Perl：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/grxzcdqng.sHtML

"值: $a"
来源：http://3g.fanxiaobao.xyz/Article/details/gkipsivuu.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvlnjeha.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gslzpquwi.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gcowrwtls.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsqvihadn.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzjfcuwy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdoxpvbh.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddxrtnvg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcasumedx.sHtML

[T48] Perl：正则替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqmdjnxg.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/gslahjvdk.sHtML

[T49] Perl：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbyyemee.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtglzreqc.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghifwzhrf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fanxiaobao.xyz/Article/details/gfvamrbew.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbbyfkyvg.sHtML

[T51] Scala：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gmggegfrz.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlpdpwru.sHtML

[T52] Scala：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmytntpq.sHtML

val a = 1;  var b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gceqvyaax.sHtML

[T53] Scala：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gfjwjgnvs.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gufrvohxj.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gqtbdwlat.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/ggevptzmi.sHtML

[T55] Scala：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gvgeiorxs.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsbtpivq.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/gshlqdmev.sHtML

case class User(name: String, age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gojivrbre.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gyldiscec.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcrmyayr.sHtML

[T58] Scala：函数定义
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpmqcwuc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdapsdzja.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gwiakuwto.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwelbhji.sHtML

[T60] Scala：折叠
来源：http://wap.fanxiaobao.xyz/Article/details/gnpkpysfc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fanxiaobao.xyz/Article/details/gskytojum.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gnriyabiq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgdnrkdr.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvojjngs.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlysinbt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fanxiaobao.xyz/Article/details/gedpcclyo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fanxiaobao.xyz/Article/details/gyxjogfsb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gpfhvgcpq.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsgxsqjs.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fanxiaobao.xyz/Article/details/gezvxmqac.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbzbxzdt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fanxiaobao.xyz/Article/details/gffrddvep.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjafaoxmm.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/getwqwzyf.sHtML

[U06] Py：合并两个字典
来源：http://wap.fanxiaobao.xyz/Article/details/gmwhzeqaj.sHtML

{**a, **b}
来源：http://blog.fanxiaobao.xyz/Article/details/gtxehebcq.sHtML

[U07] Py：反转字典键值
来源：http://3g.fanxiaobao.xyz/Article/details/gjtinwjou.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzvnrhvt.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/gelogjumd.sHtML

[y for x in nested for y in x]
来源：http://www.share.fanxiaobao.xyz/Article/details/gdopyuqqu.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fanxiaobao.xyz/Article/details/ggwpzpclr.sHtML

max(d, key=d.get)
来源：http://wap.fanxiaobao.xyz/Article/details/gjfbqqawj.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guayhboqx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fanxiaobao.xyz/Article/details/gkninjkgd.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmpjaxqp.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsklojxcp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fanxiaobao.xyz/Article/details/guugadklt.sHtML

Counter(arr).most_common(3)
来源：http://wap.fanxiaobao.xyz/Article/details/grazbomwl.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkhsxuud.sHtML

deque(maxlen=10)
来源：http://www.share.fanxiaobao.xyz/Article/details/gphbsfhji.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fanxiaobao.xyz/Article/details/gjukytxxc.sHtML

defaultdict(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcdppesp.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxzvfqwc.sHtML

t = time.perf_counter()
来源：http://m.share.fanxiaobao.xyz/Article/details/gzifqdyxw.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/gkguvwtfp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/gbulqccpa.sHtML

[U17] Py：初始化日志
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnytktrq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlcrdxow.sHtML

[U18] Py：预编译正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrshnplt.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczizefto.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fanxiaobao.xyz/Article/details/gsyygcjwb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdegentwr.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fanxiaobao.xyz/Article/details/gchbjpxvl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbiieqawn.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdzoveeq.sHtML

@contextlib.contextmanager
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdrgdykt.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmxravck.sHtML

list(zip(*m))
来源：http://mobile.fanxiaobao.xyz/Article/details/ghximvkgo.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdkzqgrh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsfjxysu.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlbagkob.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gepgogkyq.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxbmzxhy.sHtML

csv.DictReader(f)
来源：http://3g.fanxiaobao.xyz/Article/details/gxsoarzig.sHtML

[U26] Py：并发下载
来源：http://baike.fanxiaobao.xyz/Article/details/gtqrdwifl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpetvrql.sHtML


<!-- 参考信息 -->