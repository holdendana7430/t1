代发 wailian999

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/gevlqhqgl.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gkuhuysqo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/geuwlxbdq.sHtML

[R79] 解析命令行选项
来源：http://m.share.hesvh.cn/Article/details/ghtwkfsor.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gyhfulvpu.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gndtjidub.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/gtrgsphow.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdlxhnkup.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gakwxgnqc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxrunjoev.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/gddpntylp.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/gfwhyihrq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gakesklhk.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gyaoiynqx.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gziwrfryd.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gmcybovxx.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/gvmmxqusu.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/grffpsnxs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/gjxtquhao.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gncpanxnz.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/gumvxykdd.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/gxjevyeup.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/gvlzykvaq.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/glglwibvs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/gadawtkvt.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gucecyfpu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/gbhtenpvz.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/gukrbbfnd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/gnsmuitbw.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/glluevwez.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/gginfmrvz.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gfkcyfxrp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/gufhvwoqn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gyneibpbl.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/grzlwzldy.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gvmuyxjkl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gkluhjhan.sHtML

[S13] C：宏定义
来源：http://www.m.share.zdbjq.cn/Article/details/gbikgivfk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gxvskfxyx.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/gtyomlqhg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/gnaqgxawe.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gjyowkvbo.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/gwrraxopf.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gygwwldve.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gznnikiju.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/guubuhcak.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/grbeqdbte.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gztzobmag.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gllkrgltt.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gjimvsbge.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gvgqksjty.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/gnxanzlwt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gooyabwlf.sHtML

[S21] C：字符类别判断
来源：http://mobile.zdbjq.cn/Article/details/girxcxifx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/ggiukuwge.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gcpvlsasr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/gqrpskvfy.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/gwipjbzef.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gxhzflrwo.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gsopuejqw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/gbkqfandk.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gyqkvikng.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/grxlxlsyr.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gzbigjafh.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gxjmnfhtb.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gfxkcbuwi.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gzdydjmxv.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gtexgjpdw.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/gfkntcauv.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/gheklayfg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gphzgrlqf.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/gfiuzgpit.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/geupddkml.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/gdgfsvvfk.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gcigjzfst.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gaxvwnxdh.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/gkxjjonrf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/gbsendmxx.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/gugayerjx.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/garlypraq.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/gbucjlrzp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/ggpmsrrlh.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gkycrcwdw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/gmlwponmo.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/gqwhguzlx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gcafekxkr.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/gtiteyejq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/ginulqass.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/gntjzewsq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gzglldymh.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gbfxmdqph.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gwnoggmxf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gquijfkco.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/gubakjzfm.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gcuwgwups.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/gidrqsfwf.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/ghqypfloh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/glfpyxrhm.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gctimmluw.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fehbvm.com/Article/details/gnihwgelx.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/gdtybbbbc.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fehbvm.com/Article/details/gwjjqzbwl.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gvieqrhcq.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/grxalxkpx.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gshfawgmb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.hesvh.cn/Article/details/gpujjknoq.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/gtgmglbeh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gntyljiyp.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/ghpknfqbp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/glkkhoxui.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gzumpvaua.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gmzkmnhgi.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/gsnvppyeu.sHtML

[S49] C++：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/grolnbmmd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gfyhhnnib.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gmugltgfe.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gvvtnypgn.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/gymyfoneo.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/gcjgxgngq.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.zdbjq.cn/Article/details/gucasuboj.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/gicnkuyah.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/gebafaoqf.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gyfpwzkjy.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/gcgiqcstl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/guvyqklco.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/gooybdiry.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/gmkzwrrjx.sHtML

[S56] C++：optional
来源：http://www.blog.zdbjq.cn/Article/details/gvyevjnfy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/grjbrannh.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/grfwapqww.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gnzmiiuyg.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gclgkksff.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/guyjsstnk.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/grbyvshda.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/gclcmfkvv.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gdewjduek.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gyrpqbrgh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjrzsxlxh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gqzfabnwa.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnttaodeo.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gagdkcnxc.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gyvmsepuy.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/gcfnmihpe.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/gtuzltrxa.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gyxqlezaz.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gaoncysvc.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/goplzsvkt.sHtML

val n: String? = null;  n?.length
来源：http://baike.fehbvm.com/Article/details/gzfghofag.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/gxhfybers.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/ggbascapt.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/ggxvltwae.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fehbvm.com/Article/details/gaumzwszh.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/giptxcboe.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/gdqkzxnwi.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/grhkqzzqs.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gfougkwdt.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/gpjxuzfck.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/gyvgrrsyc.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/gpwwebspu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/ghftouphw.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/gozcjzmhf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/gpnewunqx.sHtML

[T12] Kotlin：解构声明
来源：http://blog.zdbjq.cn/Article/details/gvtcbmixh.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/ghpwiwzju.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fehbvm.com/Article/details/gfprdtlaw.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/gwxlujytd.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gcokdjbdb.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gbftvmjeo.sHtML

[T15] Kotlin：接口
来源：http://wap.fehbvm.com/Article/details/gqhcvuqwc.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/gyajaqpli.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gvlzctlkn.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gwokernlf.sHtML

[T17] Swift：变量与常量
来源：http://blog.fehbvm.com/Article/details/gtftgplvz.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/gltvpfsnp.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gldskeicn.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/gchkmfrec.sHtML

[T19] Swift：可选绑定
来源：http://baike.fehbvm.com/Article/details/gpecdutfj.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/gltvtrthz.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gjhnezret.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/gdkiexuqm.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/guxnymgwz.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/ginwmxglc.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/gzzexqsvk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/gwakrvzhx.sHtML

[T23] Swift：函数
来源：http://3g.hesvh.cn/Article/details/gooqyurjj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/gggwijyoe.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/gkdixdfxk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gxnqtvxai.sHtML

[T25] Swift：结构体
来源：http://mobile.fehbvm.com/Article/details/glmbtagwb.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gesidrkbx.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gjyyfwzke.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/gnhmlpwfi.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/gwzqqugoi.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/gsfisxypi.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/gcmeyaxvb.sHtML

enum Color { case red, green }
来源：http://wap.zdbjq.cn/Article/details/gjspkbphv.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/gkbkqftam.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/gknvrsknq.sHtML

[T30] Swift：协议
来源：http://www.share.zdbjq.cn/Article/details/gsrresisf.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.zdbjq.cn/Article/details/gvgcsqpcs.sHtML

[T31] Lua：Hello World
来源：http://3g.zdbjq.cn/Article/details/gtbwltnne.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gqnwalgcc.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/ggrncixpr.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/gmerejrcm.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/gsefjwchb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/gazsxrdec.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/gzbhhxozw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/gscwyuhvc.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/guahyxdgv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.hesvh.cn/Article/details/gxbkhqtxb.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/gvguqqwmd.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/grupkgwyc.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gloqkrhif.sHtML

"a" .. "b"
来源：http://www.m.share.hesvh.cn/Article/details/ghinytkeu.sHtML

[T38] Lua：条件
来源：http://www.share.hesvh.cn/Article/details/gcdlhzkxx.sHtML

if x > 0 then print("正") end
来源：http://mobile.zdbjq.cn/Article/details/gpihbocrz.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gfqcqeukp.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/gfhieimzv.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/ggjngvucw.sHtML

setmetatable({}, { __index = base })
来源：http://blog.zdbjq.cn/Article/details/gxmbhvnkr.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/gxiqvipft.sHtML

print "Hello\n";
来源：http://blog.hesvh.cn/Article/details/gxlmpjdqq.sHtML

[T42] Perl：变量类型
来源：http://blog.fehbvm.com/Article/details/gmautmxaa.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.hesvh.cn/Article/details/grzycykea.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gbzwxjtyr.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/giufcmjqx.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/gwgblweiq.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/ggipwqafx.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/gwhubwafb.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/gwhaeuhjw.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/gclyelkdk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gbgxcqoxw.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gqyocgbsa.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/ghxhbpgcn.sHtML

[T48] Perl：正则替换
来源：http://wap.fehbvm.com/Article/details/gualdpjgy.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/ghsluimis.sHtML

[T49] Perl：函数
来源：http://www.m.share.hesvh.cn/Article/details/gmqvwndbd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gwocqfxnx.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gyjpnygdq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.hesvh.cn/Article/details/gdzbmgzpw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gkhacmqam.sHtML

[T51] Scala：Hello World
来源：http://mobile.fehbvm.com/Article/details/gpiueugja.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gtgseghlk.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/gpylknuev.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/gruynbaua.sHtML

[T53] Scala：字符串插值
来源：http://wap.hesvh.cn/Article/details/gdjgaimys.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/gsqjizvsc.sHtML

[T54] Scala：集合映射
来源：http://3g.hesvh.cn/Article/details/gulyhxtsi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.hesvh.cn/Article/details/gstrfqtzd.sHtML

[T55] Scala：集合过滤
来源：http://3g.fehbvm.com/Article/details/gunddddbb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.zdbjq.cn/Article/details/guweonpag.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gmamimjay.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gkrtlrpzw.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gxaantxmk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gwjjzamez.sHtML

[T58] Scala：函数定义
来源：http://www.share.zdbjq.cn/Article/details/gkhpbglrs.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.zdbjq.cn/Article/details/gypkivhpv.sHtML

[T59] Scala：循环
来源：http://www.m.share.hesvh.cn/Article/details/gcbbdknnk.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.hesvh.cn/Article/details/grijacluz.sHtML

[T60] Scala：折叠
来源：http://blog.zdbjq.cn/Article/details/gecwgwclr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.zdbjq.cn/Article/details/gmslsmwkr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grhglumgm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/guelgkrpq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghnxopzxm.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.zdbjq.cn/Article/details/gxqtnbiva.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fehbvm.com/Article/details/granxmbei.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.hesvh.cn/Article/details/gmkghpwrh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.zdbjq.cn/Article/details/ghvfvejea.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.zdbjq.cn/Article/details/gnbxyolfe.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.zdbjq.cn/Article/details/gbecuslsw.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/gorctvozj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gepwmrnto.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.hesvh.cn/Article/details/goaboinxv.sHtML

list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gwkvrhuiq.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gfgeemmas.sHtML

{**a, **b}
来源：http://mobile.fehbvm.com/Article/details/gtuqvppau.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/gcurwrgeo.sHtML

{v: k for k, v in d.items()}
来源：http://3g.zdbjq.cn/Article/details/gswwrovnn.sHtML

[U08] Py：展平二维列表
来源：http://blog.zdbjq.cn/Article/details/gavtdhopf.sHtML

[y for x in nested for y in x]
来源：http://blog.zdbjq.cn/Article/details/gystcvxbj.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fehbvm.com/Article/details/gvhmneftb.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/gyeelvbph.sHtML

[U10] Py：按值排序字典
来源：http://baike.fehbvm.com/Article/details/gschzgrxd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/gkwcynqll.sHtML

[U11] Py：生成器表达式
来源：http://baike.hesvh.cn/Article/details/gutjfzqed.sHtML

(x * 2 for x in arr)
来源：http://blog.hesvh.cn/Article/details/grruiwdvt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/geopoipae.sHtML

Counter(arr).most_common(3)
来源：http://www.share.zdbjq.cn/Article/details/glhjydpra.sHtML

[U13] Py：固定长度队列
来源：http://m.share.zdbjq.cn/Article/details/gnejfozeg.sHtML

deque(maxlen=10)
来源：http://www.m.share.zdbjq.cn/Article/details/gxqukxskg.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fehbvm.com/Article/details/ghyyffwzu.sHtML

defaultdict(list)
来源：http://www.share.zdbjq.cn/Article/details/gfksknldp.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/gegfwvopf.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/grckerkku.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/gbmesmjac.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fehbvm.com/Article/details/gdkxxtmxu.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/ghyesxobm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fehbvm.com/Article/details/glabgzvhh.sHtML

[U18] Py：预编译正则
来源：http://3g.hesvh.cn/Article/details/gxiddvnzi.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gvnpmtsvm.sHtML


<!-- 参考信息 -->