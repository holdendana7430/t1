代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/gvrusftrh.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fehbvm.com/Article/details/gbsabmfxu.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gevbocmnm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gskwgbaru.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gtsbkceoi.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxcfyncej.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/gzwkaamie.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gbzymguna.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.zdbjq.cn/Article/details/grfyumpnu.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gwnkkaiic.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gsnedvkzr.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gptcfwfnf.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/gxqquxkku.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gslvjwjla.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gbcglqstd.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/gnyizkppr.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gfgiqapls.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/gvgvnwlsy.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/galrcvcwz.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/gnuifztdt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/guxdcjoby.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gitrpfbpt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/gbuelibti.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gqumwqxul.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/gyhjxsqlo.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gchpnzhfk.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/guakpvfia.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gntwdwivh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/gqjmqvffn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gkngscfiv.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gkgvtitud.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gbfsgzkcu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gducivcng.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gniqnkuth.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/gdnqthajc.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gtcfmutgq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/gxrpcbeqz.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/geudxsswz.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gvkbojjfx.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gkhutpmxd.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gxvcprbkm.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/glgfzhsnr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/glhtwftfq.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gxsrysfcu.sHtML

int main(int argc, char **argv)
来源：http://blog.hesvh.cn/Article/details/gkgqsrvgx.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gokddbhcp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/ghnmokwew.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/gqvsonapq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gghosyhlb.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gomizmzmh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/gimueeqho.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gimlaghvr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gaekqllyq.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gkmsdzwed.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gpapqwfvp.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/gvahfbocx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gijfaeklu.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/gmustouvl.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gvcvotthk.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/gyxfjooux.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/guxxkxere.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gauhqewji.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/ggjfnndvi.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gdwormntf.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gassghqdf.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/gsyefzgax.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gsmcgwada.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gfeyypgaj.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/guiekzaxm.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/gkkrdwhiq.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gwocnaeaf.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/ghbvdnhwy.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/geflvcgmo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.hesvh.cn/Article/details/gbrzgwnrf.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gowkxihar.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gfgnrjatw.sHtML

[S33] C++：vector 增删
来源：http://www.share.hesvh.cn/Article/details/gwhzgmzuc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gbnsahudq.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/gknmejmqv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/gdmjyosyo.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gcawciwwr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gpbtjxvwl.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/ggmauetyt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gzemrseao.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gymebmvne.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gqcljljnk.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/gqnjvbmvx.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gcolnbsyt.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gpxplkpxz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gzmpqnjjd.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gsmzjnkdt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.hesvh.cn/Article/details/gjhghnonf.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/geaflkzyo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gxepttqda.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/gfrdqpcxs.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/gqlszlnqy.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gsxzibnwx.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/gnhnpockm.sHtML

[S44] C++：引用传参
来源：http://baike.hesvh.cn/Article/details/goxbxeagp.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/gpoutwpak.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/ggjbmolpr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/griwogsic.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gtkhjnzpv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/ggxkvrhim.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gpvsqagzx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gdemilmse.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gvhejoksm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/gccawyrif.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/gczoekzds.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/gratzsett.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gthcwbahj.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/gxylhpsdz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gwkdozgds.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/gfqzgpsxq.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/gdrjfmebs.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fehbvm.com/Article/details/gnwbbywzy.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/govtjiyfh.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/gupzoflhi.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gyngozapw.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/grvjbhole.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gwvizcfjq.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/gxkgojkjt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gkjikbdfz.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/gxsqwmttn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gaolgyhto.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gioupxkea.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/gzkqlugju.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gtolrwtsk.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gwzdgmsik.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gciezxpqt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/gcgccickz.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gpvaadrac.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/goerykplm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfvtvusom.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/giehejgoi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grarmllxk.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gynylxlxl.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gpgwtqcbo.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gtleouobn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gcjlttojk.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/geytyznbh.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gmeajktqh.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gjgapyqeo.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/gdbwnpebp.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gazagjrwl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/grlovesgb.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gnhfjdqoi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/ghwmzsvpl.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/guyssflcn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/giypmioip.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/glypudfvh.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gffomhijh.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.zdbjq.cn/Article/details/gvbhfybnt.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gamedvbxb.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gsmdoolcs.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gxmfmbgln.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/gyvljvepz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/ggsmnmwyp.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gkvzpaytx.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/grdmcxmzi.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/glfdrtodd.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/gstjjdptl.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gueeiyscf.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gixpyjcie.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/guonqhdhr.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/gryxdagwi.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gehrlusak.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gkidcuusq.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/gzxjmnexd.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gydzmhsyc.sHtML

[T18] Swift：字符串插值
来源：http://read.share.hesvh.cn/Article/details/ghudcooon.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/gwgynsgoe.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/gygerppkh.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/guaagsdtf.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/guscxxncc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/giylvtmty.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/grqwgoolu.sHtML

for x in a { print(x) }
来源：http://www.m.share.hesvh.cn/Article/details/gsksisurp.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/ghojwkzge.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.hesvh.cn/Article/details/gsupwzpsb.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/gxlieaxda.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/gthtqraio.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/gwehhilvn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gktjtjabx.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/giqfbhmor.sHtML

struct P { var x: Int }
来源：http://www.m.share.hesvh.cn/Article/details/gtdubouvz.sHtML

[T26] Swift：类与重写
来源：http://www.blog.zdbjq.cn/Article/details/gpunupybt.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/ggvyegdvs.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/gqdzdhzzu.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/ghhrqaqgw.sHtML

[T28] Swift：枚举
来源：http://3g.fehbvm.com/Article/details/gzmwfywpx.sHtML

enum Color { case red, green }
来源：http://m.share.hesvh.cn/Article/details/grjccocpi.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.zdbjq.cn/Article/details/gqrgmrhdj.sHtML

guard let x = opt else { return }
来源：http://mobile.hesvh.cn/Article/details/gefeuqqca.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/giyjrxzjk.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/gkdmrosrh.sHtML

[T31] Lua：Hello World
来源：http://blog.zdbjq.cn/Article/details/gelkvilzt.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gcpgrnxlr.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/gfdefjbhf.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/gfbxccefj.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/gtmtupmwp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/gllsuznam.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/gbirrfcty.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.zdbjq.cn/Article/details/gtwqgkgfy.sHtML

[T35] Lua：字典表
来源：http://mobile.zdbjq.cn/Article/details/gplkcgadc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/gtpegbobh.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/gmkistdqz.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.hesvh.cn/Article/details/gunayumny.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gnukczeec.sHtML

"a" .. "b"
来源：http://3g.zdbjq.cn/Article/details/gugywrbpd.sHtML

[T38] Lua：条件
来源：http://read.share.fehbvm.com/Article/details/gsmbnwatd.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/ghmrxvhjj.sHtML

[T39] Lua：模式匹配
来源：http://mobile.hesvh.cn/Article/details/ggedltwni.sHtML

string.find(s, "%d+")
来源：http://3g.hesvh.cn/Article/details/gvxbrimpr.sHtML

[T40] Lua：元表
来源：http://m.share.fehbvm.com/Article/details/ginzgecqy.sHtML

setmetatable({}, { __index = base })
来源：http://wap.hesvh.cn/Article/details/gscyldgmm.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gpsserhyl.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/gdpdstftm.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gquaosxlu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/gyhrbiezr.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gpbaojdqb.sHtML

"值: $a"
来源：http://www.blog.zdbjq.cn/Article/details/gcfteigaa.sHtML

[T44] Perl：条件
来源：http://read.share.hesvh.cn/Article/details/gxummrmlg.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gyuclcqdv.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/gmghgrrmc.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/genfhxezk.sHtML

[T46] Perl：哈希操作
来源：http://wap.fehbvm.com/Article/details/gihvbfwld.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fehbvm.com/Article/details/gcznxmakb.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fehbvm.com/Article/details/gwikdgjsp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/gbebmtsmo.sHtML

[T48] Perl：正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gugfhaewj.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/gqcdllror.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/glfrfioxd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gsmouuanc.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gwhupkwfb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fehbvm.com/Article/details/gphwftibh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.hesvh.cn/Article/details/gueoyzkie.sHtML

[T51] Scala：Hello World
来源：http://read.share.fehbvm.com/Article/details/gptjqxyin.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gbcyqrwdq.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/gzmkgnivr.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/gvcbrotth.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/glydxsuyu.sHtML

s"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gvsanpoyg.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gvapmtfnh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.zdbjq.cn/Article/details/gkxqanbxx.sHtML

[T55] Scala：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gnnsjhpoz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.zdbjq.cn/Article/details/grruvypwh.sHtML

[T56] Scala：样例类
来源：http://baike.zdbjq.cn/Article/details/gghgnjjzg.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gjxuwrgcg.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gpiygstvx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.zdbjq.cn/Article/details/gipouxqyf.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/gmmkhxyyk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.hesvh.cn/Article/details/gzaoqyvfh.sHtML

[T59] Scala：循环
来源：http://mobile.zdbjq.cn/Article/details/gsifoimok.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/gocedlhqm.sHtML

[T60] Scala：折叠
来源：http://m.share.fehbvm.com/Article/details/gzygftjrp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fehbvm.com/Article/details/gsifpsqmj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gghqjkngr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gzyehrpfv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmyvarkja.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/gfiqvcbib.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fehbvm.com/Article/details/gmudvblxm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fehbvm.com/Article/details/gbcdlizwa.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.zdbjq.cn/Article/details/gjqzjsnte.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/gjnkigehz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/getrnezzq.sHtML

[U04] Py：变量调试打印
来源：http://mobile.zdbjq.cn/Article/details/gvktxpymk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.zdbjq.cn/Article/details/gwyrdapov.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/gkwkbdczb.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gyoyuglln.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/govxzyhvv.sHtML

{**a, **b}
来源：http://www.share.hesvh.cn/Article/details/gthotnmis.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fehbvm.com/Article/details/gikitqdyi.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fehbvm.com/Article/details/gkgwzolnv.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.zdbjq.cn/Article/details/gdyvpnxwb.sHtML

[y for x in nested for y in x]
来源：http://baike.hesvh.cn/Article/details/gjklsvokf.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/gvvqsxocp.sHtML

max(d, key=d.get)
来源：http://3g.fehbvm.com/Article/details/gkwcvtopy.sHtML

[U10] Py：按值排序字典
来源：http://blog.zdbjq.cn/Article/details/geifpifut.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fehbvm.com/Article/details/gmvwzoaro.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/gjyembnnn.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/gryholkqd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/gpiqymawx.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/gjgmhwmxp.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fehbvm.com/Article/details/gqombheln.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/gkjzdbrzc.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/gizxihasf.sHtML

defaultdict(list)
来源：http://www.blog.zdbjq.cn/Article/details/gihllkkpk.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/gdkpmroan.sHtML

t = time.perf_counter()
来源：http://3g.hesvh.cn/Article/details/gqkmyrqwx.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/gbnieegsu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.hesvh.cn/Article/details/gzrivwmjs.sHtML

[U17] Py：初始化日志
来源：http://read.share.hesvh.cn/Article/details/gztedffus.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.zdbjq.cn/Article/details/ggaoacjlk.sHtML

[U18] Py：预编译正则
来源：http://baike.zdbjq.cn/Article/details/grfzidooz.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/gmiyyqtxz.sHtML

[U19] Py：正则替换带回调
来源：http://blog.zdbjq.cn/Article/details/gzkvidpan.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fehbvm.com/Article/details/gxtfjtdgt.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.zdbjq.cn/Article/details/gwmtbrinl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.zdbjq.cn/Article/details/gcloaodxg.sHtML


<!-- 参考信息 -->