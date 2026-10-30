代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzihobaub.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gyesranph.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gluhprryf.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/ggiqooodg.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gddcbefff.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gwitnlkng.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gydbeivfr.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gcavnbzxk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezpdxtwl.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gegwhqymw.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvnjobmu.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/glohaudbb.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gmqmsyqpk.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gnfzphjpb.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gctpaztju.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gfdzaftsd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gripzbxkp.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcegdeahg.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gctlasvaj.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/glenlmurn.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpuvjvry.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gowgpodut.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gpftxlutd.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnehftqoa.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcmexeka.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gplgiyzej.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gkfjufjre.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gccugzdnf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gtxgsstal.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gsemjprdn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzeiopfe.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/glaztndyi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gqjtparfh.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/geshvpvea.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfbeeemk.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjipplel.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/ghrjazwwn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwqmecab.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/goqxjvuqz.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gufoaiieh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnseouscc.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcvbijzc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gvqpltapq.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcfrbltp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhitocll.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gjepmpxfg.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gdtxenfov.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gmfavrudv.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gdsdwvxaf.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpxfcbvt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbjcwvpn.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gkkcutrfj.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfeabktr.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gyslsztsp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gjscaaotp.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtfhymwj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmljakeyw.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gcvfmdhqc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gqubiyphp.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gtabjinvb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilsieysp.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmpebzdo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gpnuehtgf.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkgfnefc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqcpxxlt.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwclokig.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gruukvyfq.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszgsqpkk.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhjioeqi.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gbobnrwpf.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlqhqhgz.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdvmfjvt.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/glihszhxc.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqghvypx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gehhcvxox.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gpczjcrjw.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomdjtlol.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gtnkpyivv.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gccdvrfty.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gmggmedxb.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/ghahjyqzm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokbszpga.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gwuwaphsj.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxbzhmpl.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuqcqcdv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/golkgyqei.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gjxfxawja.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gajlyygun.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gtvyvsoer.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gezprziuf.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtoipiro.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/glygiwyhu.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/guvdkwebp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gutnxfivf.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/grkllvvfo.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/glnvozkhd.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gbexambku.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsepggtpb.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gophbevnb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gyzawhizc.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gnzzhswxm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgjqdvir.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gurmrieot.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gvociouuy.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/ggsdmtyoq.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/grpgeydkn.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gleeqysns.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gakmvickw.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkqjsffu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwuqsmvb.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gpbthkosp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/govxgatcz.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnclfzoq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmvuhdir.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcxgnxrv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjstwfeb.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvutvqbzd.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/getkvrecj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgtwuhfv.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcdmpqam.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvnitvuq.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gyhmpegxy.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaohbxona.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmtgbhxw.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrygxuuq.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/grkxsovjm.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvckqmrhv.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/ghylfztef.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvghobtas.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gujbsyjgx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjidzwmma.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gwdwxizvt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/grnfgwwjd.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/gecuknhwo.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gtnrajrcr.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjkltulw.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gtmqrxblq.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gwpvhdakt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gsuxiyktn.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gaorevhwb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjzazeaa.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ggylupsza.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrvgnvpa.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwvaxxsq.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/ghrrgfguj.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gfwsooqug.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/ggbyhlpjn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gtgmkiyvt.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/guyikqjjz.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gpitgesgv.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gknmoejep.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwlwzejn.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganqshnxx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzyhxfqt.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gaydgwjjm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gwuwvhrca.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnbzymkx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gdfsicdjw.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gjqqdjmiq.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcayfzesi.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzcznvdd.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghztnylce.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/ggjljjjtx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gwmzbstox.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gijihywlm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmogcvbt.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsinaool.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrsclurv.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmvcfivs.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gwiffrjvr.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gdqlejvdf.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gvbkcxjsi.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/gjinsfqwx.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/grgvxmwtz.sHtML

[T16] Swift：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/glelkvosw.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/ginihcoab.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gpozhqkyl.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/ghbsqkpbs.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrwjawei.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/giudxbeie.sHtML

[T19] Swift：可选绑定
来源：http://baike.fanxiaobao.xyz/Article/details/ghcliopcx.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/glydnjwuy.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gkuivafuj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxwtwond.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/giahyezsi.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpnazhnd.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzxdifjp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdwpijmk.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/giulzkjil.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gozqkngsa.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gejfzujmi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzwwcuyp.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfkcxjko.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpzsheuf.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzdvgoyx.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/glotrzcxt.sHtML

[T27] Swift：错误处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gxljqkkzi.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/gsmtkvzfq.sHtML

[T28] Swift：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxffxsea.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/gufxtsrlh.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gyytwssgh.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpgqjhgd.sHtML

[T30] Swift：协议
来源：http://wap.fanxiaobao.xyz/Article/details/gvycusocd.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduttjcxp.sHtML

[T31] Lua：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmjplxei.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/geljfkwvf.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmwlpaig.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gucvajdfh.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/gdiannhow.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/galpdhrvp.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgtjufdz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwbplxpo.sHtML

[T35] Lua：字典表
来源：http://www.share.fanxiaobao.xyz/Article/details/ggucodmvg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/grgdaxzbs.sHtML

[T36] Lua：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabgpuhhk.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskpmozas.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gdowdkwgp.sHtML

"a" .. "b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqyygzkq.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gjrtumlfb.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyvtftji.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvyrbmmx.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gggzdtwzx.sHtML

[T40] Lua：元表
来源：http://www.share.fanxiaobao.xyz/Article/details/godxivdiw.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlsqrdgk.sHtML

[T41] Perl：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gllhhatya.sHtML

print "Hello\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gxmldhvct.sHtML

[T42] Perl：变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gotyhgrny.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gnusvgecv.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwpigjwo.sHtML

"值: $a"
来源：http://mobile.fanxiaobao.xyz/Article/details/gohhxulby.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwocpjbk.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gterthqoc.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gyogssqzb.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpetotchh.sHtML

[T46] Perl：哈希操作
来源：http://wap.fanxiaobao.xyz/Article/details/gxffqvldn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfawrphk.sHtML

[T47] Perl：正则捕获
来源：http://baike.fanxiaobao.xyz/Article/details/gjlmgqmbq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwshufsr.sHtML

[T48] Perl：正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvgchvsi.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspbeacxk.sHtML

[T49] Perl：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gtmdgeisc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxeqgxeii.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkctapjan.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fanxiaobao.xyz/Article/details/gejpvexdt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/guxlvylmu.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtagqdrf.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/ggvukjtaa.sHtML

[T52] Scala：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gsebzmffe.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/ghhvvltlo.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbbvdkke.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gduyewwsf.sHtML

[T54] Scala：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gwlazmldi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsfhibkp.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gtccszfgo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fanxiaobao.xyz/Article/details/glojksxgp.sHtML

[T56] Scala：样例类
来源：http://wap.fanxiaobao.xyz/Article/details/ghujklryk.sHtML

case class User(name: String, age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gnsrmykjy.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdkbtbar.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgpatcbp.sHtML

[T58] Scala：函数定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gmugrujsy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuzyybfa.sHtML

[T59] Scala：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gyyxbklyo.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gddicibls.sHtML

[T60] Scala：折叠
来源：http://baike.fanxiaobao.xyz/Article/details/gagbuuioy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyleputtn.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ggocvispg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxprrkvsv.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gaipuucno.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsbvivct.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fanxiaobao.xyz/Article/details/golzdbnli.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvpftcpz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fanxiaobao.xyz/Article/details/girfuzocq.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrzzbgqk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcnksocr.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fanxiaobao.xyz/Article/details/giscykand.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/ggkphcejl.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fanxiaobao.xyz/Article/details/gcshlyyro.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtahtiemu.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gurnnucou.sHtML

{**a, **b}
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxeqdqcb.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fanxiaobao.xyz/Article/details/glovqftyb.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlxcsyaa.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxyssuun.sHtML

[y for x in nested for y in x]
来源：http://wap.fanxiaobao.xyz/Article/details/gclzujnlb.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fanxiaobao.xyz/Article/details/gquaygabn.sHtML

max(d, key=d.get)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvfxloub.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/goryypwbw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhkpquwi.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmbfswnb.sHtML

(x * 2 for x in arr)
来源：http://baike.fanxiaobao.xyz/Article/details/ggnpjqkgg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzkdanfe.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/giwfoqsvj.sHtML

[U13] Py：固定长度队列
来源：http://blog.fanxiaobao.xyz/Article/details/gqaucvzze.sHtML

deque(maxlen=10)
来源：http://wap.fanxiaobao.xyz/Article/details/gluqknxqe.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fanxiaobao.xyz/Article/details/gkqwmwser.sHtML

defaultdict(list)
来源：http://baike.fanxiaobao.xyz/Article/details/gxpvwnifi.sHtML

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/gtrlppkzi.sHtML

t = time.perf_counter()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbogombfn.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzisvbda.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fanxiaobao.xyz/Article/details/glivdtzot.sHtML


<!-- 参考信息 -->