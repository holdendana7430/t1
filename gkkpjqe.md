代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdyrqjnb.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrrkhibz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gdfpxlubh.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/ggggaohjt.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/grqketfta.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgbyjebo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmycbxpa.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdzvboaa.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqmnddwc.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gusofzumi.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gztzrbeyo.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/glffxuxku.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrgsawqp.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbybblww.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gpogtqjmc.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gelbczxcy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnvcsksl.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/grycjtgbe.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwlteqkn.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gsvvwlvjc.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gmogtvrll.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gxebczimb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjzhhozi.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxogsrdh.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gshjofnxh.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbeytrddb.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/geqsooprc.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/grgqegxma.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gmicqpcsm.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gxrrzufrb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gadxqyspx.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gydhoatwq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gtajcvrly.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gaveifrnz.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvrdirmi.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gjlhywntk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrwesztb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkfmgczn.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/govgdhevf.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmvilkbr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwrvqyun.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqefqyqm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzsvemeu.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gynnrbqzd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gonstjgsd.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gwayzjptc.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgsbhjrg.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzxilqee.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmiqqomht.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkuwrddjq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbumeysx.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwlatzmf.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghcwuqsv.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gplqrfihp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gnsikyfka.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gonzkwnih.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gryavtktq.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gpwkeknab.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gskdjrvyk.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhsuiepv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gihlkueje.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gklvpfrac.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzvqvvoq.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gafcryofi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gyyhdzewx.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gboeruyvr.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtikzerwm.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpludxkx.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gzdvredhj.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gwtejhchk.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gramxilao.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosifefjf.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfttquok.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gbnnpygad.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/ggscfsojb.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgzxsgqr.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gdaoqzynw.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gekteonip.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxzrtixs.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsqmtwna.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gzydcaouc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwpploto.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govcekjfs.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsadfkwk.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gtttxcbfj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gpekthhft.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzjchlsj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxstarpm.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gdgetccwu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gydaqjwoc.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvxgriqo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gaddimhzi.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gestiumxd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/ggtcsdoln.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gqkokwykr.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gonzjtjdl.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gltnkfwtz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gagpfmjop.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstlqtfwc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gewhynlzu.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gqogbudim.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gcikhjlgj.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gmgimpbsh.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gmkxdmfmx.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjkdxarp.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpplgkboa.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gsnwegtrp.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfjmkzem.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gpdxgwyky.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gdvjxqmks.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gvfemofou.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjyhyjhw.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbogmgdf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjuowafna.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gqqcvqtlt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhbxlcnw.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/goqycvdsi.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqljdsyf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gzovefpbr.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/giaomvgaa.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gwvlvgumo.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/goruzsamk.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzqxvxxm.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjtjjalc.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtozxwqwd.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/guoyfbpjt.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpqwcfeb.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gyjhsizuj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwyezjpi.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gxdplejmg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gijysumho.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqixjonu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/glyrdyqyp.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdeexxyt.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gklpdqvqd.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/ggzctalfk.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gizppxavp.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/ghmxnbhee.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxuqkpwm.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtmigvcn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gxfcqzlfb.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gazmlrqzp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/ggvbgwnsp.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxeyrkmdc.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gghedkolp.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpymmlgai.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gphfkbmcj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gemeggsuj.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/ggvxzgrnv.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gfztrwkuq.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlqrzhpv.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/gbancnnkz.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gxksrfrjh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/grqkglknv.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwmqslpq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkkwfziy.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gpcvmhbik.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/goagqdpty.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gstzsodbs.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdzmafqx.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/gkjpgitgj.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwupgadny.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyenkszeh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/gswxsnyat.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzydroygq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzeeziylf.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gropdpcsp.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimfghnvr.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdctwaas.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcwppogb.sHtML

[T14] Kotlin：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqbnrbiv.sHtML

for (i in 1..10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gllkdtaek.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjkldzds.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtifswavp.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghiuphgth.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gghrugygp.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gduqgdefg.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gonnicist.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gdvdijptq.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/gzqjaumyr.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwtyfaav.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gikzraxpy.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gppuiqjck.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gebxqposq.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gipvthivz.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrfhxkrd.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmngfaqt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gauxzzqox.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghohkvkfi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwzzknli.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmyglzuc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpbzisrs.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/gyutuizao.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcirbjbg.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvblshkz.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjqoxvaz.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gkzmekhrj.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqicuxusr.sHtML

[T28] Swift：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gonyyegay.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnphmrvyk.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gmopcrtpc.sHtML

guard let x = opt else { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gpdkijhio.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/ghikfyzqg.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gbouifrpe.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gdidsvidx.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlzijtqd.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gohapoefg.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvdjgjtv.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffitftit.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhfgkwfz.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/gqeouswre.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrzgmjxa.sHtML

[T35] Lua：字典表
来源：http://3g.fanxiaobao.xyz/Article/details/grywbxaef.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqychuohc.sHtML

[T36] Lua：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/guqatxnlc.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/ggjwywkob.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gmrotyhdy.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/glncnljfm.sHtML

[T38] Lua：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtzhiebr.sHtML

if x > 0 then print("正") end
来源：http://www.share.fanxiaobao.xyz/Article/details/goycxwslj.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/guiltvmyr.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtgnxpqn.sHtML

[T40] Lua：元表
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnaizhfl.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/gledjfbpn.sHtML

[T41] Perl：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzwpwkjg.sHtML

print "Hello\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggigexhsu.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkexzinvg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fanxiaobao.xyz/Article/details/ggbacvxsk.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfpcwybv.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/gkupocvcd.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfqayilf.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyohfypwn.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gqrwvqjzk.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrxnhcba.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/gopcsbluh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfzubjmi.sHtML

[T47] Perl：正则捕获
来源：http://blog.fanxiaobao.xyz/Article/details/gubwokbyl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gaopnujlu.sHtML

[T48] Perl：正则替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqfblzwi.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcnusfyq.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gmyjkfiwf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpoawxttx.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjyvwziy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fanxiaobao.xyz/Article/details/gbsfapwgm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzsdewgoq.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcycbszh.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejugdrha.sHtML

[T52] Scala：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gmeragmbv.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gqcscgbxb.sHtML

[T53] Scala：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gtgtyymzs.sHtML

s"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/ghnwbcsfa.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/geheolgmu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gqnnthevm.sHtML

[T55] Scala：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gvlkebuyk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqimnlcxq.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduzzrtgt.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gmgjjhoge.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/ghntkovya.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/gdwnnlmsu.sHtML

[T58] Scala：函数定义
来源：http://baike.fanxiaobao.xyz/Article/details/gjxxcufno.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gexocqpun.sHtML

[T59] Scala：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/guvleaqiy.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrfgdkvy.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/gazyccdvt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpawewxtt.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gauneqorg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gxtcbyllw.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/guiwdvgqc.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gqridmtqi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjxtcfkg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqpwuoxb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gtakcxxkc.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fanxiaobao.xyz/Article/details/glvllhfyb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmfpkogr.sHtML

[U04] Py：变量调试打印
来源：http://3g.fanxiaobao.xyz/Article/details/gvqgxafph.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fanxiaobao.xyz/Article/details/gmecxzgdy.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/gykoftlhm.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gnrecvwkm.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdfbhsoy.sHtML

{**a, **b}
来源：http://3g.fanxiaobao.xyz/Article/details/gxtnxqopv.sHtML

[U07] Py：反转字典键值
来源：http://baike.fanxiaobao.xyz/Article/details/gbmtdkiaf.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fanxiaobao.xyz/Article/details/gnpvxwfkn.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbxgptlw.sHtML

[y for x in nested for y in x]
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsnkpmiv.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fanxiaobao.xyz/Article/details/gslxaimnh.sHtML

max(d, key=d.get)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfeiuhdpj.sHtML

[U10] Py：按值排序字典
来源：http://blog.fanxiaobao.xyz/Article/details/gqdvmhjdm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmpafftf.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvylpvzm.sHtML

(x * 2 for x in arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxtnlsut.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fanxiaobao.xyz/Article/details/gsrlkykar.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gszpojhzu.sHtML

[U13] Py：固定长度队列
来源：http://baike.fanxiaobao.xyz/Article/details/ghvjwvvqn.sHtML

deque(maxlen=10)
来源：http://blog.fanxiaobao.xyz/Article/details/gdunflpat.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fanxiaobao.xyz/Article/details/gcosehxco.sHtML

defaultdict(list)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgtikgwz.sHtML

[U15] Py：高精度计时
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrquxdvr.sHtML

t = time.perf_counter()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqnocbyi.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgcwadro.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsxnalsr.sHtML


<!-- 参考信息 -->