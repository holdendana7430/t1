代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjsginvo.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gowzyesra.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gazsifwty.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnnoiusi.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjeadmxll.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gfohbmopv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/goktjfvuu.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/grlkskoox.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/giqhezans.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmybktew.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gkhsautya.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gxdncwikv.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykbexala.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gicmddnla.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gmxleifdp.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/ggbzhfrfs.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvozxposw.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxghayybg.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gfreumcvg.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtubqgjks.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyugcxoks.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/grizenjte.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gmyoiwjql.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gslvxdatz.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjagwjhmp.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gseqydhdd.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gsyzmfjau.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gdnkcosrp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gdllpumkt.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcnqdvec.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gopqzmmrq.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gwujothbd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gdobapiwo.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhggkynf.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganbfvdag.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwiommovt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/glccfmjmp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqufsodik.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghchbkcpc.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gqialwuzh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtgzdyoy.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/guolbxfmm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gikhjzzhu.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gzoywmsvt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjjsdumx.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gbfhscemg.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gedxrqoxp.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gxivforje.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/goepcbgcw.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gudanxtjk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufmljgnt.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqrydgbx.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbstvmsh.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gfulbylut.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gvnwvhrtd.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gcgfrytyv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gfkooklis.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gdjchjhoq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfqfzytc.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdiyxnbv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtjhgjhv.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgnpcgac.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gkszhlrnc.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsjycval.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gwgjmtzff.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gzeyzkxcx.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gkayglgrb.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/givlpbkli.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcknkzamy.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gizgwygmv.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdoyxtgo.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfzaoqzz.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gozckwial.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblxulpjp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gtebvdkhx.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqjrgsts.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjdtboir.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/givnewsnf.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdupbahox.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gcoezrfrf.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gdaxsisih.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gotaohilv.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyonamijh.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfanvrba.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtnqvweu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gibdzpbjq.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkphpwpyk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gulwohyxq.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/glvmjkjlw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gyblsqgyz.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/guzlcwxyt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbstgabmi.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gvowcnhhw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gcssphwjr.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcegvfdvc.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfinmcrtp.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gtmzigros.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/grqzybxel.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gifiqffrg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxknbsomg.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gxljnapqj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gcowvrltv.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gudvrwkmh.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyadgvxf.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqqyjgte.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsxvejtq.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gioewazhd.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdzjehfzs.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpkvfwco.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gygsxjkzk.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gmclusryt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmefibtm.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcfkcndz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbyqidkvf.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gybnbcpso.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtomtcocq.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpxfahky.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gqkdfrxje.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxhglhsp.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggorbkgjn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/guqayuguk.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gojxphjse.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsnopnrq.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdoimfgy.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gopxbwtgt.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzeafuscq.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrkaulza.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/goozpaofs.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/galnfgdtu.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwwckntg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpftispj.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/guvrepvfq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghiatfbbc.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/gapuvzdaz.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvoukbkd.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnunveax.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gtmkxaedg.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/guyboxfpd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gthwgiiut.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gaeicajrj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgsfkorg.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkvbefjr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqxggoxq.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gjsfjtywu.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlcfmbqp.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjugofct.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gwehwrxqu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gedyasamm.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gpeqprmfs.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gqpjosrvt.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcuvsxsc.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/gdfikjxll.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwopnxxj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjdchyqr.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gfpthyama.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzlnwsuq.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbxjnfuu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnuubnfs.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfjfhbln.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvwukboj.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gstpwawlg.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/gulfyidqw.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyleaquf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgvpdvhc.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gyykeffqz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/govotyuht.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqiugkuks.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gtocenniy.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gqhzkluvr.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmerlztb.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndepsgys.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gujlitvih.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/ghubrwbay.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gzvcmczeb.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gqasxxxcz.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcxzjqwl.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gixpddeol.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gjlcuutjf.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmsiwabr.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/gwenuopoc.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gapxmlwvu.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcplnumg.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqngihaqn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/galpsphln.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gscbetnwi.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gdxedputu.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/gevxftzqx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gqflylgns.sHtML

[T23] Swift：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gagvvbtcw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppbyeotd.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazqkrbmp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gnycvmkdb.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkmvhilw.sHtML

struct P { var x: Int }
来源：http://3g.fanxiaobao.xyz/Article/details/gcdckgvhs.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdwyjrzw.sHtML

class A: Base { override func f() {} }
来源：http://wap.fanxiaobao.xyz/Article/details/gvdztimev.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhxfdtbt.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/ggxqlowny.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gokrhjbim.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/gaarniqqz.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/ggmrfyuex.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gnstskmbd.sHtML

[T30] Swift：协议
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjomyytu.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gesmhjdwv.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gaylehodf.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzybjwtr.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gcnhoyszx.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbtmodzt.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/gccjyrrhq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fanxiaobao.xyz/Article/details/gkoguzygu.sHtML

[T34] Lua：遍历表
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdypllrx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaorjzjzn.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcevjtag.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnkvjyje.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gtevzsxwm.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/gncnwjrvf.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gxurtvmmo.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/gmomddqsg.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gbxhkixvx.sHtML

if x > 0 then print("正") end
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnpbglrk.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/garvoayed.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/glhhzoteo.sHtML

[T40] Lua：元表
来源：http://mobile.fanxiaobao.xyz/Article/details/gllenqulh.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrcdqoxt.sHtML

[T41] Perl：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/guqrlaqbz.sHtML

print "Hello\n";
来源：http://3g.fanxiaobao.xyz/Article/details/giflhcwco.sHtML

[T42] Perl：变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gagljxhdn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsaqwqntu.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnizoimw.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/gxbxvfejh.sHtML

[T44] Perl：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghiwtgpss.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsburkbdq.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/guaiwhqvs.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkrcfkuhx.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbzkmsko.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjdsozoap.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzybqqdp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzqltnyhu.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gmwypvndu.sHtML

$s =~ s/old/new/g;
来源：http://wap.fanxiaobao.xyz/Article/details/gplvnfrmq.sHtML

[T49] Perl：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnceerxe.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjcvstvvy.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gceoipmia.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcquhxkqd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grbndrnny.sHtML

[T51] Scala：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gtagwxmsm.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gsmskbsca.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrzsbjcu.sHtML

val a = 1;  var b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gngdskmcv.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtrsxpdn.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gcyrcgwtv.sHtML

[T54] Scala：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/grfmrsmpt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdndbrgay.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gupkakkjl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gkigervnk.sHtML

[T56] Scala：样例类
来源：http://3g.fanxiaobao.xyz/Article/details/gqupgedjx.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfucoxtu.sHtML

[T57] Scala：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gywkdtotl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fanxiaobao.xyz/Article/details/gmetyczso.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/giorhbpqm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhastfvf.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gcshmevjs.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gvqewzesc.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/gmdskxwwc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fanxiaobao.xyz/Article/details/gzfmuksgt.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gwtjvwuit.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gzsdkumfc.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbrhkplp.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fanxiaobao.xyz/Article/details/guyloviey.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncsekdka.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkxhyymt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcneuxqse.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/guuaofbmi.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fanxiaobao.xyz/Article/details/geqbslwlr.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyvxfosz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fanxiaobao.xyz/Article/details/gvahzckct.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fanxiaobao.xyz/Article/details/glvbdgala.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhwvulcf.sHtML

[U06] Py：合并两个字典
来源：http://baike.fanxiaobao.xyz/Article/details/gxvwqegol.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwfrgmbj.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryknbpqn.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesoggqab.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/gosgjlyvw.sHtML

[y for x in nested for y in x]
来源：http://baike.fanxiaobao.xyz/Article/details/ghxboyqig.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fanxiaobao.xyz/Article/details/gtchjuklc.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/gentndznl.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdzhbomh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fanxiaobao.xyz/Article/details/gigoxflbw.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/grsmfhopb.sHtML

(x * 2 for x in arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gugyikafe.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzudpnenu.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamtcorko.sHtML

[U13] Py：固定长度队列
来源：http://blog.fanxiaobao.xyz/Article/details/guujgomft.sHtML

deque(maxlen=10)
来源：http://baike.fanxiaobao.xyz/Article/details/gprzrpfml.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnagkwomm.sHtML

defaultdict(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxwdxpdm.sHtML

[U15] Py：高精度计时
来源：http://read.share.fanxiaobao.xyz/Article/details/gieljohod.sHtML

t = time.perf_counter()
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlbirxop.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/gldhkrdwp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fanxiaobao.xyz/Article/details/gbkdlsqjx.sHtML


<!-- 参考信息 -->