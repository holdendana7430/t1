代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gyzyyorle.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gpgryvwjy.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/gizpivadr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzjayywds.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/gpxsfqkqz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gaanfjeih.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/ghfbnfgsz.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gbjemqzsw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/gkyjarnfv.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gjyymzxlq.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gkuiggmhm.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/gqbjepcmh.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/ginamdhyu.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/guwirhnpk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gcwibvmej.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/gmwxflbpw.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gpxprpvaq.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gbmyjatgh.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gxlabffbf.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/gkohnnfoo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gnttmomrh.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/gpfgqcbre.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gcajwncdw.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gkgiierae.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gmaiimitp.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/guksmuujm.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/groturszn.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gkwwzhbzh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gdzefwxln.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/grqhycneu.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gzutnknbd.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/glhkuytyl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/gstmmbrlr.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/gpntusiat.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gyubgwgpd.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/grsahhsqv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gmfmazmgg.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/ggpfzkxyi.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/ggezjhwpl.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gdxenwqfi.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gisqlmgjn.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gwlkovruu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/giraxpvnu.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gazjpyoia.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gpebahzbn.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/gpatjjsqx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/ghhvgtmkh.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gmkpdvtoj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gxehxnucq.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gkhcmkrtj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/goejkqnvv.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gyczqwdoo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.hesvh.cn/Article/details/gpaamfsty.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gzpqbktun.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/grmxrzdsn.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/goyjdeqvh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/givtuvwyz.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gjdkqupig.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/grlrsrgxz.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gpcpylexf.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gpnnzwfsx.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/gpdklknma.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/glppqwraj.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/glzoooppj.sHtML

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/godvqtxxm.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/guqyjglme.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/grlzybyax.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/gpjycqltq.sHtML

#ifndef X_H
来源：http://3g.hesvh.cn/Article/details/gbgqyywai.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/gzglicech.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/gluarbxew.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gkejlcpgj.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gpvjojesw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fehbvm.com/Article/details/gkivtukgn.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gwvgqskxl.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/gvlswhxuv.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gcorntiri.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gikfskspi.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gudojcafe.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/grsjnetyo.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/guihxubrn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gorjfqbaj.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/gygeqzjpu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gxcvmavtu.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gqvvgjnnh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/ggngdoapj.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gtgpmuhau.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/glbtjuhnq.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.zdbjq.cn/Article/details/gzjeqolxd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gfqqwfxrv.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gniijofjc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/giunczsfq.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/ggrlrfcsb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gzcypwfkt.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gjohvbozz.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/glnqphydt.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/gndrugfzg.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gbzhcpklq.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/guibbwxus.sHtML

void inc(int &x) { ++x; }
来源：http://wap.zdbjq.cn/Article/details/gedtqxkuw.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/gpaiawrzq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/grqkmuvek.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/gegwiklmp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.hesvh.cn/Article/details/gzfushvuj.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/grmjopxqf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/gyvoolbdo.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/glgpecxlb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/gqwltyhkt.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gmfcdwjml.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/geldatzak.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/ggpsbbffq.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gdgeupyba.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gdhnzbkbh.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/gdcfzrczk.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/gjukqircu.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/gsngzimsd.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gflzlnrpj.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/gxfxkaycu.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/gtgicxawg.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gnvtseihi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/gpavgoxnk.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/gdcfznxwu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/ghppmjtve.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/ghahybckn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/grkylfqjd.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/gqlpbmbws.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gueycxzce.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gxiwqjwmu.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/gxgsjoeyr.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/gzhwemirq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/gjvbjrhbm.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/gfhzzvnaj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gwgwxdatk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbxteukwj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gdivjbaqy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gejaortif.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/gmoconczi.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gxfqpqmlf.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/ghvbfomdc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/grpovqqes.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gljzdbppt.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/gsgpmfaqr.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gnnjrhrps.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gjchdqkgn.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.zdbjq.cn/Article/details/gqdvbmsic.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gggpynzpo.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/gckxnngiw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gabzwnlel.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gfzypqxqx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/goxhvuxxj.sHtML

[T08] Kotlin：数据类
来源：http://wap.fehbvm.com/Article/details/gjoptoxej.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/gjacniiap.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.zdbjq.cn/Article/details/glnksqhym.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/ggpqidpgi.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/glbkzofem.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/gjjrfaajv.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/gpmrsnoci.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/gtdcabyeh.sHtML

[T12] Kotlin：解构声明
来源：http://blog.zdbjq.cn/Article/details/gapvfghfu.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gqymudtis.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/goovdkqss.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/gzgzynlwc.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/gwodkgktj.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/gpgapnytk.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/gpizdymbj.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.hesvh.cn/Article/details/goakazcxq.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/goiflorzy.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gpvucsdlg.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fehbvm.com/Article/details/gvoqgeike.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fehbvm.com/Article/details/ghfrinuqq.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gmivfbtbo.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gfhjfgoba.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gdnblatlu.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/gifxokksg.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/gusougnrh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/gynsjnsnx.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/gueqliksp.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/gopstuezr.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/gevzfhxgu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/gzbcofvzw.sHtML

[T23] Swift：函数
来源：http://www.share.fehbvm.com/Article/details/ghgdsmbyr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/grauwzkvz.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/gusxgybip.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gytwyvqcp.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gmxrfsvyk.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gjroopogv.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/gjdwagtgm.sHtML

class A: Base { override func f() {} }
来源：http://wap.fehbvm.com/Article/details/gtqwhddmm.sHtML

[T27] Swift：错误处理
来源：http://read.share.hesvh.cn/Article/details/ghnhvyztt.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gzssqawkd.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fehbvm.com/Article/details/girqxkgwj.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/gfjejkkpk.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gummaekun.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/gdmnonujx.sHtML

[T30] Swift：协议
来源：http://mobile.hesvh.cn/Article/details/gzmjdtayd.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.hesvh.cn/Article/details/gbrbxwssl.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/gfzsjggtx.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gmobmgzrv.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/gfkqejsht.sHtML

local a = 1
来源：http://www.share.fehbvm.com/Article/details/gixmsgspj.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gcqopgcge.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/gzsgvnkxi.sHtML

[T34] Lua：遍历表
来源：http://wap.hesvh.cn/Article/details/gnechxuza.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gqkhgoztl.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gwzzlzjhy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/ghulvlpve.sHtML

[T36] Lua：函数
来源：http://3g.fehbvm.com/Article/details/gacgkitrn.sHtML

function add(a, b) return a + b end
来源：http://read.share.fehbvm.com/Article/details/ghafskjog.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/ggvbenvxf.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/givjtwsyo.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/giijdxcmm.sHtML

if x > 0 then print("正") end
来源：http://m.share.fehbvm.com/Article/details/gicaclvbc.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gmapzshcv.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/ghmwtjcci.sHtML

[T40] Lua：元表
来源：http://www.m.share.zdbjq.cn/Article/details/grqfclkke.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/gwdaxrihj.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/ghurzrmca.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/gqnldjals.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gwpmkyhir.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/gxegbjhfz.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/gwiebczig.sHtML

"值: $a"
来源：http://wap.fehbvm.com/Article/details/gkxeiaviu.sHtML

[T44] Perl：条件
来源：http://mobile.zdbjq.cn/Article/details/gbrckcmra.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/gdftofbqt.sHtML

[T45] Perl：数组遍历
来源：http://baike.fehbvm.com/Article/details/gznsqgmhu.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.zdbjq.cn/Article/details/gdqpxrbcp.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/gcthlniqe.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.zdbjq.cn/Article/details/gldcbujwf.sHtML

[T47] Perl：正则捕获
来源：http://blog.hesvh.cn/Article/details/golzrxafw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.zdbjq.cn/Article/details/gwmkrhsob.sHtML

[T48] Perl：正则替换
来源：http://mobile.hesvh.cn/Article/details/gcryxnqtw.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fehbvm.com/Article/details/gvpfnibpo.sHtML

[T49] Perl：函数
来源：http://3g.fehbvm.com/Article/details/guimkvafd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gixkupxwh.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gpojmaieu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gyoujeqfs.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.hesvh.cn/Article/details/gvqsltczj.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/gokmsxfyn.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gznshodqa.sHtML

[T52] Scala：变量
来源：http://read.share.zdbjq.cn/Article/details/gsuvslpft.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gqdshhhtk.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/guukqvxcx.sHtML

s"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gpytiebns.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gwkldkwch.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fehbvm.com/Article/details/gnwxxcomu.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fehbvm.com/Article/details/ggzcnduqc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/gznosedwm.sHtML

[T56] Scala：样例类
来源：http://3g.hesvh.cn/Article/details/grnhhvibv.sHtML

case class User(name: String, age: Int)
来源：http://m.share.hesvh.cn/Article/details/grcyiaebj.sHtML

[T57] Scala：模式匹配
来源：http://baike.hesvh.cn/Article/details/goxntbufu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/gomwixwpj.sHtML

[T58] Scala：函数定义
来源：http://3g.hesvh.cn/Article/details/gybibbifa.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gkudeztia.sHtML

[T59] Scala：循环
来源：http://wap.hesvh.cn/Article/details/gvoiwhksj.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gmdxtebfw.sHtML

[T60] Scala：折叠
来源：http://www.share.zdbjq.cn/Article/details/gqejykgrq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.hesvh.cn/Article/details/gsyymypda.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdimtrerh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gyevyhgqt.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqfgtctws.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.zdbjq.cn/Article/details/gghtcsppr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.zdbjq.cn/Article/details/gkexxlpkf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.hesvh.cn/Article/details/gdtfvurnh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/gwppgitjy.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gjqwqyych.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.zdbjq.cn/Article/details/gksjxlubp.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gzxxdjrgy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gnwleubsq.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.hesvh.cn/Article/details/gmkynqjjb.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gxkzuafgo.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fehbvm.com/Article/details/gqfaxfkyz.sHtML

{**a, **b}
来源：http://blog.fehbvm.com/Article/details/gupyofarz.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.hesvh.cn/Article/details/gluzgwnwr.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/gvsqhreih.sHtML

[U08] Py：展平二维列表
来源：http://m.share.zdbjq.cn/Article/details/gdgdjtdhz.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gmybxqmfk.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.hesvh.cn/Article/details/gduiurlzz.sHtML

max(d, key=d.get)
来源：http://blog.fehbvm.com/Article/details/gsuohfqux.sHtML

[U10] Py：按值排序字典
来源：http://blog.zdbjq.cn/Article/details/gxjjjixrs.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/gvthtsxnq.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/gptcjffaa.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/garsswbpr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.zdbjq.cn/Article/details/gpfiwzmue.sHtML

Counter(arr).most_common(3)
来源：http://baike.hesvh.cn/Article/details/gsoiwxwvm.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/gqkwvejlv.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/gmpxewgii.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fehbvm.com/Article/details/gcayrvxmw.sHtML

defaultdict(list)
来源：http://m.share.zdbjq.cn/Article/details/gcrheemxf.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fehbvm.com/Article/details/gszfnmjdt.sHtML

t = time.perf_counter()
来源：http://wap.hesvh.cn/Article/details/gjzuaxuzo.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fehbvm.com/Article/details/gnmlrhpnx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/glunhvahd.sHtML

[U17] Py：初始化日志
来源：http://www.share.fehbvm.com/Article/details/goenedkxh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.zdbjq.cn/Article/details/gfajvdbdv.sHtML

[U18] Py：预编译正则
来源：http://m.share.hesvh.cn/Article/details/gmyflwzxn.sHtML

pat = re.compile(r"\d+")
来源：http://baike.zdbjq.cn/Article/details/gpzaguilf.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.hesvh.cn/Article/details/gzvmpdgec.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.hesvh.cn/Article/details/gjnrbzcwn.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.hesvh.cn/Article/details/ggezlseet.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fehbvm.com/Article/details/glhmkegmi.sHtML


<!-- 参考信息 -->