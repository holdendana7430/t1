代发 wailian999

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/gnskogsfk.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gwpvkqaou.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gxtumypey.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/globmdrxy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/gamnegszx.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/gbsfwcgzq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/ghcvtvwsp.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gyxmxtnlo.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/grgjlrwir.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gdykdkjtv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/gmxfftvqx.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/gqxesiqzh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gounlothj.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/gjqifkqum.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/ghakdibmn.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcbacmtfc.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gwglopoio.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmqffmtlv.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/gxexjibhr.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/gnanuppvo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/gfvwqfepo.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/gldqyacjq.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fehbvm.com/Article/details/glzhtipch.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/gauzckbyb.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gictzgvhf.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gxvhbvois.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/gfllxbqlg.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/gaoctveag.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gpacdnkhl.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/gcrfolcco.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/grhxbncoo.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gldwayjrl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/guwhqbonw.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/ggyqxkyml.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/ghlzjkwoe.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gjjhhnoed.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gffanzrrm.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gnonyczxk.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/gxviryfji.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gggquwztl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gerloosdy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/giemlxvps.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gigqroxix.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/ghmybhtzd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gxzeomjqv.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/gmecopfmk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/gcjuszdbe.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/ggbnhrdfm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gsbombzlz.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/glbkherfi.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/gsvicxukt.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gehjmjltd.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/gwiaafphv.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/ggvgnvwpw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gdsahldfm.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gymxtrefa.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/goiuavswe.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gvoorhuyq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gfgemttmw.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/goaptyrcm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gixewglvl.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/gbkbuowrx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/gmyjzdlwi.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/gnipfqlzy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/gsyzrcpwe.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/gtauroarg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gnvmwwzio.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/glvjrszka.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/gumgjqufi.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/geukochyb.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/gctjqobzk.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/gdwjnxypy.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gmwqhvtzw.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gzsfgtrfk.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gwlejccfn.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gpkadspjr.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/gjjlhelzj.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gjsmmpbri.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gsgeabiyj.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gzbrbcdhh.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/grtoxmrcb.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gjwwuuzaj.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/gazeggqyx.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/grwtogbub.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gtyjfdhdg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/giajvhbsn.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gpujdluop.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gqywxkelw.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gykqbstqx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/gmunonaqg.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/gmglrpmrm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/ggrgpvqjf.sHtML

[S35] C++：map
来源：http://read.share.hesvh.cn/Article/details/grazdbgjx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gjjfpoqyv.sHtML

[S36] C++：unordered_map
来源：http://wap.fehbvm.com/Article/details/gxyauxwgf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gouqsxubg.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/garhvyxwj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/gsilwvfxy.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gawcegiwz.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gklpxqjyi.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/guaoifrtd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gjwyoulag.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/giapolplt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gdjvswfhb.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gmsbqzmyh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gvqngdvks.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/gvggmynep.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gdriaaorn.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/gccehywrr.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/grjwngfap.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gbelkyxjq.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/gcoxmtxnu.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gzgmpluxy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/gnjlswlwt.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gxwgsqtgy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/ghykpjqxk.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/ggmogcwff.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gohdctpyi.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gcbpzwhsq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fehbvm.com/Article/details/gmxhssnmk.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gminayjot.sHtML

[S49] C++：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gewwzotnv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gsassibki.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/gygvhyvlb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gwomaklqz.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/grfpjyrox.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/ghcvjgjsu.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/gdpdudjeb.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/goicixaoy.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/gimmatvtm.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/gxtafyfkh.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gkyxdjtod.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gxvquvsmk.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/giagtjfld.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gjitdwkpw.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gbquyxmwy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/gwrqvnvki.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/grvnkoouo.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gmfurwtsk.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gjifpuurd.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.hesvh.cn/Article/details/gkuqsowlm.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gxqauxrsg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/gbqlhjyzs.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gycvtctwp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/gvlphguem.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtcdxcbst.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gbpgiumog.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbvixnuuj.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/gdfrqojpm.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gczmdnqii.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/grieshhbx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gvwqppdwq.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/galpykczp.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/gkgkonuui.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/glmqzaumt.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/gzhhggnkd.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gsyozpuwx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/giliubsrr.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/gtcxixzqs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/gfbfnbggh.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gxlaojzzj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/glhfsjokm.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/gactuvelx.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gjgeigwba.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gbmqfcrff.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gaupsbect.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gcjrzldrx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/gcloppgvw.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/gyojevirc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fehbvm.com/Article/details/gfvfqqwld.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/goxggxyhh.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gwdoatltw.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/gtalfvdzv.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gzlgkgzpo.sHtML

[T14] Kotlin：循环
来源：http://wap.hesvh.cn/Article/details/gyhovykej.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gnlkxsfjr.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gvutcktwa.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gdeezbhpv.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gwjjlcfuk.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/ghjcecfbh.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/glxnjekmq.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/gktfqwlst.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gnalreumk.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/gsauxpulc.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gxwzmeusn.sHtML

if let n = opt { print(n) }
来源：http://3g.fehbvm.com/Article/details/gzllxkpnj.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/glfgyfdgb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gwjnyxrlu.sHtML

[T21] Swift：遍历
来源：http://3g.fehbvm.com/Article/details/gkoftjpza.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gvveutaqt.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/gmkvegofe.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.zdbjq.cn/Article/details/gdbmustxr.sHtML

[T23] Swift：函数
来源：http://www.blog.hesvh.cn/Article/details/gwzquhrcg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.zdbjq.cn/Article/details/gwwoialxt.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/gdozgpblf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/gscmpkpxh.sHtML

[T25] Swift：结构体
来源：http://3g.zdbjq.cn/Article/details/gcvpygtls.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/glnksfavq.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/gafskboni.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gdwbrgffy.sHtML

[T27] Swift：错误处理
来源：http://www.blog.zdbjq.cn/Article/details/grwlennlk.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.zdbjq.cn/Article/details/gemobvnzv.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/gfcwhrblq.sHtML

enum Color { case red, green }
来源：http://blog.hesvh.cn/Article/details/ggmjekhdm.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.zdbjq.cn/Article/details/gfmxqedwv.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/gkcmfhwzj.sHtML

[T30] Swift：协议
来源：http://read.share.fehbvm.com/Article/details/gcldvdhvz.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fehbvm.com/Article/details/gitpsdydt.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gbuifcoba.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gjktztzuu.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gadvwvhlr.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/gpcrruohp.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fehbvm.com/Article/details/gmlmggwmu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.hesvh.cn/Article/details/gomuacfqy.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/gdrxbtmpq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/gkxeeeoax.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/glyqgxild.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/gyxppxjgx.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/glfqsyirx.sHtML

function add(a, b) return a + b end
来源：http://m.share.zdbjq.cn/Article/details/glhqjglkt.sHtML

[T37] Lua：字符串拼接
来源：http://wap.hesvh.cn/Article/details/ggaudghik.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/gfdyjinlh.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/gqbltwkea.sHtML

if x > 0 then print("正") end
来源：http://mobile.fehbvm.com/Article/details/gusoheqjd.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/gcajnlwsp.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/gyrcyfdvw.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/gscpqphbn.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fehbvm.com/Article/details/gwccvwsfl.sHtML

[T41] Perl：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gikgcvjqz.sHtML

print "Hello\n";
来源：http://mobile.hesvh.cn/Article/details/gncrluuwx.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/guqlbddwx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/gmsbfialg.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gwvrcovmz.sHtML

"值: $a"
来源：http://www.m.share.fehbvm.com/Article/details/glkaowpqp.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/gumraitfw.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gystbslaw.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/gonsoymvn.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.hesvh.cn/Article/details/gljmjvzwa.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/gnyeyhgfa.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/gtdgjyvqa.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fehbvm.com/Article/details/gzxeeatar.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/gnmkfaful.sHtML

[T48] Perl：正则替换
来源：http://read.share.fehbvm.com/Article/details/grbspzamq.sHtML

$s =~ s/old/new/g;
来源：http://blog.fehbvm.com/Article/details/gfaxylzkv.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/gdaoiyndj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gkwspeshl.sHtML

[T50] Perl：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gfzuzempm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.hesvh.cn/Article/details/gpaqjthgr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/gsnoiehjr.sHtML

[T51] Scala：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gajaszbft.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/glrzlhgwv.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/glmtucygw.sHtML

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/gfxpvxuiz.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/gcxskqtka.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/gcasgzkeu.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gpfztsqze.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/gthpevwwa.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gpbnnopok.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/gvjcemggl.sHtML

[T56] Scala：样例类
来源：http://blog.zdbjq.cn/Article/details/gnuuelkwe.sHtML

case class User(name: String, age: Int)
来源：http://wap.zdbjq.cn/Article/details/gxmnlsmko.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gckpuoklg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fehbvm.com/Article/details/gqhglcjwo.sHtML

[T58] Scala：函数定义
来源：http://mobile.fehbvm.com/Article/details/glbvfhxtx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.zdbjq.cn/Article/details/gzurlfmsq.sHtML

[T59] Scala：循环
来源：http://blog.fehbvm.com/Article/details/gjiwajliy.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gcixdjfmr.sHtML

[T60] Scala：折叠
来源：http://baike.zdbjq.cn/Article/details/gpnzassfh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.hesvh.cn/Article/details/gwlikftca.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfylynqva.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gwewgreht.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbrsolpfz.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fehbvm.com/Article/details/ggsrdqmiz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.hesvh.cn/Article/details/gllpkhfok.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fehbvm.com/Article/details/gxwkgoosr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/gmoumakhq.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.zdbjq.cn/Article/details/gviundkif.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/gjabsmlev.sHtML

[U04] Py：变量调试打印
来源：http://m.share.hesvh.cn/Article/details/ggslgjesd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.hesvh.cn/Article/details/gphsntlbz.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/ggwztbgfl.sHtML

list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/glusedopv.sHtML

[U06] Py：合并两个字典
来源：http://3g.zdbjq.cn/Article/details/gdnvlhrsi.sHtML

{**a, **b}
来源：http://3g.fehbvm.com/Article/details/gzuebmexp.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fehbvm.com/Article/details/gyofvikem.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/gseciumgz.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/gseylcvqj.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/gtcdtfsjk.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/grdtcwrpm.sHtML

max(d, key=d.get)
来源：http://blog.zdbjq.cn/Article/details/gnjjmwkqd.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.zdbjq.cn/Article/details/gakslgnul.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/giazrovdh.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.zdbjq.cn/Article/details/gglzzznlu.sHtML

(x * 2 for x in arr)
来源：http://www.share.zdbjq.cn/Article/details/gcxqwkftf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.zdbjq.cn/Article/details/gqgxsmhmc.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fehbvm.com/Article/details/gsjkmzkdn.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.zdbjq.cn/Article/details/gkpggaitp.sHtML

deque(maxlen=10)
来源：http://wap.zdbjq.cn/Article/details/gcuudidvk.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/gjctjaxrv.sHtML

defaultdict(list)
来源：http://3g.fehbvm.com/Article/details/grzpvytlp.sHtML


<!-- 参考信息 -->