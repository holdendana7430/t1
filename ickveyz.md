代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpaorxal.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjnsckie.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/guuyeouwd.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gzbxmcdqo.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gyomytpfw.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gaftrwlpq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gmllbtdfx.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gwgoqzona.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpooatsr.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcokpjxrq.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gpdardqds.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gjxnwfyfe.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gckczyyis.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gggperwez.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gwozneynm.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/geisvqsrz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdvfyoudi.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gxzzplbja.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gyyjabkyy.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gimaaeabc.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwkmjhlx.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrbnqzno.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnntjqjt.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykwydcxq.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gvborqhnz.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gcehsburf.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gprikfjtc.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzqoyraj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gjjhraicz.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/grhztqzlq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgbbtwbu.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/ggqaxuais.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkvfowfw.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gffmwbwtd.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gichhjhvl.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghukkgiem.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsovmkxvf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbxfcrxq.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gchcovqtc.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwuwsbdo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gkqeqnjpe.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gfoezneyl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gobwezqrt.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpjmyvzj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/ggifhifxy.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gpyxrjexm.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gkezkhhsu.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybautncb.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/guemjeeux.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/givchkbbb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gjdmijecy.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gerbtnkfw.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gverftntd.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gvzpsygbr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gxxamnlno.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/guypqmkte.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzvgqpdf.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjvyeywg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gryzeivwm.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gmwjnrhen.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxfpaxnq.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjjpqtel.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/girgckmzf.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gdvcfmzbf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/guzufmctl.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzjvxida.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gtvrhgpwy.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxytsxww.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gibsnywtw.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gdudtqdqu.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gpbtevngw.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubfjwnpq.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gvdvxrova.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gbldgkqdi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/giavfxuvi.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gnrqoeorp.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gheamddty.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhgarjlw.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gkykgjsyj.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfnwqgsf.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gsgogmntv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbptkyyia.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gjivtopbq.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/ginqmrbnj.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/grramiall.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gtpfjtfma.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gbolgxrqb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldsrukxo.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gfmeimeyy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghguljusg.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqkhtndz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/givenyhin.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gylmiambc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjlpqvrh.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gyerdndcy.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerdzoegg.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gjdcmajxf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gofutrxvc.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gsatsdvsv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrbdpvfn.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsfbautd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtizhiykv.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gzmnhbojk.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gqavqnukp.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqfjavzi.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulscqops.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/grmlazojq.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtspnyazt.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsoysfadf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gwupulbas.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gnccigswf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvshvznd.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbgyshdj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmpfksis.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjkittra.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyoukqaz.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gcqayoyba.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gzghishre.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthmwsnvt.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gzzghahsv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfoheefnx.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuqoujwy.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gqmumvkgo.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdsokymv.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/guapwevha.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gtoyolumw.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gynzyymqc.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjwtmaou.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gfqvdmfoh.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfazdsdv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gxdtafgkw.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/guafvxxqc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gveuzytsp.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrewpizf.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gfbvygvla.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gcqpsbtvs.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gutaykbgu.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/ggdrutfvy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gdemzdetm.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfvhayyq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcjqzbmf.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ganfjthok.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjtbalni.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gxtgjkpsk.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/grnvkaism.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/grhkzaxlr.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gcbvhoeug.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/grvnmctky.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsuwsuvnj.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/glvohptyi.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gkwupbfcp.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/giligjyzs.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvxggqow.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gqpaaihah.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/guexzebve.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gviudxxqa.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyzmtbrm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbfhuxgi.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gevatulju.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gihcwbqyp.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gkewcfavc.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuzjdamo.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkcwlfay.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzikuegz.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/genyeatiy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjjmfogm.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghryancrj.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdzakhri.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhulynec.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gvqilxaqe.sHtML

[T14] Kotlin：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/goferkdkv.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxpblnga.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gsibjzgfc.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdceqfjrx.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gixbpeeou.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/golvfzabl.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/gxhreityp.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzenmiiwg.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdryvzvb.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxkoyedf.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gvcckryby.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gpmygafow.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmdmdaql.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjiuzrsp.sHtML

[T21] Swift：遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gkodpqgpu.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrowzjky.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/gbkmxfrvk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwkwirfg.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gkvkeekns.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqubnzetl.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutsqkjjd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/geemuhfuy.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/glcjycbju.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlgpjzmj.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/guginqeur.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/grvgkeqak.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/glydaerpf.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylfuwcup.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvoxuxtnr.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/gaapuievz.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnemynal.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/gjtesrlgm.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvsjoajv.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrgpazza.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gghslslzp.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gfihksjvu.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfpcgqug.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvfyxvyo.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfhxattz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmxkfeea.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/glqxwnqsx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhlflcpw.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/gaqrmvfbl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gyexentqe.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsrhfvxz.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/gdzbqodth.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/glgwwunzk.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/gggnkktbj.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/geczxhfkw.sHtML

if x > 0 then print("正") end
来源：http://3g.fanxiaobao.xyz/Article/details/gsetqqazm.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gaumdkymx.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzsmrzal.sHtML

[T40] Lua：元表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmzhatus.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/gmgcykozf.sHtML

[T41] Perl：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqvwghod.sHtML

print "Hello\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gjhzpriyw.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlbnwdzq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fanxiaobao.xyz/Article/details/glcvbtkax.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjapsqrv.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkypiovrt.sHtML

[T44] Perl：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gxawkgyec.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gntleoiis.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gxbqpwtzy.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaoqeefsh.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/gwsnveavu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkimaisvh.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpfvukiv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghtshxvbu.sHtML

[T48] Perl：正则替换
来源：http://baike.fanxiaobao.xyz/Article/details/gfiambknl.sHtML

$s =~ s/old/new/g;
来源：http://3g.fanxiaobao.xyz/Article/details/gmkpocdlu.sHtML

[T49] Perl：函数
来源：http://3g.fanxiaobao.xyz/Article/details/giofnhpco.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyahcywio.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gcnbzgnhw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzylobqhp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhlayhaf.sHtML

[T51] Scala：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gwjhmbhas.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmprhqivf.sHtML

[T52] Scala：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gayuqzsni.sHtML

val a = 1;  var b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/guwmzhvtl.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvgxsvrs.sHtML

s"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnebmoffn.sHtML

[T54] Scala：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmvwqmbx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/guitqduoj.sHtML

[T55] Scala：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gfysyyofb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gtjtmjrru.sHtML

[T56] Scala：样例类
来源：http://wap.fanxiaobao.xyz/Article/details/gmzpmwrec.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkglqyqcf.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gfobksect.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyhorrhx.sHtML

[T58] Scala：函数定义
来源：http://www.share.fanxiaobao.xyz/Article/details/glsixfutr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcckafaa.sHtML

[T59] Scala：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhlpvemy.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuztjetc.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/gkqwwtctn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmuvzdrzq.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzkcoogw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gfipdlzox.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcfhbpvv.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fanxiaobao.xyz/Article/details/gmojazllv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fanxiaobao.xyz/Article/details/guvspvfxs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fanxiaobao.xyz/Article/details/grfvnmfoo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/glqygsswf.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fanxiaobao.xyz/Article/details/gwlbjmogk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlpswwlv.sHtML

[U04] Py：变量调试打印
来源：http://wap.fanxiaobao.xyz/Article/details/goiccpntr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fanxiaobao.xyz/Article/details/gnkpixuwv.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fanxiaobao.xyz/Article/details/goqssbnlm.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gxfgontnc.sHtML

[U06] Py：合并两个字典
来源：http://3g.fanxiaobao.xyz/Article/details/gppufwock.sHtML

{**a, **b}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghadcmpyq.sHtML

[U07] Py：反转字典键值
来源：http://wap.fanxiaobao.xyz/Article/details/gnvqmbxhe.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fanxiaobao.xyz/Article/details/gtsbnfobd.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjhhzeyx.sHtML

[y for x in nested for y in x]
来源：http://3g.fanxiaobao.xyz/Article/details/gtyihehkj.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fanxiaobao.xyz/Article/details/gybdcehqz.sHtML

max(d, key=d.get)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyxlytez.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvuuvgxh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fanxiaobao.xyz/Article/details/gcgdfphak.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpcypnww.sHtML

(x * 2 for x in arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/geyifxphi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtabepaoc.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmzeszki.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gvoesweml.sHtML

deque(maxlen=10)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzfamwou.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fanxiaobao.xyz/Article/details/ggdmqrujs.sHtML

defaultdict(list)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhizirdr.sHtML

[U15] Py：高精度计时
来源：http://wap.fanxiaobao.xyz/Article/details/gvlwwwtxb.sHtML

t = time.perf_counter()
来源：http://www.share.fanxiaobao.xyz/Article/details/ggohkturr.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fanxiaobao.xyz/Article/details/gmufhjlus.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fanxiaobao.xyz/Article/details/gsfzlfajc.sHtML


<!-- 参考信息 -->