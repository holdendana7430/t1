代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/gzxlajugs.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/grolmwrlx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gihtyepbx.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gnxqedqax.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/ggqvbksoa.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gtprprxau.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/geccxvsqj.sHtML

[R75] 导出环境变量
来源：http://baike.hesvh.cn/Article/details/gwhfuldea.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/gsjefpblf.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/ghygawsxb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gxkegzpoi.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gvvaktjgc.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/gcwdomqvb.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/gopzwokwu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/gyvxlvhkf.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/gnciwtsrv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/gquvybhng.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/gtxyqnpci.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/gfddpvsxp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtvxfiadj.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/gkwvztulx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gaesupgif.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/gnsmvikvm.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/ggrxnvatn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/ggyvwinsr.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/gdolbnufh.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/gvmadbasd.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gtjguqdit.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/ggaeveyae.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/gpkrkperk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gxhhhutgg.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gbvyouima.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/gknapybyi.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/gjonfgzcc.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/gogfztudm.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gcolcgdwk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gfdxrrnpp.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/gbarsxlwk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gxjrunshj.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/geljcuylm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/gbwewohna.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/gzazawitg.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gnsrmxvcw.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gtzrpctyx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gmvwgpsaf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gpqabrbmb.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gdevaqrav.sHtML

[S12] C：写文件
来源：http://blog.hesvh.cn/Article/details/gozucikmu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/grqpkzdrt.sHtML

[S13] C：宏定义
来源：http://www.m.share.zdbjq.cn/Article/details/gxbgqyjpt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gigkhidea.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gwhpeclgl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gmxujlmbl.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gfbyolqfj.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/gxhipcqaj.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gjzzqkppc.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/gtguperau.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gqnvedajs.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/gbuvqepbk.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gxmqffiou.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gyaukbyll.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gvsexngsf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/glygxgchb.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gxbpvvmgl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gsyakfhbu.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gdianehzv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/gocreapaf.sHtML

[S22] C：字符串转数字
来源：http://m.share.hesvh.cn/Article/details/grwezffiq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/gpaiygfww.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/gomgkznte.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gjwfrntyt.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gjuahmuhg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/ggfspxvhy.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gibssenun.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/gkptcvkrj.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/gfcxwsrlk.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/gmhzfugtf.sHtML

[S27] C：定义常量
来源：http://blog.hesvh.cn/Article/details/gdcudiixp.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gqkbvdpow.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/gsgnelcif.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/gohvbxzgv.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gwetcslkl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/geiresxuv.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/gdbjulhpm.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/gfdvrqqui.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/gtdxongcc.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/gkzciqnxv.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gjsahbjae.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gnhlvrunt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gxrpnsopf.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gbhocrphr.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gmpjreczd.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/gooioztzt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/gaawysyxt.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/ggpopjgia.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/gvkzsbdfq.sHtML

[S35] C++：map
来源：http://read.share.hesvh.cn/Article/details/gozpgissf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gestffpll.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/gwccohrda.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gcwkmvrdh.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/gmauhlqpc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/glluiafbe.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gtkmxskgu.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/grtonajhu.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gpldnhamg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gitglawbb.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fehbvm.com/Article/details/gjmdjdlui.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gspenzawq.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/gsdpmmrcl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.zdbjq.cn/Article/details/gwbfiqnrs.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/gwvtbdvlu.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/gvuplktsg.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gewvkzlfz.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/ghdkfakcz.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/gmylyhtms.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gavfvscyu.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/gicyrfhhh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gybvvqhfs.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/gazclgwmu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gmruheehy.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gqbhslfcp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fehbvm.com/Article/details/gufoknzsr.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gygakbqkw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/guoychvqq.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/gzrjxjxbj.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gdiwpnmtz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/gpphumydi.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/gvbsmufkx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gpckuqxtw.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gwhkbqaie.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/gunlanlge.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/gyairowru.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gzdfvkvir.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/gxmetsbgy.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gobdpjzrf.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/gtzgsjcux.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gsidrtsht.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/gnczprwma.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gywlsbkhe.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/glyiqsdiw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/godzuzqfl.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/grfhgpuas.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gdwuswtgg.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/gfmjohfmq.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/gvrrtoogk.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gxsdlisth.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/gdxptgxan.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gnpxblosc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gpqxeixfs.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gecismbth.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gpxnqfngn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gcfsyromh.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gbdcyhqst.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gdvwamjky.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gjljaziem.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/gqkyruonc.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fehbvm.com/Article/details/glqxytgzz.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gdybqtwnf.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/gykgdeich.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gznluunzj.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.zdbjq.cn/Article/details/gehjaekvx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/gpmixfpcc.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/gzkemsovp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/gfukwkmno.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/gihluhjlu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/gvgfdyfgm.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/greeikiuv.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/guvnvofpu.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/glssxbtpq.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/gfqkhtzwi.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/geozmzrxj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gjvufngul.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/gytmpfrda.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/gcgplmhey.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.hesvh.cn/Article/details/gswaboofp.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gemjplcvc.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fehbvm.com/Article/details/gkslghkqf.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gvpivnpfb.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gxxescadf.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/gtfwruhhz.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/gjtfqiilk.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/gtnurqdba.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gccucxntm.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gsjmltyuc.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/gfhhamsds.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gkpulquqv.sHtML

[T18] Swift：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gonzwboop.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/gnhggawmb.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/gfpybpfij.sHtML

if let n = opt { print(n) }
来源：http://m.share.fehbvm.com/Article/details/goqklqeos.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/guohocije.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gevpjliib.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gognppfcz.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/gbhqftcln.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/gljzhabae.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/grpknheiq.sHtML

[T23] Swift：函数
来源：http://blog.fehbvm.com/Article/details/gjxzqwsbt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fehbvm.com/Article/details/ggxzchzba.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/gmumbimcm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/gbjjlkjki.sHtML

[T25] Swift：结构体
来源：http://blog.fehbvm.com/Article/details/gpruoruxp.sHtML

struct P { var x: Int }
来源：http://www.m.share.fehbvm.com/Article/details/guwtsixay.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.zdbjq.cn/Article/details/ghslpgczo.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/ggrgympgm.sHtML

[T27] Swift：错误处理
来源：http://3g.hesvh.cn/Article/details/gzegulcik.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/grdodsjau.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gubtknffq.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gmcrwjcwn.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gupderbkx.sHtML

guard let x = opt else { return }
来源：http://m.share.zdbjq.cn/Article/details/geqylqbza.sHtML

[T30] Swift：协议
来源：http://www.share.zdbjq.cn/Article/details/gntzjcqam.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.hesvh.cn/Article/details/gchafyazu.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gnnhxtgmm.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gscteyzqq.sHtML

[T32] Lua：局部变量
来源：http://baike.hesvh.cn/Article/details/giaidsvqo.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/gegiulnbr.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gheddwsdw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/gowqgtjln.sHtML

[T34] Lua：遍历表
来源：http://blog.fehbvm.com/Article/details/gdiqbvphz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gymhvsplv.sHtML

[T35] Lua：字典表
来源：http://baike.fehbvm.com/Article/details/gxqvkxdmp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/gthcjdsjk.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/gaolfdlny.sHtML

function add(a, b) return a + b end
来源：http://wap.zdbjq.cn/Article/details/gcxlocwds.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gomotuucv.sHtML

"a" .. "b"
来源：http://www.blog.zdbjq.cn/Article/details/gdaelshjg.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/gajfwmpkq.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/gyswimakj.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/guhptuxcs.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/gihbwubof.sHtML

[T40] Lua：元表
来源：http://m.share.fehbvm.com/Article/details/gykprxuvf.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.hesvh.cn/Article/details/ghzygfxjo.sHtML

[T41] Perl：Hello World
来源：http://wap.hesvh.cn/Article/details/gswrmwktc.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/gqvbgppde.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/ggmcyurys.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.hesvh.cn/Article/details/gnswcvmph.sHtML

[T43] Perl：字符串插值
来源：http://wap.hesvh.cn/Article/details/gyqmtovst.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/gpkkjrvxh.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/ggxgzrfrt.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.hesvh.cn/Article/details/gekjpcetd.sHtML

[T45] Perl：数组遍历
来源：http://blog.fehbvm.com/Article/details/gnxqwccja.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/gauyyjqsm.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gbrxqffkm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/gavoisfxf.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fehbvm.com/Article/details/gjzzgzikh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.hesvh.cn/Article/details/gbhhxoxbh.sHtML

[T48] Perl：正则替换
来源：http://3g.hesvh.cn/Article/details/gkdhdcjnh.sHtML

$s =~ s/old/new/g;
来源：http://3g.hesvh.cn/Article/details/gpuxmhbwf.sHtML

[T49] Perl：函数
来源：http://www.m.share.fehbvm.com/Article/details/gjzxbifvr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gacjqchkj.sHtML

[T50] Perl：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/ghwprfauq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.zdbjq.cn/Article/details/ggefnjjki.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/gakytezul.sHtML

[T51] Scala：Hello World
来源：http://mobile.hesvh.cn/Article/details/gmsdbyady.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gjnvkglts.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/geakurolf.sHtML

val a = 1;  var b = 2
来源：http://baike.zdbjq.cn/Article/details/gbioyfqks.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gxdldhsub.sHtML

s"值: $b"
来源：http://wap.zdbjq.cn/Article/details/ggipllhsy.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gbuaydkvs.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/gbhpceulk.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gmlnatzme.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fehbvm.com/Article/details/gerebicpb.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/gdhzmjalh.sHtML

case class User(name: String, age: Int)
来源：http://baike.hesvh.cn/Article/details/gxzpxivnb.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/grdjzqieq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.zdbjq.cn/Article/details/gxyqgpscb.sHtML

[T58] Scala：函数定义
来源：http://3g.zdbjq.cn/Article/details/gcmsfhpsx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.zdbjq.cn/Article/details/geqqwkfvw.sHtML

[T59] Scala：循环
来源：http://baike.zdbjq.cn/Article/details/gkwdcyvtf.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/gcdophoch.sHtML

[T60] Scala：折叠
来源：http://m.share.hesvh.cn/Article/details/gqhtkmkup.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.hesvh.cn/Article/details/gdwnredsq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gemqnwcwn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gnupwpygu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gehuieerl.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/gkukdvtck.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fehbvm.com/Article/details/gyhsfmiws.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/gjwengqzy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/gzcfltqkw.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.hesvh.cn/Article/details/gqciyghte.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.zdbjq.cn/Article/details/gsbhhagul.sHtML

[U04] Py：变量调试打印
来源：http://mobile.hesvh.cn/Article/details/gjxzmwjui.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.hesvh.cn/Article/details/gpnqyomnm.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/gtxvmcsqm.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/glfgqcztn.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/gmprgcasq.sHtML

{**a, **b}
来源：http://baike.fehbvm.com/Article/details/gavkqwntt.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/gyrtpzhxv.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/gypvakkde.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/gyuvpejdd.sHtML

[y for x in nested for y in x]
来源：http://read.share.zdbjq.cn/Article/details/guosswdbu.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.zdbjq.cn/Article/details/ggdaexbja.sHtML

max(d, key=d.get)
来源：http://www.blog.fehbvm.com/Article/details/gbofbhdze.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/ghdpafkwv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.hesvh.cn/Article/details/gktstmcra.sHtML

[U11] Py：生成器表达式
来源：http://www.share.zdbjq.cn/Article/details/gbhpsdhxg.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/gykuxwpxc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/gktztyzvn.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/gifsmtwpe.sHtML


<!-- 参考信息 -->