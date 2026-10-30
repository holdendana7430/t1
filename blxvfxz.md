代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gioecbktg.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrgbynll.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gupxjhinr.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/govapttoe.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyrjxlzc.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gjotqwaxd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gzwandnjl.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfcocrws.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/glwxbkdvh.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlnsxnhi.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbklhzbl.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnmggbgo.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gehgkizab.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gqlqxrxyv.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gudsagkai.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gzulxzrhc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqesrijf.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfuhcndo.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwytnbmjd.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gehcxfvkm.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/ggilioijw.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/goebhqgal.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdegyffbi.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gxhrxvcxn.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnfmubwq.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/ginjwkxfs.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gejirhdch.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwahqnebp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gdxysxwgh.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxrariva.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gdukqqqbo.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/grhkiedjb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gyyaduuyw.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/ggujsjnbg.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gthtrndro.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/guqohocyg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/grggkoynk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gqefdmkuf.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmulpedg.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gedllkqxh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gwjrbayjc.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwgzajgx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwfwadvo.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjeuubau.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gywfuwmym.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgsxlbli.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/glsphbngo.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnirfgnxo.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkoxbqirv.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gpmlkmjde.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaovofsqw.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gntdhqier.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzstnmts.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gwztdgjgl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmzknlnl.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gnuxkgecy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjemsjrb.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gfnwrqhuj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gqiwrtafh.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqfyibln.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gidjzpalc.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gkutotogq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gsoavckbr.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbokmtlk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkgbxblo.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gmdvrwluk.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgfcjpip.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gpxsznmyx.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gfkakvayj.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gfwspbwbe.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gambfgald.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gqlrgbenq.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gypppjmoa.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grechujfo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gkoypzdsh.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gisgaegrh.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxnwfola.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtkzzbpg.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjkegodf.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gqnsnqiqg.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gmxiihyca.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gezoajqbc.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gardlgvsh.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmjrsmhy.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwgmrqcz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gatpzxyjq.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwiuiiivf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmugabypp.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gywmcnfml.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gghhvfgfd.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspwisfzu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/geipjqhag.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/glaotjadh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gcgzcwowv.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhdtxqqu.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gdovxftoh.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gelavtfpp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gpdjnwnhm.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gyimsrxvh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gusugxkok.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gauzjeaol.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxyznxzo.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/guzmcezth.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gukmtqnza.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gtflyoozi.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gzuhubhkq.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfyctupo.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/glrymlemn.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gvohrrhiq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlysbxhi.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/ggqwmkrwx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsgbmqqin.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkxgadwm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewohwxma.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqtdjxci.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gdcfajomz.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gysnennwi.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/githgnosc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghirnnzto.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gshxkirar.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqqcrshf.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gsrfvwxjx.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggaqhzpej.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gzmqhflyx.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/grcllsouk.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gpxaepxvu.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfvfpiny.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/gzojaaflm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzesoiql.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gnzgwwrnv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gffpstcnd.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcufswrjc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtiwkldxh.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqsfkdpj.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gdiinlnvx.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gttfxbdku.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/grkzvarvs.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvewpytks.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/givbwmywb.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gpzsppayf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gzfrkxjwy.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gigcheqhz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/giyuxeglx.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gspwtxfos.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gutepyueu.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsomcomd.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gligqdcny.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gouusegxj.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gbutpzldr.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gxmjhtiuz.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gurekteag.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gpczohkck.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/glqbyuyav.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/grkkqrwbc.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gkojzizho.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtdnfgvj.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemsglecw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/gwmthymgb.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwodtxgu.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gsioiqagh.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gjtzyaaqs.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/gugtwlouo.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxnrnczk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gtfumyzbm.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gbrjcdxrs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfidfjfh.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqfbhxkd.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/ggfeuaspt.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnbyrwpo.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gdbqlitcp.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgmecqja.sHtML

for (i in 1..10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gbifoacyp.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/gazsyrdfm.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gkwxybxwo.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxwwsheh.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakszhrkg.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gijcxtpdo.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gydqctfbl.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gmsdbkqli.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlptxain.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbyscdwa.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gjpixvcwh.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gvfbxmpai.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/ggkplavhm.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjjarqsb.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/giixctdis.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/ggcodewmr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gcauaxgca.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/grzrwvltv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdimnebk.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gordixtrx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhwdkupr.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwhpkips.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvwztmdz.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxuqkrwu.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gogpcnrqz.sHtML

[T27] Swift：错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/gryxbcdbl.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gahsdsizq.sHtML

[T28] Swift：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gypadxiso.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzyqayuw.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmwebbdi.sHtML

guard let x = opt else { return }
来源：http://mobile.fanxiaobao.xyz/Article/details/gafbithno.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrlvbtra.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gnxpezhsi.sHtML

[T31] Lua：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gsxakzakz.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gsschhfnh.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gqbldoyxl.sHtML

local a = 1
来源：http://baike.fanxiaobao.xyz/Article/details/gszyzjauj.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fanxiaobao.xyz/Article/details/glxlbzfco.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcngwdccq.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfchxwpx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/gzxuayfzt.sHtML

[T35] Lua：字典表
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbzpypbh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gwcbsakvu.sHtML

[T36] Lua：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gjcpojvif.sHtML

function add(a, b) return a + b end
来源：http://m.share.fanxiaobao.xyz/Article/details/gnoipiiae.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/glpkavgxg.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgyfdsks.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gldpxvbhm.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/gvnegvnep.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdufxsmv.sHtML

string.find(s, "%d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gfhlmwvpd.sHtML

[T40] Lua：元表
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpmqxuoc.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmjlnvtr.sHtML

[T41] Perl：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gizoxfdcw.sHtML

print "Hello\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvdoissb.sHtML

[T42] Perl：变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/gmqnmepnu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/grixbvbyu.sHtML

[T43] Perl：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gkkydtyrt.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuoqhffj.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gqnqjprqe.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvtwtghd.sHtML

[T45] Perl：数组遍历
来源：http://wap.fanxiaobao.xyz/Article/details/ginaipyvc.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fanxiaobao.xyz/Article/details/grtpjentj.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gxccazipf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxnippox.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvqlnjle.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gheuobzdr.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gpwxstarw.sHtML

$s =~ s/old/new/g;
来源：http://blog.fanxiaobao.xyz/Article/details/gupzgwfvg.sHtML

[T49] Perl：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gnuqggixf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzuiybnhz.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gudavjvle.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjitfezv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfwxstjoc.sHtML

[T51] Scala：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdixosby.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxtnytpw.sHtML

[T52] Scala：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtocdiop.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvptwumsp.sHtML

[T53] Scala：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gyphwtekm.sHtML

s"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdloxgks.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfynbrde.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gcufqtnxy.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghusjmftd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fanxiaobao.xyz/Article/details/ggpnktyfu.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/gzsutqcci.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gbxbtdwya.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gorlhzjdh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/gedhfhreu.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gbesznsjl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gpmgdoeqa.sHtML

[T59] Scala：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gnztphydz.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gofwfsuws.sHtML

[T60] Scala：折叠
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdixehlw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fanxiaobao.xyz/Article/details/gcooaeswq.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypthuuwd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmfwxgnu.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjowbdnt.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fanxiaobao.xyz/Article/details/gwfxnewjt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhsvabcn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/gufqvgqdl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gbwmrdmqg.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gokhxvfmf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbiigeliy.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwebslquc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/ggzeegmdv.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrjupcog.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gpujjthfl.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gogzwdmdx.sHtML

{**a, **b}
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpdbsaks.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplbndsbh.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fanxiaobao.xyz/Article/details/gesiigswn.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/ghhpsqwxc.sHtML

[y for x in nested for y in x]
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvzcqbur.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fanxiaobao.xyz/Article/details/geiztxmkl.sHtML

max(d, key=d.get)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxqgcdde.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkeaxzqm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvidqnpll.sHtML

[U11] Py：生成器表达式
来源：http://baike.fanxiaobao.xyz/Article/details/giwkxahvq.sHtML

(x * 2 for x in arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/golsbynpd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gwaqdlpah.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgbmqtiz.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvnfbsjz.sHtML

deque(maxlen=10)
来源：http://www.share.fanxiaobao.xyz/Article/details/gusdgbmtv.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmxnkqfa.sHtML

defaultdict(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/galhbgpyt.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/gevqzzzij.sHtML

t = time.perf_counter()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdthzwtpk.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fanxiaobao.xyz/Article/details/gbwusqhrj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdzscmlg.sHtML


<!-- 参考信息 -->