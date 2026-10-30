代发 wailian999

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gtpqfmmrd.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtoklpqe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gubycklpo.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gnghyisdg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/giturneay.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgfonpeh.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbpdtqkv.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gsujjyivm.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gywthepeo.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/godbojqoh.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/grgtylrtg.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyncryfp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtjsrkvbj.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsvqazyl.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gypmjchjk.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzymuciro.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfotssjzu.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhozimxd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gbayfkmgh.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gbshjgtbs.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gcjcpjvwc.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gzdsameka.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgadmzui.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gzgqwsugz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxeedeac.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gifeaxyof.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gfvdsiavk.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gssoghmgu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gvwvwydwk.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmyohyef.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/giajoeqov.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggaasixjl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxciynile.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gudnzcmnb.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/geeqtikgr.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gukqddyby.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gspjcqlxz.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/garhxifbw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhniolik.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/ggatnujic.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gktjkftvz.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/ggmduszxo.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gieoiagdb.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gbknquznv.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gfpxnpfjc.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gsimzhnar.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gswwqiabm.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gssmzksns.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvoicaqvt.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/guruhujwj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsrnntkn.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/grzsvcaxw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/garqyayzp.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gwkqhoczo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gohsqwvun.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyojbivb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxocpqvzm.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gnoqunvbf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gweiuzdje.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gqemzcpij.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gsbnmmkwh.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwgsgnww.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlderqfm.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjmhbdgz.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhenssgm.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gknlrjmhk.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gptxlyrgh.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gbciyxyhb.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gimflltzh.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydkpxodh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gymxxtehd.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gptniclrw.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gziwvvxxq.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gjijbbgrq.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcylmxzop.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gozxiujzy.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gztlduhdw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gftsemnji.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gmauqvnyj.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gmogddqiw.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwyyvhsr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/glexfljej.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gutzfrcew.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwtzuwkc.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gvygubhog.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/glfpzypmh.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gqxecvbob.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsaielnip.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtedulsmh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gisxovhvu.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gappcqexw.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gsqtqpmje.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gsyosglcj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/gwopimkbi.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gsyfhttrh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvsaumfx.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gmvltxddc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghaznmaof.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/goitzhgqb.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gurzylfst.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdsqbsap.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/glqirqfpd.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqfumdgg.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxubwxqe.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gsuthczny.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/girtzrvgd.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gdeiapeqg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gifnmxric.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbebnpahq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnvkfxxox.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmquvsjb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/grzbvtyzi.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gxwcrvrpc.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxfhybxi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gucwrrrct.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gueeodufw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gikaizmnh.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljuevtfq.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/grvdyoerq.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gqrohuefa.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzpsubnkf.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgntnfkm.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghayewbur.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gecjadggq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdlsacyi.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/grwpttkrn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gexxsknlo.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gsubpgsck.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gapyzwdnl.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gzykzuhuz.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gzchdnpvj.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnjctyue.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsgcgfeg.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/giybeabwv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwylrzsbz.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gblmorokd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnigsnuyh.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gwuubsraz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurvhlblr.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gztokdbex.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gdlxjymsc.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrzlpneq.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/godkiryhv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/guburwexp.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhhgiuvi.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gcvjjyryp.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijouajls.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gweaupawl.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gelfdihxx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcmwuuuv.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gfnewkcav.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflphrvoo.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzgzznne.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/gwhshsbhf.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhcjznxh.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/giewrpikb.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehmbwixo.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqealzse.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypvykssc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/ghmveakma.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gputrvwla.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/gljbtmdwp.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyeajwnk.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gnwxyrosg.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmirqwrz.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnasthbhn.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giauwpimg.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxuhmpfy.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/galqtdwhz.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpddjdpu.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxhjysax.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gwcpvribf.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwdlwjko.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtqlxuzq.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gbhtiksro.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/ggamwmsec.sHtML

[T19] Swift：可选绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gmrfthdna.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gghwratch.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/geidygaxf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwibohbf.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gddautgqv.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gbcvhytsu.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/gfjoadicg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gvkutltij.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/goodthjhz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcxhblqt.sHtML

[T24] Swift：闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtbkrmvt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gxeopzesp.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/ggsgvwcqc.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/gfwvvljxr.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/guzkaeymh.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcarvdab.sHtML

[T27] Swift：错误处理
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjfpwgli.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghawpleur.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsmhswfc.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/gzhffcojn.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gilbuseyf.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gwlabfagy.sHtML

[T30] Swift：协议
来源：http://baike.fanxiaobao.xyz/Article/details/gcheeqdqt.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqysmohz.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamtombyc.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/griesciir.sHtML

[T32] Lua：局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvdqtxvu.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gvjeqthbg.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/glovliydd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fanxiaobao.xyz/Article/details/gvffpayhm.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmerpirnh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmkhcbwj.sHtML

[T35] Lua：字典表
来源：http://read.share.fanxiaobao.xyz/Article/details/gterxnpkk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpzoybhl.sHtML

[T36] Lua：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsmdkcnv.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/gahafipti.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gsthccxsd.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/guanhcwmb.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgkqhvot.sHtML

if x > 0 then print("正") end
来源：http://wap.fanxiaobao.xyz/Article/details/gzjrugago.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfblffmt.sHtML

string.find(s, "%d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysimuczi.sHtML

[T40] Lua：元表
来源：http://blog.fanxiaobao.xyz/Article/details/ghaywtdbg.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhvzemjy.sHtML

[T41] Perl：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gxqibtetg.sHtML

print "Hello\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxnahbie.sHtML

[T42] Perl：变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gywpkgddm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/gjvomxyri.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdbokngk.sHtML

"值: $a"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpfbqumi.sHtML

[T44] Perl：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsgotabl.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbnyxwoz.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcynwbnll.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyayclzc.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwymthki.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmduobfmu.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fanxiaobao.xyz/Article/details/gaarmtzaq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glxmlfyoa.sHtML

[T48] Perl：正则替换
来源：http://baike.fanxiaobao.xyz/Article/details/gbizpvlzc.sHtML

$s =~ s/old/new/g;
来源：http://3g.fanxiaobao.xyz/Article/details/geqthssvz.sHtML

[T49] Perl：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezulfyor.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjljafuhu.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gfpwosvdn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnivlxfk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gusgtxjwk.sHtML

[T51] Scala：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/glcbhlrlc.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gaztypuvh.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/grejllnly.sHtML

val a = 1;  var b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkaikozb.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjbokaje.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwwxwlom.sHtML

[T54] Scala：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gpchbvcba.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gbmxtxxjy.sHtML

[T55] Scala：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gsshpbujx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glozgnlmz.sHtML

[T56] Scala：样例类
来源：http://wap.fanxiaobao.xyz/Article/details/gbtdvwuaq.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gekruwjxu.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqymrjcr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxorjexdu.sHtML

[T58] Scala：函数定义
来源：http://3g.fanxiaobao.xyz/Article/details/goltnqdpu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fanxiaobao.xyz/Article/details/gklavuubi.sHtML

[T59] Scala：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwltsrrrb.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwkrsltb.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/gbifxwiva.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhkvuheu.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gbegkusnd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffdgofqa.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/giagnldme.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fanxiaobao.xyz/Article/details/ggcwoppfw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fanxiaobao.xyz/Article/details/grnjkluyf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/gpqdztbhq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgtfigeh.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/gprehgfov.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geafmwemv.sHtML

[U04] Py：变量调试打印
来源：http://wap.fanxiaobao.xyz/Article/details/goirogoaz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fanxiaobao.xyz/Article/details/gknombgle.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/gfziufauz.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fanxiaobao.xyz/Article/details/godzsovkt.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fanxiaobao.xyz/Article/details/glohjxdbd.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/grsjdskds.sHtML

[U07] Py：反转字典键值
来源：http://wap.fanxiaobao.xyz/Article/details/gcymxifai.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/gppvkuoud.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcyttsmr.sHtML

[y for x in nested for y in x]
来源：http://m.share.fanxiaobao.xyz/Article/details/groctvjhf.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fanxiaobao.xyz/Article/details/gpveqeptb.sHtML

max(d, key=d.get)
来源：http://3g.fanxiaobao.xyz/Article/details/gjurgwibg.sHtML

[U10] Py：按值排序字典
来源：http://blog.fanxiaobao.xyz/Article/details/gokdfrfro.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fanxiaobao.xyz/Article/details/gzjsgyayu.sHtML

[U11] Py：生成器表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gozqewwry.sHtML

(x * 2 for x in arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/geamazera.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsuwtemp.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjziapsun.sHtML

[U13] Py：固定长度队列
来源：http://3g.fanxiaobao.xyz/Article/details/gsdgjoevh.sHtML

deque(maxlen=10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxwxzqbw.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fanxiaobao.xyz/Article/details/gfbbyhlrp.sHtML

defaultdict(list)
来源：http://blog.fanxiaobao.xyz/Article/details/gtxrwzerx.sHtML

[U15] Py：高精度计时
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxommzea.sHtML

t = time.perf_counter()
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxmiaqjs.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fanxiaobao.xyz/Article/details/gsecyhcks.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fanxiaobao.xyz/Article/details/gnjukiewe.sHtML

[U17] Py：初始化日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgupswry.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fanxiaobao.xyz/Article/details/gbmnewuxm.sHtML

[U18] Py：预编译正则
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbhaqijz.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxirextax.sHtML


<!-- 参考信息 -->