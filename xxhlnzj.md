代发 wailian999

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/gjfaijcec.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/gdinuhzao.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gpsiyycgl.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/gwyanovkc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/gocveldpp.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fehbvm.com/Article/details/gulswnxha.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gixtprjdm.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/gdlagaqyc.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/gvptkykuh.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/gxsmjqqpy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/ggbblogty.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gforuabpq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/ghrqfonfp.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gwqoyfegp.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/gijaglird.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grrhkzilr.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/gjcfiehlz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grfmluqqz.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/gkhizseri.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gyhcttpbb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gqflkogfg.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/ghrvmxsdc.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/gumfbvxcj.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gkianxnmm.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fehbvm.com/Article/details/gicjfezgn.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gocwjahvo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/gyccfekyz.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/guxlruvfy.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gtegclngm.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/gddjdzixq.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/ggfcadueu.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/gqcgnpuqo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/gyxvesliq.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gwgjlgcyk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/gpjkrphmh.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/gdayrugsy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gzykukuyh.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/goqltqpse.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/gfjqdbhba.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gggnyoncu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gfwlvfppc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gqorxqbkq.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gacdoprhm.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/gvlyfmbdb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/gaeuvhrlw.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/ggaldgivz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/getdyqjuf.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/getplvguj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/goxrgrtlu.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gpqylrzqm.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gdfpmxmtm.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/glhpaiijr.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gqdjcuhwa.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/gsgwdblda.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gkjpzlols.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gzxhlgipx.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gabddqrqv.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gitchktsj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gwvinmkpe.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/gjaiahalg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gdthhkcsr.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gwnhmlncx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/gdbksxiwd.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gvlivwpfb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/guyhmwmbe.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/ggnalouii.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gjvddxtvv.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gmyuvwenr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gzrdjtbcn.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/gteurksqf.sHtML

memcpy(dst, src, n);
来源：http://baike.fehbvm.com/Article/details/gegluykvh.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gfynzwizt.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gicrsdpxh.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gciwstdrb.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gqsoofexz.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/guduepcfv.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gamxdvuhk.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/gufnzexca.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gbeskotaw.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/giaahogdr.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/giktetftu.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/glisqirul.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/gonllubeu.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gpwbsajil.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/gbqiskcwz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gddeoxikl.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gkcvuwgsk.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/grifqgsax.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gmbcfachj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/gzjcacuip.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/gysqxlixb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/gwgluhdvk.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/ghkwtxaut.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gbodiugge.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/gkpxlsycx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gfsifsnse.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/ghtcqgmiu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/gmfcuwgcu.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/giwromydj.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/gmiuptkgn.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gzfdwdvah.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/grlqmimos.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/glkiusmmp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gvqigeltp.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/ggixftsrb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/gdleufgcv.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gwamrpofb.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gbahdfpam.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/ggvlcdbtb.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/geqckkeqy.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/gznfdpyvi.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/ggatbuxvh.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/gmyhlgejj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/gozxjjnyz.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/gmbvqzstk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/gmnzldcbd.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gmowjpyfs.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/guygcsjrw.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gneoojorb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/grwxxdydb.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gjfnvjjvu.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/ghhzkguzb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/gifwelqds.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/gkythddom.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gjliusbqj.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/gmvxivpeb.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/gdzwmjxun.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/gkjljswcj.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/gfvpxgbpk.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/gtpzbbecc.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fehbvm.com/Article/details/gmyynblov.sHtML

[S54] C++：异常处理
来源：http://read.share.hesvh.cn/Article/details/gdhodegjf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/ghsvlhpbf.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/guucyozkc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/gbleospgy.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gceaphwib.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.zdbjq.cn/Article/details/gxdjclhyf.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gvpzrcgtz.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/geutalxqo.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/gbqorbptd.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gwvfwydwl.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/getitqnhd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/ghgxhmlaf.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/giecawdca.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gahyfegwk.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/goytntxtt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gbeieqqgn.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjlpkeacw.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/glmyktwme.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gxtvdyjrn.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/ggkkplvlw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/ghvrgscpq.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/grmruwapa.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/gqqhjimln.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/gipeelwsi.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gpxfwsbei.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gycyiqeoi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gwekmhile.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fehbvm.com/Article/details/gsdveskwl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gafbrjnyy.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gksnlfzpp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gtbrxycdi.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/grzzrtcqp.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gkiocczhj.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/ghizlgons.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/gwwvtetxr.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/glpxnlnld.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/gghfhcvor.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gsosxowjd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/gmjdngvmn.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.hesvh.cn/Article/details/gcupslgjm.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/ghuqhdonl.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/gvfdfogdw.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gpvpvgmbb.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gkymllkeg.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/gmrzvwcqg.sHtML

[T15] Kotlin：接口
来源：http://m.share.hesvh.cn/Article/details/gwyuuqevl.sHtML

interface Shape { fun area(): Double }
来源：http://blog.zdbjq.cn/Article/details/gjtypxzua.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/gkyorkkgb.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gmwzvaljv.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.zdbjq.cn/Article/details/gmcsvvmxt.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/ggarqejed.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gzimljcxu.sHtML

"值: \(b)"
来源：http://www.m.share.hesvh.cn/Article/details/gcmpsjmlf.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gkalikznh.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gwlpplaff.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/gmfwqvpsg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gshikkqwl.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/ghyoboxjh.sHtML

for x in a { print(x) }
来源：http://www.m.share.zdbjq.cn/Article/details/gaqzbctmk.sHtML

[T22] Swift：字典
来源：http://blog.fehbvm.com/Article/details/gadrrnqlm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.zdbjq.cn/Article/details/gmgzabuar.sHtML

[T23] Swift：函数
来源：http://mobile.fehbvm.com/Article/details/gacvagbxd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/gqbaenaph.sHtML

[T24] Swift：闭包
来源：http://blog.fehbvm.com/Article/details/gdzxykxba.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gulsrffqx.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/ggmtlkklx.sHtML

struct P { var x: Int }
来源：http://mobile.fehbvm.com/Article/details/gqaohggxu.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/gcaabnsbn.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/gnnzhnxax.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/gfkldvwhl.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/gdomzlskz.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/gmihlkirr.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/gakrxxzld.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gxtmmficf.sHtML

guard let x = opt else { return }
来源：http://mobile.hesvh.cn/Article/details/giqldjwrj.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/ggovixbla.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.zdbjq.cn/Article/details/gxtyydpzp.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gsfyawecj.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gcnavbagn.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/goeedddzm.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gnahcvwag.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fehbvm.com/Article/details/gypywrdyk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/ggyjnujgb.sHtML

[T34] Lua：遍历表
来源：http://blog.fehbvm.com/Article/details/gyqdmyukv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/gcgyectjb.sHtML

[T35] Lua：字典表
来源：http://m.share.fehbvm.com/Article/details/gvkwdmnbn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gzbspowrd.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/gvuvxdocj.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/gskpfsjig.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gtpvnjdnr.sHtML

"a" .. "b"
来源：http://www.share.fehbvm.com/Article/details/gukljxtmv.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/goukbipsk.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/gzqogrhla.sHtML

[T39] Lua：模式匹配
来源：http://3g.fehbvm.com/Article/details/geluimynp.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/gmnnwznyu.sHtML

[T40] Lua：元表
来源：http://baike.fehbvm.com/Article/details/gvhiekuki.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fehbvm.com/Article/details/getmurdku.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gyrdxthrx.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/gdiazgjcj.sHtML

[T42] Perl：变量类型
来源：http://baike.hesvh.cn/Article/details/gwcjfuvqw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/ghojhkjpy.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/gjqeafwme.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/guvxxslkk.sHtML

[T44] Perl：条件
来源：http://3g.hesvh.cn/Article/details/ggmhctrkt.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fehbvm.com/Article/details/gtqlkyrnv.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/gsrxwhzbu.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/grlevcmdx.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/gedoyavlu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gonhfgbwb.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fehbvm.com/Article/details/gxesfneok.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/gfipecktx.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/giafqiolt.sHtML

$s =~ s/old/new/g;
来源：http://baike.zdbjq.cn/Article/details/gcyzqbabu.sHtML

[T49] Perl：函数
来源：http://www.blog.fehbvm.com/Article/details/gthfgrdla.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gwkenhffz.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gfziqlpvk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/gjqtirsiy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.hesvh.cn/Article/details/gvdzevhnu.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/gdnotxrww.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gmcqlxnpp.sHtML

[T52] Scala：变量
来源：http://www.blog.fehbvm.com/Article/details/ggvaqsbet.sHtML

val a = 1;  var b = 2
来源：http://www.share.zdbjq.cn/Article/details/getakswdi.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gevpsprvj.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/gzalafgfd.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gccsptkka.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.zdbjq.cn/Article/details/gavpmrkmg.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/glohhojun.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.zdbjq.cn/Article/details/gsinhrgjf.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gesuyqrpx.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/geaheavfm.sHtML

[T57] Scala：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gjdasqfte.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.hesvh.cn/Article/details/gsjqsugyc.sHtML

[T58] Scala：函数定义
来源：http://mobile.fehbvm.com/Article/details/gglpdlqrt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.zdbjq.cn/Article/details/gokqvpmpx.sHtML

[T59] Scala：循环
来源：http://wap.hesvh.cn/Article/details/gullpumlc.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gdwjcvoow.sHtML

[T60] Scala：折叠
来源：http://read.share.hesvh.cn/Article/details/gtiicihfp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.hesvh.cn/Article/details/gdvaduldu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gisjszuvc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/glkgqxizr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbqvxorfg.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fehbvm.com/Article/details/gmmoplthy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/gpdsqooby.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.hesvh.cn/Article/details/glnyhpoxt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fehbvm.com/Article/details/gehdfolfo.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.zdbjq.cn/Article/details/gmletxftk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.zdbjq.cn/Article/details/gvhebizif.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gqteuqzvg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.zdbjq.cn/Article/details/grblyaoky.sHtML

[U05] Py：列表去重且保序
来源：http://wap.hesvh.cn/Article/details/gohflguxu.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gczdquwim.sHtML

[U06] Py：合并两个字典
来源：http://baike.fehbvm.com/Article/details/gvmqndmjy.sHtML

{**a, **b}
来源：http://www.share.fehbvm.com/Article/details/gqwdbbvxk.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/ghawceoad.sHtML

{v: k for k, v in d.items()}
来源：http://3g.hesvh.cn/Article/details/gymbvrfvj.sHtML

[U08] Py：展平二维列表
来源：http://baike.zdbjq.cn/Article/details/gnbvoekef.sHtML

[y for x in nested for y in x]
来源：http://www.blog.hesvh.cn/Article/details/getnxltqm.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fehbvm.com/Article/details/ggizhwpdb.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gqqtknlol.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.zdbjq.cn/Article/details/gqiaxircl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fehbvm.com/Article/details/gxgmayyrg.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fehbvm.com/Article/details/gwxukjofo.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fehbvm.com/Article/details/ggkvtgwcp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fehbvm.com/Article/details/garoiaxbk.sHtML

Counter(arr).most_common(3)
来源：http://wap.hesvh.cn/Article/details/grdawoqlb.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/grvzwuuat.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/gcvyubpgq.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.zdbjq.cn/Article/details/gmapwsedc.sHtML

defaultdict(list)
来源：http://wap.hesvh.cn/Article/details/gsgcdzkri.sHtML


<!-- 参考信息 -->