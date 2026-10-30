代发 wailian999

S. C / C++ 专题
来源：http://3g.fehbvm.com/Article/details/gjbpxhcqv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggrcwxuey.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gixxcromo.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/grrdlntct.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gglnzskhb.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gtebwhmyl.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gbwvnenie.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/gjcqexjeh.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gaqztcych.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gelpicnvn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gezkhezmm.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/gsytofehl.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gvihvuybg.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gbypqtkmy.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/gnnwtvqxz.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gvmjtxhtm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/gcqrlgpwh.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/ghihgkyph.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gomouskxm.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/gozqkqsku.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gqfymgtdv.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gspxmatkb.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gnpaedlsx.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gtozmjism.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/gsyxfbxwk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gjdrybixp.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/gjxkwwjuo.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gavyavivz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gylozlelz.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/ghtubkhrw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gjxdajwyr.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/gvqtlawdo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gawnjnbsd.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/giqujomdk.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/garvbhgnh.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gfhptpita.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/ghiluwljl.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gmjhsiahg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/gcjgejvqe.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/grycpyscw.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gawbpuqtm.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/glltegrlc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gtnpsiekp.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gtdpbooap.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gmoninxay.sHtML

[S21] C：字符类别判断
来源：http://wap.zdbjq.cn/Article/details/glufmvjea.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/gqxibyiqf.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gxtsyaclp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/gdambnuna.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/gjesmajvb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/guroqlgxy.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gmcddvqpq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gntivfvac.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/gzadiqogb.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gtsybkkkw.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/gfxybhfyi.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/gheupnluy.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/gskptpwst.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gcpqmeuwy.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gllbfyhxt.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gfdgwszlp.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gafsqzchb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gagvaexju.sHtML

[S30] C：头文件保护
来源：http://blog.zdbjq.cn/Article/details/gafffjklu.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gejieailo.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gifcftiqt.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/gprzqxxmt.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/glqkhrxib.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/grmtgaolm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/garcpmrzp.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gvczdibyq.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/gqiyuouut.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gbtpfmaba.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/ghpfsqaev.sHtML

[S34] C++：遍历 vector
来源：http://wap.zdbjq.cn/Article/details/gcsmhwjrr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gnriqyvan.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gowqpaslp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gavdsdils.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/gmaspakfn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gemavgohx.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gypgoishh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/guzjbhhmv.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/gzvdidpmd.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gahfoboww.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/gpbzicavt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gnwencyah.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/ghluyuysk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/gipaimbav.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/grjwnntyp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.zdbjq.cn/Article/details/gbefeiylk.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/gnlcfgavk.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gxtauehiv.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/giiprwdca.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/gjxkdaeku.sHtML

[S44] C++：引用传参
来源：http://read.share.zdbjq.cn/Article/details/grbtjrugo.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gqapltsnr.sHtML

[S45] C++：lambda
来源：http://wap.hesvh.cn/Article/details/gslioslpr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/gvfxeloeg.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/ghqbrvzkf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/gkrrzkiey.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gatzntlhl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.zdbjq.cn/Article/details/ghsoizcwu.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gvejonyem.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gfnuwtilu.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/gctfbzylf.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gyrxhovux.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gqfittuma.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/gxpqyvddb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gxnupfwkb.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gxohbbshu.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gnmirfnvq.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/guvvmyjtf.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gzrmuuvtb.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gauowbrva.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/grtwnnqbk.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/gonewwhgr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gknclkqrc.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gtkflbhnm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/gjluihlet.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gtasohafc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.hesvh.cn/Article/details/ggveqorfg.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/guvyfkuus.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/gbrtukeyf.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gdtwtbrlr.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/gjlflxhzk.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/gyliiryib.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/gnfnxmxxd.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gpbwpperx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/gkdhcvcch.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsfsvjlpd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/ggbctasah.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghjpgkfwc.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gudgvugsh.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/ghfbpznhc.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/gmljutaal.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/gwrstaxcn.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fehbvm.com/Article/details/gaefqzkyz.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/gaoqabjqw.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/geinxbccc.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/ghifkalet.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/ggsnbksbb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gsjwvciby.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/gvqgudbnb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/gyrdlirwg.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gifhlomdd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/gbzeeigdd.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/gzobnvxqg.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gacfmaehy.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gizdikcxn.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/gcrduhdfv.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gxrbzmjdf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.hesvh.cn/Article/details/ggalpolpu.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/gdmhkvhsx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/gltoewedr.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/gipegkfrg.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gucvdobku.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/gqnuwxpsu.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/gphombrpi.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/gdqwewhbj.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/gbwudpsja.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/geawszouc.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/gtnrlfwve.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/gdsjsfezj.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gbyjghtqq.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fehbvm.com/Article/details/gwyfihncg.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gkvxmofpm.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gchjyqszz.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gscyumksb.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/gnzsvroes.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/girlnvpza.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/ggzwswbeg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/gqwfsewoh.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/gztkcbojd.sHtML

for x in a { print(x) }
来源：http://www.m.share.fehbvm.com/Article/details/gzpsxcats.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/gwbbwcowx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/grtbtsbeh.sHtML

[T23] Swift：函数
来源：http://3g.hesvh.cn/Article/details/gjjhoiwos.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.zdbjq.cn/Article/details/gbiqdkdnk.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/gscxqxvbo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gflntdoco.sHtML

[T25] Swift：结构体
来源：http://mobile.zdbjq.cn/Article/details/gjhaktjcy.sHtML

struct P { var x: Int }
来源：http://mobile.fehbvm.com/Article/details/gwpubhegu.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/gkqtdczsc.sHtML

class A: Base { override func f() {} }
来源：http://blog.zdbjq.cn/Article/details/gxkonhffx.sHtML

[T27] Swift：错误处理
来源：http://3g.hesvh.cn/Article/details/ghjapcogj.sHtML

do { try f() } catch { print(error) }
来源：http://wap.zdbjq.cn/Article/details/gwdxylgso.sHtML

[T28] Swift：枚举
来源：http://blog.fehbvm.com/Article/details/gkdqjzvsp.sHtML

enum Color { case red, green }
来源：http://www.blog.zdbjq.cn/Article/details/gpwfgvkvy.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.zdbjq.cn/Article/details/grqvfpqir.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/gyphubxvm.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/gniuenbva.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fehbvm.com/Article/details/gmocmrxhm.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/gtttzduxr.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gvnvefwzc.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/gszdzcsuu.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/gqfrygtsy.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/gtqiosheo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.zdbjq.cn/Article/details/gprrfaabs.sHtML

[T34] Lua：遍历表
来源：http://3g.hesvh.cn/Article/details/gahppbkjm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.hesvh.cn/Article/details/gwgfhxysj.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/gogmxmccy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fehbvm.com/Article/details/gefxchwwg.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/gbkgejcrp.sHtML

function add(a, b) return a + b end
来源：http://wap.hesvh.cn/Article/details/gyatikanp.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gpkugklwd.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/gyyciruwv.sHtML

[T38] Lua：条件
来源：http://read.share.zdbjq.cn/Article/details/gqsyvrqsq.sHtML

if x > 0 then print("正") end
来源：http://blog.fehbvm.com/Article/details/gjwapmxnx.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/ghutuvgec.sHtML

string.find(s, "%d+")
来源：http://blog.hesvh.cn/Article/details/gnghcgfpw.sHtML

[T40] Lua：元表
来源：http://www.share.zdbjq.cn/Article/details/gwnopycnn.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.hesvh.cn/Article/details/gzstokrbn.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gcgakbhfq.sHtML

print "Hello\n";
来源：http://read.share.hesvh.cn/Article/details/gcdrjfzpg.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gqnvsdifv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/gsiyebswn.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gjjvuldya.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/gewsernjf.sHtML

[T44] Perl：条件
来源：http://read.share.hesvh.cn/Article/details/godgcyqxa.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.zdbjq.cn/Article/details/guinupwtl.sHtML

[T45] Perl：数组遍历
来源：http://mobile.hesvh.cn/Article/details/gbsodusuo.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/gshnvnasb.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/gnasfloxx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fehbvm.com/Article/details/geikeqiic.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gsnpiimny.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.hesvh.cn/Article/details/gfylgzvtd.sHtML

[T48] Perl：正则替换
来源：http://mobile.hesvh.cn/Article/details/ggbfyhiub.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/gxcrwhmgy.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/gkmreakzy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gflfthmey.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gvdcoskpz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.hesvh.cn/Article/details/gcvdirscd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/gkiwmergr.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gsxwfbzru.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/glxdbaxvz.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/gqpsahmvs.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gptndohck.sHtML

[T53] Scala：字符串插值
来源：http://baike.hesvh.cn/Article/details/gergmfmtb.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gskyydluf.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gonhyeith.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.zdbjq.cn/Article/details/gkosmkbot.sHtML

[T55] Scala：集合过滤
来源：http://3g.hesvh.cn/Article/details/gkkrzsbvs.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/gqxpigcwd.sHtML

[T56] Scala：样例类
来源：http://wap.hesvh.cn/Article/details/guamfqtyx.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/ggbnqpxqx.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gozjokdhu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/ghjqwmlin.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/guouurvwh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.hesvh.cn/Article/details/gqesjuenp.sHtML

[T59] Scala：循环
来源：http://www.share.zdbjq.cn/Article/details/gmzhtzvtv.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gcfsnkziq.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/gwceqsrdg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/gypitvlgz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghdsuvphq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gsbbzbymi.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnmgotjmg.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.zdbjq.cn/Article/details/gkyyfnbkn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/gjalnihxu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.zdbjq.cn/Article/details/gwcpovwap.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fehbvm.com/Article/details/gsxyghjip.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.hesvh.cn/Article/details/gdzyuokdw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/ghiwrpqqu.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fehbvm.com/Article/details/gbwwysovw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.zdbjq.cn/Article/details/gmegahqpx.sHtML

[U05] Py：列表去重且保序
来源：http://baike.hesvh.cn/Article/details/geezkerwi.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gudqkwbqb.sHtML

[U06] Py：合并两个字典
来源：http://read.share.zdbjq.cn/Article/details/gvtsegxjy.sHtML

{**a, **b}
来源：http://wap.fehbvm.com/Article/details/ggbayzejg.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/gjitzjgve.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fehbvm.com/Article/details/gngpgevbm.sHtML

[U08] Py：展平二维列表
来源：http://3g.fehbvm.com/Article/details/ghmckrras.sHtML

[y for x in nested for y in x]
来源：http://3g.zdbjq.cn/Article/details/gpdzirnik.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.zdbjq.cn/Article/details/ggddtmzqf.sHtML

max(d, key=d.get)
来源：http://baike.zdbjq.cn/Article/details/gywsfaqlt.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.zdbjq.cn/Article/details/geplrzwfj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/gyvjsnuzd.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/gjiozeqma.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gdlksfrap.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/gfkggdakb.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/gracierfg.sHtML

[U13] Py：固定长度队列
来源：http://wap.hesvh.cn/Article/details/gtzfjyuah.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gweiahqwu.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/gkkmrrzkp.sHtML

defaultdict(list)
来源：http://read.share.fehbvm.com/Article/details/gnqcmdlrp.sHtML

[U15] Py：高精度计时
来源：http://m.share.hesvh.cn/Article/details/gaikxaujs.sHtML

t = time.perf_counter()
来源：http://wap.hesvh.cn/Article/details/gplfrtmbr.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.zdbjq.cn/Article/details/grrcweqbk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.hesvh.cn/Article/details/gybeebiou.sHtML

[U17] Py：初始化日志
来源：http://read.share.zdbjq.cn/Article/details/gpmgbvypu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.zdbjq.cn/Article/details/grjasnwgb.sHtML

[U18] Py：预编译正则
来源：http://read.share.hesvh.cn/Article/details/gtkofchqt.sHtML

pat = re.compile(r"\d+")
来源：http://baike.hesvh.cn/Article/details/gombnvljy.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fehbvm.com/Article/details/gnkesueso.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.zdbjq.cn/Article/details/ghloucnfw.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.hesvh.cn/Article/details/gmuhnnbsy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fehbvm.com/Article/details/ghctzftve.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.zdbjq.cn/Article/details/gsklswjqt.sHtML

@contextlib.contextmanager
来源：http://www.share.fehbvm.com/Article/details/gkbzejpud.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/gjbxuazjz.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/gwcprmruq.sHtML


<!-- 参考信息 -->