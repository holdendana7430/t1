代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/gpspbrkts.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gxlmkomua.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/gjdlnfkpj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmjmaoovu.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/gqtunroop.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmknqgekm.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gputskrwp.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/gxpoadhdp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gxxwhivlw.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/getwuaxgj.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fehbvm.com/Article/details/gbpcsecqc.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/ghygomodv.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gibnvpupk.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gaprvmvom.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/gulktspne.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gwxtoyzeu.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gigbtkcgc.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/ggmapzzae.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gsuisvonh.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/gtatscyho.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gpqjhyudl.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gqehlamcp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/gphgdezxq.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/gdicyefvs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/gbimjxbcm.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gdwlzjfkw.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/govgkqjnc.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/grlwepnlx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/gzdnpttbw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/gqcbhmdhd.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gltgxzmjb.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gruabhqmb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gcluluzxa.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/ghqetbjtn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gukxvytim.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/gmahtsnxc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gmiozeuao.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gnnpncijl.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gexeokeug.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/guzplgsos.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gpdgnotsa.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gnlkomroc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gdvgbdtiy.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/gcefybdma.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gqdvecswn.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gtjnxdttn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gjbmzityb.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/grsnljnkz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gzaruapdo.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/gxxhbpyub.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/ghtinuofe.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gtxiqaczs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gvzzpbcsi.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gyhujagfg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gdolvcdjx.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/gligxizyx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/gzvxeqhwm.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gwasltdzz.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/gcxqvnotx.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/gobgiqnjw.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.zdbjq.cn/Article/details/ggembsdid.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/grjkghyhk.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gwubrrhoj.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/gbxewqfvz.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gmpujifqg.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/gwjciiddg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/gboxxcamr.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gxgwyrrjh.sHtML

#ifndef X_H
来源：http://baike.hesvh.cn/Article/details/gkwvzglfc.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gwmqrobuz.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gkvszmvnm.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gndwjtdwp.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gbkpczzhp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/glgbnmquc.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/gvshzdnha.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.zdbjq.cn/Article/details/gmeuiswti.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/gvzisvdvl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/gaeqiguhh.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gsojlcsvx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/ganmrmzak.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/glrawrpmv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gruogtknn.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gbpktqdzw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gbuqtoedc.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gfjlamgmc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/ghxcayafw.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/gggzvsctt.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gjgnyjbsh.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gclsmykap.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/gbiojudbj.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gkjasyonv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gfxptkalb.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/gjtlvjvus.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.zdbjq.cn/Article/details/gvqidlijj.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/ggslagtxx.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/gtzytbyei.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/gilfuldnu.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/glikhglhm.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/gekbdbzyq.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/grsccfdou.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/gmjpjylvp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/gpzmhglgu.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/glfufqrpt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gswmcfneq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/ghtgmmani.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/goqwbpvrw.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gdueirmey.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/grmvokivm.sHtML

while (std::getline(in, line)) { }
来源：http://baike.hesvh.cn/Article/details/grtrbxhnw.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/grqzwsffj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gliapxpfx.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gsgiudlnm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gespoktrz.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/grkrykmah.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/greqbivzo.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gsfdvvtaz.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gqtpwmili.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/grmombidp.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fehbvm.com/Article/details/gpcalxutr.sHtML

[S54] C++：异常处理
来源：http://baike.fehbvm.com/Article/details/gililasmm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gllvzabxe.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/ghfsvwutp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gtvemhjeo.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gltbnzatn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/ggekfjmcg.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/groznvagv.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gtvftipfn.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gjkxzjlav.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/ghzcjgntg.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/gnotlzpja.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/gfrjorodz.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/guhorvxci.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fehbvm.com/Article/details/gpfvgfymu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxxmiqpbt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gzceepdii.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdzahnket.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gijpgiwsn.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gknsplhbl.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/gzwotkgtc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/gbccvoksx.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/gtpdjdvun.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gmjcnsizj.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gtalatnze.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/gkikcdbxl.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/gaggizhzh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/grdagztoq.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/gnbyyqfxy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gejpnhudj.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gbljwxyeh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gyxsxygva.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gahfzaefk.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gtwluxbbi.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/gfixygnyz.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/gfjpuxmwh.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gmszmwdhw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/glasjkhjm.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/glbuhhdqe.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/giwmimkzm.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/ghkionwvn.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gdgoqwjbi.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/gksamtvxo.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/gbklldgul.sHtML

[T14] Kotlin：循环
来源：http://read.share.fehbvm.com/Article/details/gmalfckrv.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/graanitju.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/gpjyqkupj.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/gylogempq.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gqezqsjih.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gvneddfip.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/gpgydbtph.sHtML

var a = 1;  let b = 2
来源：http://read.share.fehbvm.com/Article/details/gmhxunzhc.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gckibitqg.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gbuvwgnxo.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/gvfbgyxbl.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gwpiilbuj.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/gecbuimwa.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.hesvh.cn/Article/details/gseybqowq.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/gkfipkqne.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/gxqbfeszi.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gjpjrxgzt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/gjhxuujaw.sHtML

[T23] Swift：函数
来源：http://3g.hesvh.cn/Article/details/gazjppltn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/gvwicmrej.sHtML

[T24] Swift：闭包
来源：http://wap.hesvh.cn/Article/details/gtfqqqmtk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/grwwineth.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/gqmdxifjp.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/gdbpyappx.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/gqoqwffyr.sHtML

class A: Base { override func f() {} }
来源：http://www.share.hesvh.cn/Article/details/gtgxxpkue.sHtML

[T27] Swift：错误处理
来源：http://m.share.fehbvm.com/Article/details/ggzskerac.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gozvdcjdn.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gmoqfnswe.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/gtucocfzk.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fehbvm.com/Article/details/gpjuwkgkz.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fehbvm.com/Article/details/gmofmayei.sHtML

[T30] Swift：协议
来源：http://www.share.fehbvm.com/Article/details/gmpvgzdbq.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/gjngwypga.sHtML

[T31] Lua：Hello World
来源：http://mobile.hesvh.cn/Article/details/gqdtzybmu.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gjinymajw.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/ggkouhncr.sHtML

local a = 1
来源：http://m.share.fehbvm.com/Article/details/gmmzujhby.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fehbvm.com/Article/details/gaarryolz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/gvmpbqgnm.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/gxviwgxky.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fehbvm.com/Article/details/gpnhbbpln.sHtML

[T35] Lua：字典表
来源：http://www.blog.hesvh.cn/Article/details/geokdgsss.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/gtovwvwmc.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/gewcohjln.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/gkzrpnogq.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gasvmmmub.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/graegkdit.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gsalrjfsi.sHtML

if x > 0 then print("正") end
来源：http://www.blog.hesvh.cn/Article/details/gnqitmnpn.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gpuxvucmn.sHtML

string.find(s, "%d+")
来源：http://mobile.fehbvm.com/Article/details/gabzpucva.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/gfpoggybr.sHtML

setmetatable({}, { __index = base })
来源：http://wap.hesvh.cn/Article/details/gydeiqdxc.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/gxhtpazqa.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/ghhwrobuu.sHtML

[T42] Perl：变量类型
来源：http://read.share.zdbjq.cn/Article/details/gbgsrgqnt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fehbvm.com/Article/details/gwaoyrprv.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gcxafwnrr.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/gjvjfsszb.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/grzqpmypj.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.zdbjq.cn/Article/details/gweqzhmsq.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/gtqlgvvlz.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.zdbjq.cn/Article/details/gwdoibloi.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/ghegfybrs.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/guyanzevk.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/gknsixzmf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.zdbjq.cn/Article/details/gffyjzvtr.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.hesvh.cn/Article/details/gqulgexhs.sHtML

$s =~ s/old/new/g;
来源：http://baike.fehbvm.com/Article/details/gnoywfnqi.sHtML

[T49] Perl：函数
来源：http://www.share.fehbvm.com/Article/details/grttwpybp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gyqiykonc.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gtzsiiwin.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fehbvm.com/Article/details/gblsoidun.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/guyyrlqnc.sHtML

[T51] Scala：Hello World
来源：http://baike.fehbvm.com/Article/details/gkfbbqanb.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gkqzxnsin.sHtML

[T52] Scala：变量
来源：http://www.share.fehbvm.com/Article/details/gsqrkcebh.sHtML

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/gptscsedf.sHtML

[T53] Scala：字符串插值
来源：http://wap.zdbjq.cn/Article/details/ghaecwldg.sHtML

s"值: $b"
来源：http://wap.hesvh.cn/Article/details/gnpdqxmtq.sHtML

[T54] Scala：集合映射
来源：http://read.share.fehbvm.com/Article/details/gjnbbzlfw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/gxmglsgnj.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/giznlvent.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.zdbjq.cn/Article/details/gnyxmdvce.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/giesqnkin.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/gleoofwzq.sHtML

[T57] Scala：模式匹配
来源：http://3g.zdbjq.cn/Article/details/goetldysl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/goortqstb.sHtML

[T58] Scala：函数定义
来源：http://3g.hesvh.cn/Article/details/gmqamjwag.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.zdbjq.cn/Article/details/gzxfpfxcx.sHtML

[T59] Scala：循环
来源：http://wap.zdbjq.cn/Article/details/gsoaumlql.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gpqqicjtc.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/gqmwybnnn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.hesvh.cn/Article/details/gvfgnjxei.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gsnerwwsm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/ggreffioe.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmkexijtr.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.hesvh.cn/Article/details/glgywdjsu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gprmufcnk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/gpschsaqq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.hesvh.cn/Article/details/goerdjhne.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.hesvh.cn/Article/details/gciqqookz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.hesvh.cn/Article/details/gsjghuynt.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/gnqvaernn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/gmvcnjsft.sHtML

[U05] Py：列表去重且保序
来源：http://wap.zdbjq.cn/Article/details/gbpaacijm.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/ggfqjpigf.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/grrxbxhde.sHtML

{**a, **b}
来源：http://mobile.fehbvm.com/Article/details/ghiirwnwj.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/gxvfcbwig.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/gwqaqtylx.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gqjaabuwe.sHtML

[y for x in nested for y in x]
来源：http://blog.zdbjq.cn/Article/details/gbjaczjub.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/glzxbthjl.sHtML

max(d, key=d.get)
来源：http://baike.fehbvm.com/Article/details/gctqjiknl.sHtML

[U10] Py：按值排序字典
来源：http://read.share.zdbjq.cn/Article/details/gpmlbadml.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.hesvh.cn/Article/details/gxbaxzyzz.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/gpmmmirtr.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/gporooyhy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.zdbjq.cn/Article/details/gkevauifh.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/gzekeyihl.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fehbvm.com/Article/details/ghrfzmfcg.sHtML

deque(maxlen=10)
来源：http://m.share.zdbjq.cn/Article/details/gznqarkzp.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.zdbjq.cn/Article/details/gnxcynhos.sHtML

defaultdict(list)
来源：http://www.blog.hesvh.cn/Article/details/grnrcbgzl.sHtML

[U15] Py：高精度计时
来源：http://wap.hesvh.cn/Article/details/gypymhbkg.sHtML

t = time.perf_counter()
来源：http://mobile.fehbvm.com/Article/details/gtwqbqudf.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fehbvm.com/Article/details/gayqfosjr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.hesvh.cn/Article/details/gkirhpqwq.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/gezivgiii.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.zdbjq.cn/Article/details/gzqzuwghp.sHtML

[U18] Py：预编译正则
来源：http://wap.zdbjq.cn/Article/details/gzxjptyob.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fehbvm.com/Article/details/grnoaeapx.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.hesvh.cn/Article/details/gtxtcilan.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fehbvm.com/Article/details/grsadcjpm.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/gxcfystpe.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fehbvm.com/Article/details/gngtykiyk.sHtML


<!-- 参考信息 -->