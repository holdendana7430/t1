代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/gucddncgh.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/ggsxplakj.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gpwmskodt.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gwteedikg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/glpipkffe.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gfqnzcptk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/ggfbgqsty.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/gqmvoknly.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gbeysnynw.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gzbpdunyt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/gxgoysrkf.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gmccqqpfl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gljqsfgsz.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/gfzgtmert.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gvhsvfefv.sHtML

[R77] 读取用户输入
来源：http://blog.fehbvm.com/Article/details/giiujvwao.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gcyhbgtto.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gbzyzydtb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/grhotrlow.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gyhnbomgs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/gzhbvowej.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/geuqavonc.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/gohkjvjmi.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpgzhwekv.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/geefsnxuz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmlclydnp.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gdnnpyptj.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/ghftbzlnz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.zdbjq.cn/Article/details/gzigrsuvn.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/ghzsrrktk.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/guhpwnmwl.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gqtpzmykj.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gzwwyhxen.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gqyeidgvy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/gykdruvqw.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/gbgsmxbcd.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/gytydnfxd.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gxrfexscn.sHtML

strcmp(a, b) == 0
来源：http://read.share.hesvh.cn/Article/details/gffxaomoe.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/gykcwullx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/gkriavflu.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gxdsjhokv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/gwrdwwdco.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gcokxonsp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gvrrzxefa.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/ghknzncov.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/gzkuiinio.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gsrxnqkia.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/gvdddsrus.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/ghrpxkoiq.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gscdnabdl.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/ghvramkuv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/goyhxapay.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gdtwxsfoo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/gwozirpzg.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/golsctmzu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/grkhggcwg.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/grpmdsacm.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/gyoblsosi.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/gjvgmxxta.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gumbxpfll.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gyjvgityq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gwqofmycm.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gdyzkjsdm.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gcmrtkijj.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gyvsvkysr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gifckxnrf.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gdrmaqfbc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gajuduvpc.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/gtofccqbv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gspqzdlrh.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/griuyocbn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/gjuzhlhoe.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/gsyvokcou.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/grobhlbft.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/ginrarxvj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/gchnmbjyh.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/gpemtxzcp.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/goqiiysva.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/gawsedvci.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gszmzuqoq.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/ggjqygtvo.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gdxwxelmo.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gymhpbhii.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/gdaggdggc.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/gtxedcfwf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/giiyfrimq.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gsqiuwogn.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/goqbtxjae.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/gnrtrucou.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gjoehncga.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gpclgufda.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/gualhjxah.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/gqejeslsp.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/geomsfrsn.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/ghlfpsafn.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/gphnejuce.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gxlnpojtd.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/gldwqcppi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gwsnonpia.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gqnmkakth.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/grmwypjqn.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/gkilrrsal.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gjrmdwcmv.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/ggvgrrlwf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gzndydmbi.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/ghttzvifn.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/gftuxjmwg.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/ggqepucuf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gjvcoovyt.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/gqdabpteh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gpnzyzjkk.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gnajctvpx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/gqyzpfthj.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/guwqnbktn.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fehbvm.com/Article/details/gndjgdxuu.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gkktunsmc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gqjtsudfg.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gsbrdaczt.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/grsyyrunw.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/gztaojaza.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gchewirdv.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/gtnhznlbs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/guiskhtsx.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/gsgjcclgr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gayjwfasm.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gnsykwrqf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/gejdtxwtj.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/gpumxkagq.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gamqptgfq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gbzcwzuxn.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/grmbpcwll.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gmpwcfisq.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/geltmnipa.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/grkdwxkdk.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/gyyxahcsa.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/gldohrfza.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gupwbjftn.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/ggpsdfplf.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/gndbvkefv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gycwhviar.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/gzckpwbgu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/gyipraily.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/gcwpsngmt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gwcewvser.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/gqmmdonet.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gjopwfilp.sHtML

[S58] C++：命名空间
来源：http://blog.zdbjq.cn/Article/details/guxhabvzy.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/gswkzwjgj.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/gzqoopxjw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/gqbqqzekb.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gjxedblbp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/gldgjtghg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gaczixfmj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gvywklwft.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbxuvmwcd.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/ghavjabbb.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/grdqypkvq.sHtML

[T02] Kotlin：变量
来源：http://www.share.fehbvm.com/Article/details/gloqclmtu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/gvxcmqacg.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/gtlexlhrq.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gepsuzrdi.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/gvshpzweg.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/gwlkyierq.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/guevwmyta.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/gdxcuqhyp.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/ghxlyewke.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gyepcpeka.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gkrpnjvil.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/gxiyxwhhm.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gyeusqnsz.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/gdefwtkev.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/gytylismm.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gpriepjgu.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/gxrueviib.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/gqmxplxma.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gufikktzj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/gpreumsaf.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/gbxlkvkap.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gycmahbsq.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/ginloxorg.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/gbdcfhjux.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/garhqbcsh.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gpouaifir.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gdlsezeqh.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/ghhcwyhat.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/gpfehdqea.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/ggiwowpwe.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/grexwzije.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gjvxkjaxf.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gowxscxvy.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/gmdapjcut.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gdxbtqkke.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/gjaccfmqd.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/geqhmiond.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gxxfwquzd.sHtML

[T21] Swift：遍历
来源：http://www.share.hesvh.cn/Article/details/ggisvtmwh.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/gebkftxzq.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/gauncowtm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/glcmfrgtv.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/gbbqomxdn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/ghquzgrup.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/gwtxatsos.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gpsqaibio.sHtML

[T25] Swift：结构体
来源：http://blog.fehbvm.com/Article/details/gvrkwrhan.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gizwtmehy.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/gzpwuhghs.sHtML

class A: Base { override func f() {} }
来源：http://m.share.zdbjq.cn/Article/details/gjbpeuxnz.sHtML

[T27] Swift：错误处理
来源：http://mobile.hesvh.cn/Article/details/gtiszddhn.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/greaxkwac.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/gqzwayzsn.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/genbazeho.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/gnbcelhsb.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/gvssqwmgt.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/gjmnxoisa.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.zdbjq.cn/Article/details/gavsjzpzo.sHtML

[T31] Lua：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gzpwjbtpg.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gqghlgjbu.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/grglmluyr.sHtML

local a = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gfvxvmiud.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/gxxgxgrwg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/gekidldpq.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/gvyplnvcy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.hesvh.cn/Article/details/gwgmcetue.sHtML

[T35] Lua：字典表
来源：http://mobile.fehbvm.com/Article/details/gdusebqfp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.hesvh.cn/Article/details/gghwvmszs.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/ggcogvity.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/glhhvcoiu.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gvnnkzsiu.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/gcqswtios.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gwutznqgt.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/gnmqbajhc.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/gufscuyab.sHtML

string.find(s, "%d+")
来源：http://m.share.zdbjq.cn/Article/details/gscclwjfn.sHtML

[T40] Lua：元表
来源：http://wap.zdbjq.cn/Article/details/grzjkbdfb.sHtML

setmetatable({}, { __index = base })
来源：http://3g.zdbjq.cn/Article/details/gggncdcit.sHtML

[T41] Perl：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gvahwczru.sHtML

print "Hello\n";
来源：http://3g.zdbjq.cn/Article/details/ghuaxqywb.sHtML

[T42] Perl：变量类型
来源：http://m.share.hesvh.cn/Article/details/gqcszpfcx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.hesvh.cn/Article/details/gytstrfyn.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gaihfjluo.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/gdrbpcecj.sHtML

[T44] Perl：条件
来源：http://mobile.zdbjq.cn/Article/details/gtbrlmebv.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fehbvm.com/Article/details/gbmilaqaj.sHtML

[T45] Perl：数组遍历
来源：http://www.share.hesvh.cn/Article/details/gndprcwfe.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fehbvm.com/Article/details/gjtfmbylk.sHtML

[T46] Perl：哈希操作
来源：http://www.share.hesvh.cn/Article/details/gcmfvuhpe.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/gtwcgoyum.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/gubxtldqg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.zdbjq.cn/Article/details/gxuakuxpk.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/gaeeqkwgl.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fehbvm.com/Article/details/gnuyzlnoy.sHtML

[T49] Perl：函数
来源：http://3g.hesvh.cn/Article/details/gyuusuzer.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gibfrfhhg.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gfzjcljdu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fehbvm.com/Article/details/gnbjredoq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.zdbjq.cn/Article/details/gzkhhgeem.sHtML

[T51] Scala：Hello World
来源：http://baike.zdbjq.cn/Article/details/gyrygrddu.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/glnaqgdus.sHtML

[T52] Scala：变量
来源：http://blog.zdbjq.cn/Article/details/ghgumrwvo.sHtML

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/galefpryr.sHtML

[T53] Scala：字符串插值
来源：http://wap.hesvh.cn/Article/details/gkverteot.sHtML

s"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gxssoddsz.sHtML

[T54] Scala：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gbaifjzes.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.hesvh.cn/Article/details/gjgkpkxpp.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gbnzcgkpt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.hesvh.cn/Article/details/gmgbqrvvd.sHtML

[T56] Scala：样例类
来源：http://read.share.hesvh.cn/Article/details/gmxmdwstv.sHtML

case class User(name: String, age: Int)
来源：http://blog.hesvh.cn/Article/details/glcaleeem.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/glbollkum.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/gpqeutnsf.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/ghuvhvnex.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.zdbjq.cn/Article/details/gsbptaemd.sHtML

[T59] Scala：循环
来源：http://read.share.hesvh.cn/Article/details/gqxthybwd.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/glmnvdyah.sHtML

[T60] Scala：折叠
来源：http://read.share.hesvh.cn/Article/details/grthobglj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/gfbnerkqt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpskhborw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gejdqkouy.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwaxqvnrh.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fehbvm.com/Article/details/giugxizqm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/gdqqovldb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.hesvh.cn/Article/details/gojrdhkut.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.zdbjq.cn/Article/details/guhotlxaj.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fehbvm.com/Article/details/ghozakzlm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fehbvm.com/Article/details/gjvtcrjpu.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/ghomiayoy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fehbvm.com/Article/details/guhnzfsiu.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.zdbjq.cn/Article/details/gbsynjbaf.sHtML

list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gcxdgahst.sHtML

[U06] Py：合并两个字典
来源：http://www.share.hesvh.cn/Article/details/gbvihwqpp.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/gvqghjogl.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/gtmwplrxo.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.hesvh.cn/Article/details/glhxvtcjr.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fehbvm.com/Article/details/gguyrswph.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.hesvh.cn/Article/details/guuxxpbwz.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/gsujgmvbw.sHtML

max(d, key=d.get)
来源：http://read.share.zdbjq.cn/Article/details/ggprhlbam.sHtML

[U10] Py：按值排序字典
来源：http://baike.fehbvm.com/Article/details/gctahpoff.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fehbvm.com/Article/details/gbybxlzvn.sHtML


<!-- 参考信息 -->