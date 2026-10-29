代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/godsvofyy.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/goxwhoujc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gxdywgewi.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/gomgpaddi.sHtML

read -rp "请输入: " ans
来源：http://www.share.zdbjq.cn/Article/details/gqijlprvz.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/geklbnmoy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/gqwwrdojb.sHtML

[R79] 解析命令行选项
来源：http://mobile.hesvh.cn/Article/details/gpocriotb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gabmrjsel.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gucnorepy.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gpwenltns.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghmbbboof.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gebxhdymp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggxtdsiut.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/gxapakgjt.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gnqjmacte.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/gfcmtqlif.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gbvbeqkgy.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/gjxscstuy.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/gneixudsc.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gyfszxljv.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gcbnoqged.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/ggbhylyhn.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/gfekuqixz.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gslpbvvmt.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/grpxkxwkb.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gejnprczw.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/gnnxhlphy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gmjlpujty.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gpubrltzg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/gxzutqwol.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/gjhvezbdj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fehbvm.com/Article/details/ggyqvqbno.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/gheijtdqh.sHtML

int *p = &a;  *p = 5;
来源：http://baike.zdbjq.cn/Article/details/gumqtjogs.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gjuymyqag.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gixaswdbq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/ggqpyzgdy.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gtzsriddh.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gliyijlbi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gxrwqwmow.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/giviazusj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gteskbprm.sHtML

[S14] C：枚举
来源：http://m.share.zdbjq.cn/Article/details/gpsyckdhg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/gbyaqalqh.sHtML

[S15] C：类型转换
来源：http://wap.zdbjq.cn/Article/details/gieonwkym.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/gnfczvyyb.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/glyehwnfz.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/gybtlyjqy.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/gousbhnmh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gmickoinp.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gipzfmupj.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gbqlgrxyk.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gjqqolvwp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gdhyngyxu.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/goyrfltpf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gpkcvloqa.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/ggynlqpqh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gqpndcpdj.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gsikvmqbl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/gbtabetnf.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/gcjyjhygn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/ghdsvngbk.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/gcmvikjzx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gcgcalctc.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gusccpirq.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gnwuwxypa.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gjrkquqkz.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/glpyeihct.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/guvphcloj.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gljtqavqj.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/gunubmtkf.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gkzorvjdv.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gzfiqxytc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fehbvm.com/Article/details/gybgcwqia.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/gehhcnurn.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/giprwtsls.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/giudtegfi.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/ghfjaikmk.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/glhobhvdk.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/gptkffrqe.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.zdbjq.cn/Article/details/gldilflbh.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gtkcmwaop.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gyrrdhqkg.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gkjsabpsp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gtvtfcqsi.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/grtkogoow.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gwrwwqehf.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gpjyoqgiu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gpmbnykxt.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gpkvcwsqd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gkzdfulzx.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gzkqpfczo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gyulqjpbt.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gtgokeszx.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/ggvhfudsp.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gkkpxkuwt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/gjbqsykup.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gpiimnzfb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gsdfdxevj.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gbjkwtvlf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/ghcyqgojb.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/gkxwdcgcw.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gvlygmqsc.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/goxmrhurj.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/gvuroxzxp.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gzzbozsgd.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gzvgosakb.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/gizggrgqd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gznrpgfqy.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gtssbixje.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.hesvh.cn/Article/details/gfsreqjkv.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/grnoumlqe.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gzvdchkmm.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gzewxflkt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fehbvm.com/Article/details/gzqsnyjbq.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/gchyykgnh.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gzzemqpzs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/gibiuwgqz.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gqnmijshp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gfrwgvbfk.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gdnveatjt.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gocfwmasi.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/ghotkfpgs.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/gprsnasqn.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/gicleabuq.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/ghjybdduz.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/govxawwyj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fehbvm.com/Article/details/ghqhltznb.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/gmtijlgwc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/geccftcqr.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gwogqhaea.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gubqddquf.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gfgmfbloj.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/gxjqsjvrp.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/ghxmajmaf.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gicdrhhwb.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gvwgvogtk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/gmivbpfvp.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/glkeceqac.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gvcjsvcjw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjffhgwhv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gbchehtio.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjevtkrns.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gurvcapmb.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/ggbgwiydc.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gxkmwxsrq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gqigvuhbx.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gopffzxcz.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/glqrryork.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/guknwvdca.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/gyowogrhw.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/ghkdsmbcj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.zdbjq.cn/Article/details/gqfqxjbod.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gqcaninfj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/grempplnk.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gbbhwrart.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/glijabazf.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/gwebfhsvm.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/gpuaptooy.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gdccdzten.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/gtasklvme.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gechqgwea.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/gtbfweopb.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/grnguljmt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gqpshufji.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/gvddejyyw.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gytaqhulo.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/gqokwgffr.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gjdkqyktp.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/grgtyjmmi.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/gyivwzpgi.sHtML

[T15] Kotlin：接口
来源：http://wap.fehbvm.com/Article/details/gysekzwno.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/gqrduutuz.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gwqqmxgpt.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gjlaoggpe.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/ggsgfvftq.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gybaqnlkn.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/ghkqxhctv.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/gechjddhz.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/gzabxasoy.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/gjaebuhbf.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/gpphtpafx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/gnjflscah.sHtML

[T21] Swift：遍历
来源：http://baike.fehbvm.com/Article/details/gconjsdzt.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/gqlqvtuax.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/gyoxnvlvt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gxtighsca.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gajzgbgmd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/giyvywsvs.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/giivjgmhi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gvpnuyizj.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gotjpgtie.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/glbgggwae.sHtML

[T26] Swift：类与重写
来源：http://3g.hesvh.cn/Article/details/gbdrkevov.sHtML

class A: Base { override func f() {} }
来源：http://mobile.hesvh.cn/Article/details/gwzbcexcp.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/giuwsohub.sHtML

do { try f() } catch { print(error) }
来源：http://baike.zdbjq.cn/Article/details/gagvyzgmu.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/goojteohg.sHtML

enum Color { case red, green }
来源：http://3g.hesvh.cn/Article/details/gnqptdivx.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/gdvygafzl.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/gtoaijvdz.sHtML

[T30] Swift：协议
来源：http://baike.zdbjq.cn/Article/details/gennirnpl.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fehbvm.com/Article/details/gbajdifye.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/gmjqszxjg.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gdwfafaup.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gmakjydvn.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/gjzifddlz.sHtML

[T33] Lua：表（数组）
来源：http://mobile.hesvh.cn/Article/details/gufkrjdku.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/gzevsgecu.sHtML

[T34] Lua：遍历表
来源：http://read.share.fehbvm.com/Article/details/gucwhzrjy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gscuqltsg.sHtML

[T35] Lua：字典表
来源：http://m.share.zdbjq.cn/Article/details/gpgfgrhpl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.hesvh.cn/Article/details/gqmfxtahs.sHtML

[T36] Lua：函数
来源：http://www.share.fehbvm.com/Article/details/gvddqwsjh.sHtML

function add(a, b) return a + b end
来源：http://m.share.hesvh.cn/Article/details/gyaahpbdr.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gebbvyzoq.sHtML

"a" .. "b"
来源：http://read.share.zdbjq.cn/Article/details/gzppfrpbh.sHtML

[T38] Lua：条件
来源：http://3g.zdbjq.cn/Article/details/gefecnwqj.sHtML

if x > 0 then print("正") end
来源：http://read.share.hesvh.cn/Article/details/gxepnwwkm.sHtML

[T39] Lua：模式匹配
来源：http://3g.hesvh.cn/Article/details/gwtwvejjg.sHtML

string.find(s, "%d+")
来源：http://www.blog.fehbvm.com/Article/details/geclijqzl.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/gikxrjlrw.sHtML

setmetatable({}, { __index = base })
来源：http://blog.zdbjq.cn/Article/details/gbcbntesd.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/gxayegssu.sHtML

print "Hello\n";
来源：http://mobile.zdbjq.cn/Article/details/gaadbxmzx.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/gkoyyejli.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/geyouieyk.sHtML

[T43] Perl：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gzrppwqno.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/ghqpzwlmx.sHtML

[T44] Perl：条件
来源：http://blog.zdbjq.cn/Article/details/gnaeafysx.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/gvhqewprm.sHtML

[T45] Perl：数组遍历
来源：http://baike.fehbvm.com/Article/details/gweqlfaer.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/gryllutlk.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.zdbjq.cn/Article/details/ghgyngguf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/gmwogkpvp.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/gakmhcxbl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.hesvh.cn/Article/details/gyiwpopgu.sHtML

[T48] Perl：正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gadvzqwwr.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gxiyxdmbl.sHtML

[T49] Perl：函数
来源：http://baike.zdbjq.cn/Article/details/gijglijbc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/grdcajzye.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gpptixnxb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fehbvm.com/Article/details/grdywidsq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/gbzcofshp.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gpfzvzttp.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/ghgdxuevk.sHtML

[T52] Scala：变量
来源：http://m.share.zdbjq.cn/Article/details/goxvznfzh.sHtML

val a = 1;  var b = 2
来源：http://wap.zdbjq.cn/Article/details/gppvempkd.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gjtcvdbmh.sHtML

s"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gkxschqyq.sHtML

[T54] Scala：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gsltdsbwp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.hesvh.cn/Article/details/gmpegzike.sHtML

[T55] Scala：集合过滤
来源：http://blog.hesvh.cn/Article/details/gkvdrmejh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.zdbjq.cn/Article/details/gfzuuhkmt.sHtML

[T56] Scala：样例类
来源：http://3g.hesvh.cn/Article/details/gnffmurzv.sHtML

case class User(name: String, age: Int)
来源：http://blog.hesvh.cn/Article/details/gflcdovqw.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gyfnyofju.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.hesvh.cn/Article/details/gpmsirquo.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/gxethnzlw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fehbvm.com/Article/details/gxkygydoj.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gwmdediyu.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gxxoesvyv.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gscddqhnc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fehbvm.com/Article/details/gqfgxhgje.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gukrpmqkd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gwavxrcpq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxdmmuyyh.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/gdjccfujk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.hesvh.cn/Article/details/gdldzditj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/gzygsxxye.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.hesvh.cn/Article/details/gkkvzhzbn.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.hesvh.cn/Article/details/gbhrmfufw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/gctddpbdf.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fehbvm.com/Article/details/gksccyeso.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/gtawuphdx.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fehbvm.com/Article/details/gybagbykk.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gzcadbqkj.sHtML

[U06] Py：合并两个字典
来源：http://wap.hesvh.cn/Article/details/gkvegkzyd.sHtML

{**a, **b}
来源：http://www.share.hesvh.cn/Article/details/gdufmrzru.sHtML

[U07] Py：反转字典键值
来源：http://baike.zdbjq.cn/Article/details/gwksunrjs.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/geipxiags.sHtML

[U08] Py：展平二维列表
来源：http://wap.zdbjq.cn/Article/details/gaujuivaw.sHtML

[y for x in nested for y in x]
来源：http://3g.fehbvm.com/Article/details/gyvnixshg.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.zdbjq.cn/Article/details/gfdfgpjit.sHtML

max(d, key=d.get)
来源：http://www.blog.zdbjq.cn/Article/details/gjpbeddxx.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fehbvm.com/Article/details/grpvcozbz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fehbvm.com/Article/details/gsezziiuf.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/gbnzbfhlb.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/gwmjjmher.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/gbetfenhs.sHtML

Counter(arr).most_common(3)
来源：http://3g.zdbjq.cn/Article/details/gkfwtznbf.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fehbvm.com/Article/details/ghzhgrlkc.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/gnymdasrp.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fehbvm.com/Article/details/gypyfanqa.sHtML

defaultdict(list)
来源：http://blog.zdbjq.cn/Article/details/gkcigmkui.sHtML

[U15] Py：高精度计时
来源：http://mobile.zdbjq.cn/Article/details/gthmjzjuj.sHtML

t = time.perf_counter()
来源：http://www.share.zdbjq.cn/Article/details/gfhmzqdbk.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/gbrwrhwnq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fehbvm.com/Article/details/gnfatqrsh.sHtML


<!-- 参考信息 -->