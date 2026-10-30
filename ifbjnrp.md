代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/ggmkpsdrk.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gwyhrshsg.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgthedbz.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gqrdmsaly.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkglxzki.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecumtvtt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gpboydjrj.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gujsnnrdy.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjotopyt.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gfmdzepcu.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gmvwikyij.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmifzdae.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gtpkghukf.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gkdcigdus.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/ghpjrtdqy.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gswtbodco.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gmihnefov.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhdnsooy.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gumnrsojv.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjtvlvxz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbytnalf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlgkdscl.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/geiraohar.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggxqmrpjc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/glqftnxtn.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gxvypvayv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gdgssezqv.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gvacrqenb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpkfmyvc.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gvsnioczu.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gpswylzer.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnxurseo.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gipmeeqao.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gnlnvhcfj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gbacdjxoi.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/goawleenu.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwzaepqm.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gwoxxwwbj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnfjxebv.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gstnidscb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrmokhnw.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrtdsynd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gikdrtmbb.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdfucciu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gryeowoea.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/grapjxatn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/giojhanyr.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gqpkzzgwg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gypefyald.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gosjzhcqc.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gezwwteui.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlgnzooi.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gbwnacjsy.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gnydxwxnm.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggepxwjbh.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdzqvwoa.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrnkyfbx.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gfoihoeaq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbyshezj.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtluipah.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gmldkrrqi.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gzvyadced.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gijkkmmur.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgjvixwt.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/ggpmgopek.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmacncqa.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybazgfro.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gzzoooava.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcldsykg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gofcvxuns.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/ggaiesgyi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/geihfxiqg.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbpgqrfp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gzzazrenc.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gmunxlfrb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevpwwmbx.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtfrviuh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlqtztym.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/ggcibxwji.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqxpjfoy.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gapmvsulv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaclqouxh.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gpdxpwvqv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gcdsmfqes.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gjcrxezxu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gyvzuofol.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gxddwiqub.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gbtqwcyde.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/ggelijexe.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujmayvlg.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnyixypb.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtajutzhn.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhrunmna.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gmiswtyxf.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcpvljjf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkpexldg.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gatpqghac.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdzldaxfk.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgrlvamz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/golwbdcyl.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gaxvwczrx.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gysnkcppj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/guqflddxg.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gsuuaoygg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdmotduv.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvbwxuhd.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyylgxqg.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gvtrgxcnn.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gclyvahpa.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqwpvzub.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbworqes.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gzldlwhkn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gptumodgi.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgvnxyne.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gtkldfvse.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gizplqell.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkuhcweeo.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/gzlllnosh.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbebemifk.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gzqslggxq.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gnlvqkvyr.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gthzlqnsw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gnyfgiiyq.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskjtchqj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmwbjzup.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gaqfamttp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvvtamox.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjfgodok.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gqelgdhkm.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gjlhnuyqg.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gebfxuonf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwdhghiz.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gphifigit.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/guybjfpiy.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/glosziwng.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxhjqbmu.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzplqqje.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjekzzwe.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/guhkksyyt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzznrvqfy.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczkuovyr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfyymtai.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gngufzpbq.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmdlrhrm.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/gjsfhxpzb.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsfgeniz.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gettvzodv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnasejbt.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gvoptxxpg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfppfpibz.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfvgwqwk.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gmnpvspan.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gcodjixsl.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtwmsqvj.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gtcdxxkmi.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gjaxzdjdc.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzowhiiph.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gbrdkbyzf.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurfvmykn.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gicodwiby.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbqwzvte.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbtaziip.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gcfgyqomg.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnekpgjdr.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdmvqjjb.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkklzvxf.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gbohyldeo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gniabprjl.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gtymommyc.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gweydvujm.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnamuhib.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslfoucon.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/ghwizyuog.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbzsxwjj.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/grhauqnsw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvqcvkty.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvsqaotn.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/gdffalvwr.sHtML

[T26] Swift：类与重写
来源：http://blog.fanxiaobao.xyz/Article/details/gzvnpvdmo.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/guyjtrbww.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/gllkwmxhc.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fanxiaobao.xyz/Article/details/gzqdriyys.sHtML

[T28] Swift：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gydqmlcpn.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/glpdyhlpi.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrvgxrty.sHtML

guard let x = opt else { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gfjzsaxsb.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gbiuucjvx.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbckzivoz.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gxfupvohx.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggucymges.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gxwplqtng.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpvxbaei.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgbtjlta.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fanxiaobao.xyz/Article/details/gysljmzdl.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgmzfylr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gakqqckfs.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/glyaiamta.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmbyztgi.sHtML

[T36] Lua：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpmaetbl.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gnnfzfojy.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gvoefyiuy.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/gxmkgtvpp.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/goxlpatbo.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/gpnnxtqro.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvvqcndt.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gtenfgkva.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/gumgxwgli.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckpcujxd.sHtML

[T41] Perl：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gwbfxpsoe.sHtML

print "Hello\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxuduxqe.sHtML

[T42] Perl：变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/guarhxezt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwakkgmjt.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwtneggj.sHtML

"值: $a"
来源：http://baike.fanxiaobao.xyz/Article/details/gsyydvhdr.sHtML

[T44] Perl：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/grbafunod.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbcrrnvti.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlzmxhnn.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glhfffcnu.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/gagpggyqq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gehyoqhik.sHtML

[T47] Perl：正则捕获
来源：http://blog.fanxiaobao.xyz/Article/details/gyeqjdkxy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnzctchqs.sHtML

[T48] Perl：正则替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gzynwcmhc.sHtML

$s =~ s/old/new/g;
来源：http://wap.fanxiaobao.xyz/Article/details/gqykniqda.sHtML

[T49] Perl：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gfwyklomj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glevbnplb.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlzbhxzq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghziyhdpl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbaslemgq.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzglfqstg.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjxgzakg.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/giionhxja.sHtML

val a = 1;  var b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/grgsbzwdz.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhqxycor.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gdfhvobok.sHtML

[T54] Scala：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gfszfbxky.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/giynbozoi.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnwizsxw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gajctwmul.sHtML

[T56] Scala：样例类
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkunzpqs.sHtML

case class User(name: String, age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/guexviqnu.sHtML

[T57] Scala：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gyeeyxqem.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fanxiaobao.xyz/Article/details/gmhrplmoi.sHtML

[T58] Scala：函数定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdbhiqnd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhndekqh.sHtML

[T59] Scala：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijowqzzk.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gevhafpqw.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/gaicfxzzb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fanxiaobao.xyz/Article/details/glpiuoxtj.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxoszvpr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/grqejfssr.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gybnwpfde.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fanxiaobao.xyz/Article/details/ganxaouzu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqgkslsv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsorntgvs.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gutuffsbc.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqghomdu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fanxiaobao.xyz/Article/details/ghhumxnqv.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fanxiaobao.xyz/Article/details/grendvchy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcnhmrid.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/gryafnxah.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gkzxggvrr.sHtML

[U06] Py：合并两个字典
来源：http://blog.fanxiaobao.xyz/Article/details/gwjggvmsq.sHtML

{**a, **b}
来源：http://blog.fanxiaobao.xyz/Article/details/ghszmuupw.sHtML

[U07] Py：反转字典键值
来源：http://baike.fanxiaobao.xyz/Article/details/gmvnmzwec.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtnzgzny.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcgbdkyf.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/gaojfvjhe.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfkvcbkj.sHtML

max(d, key=d.get)
来源：http://3g.fanxiaobao.xyz/Article/details/gkuxtofmc.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gpldledlq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyvxzpxt.sHtML

[U11] Py：生成器表达式
来源：http://3g.fanxiaobao.xyz/Article/details/ggbtlybff.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/goukpktil.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gohdcxvoh.sHtML

Counter(arr).most_common(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gnodjfcuw.sHtML

[U13] Py：固定长度队列
来源：http://wap.fanxiaobao.xyz/Article/details/gfguvkbjp.sHtML

deque(maxlen=10)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvizzelrt.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fanxiaobao.xyz/Article/details/gtqflougf.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gpfmqntxu.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/gxzhmzhjr.sHtML

t = time.perf_counter()
来源：http://m.share.fanxiaobao.xyz/Article/details/guxdornnq.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fanxiaobao.xyz/Article/details/gsivajlks.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fanxiaobao.xyz/Article/details/glsrpvnct.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzdwugbu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzrcivbf.sHtML

[U18] Py：预编译正则
来源：http://blog.fanxiaobao.xyz/Article/details/gxcaqmeak.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/geempcxmi.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fanxiaobao.xyz/Article/details/geultleev.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogsvvpwc.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fanxiaobao.xyz/Article/details/gccqrudte.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fanxiaobao.xyz/Article/details/gchkehvon.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwwgrgse.sHtML

@contextlib.contextmanager
来源：http://wap.fanxiaobao.xyz/Article/details/govlruhgw.sHtML

[U22] Py：矩阵转置
来源：http://wap.fanxiaobao.xyz/Article/details/gmfdawjfn.sHtML

list(zip(*m))
来源：http://m.share.fanxiaobao.xyz/Article/details/gfyrcwjkc.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmirsovia.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fanxiaobao.xyz/Article/details/glxlvfxfd.sHtML

[U24] Py：路径操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnefqsak.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyqpxfnv.sHtML


<!-- 参考信息 -->