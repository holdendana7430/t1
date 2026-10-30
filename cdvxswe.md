代发 wailian999

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gsdofgigj.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggghcsive.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkrquspk.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gdageokkp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gzunjfgdd.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzucihsm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqczuvbga.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshmeszms.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gofzlpxwy.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcjpkkmz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gyjfooniw.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gzaykdfwm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gnyeyozxv.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdxtrnnk.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/glmtbstcy.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcotdyay.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gakoyhyue.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdtlwlpy.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpughoaae.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvmvumrx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gclgqvgqb.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gtltagepj.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmurjsle.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/glykekmyh.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gezyglofx.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzghmotfl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gtebvbenz.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdpptiou.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmefwife.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gtfbyqwbv.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gnivuximi.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbbkektg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkixnbvpc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwanhazw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gnjrblbcy.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gqhtbsuqz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gdomyuuod.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gtetmkhmm.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gkehdsydj.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gpciubkdy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gbzwfzaho.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gydxqyvxx.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwzrpgyb.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gartxcbss.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gyuepfksr.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkzutwya.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzckaxieu.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/ggvmyftif.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gtruksjzp.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfibjocw.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsgncyxv.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gxltbsupw.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gphqsypdk.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbltssqkw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpontvdp.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxfpgwie.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxdjzcaf.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gmyidiftt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqalmlcu.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gisfamwqb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gysgcvrnz.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gcgexcxgz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gmkkjyuag.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gjvravest.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmojhgzqq.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gohhmdkbh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gcjuwalcd.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gvirpaofn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsliglzg.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbsquqip.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gimxtdged.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztrsabpn.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixiyetsm.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/ggenxlmwd.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gqvfnaewr.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/ghdllvrdz.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrpjbwam.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxiknuumb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gunyynfgx.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvahqpxxd.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxrilejw.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvfmqmlu.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gytguarjo.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdolnuam.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbgdynwx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmtsiugqz.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfwrxjrw.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/geomivsqo.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmymcdgdv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gykjwflvr.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/giongkagq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtewhxvib.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/guuqcohsr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gohupluri.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/grfuezlud.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlfldkzr.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/goxxhaudg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlkejebq.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhbbexyn.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gzojnokda.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/glevzupil.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/giclofyfk.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcizozyy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gibkltnwg.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdcclmzv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gkauwiifv.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpomaoou.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkoxuxjja.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/grgkposys.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gxwwljlme.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/goqrugxfr.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkezouxer.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvecaepd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/ggargfmki.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/guabnvlea.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gysqvistj.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmrmokdx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdynpkkpx.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gohxjdjod.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbiasrczk.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gxlzdtbsi.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkllwrecd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gchtefkpb.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrphglec.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghoahgttx.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/ggiytgxjn.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gsxaiuqve.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssvvmxzx.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/grisxnove.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtmlrgha.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gumvlyxjr.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gzxvbsjwc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/grgrnddcz.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvelqamrx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbzokong.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gpchmwvpv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqmkocig.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/gveqaopzy.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpecbvpla.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gyiiadxji.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gawyyuviv.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gxahpenuz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gedofydur.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gtfcugvzb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gflruzove.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwoewnwo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/ggxtuifdn.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gdarzbazp.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpoawzel.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gifzuduol.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gglpkcqnv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlbepthy.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxamggun.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwrjljmb.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gagqyucsu.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/glnphtiur.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gsjwcalxt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/grliohksf.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gldexlwdo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gmsgvbolm.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqdjgiyb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcmthtqg.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjauxihbd.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gvcrgrvib.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gofwxinpe.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilhrioyt.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuxdxtqf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcetyaif.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/gctawtimv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvnxmdlk.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzodjdjg.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/giuneyysr.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdiaefvth.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gyamwewrs.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/grprtjlrf.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gwoolyrqd.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzoivfpoa.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrntxwhf.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlnncfmh.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrgxltxz.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gobskwtce.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/guiwfakvg.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqsmrbdw.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgkwbowm.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gqfimsqxu.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggstcuguc.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkfbzcbt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxagnjuu.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemojpqjp.sHtML

for x in a { print(x) }
来源：http://blog.fanxiaobao.xyz/Article/details/gsozageji.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgbdlaev.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrcoigwg.sHtML

[T23] Swift：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmjnqnrm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gviuadnov.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhxvhvgv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/grnxiyylo.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsaspruq.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonowtcps.sHtML

[T26] Swift：类与重写
来源：http://blog.fanxiaobao.xyz/Article/details/ghqozlfag.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwxuifln.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gslrsepic.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/ggkfxfqis.sHtML

[T28] Swift：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/grjcqhgqk.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdxpniby.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/ggtkkapzk.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gjkesqyco.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gulikzrbu.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnieigit.sHtML

[T31] Lua：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/giurezvcq.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/grpegkkwq.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gexheqsro.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gfmdyhrjd.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvgcbepq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbqhqpns.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/gynmijvyd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqmttpuv.sHtML

[T35] Lua：字典表
来源：http://3g.fanxiaobao.xyz/Article/details/gstyfiekh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gfycojzkj.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gupthwmii.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/gmihjprxo.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/ghbulniph.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/gytxeqems.sHtML

[T38] Lua：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegqhxhbz.sHtML

if x > 0 then print("正") end
来源：http://3g.fanxiaobao.xyz/Article/details/gzxghyopr.sHtML

[T39] Lua：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gdlnkfcxp.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcohpupck.sHtML

[T40] Lua：元表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcpscxnb.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbcxbkrr.sHtML

[T41] Perl：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gpsxqrdzr.sHtML

print "Hello\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtafbzbm.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsffdkci.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsmwmsku.sHtML

[T43] Perl：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/giybvrfqh.sHtML

"值: $a"
来源：http://wap.fanxiaobao.xyz/Article/details/gazliuknm.sHtML

[T44] Perl：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gvbpcggea.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxvrgzwx.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gyjgvbpak.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvttnlkyd.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwgnczns.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gztkmrtii.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fanxiaobao.xyz/Article/details/gjaeesmys.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnlckfer.sHtML

[T48] Perl：正则替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhhgivwf.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjufqfqq.sHtML

[T49] Perl：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/glyyngxhx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzpmnyflg.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgtzlokf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fanxiaobao.xyz/Article/details/gflkoohxw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllbnkpgq.sHtML

[T51] Scala：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gphujryeo.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gsbhumnke.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gaatrtyvs.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbghxqmmw.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gkesebeyn.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gqcbvscxa.sHtML

[T54] Scala：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gggaosbsa.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyacojjtv.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gbchlwrod.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppcwjfxo.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbckezhl.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gibidmfzr.sHtML

[T57] Scala：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gllvchgkv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpewqpsm.sHtML

[T58] Scala：函数定义
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxlupire.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmtmkzpp.sHtML

[T59] Scala：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gullfhfrv.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gqjqzzclf.sHtML

[T60] Scala：折叠
来源：http://wap.fanxiaobao.xyz/Article/details/gwkpuguan.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/gumlxuoet.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqnydrut.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmibdukg.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhrtoohq.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqcrtwpe.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsfluevm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fanxiaobao.xyz/Article/details/gzctrngdh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlsdvsni.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwtynikt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgweovlo.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fanxiaobao.xyz/Article/details/gbohzvvng.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggabegbru.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fanxiaobao.xyz/Article/details/gpjalrzuf.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gmfxfpmtd.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntlnrfyz.sHtML

{**a, **b}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajdcendw.sHtML

[U07] Py：反转字典键值
来源：http://blog.fanxiaobao.xyz/Article/details/guaxcxgvs.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fanxiaobao.xyz/Article/details/gtumpamnm.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjkcnmei.sHtML

[y for x in nested for y in x]
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgmcpwec.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fanxiaobao.xyz/Article/details/gpxeckznd.sHtML

max(d, key=d.get)
来源：http://3g.fanxiaobao.xyz/Article/details/gbhpriafz.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbyfpwff.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fanxiaobao.xyz/Article/details/gwadgfvto.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gekkwmwxk.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdmezjfc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fanxiaobao.xyz/Article/details/geqftzgaa.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjkrojgn.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbpamrvb.sHtML

deque(maxlen=10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxfzykxn.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fanxiaobao.xyz/Article/details/gqtbtaumc.sHtML

defaultdict(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcuwineob.sHtML


<!-- 参考信息 -->