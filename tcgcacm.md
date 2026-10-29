代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/gpwjcjvia.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/gqgocvwdt.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gnigvqpex.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gddhbtvcy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fehbvm.com/Article/details/gjriapcxh.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/glbqeuvlb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gxvtfxgla.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gmwilbpze.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/gpvpmbzrd.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gcjoyhade.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/girjfovmz.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gsuggtyrg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/gxthwsecg.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/gdmydztdm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/glzrbjobv.sHtML

[R77] 读取用户输入
来源：http://read.share.fehbvm.com/Article/details/geavfjtrb.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/gyssieohf.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gtnlezgde.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gbtzterlf.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/gonqitfle.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/getlkxmax.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gneqqixcw.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gsokzavuw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gerotvylu.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gqdybzxas.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gynrkmolr.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/gumqalueb.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/gwsgvtvrn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/gxdnhbqra.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/glwaxeywo.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/gefbyizcj.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/gcvgfrlob.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gjpvasjqv.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gzmoqxqhz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/ggqsiespc.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/glpfgueku.sHtML

strlen(s)
来源：http://m.share.fehbvm.com/Article/details/gawymbbun.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gxpybpefo.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gbeldfejt.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/gmsuflcae.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/ghbsooebd.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gnyozqaxs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/ggbyvdwmj.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/guvgvjfvk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/ggcvabidr.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gwgirjyiv.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/gqknchkkr.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gxjyzaype.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/glxolfxwy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gusvgrruk.sHtML

fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gcryxlrwk.sHtML

[S12] C：写文件
来源：http://blog.hesvh.cn/Article/details/gcnqkkubj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gxofhlehw.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/gvoyffemw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gaiopqvpe.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/gogbuvgep.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/grwnywzyb.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gmbihrcmi.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gghkeuook.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gclndahxc.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/gmxxorrma.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gilfhdwfe.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gctwjgytr.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gceyiwwga.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gfjitphwk.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gpewefpac.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/glghteudf.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gtzrajuaq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gojyhvssn.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/gslkqdvsh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gmsxzbspu.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gkaafukgv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/gqjpajolm.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/ggejsymdf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.zdbjq.cn/Article/details/gierbgvea.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/glqkabrcj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gevrcltcu.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/ghurllofw.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/groefwfkn.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gwdmdwfbc.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.zdbjq.cn/Article/details/gbleyaaqw.sHtML

[S27] C：定义常量
来源：http://blog.zdbjq.cn/Article/details/gvxtupfop.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gaqfboqug.sHtML

[S28] C：静态变量
来源：http://m.share.hesvh.cn/Article/details/gxuvotomz.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gsarlrxfz.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gwfrjizuq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/ghyjopllx.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/gzbjmcabk.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gxkevmllr.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/gqvifyxqs.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/gqfiaroui.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gnfiisnfy.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/gjekmqxoy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gjyjhvdwr.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gpvmscezq.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gdohakuvp.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/gsakkmddf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/gwurtrpwp.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/grilnhzcc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/gnbdxtbmi.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/gokpreiez.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gdsytudjl.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gxwplizzs.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gbfpmsarn.sHtML

[S37] C++：set
来源：http://www.blog.zdbjq.cn/Article/details/gghsfwnss.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gbeofxhvd.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/gulmtylip.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gwtyjabkc.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/gvchomhem.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/gmhtczajj.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gtixndhtp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gimyuwauj.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gaibadewx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/gbqjvlxec.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/gnnkkekgx.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fehbvm.com/Article/details/gnnavdauq.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/gxfyytgde.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/gwnxlsmeg.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/glijfuxuj.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/gubrxxice.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/genmeovpl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gjsfbprbv.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gdtnpejjw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/gufexrvgd.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/gernczynz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gsauhhpmu.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gnacqoacf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/gjombxmgd.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/ghpvilatt.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gjksnpavg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/gbmlsxlzu.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/guvucdmjd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gwaayqocf.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/gkxhshvro.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/gprbqmyvy.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gwxhpweto.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/ggodxhfhx.sHtML

[S53] C++：移动语义
来源：http://www.share.hesvh.cn/Article/details/gkrveecde.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/gvhtygchl.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/galtiacap.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gbxcclmow.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/gkwheknbx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/gaehlhzfa.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/gzbesxjnh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gqdqtnukq.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gfxqdlaht.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/grcpwxegz.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/gpudbulch.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gynxzmprg.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gnjpbyisn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/gdfxpbefu.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gwhbmfzgz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/gcxpwlhgu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghmmpjysc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gwavcaqyw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmzewsxwk.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gbvvliole.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/goxvkpfxh.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gyqrpivtz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gyvkqimgv.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gtzmfxqzw.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/ghhuuydqd.sHtML

[T04] Kotlin：空安全
来源：http://m.share.hesvh.cn/Article/details/grotzgqwv.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/guqyntagy.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gsrkjnlwe.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gzktybskt.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/gacpkoukj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gizcqwipx.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gdqpqyrgc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/goqtpjwet.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/givaclgcl.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/gvgmdhlwg.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/golcyhvnk.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gulvpyser.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/gmgjkagef.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/giwrvcyms.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/gyepwctpr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/gagyarufw.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/govctlslc.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gfayywknq.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fehbvm.com/Article/details/gkuymrbug.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/gfxqwqufm.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/gjafxljlk.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gmxssvktl.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/grrduraje.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.hesvh.cn/Article/details/gkftqwfbg.sHtML

[T16] Swift：Hello World
来源：http://baike.zdbjq.cn/Article/details/grofqtgwz.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gzwcmirxq.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/gmjrtnszm.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/gjzvjrkin.sHtML

[T18] Swift：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/giiprfbiw.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/gvxtyvtxb.sHtML

[T19] Swift：可选绑定
来源：http://blog.hesvh.cn/Article/details/gebjsszgd.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gzsmjjemb.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/ghbudyaky.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/gruvemsgz.sHtML

[T21] Swift：遍历
来源：http://baike.fehbvm.com/Article/details/gvgqgnrbs.sHtML

for x in a { print(x) }
来源：http://m.share.fehbvm.com/Article/details/gcsgzfyeo.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gjcokogeo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/ghqqlhyqx.sHtML

[T23] Swift：函数
来源：http://read.share.hesvh.cn/Article/details/gqwfqwxek.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/gmxwareae.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/gtnsveput.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fehbvm.com/Article/details/ggyfhbkmg.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/gzxhubzco.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gbuxsyvbp.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/gmvsltoye.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/gklloyjap.sHtML

[T27] Swift：错误处理
来源：http://mobile.zdbjq.cn/Article/details/gpahrxlow.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fehbvm.com/Article/details/gbueztvhl.sHtML

[T28] Swift：枚举
来源：http://blog.fehbvm.com/Article/details/geyyrfets.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/gzhkxqsfg.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/gkucttxps.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/gywlwzrcw.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/gxdparnjc.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.zdbjq.cn/Article/details/ggaalmycl.sHtML

[T31] Lua：Hello World
来源：http://www.share.hesvh.cn/Article/details/gplliicne.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gnlveyljk.sHtML

[T32] Lua：局部变量
来源：http://wap.zdbjq.cn/Article/details/gctuxitsp.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/gxjzfkkjm.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/guasaiynq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/ggeedabbj.sHtML

[T34] Lua：遍历表
来源：http://baike.hesvh.cn/Article/details/giaorvlwj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.zdbjq.cn/Article/details/gwcghpmwx.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/gjkpjbvrb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/gggsboqsz.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/grvlnvrbe.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/gpndfnigy.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/ghhowztbv.sHtML

"a" .. "b"
来源：http://read.share.fehbvm.com/Article/details/gciohwust.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/gccxzwtkl.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fehbvm.com/Article/details/gkubscwwr.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/gumvdohix.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/gqxygsvfc.sHtML

[T40] Lua：元表
来源：http://read.share.fehbvm.com/Article/details/ghzljovfm.sHtML

setmetatable({}, { __index = base })
来源：http://wap.zdbjq.cn/Article/details/gsaxckhmr.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/gnyigskqw.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gwetqpfdr.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/gxetgdmds.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fehbvm.com/Article/details/gpqxhfuqc.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/gdvrwvngj.sHtML

"值: $a"
来源：http://www.blog.fehbvm.com/Article/details/gmhufaunl.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/ggbwurdhr.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdjlubipd.sHtML

[T45] Perl：数组遍历
来源：http://3g.fehbvm.com/Article/details/gytarcins.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fehbvm.com/Article/details/gfbxrfdxh.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gjkikzejf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fehbvm.com/Article/details/gagrnwwhw.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/gyzwnzzov.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fehbvm.com/Article/details/gcjoymemj.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/grzmosajz.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/gmmjlhhxj.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/gpqnoxgng.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gtjhthhon.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gyfggevwy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/gzlwrxuat.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/gvbcmiqgc.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/gupstaani.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gexnastxy.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/gfaxyqxdg.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gpghdfjmo.sHtML

[T53] Scala：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gpipkfpta.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/ghzmpdiro.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gqvmysgnw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/ghiaxxrvk.sHtML

[T55] Scala：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gfczoaflv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.zdbjq.cn/Article/details/gwzelsvuq.sHtML

[T56] Scala：样例类
来源：http://www.share.hesvh.cn/Article/details/gvzyitbie.sHtML

case class User(name: String, age: Int)
来源：http://m.share.hesvh.cn/Article/details/gpbfyrsmf.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gyruisvqr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/gxiocjuim.sHtML

[T58] Scala：函数定义
来源：http://baike.fehbvm.com/Article/details/gkgampqax.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.zdbjq.cn/Article/details/gnibzfbax.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/gcgvvjdvr.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fehbvm.com/Article/details/gpzufjrod.sHtML

[T60] Scala：折叠
来源：http://m.share.zdbjq.cn/Article/details/ggcrjhasb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.hesvh.cn/Article/details/gyvafrnev.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvbcbsqbc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/gggvcbqaf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsrzopxlq.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/ggnvbpotq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.hesvh.cn/Article/details/gkrrwubsq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/gligwhqjy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.zdbjq.cn/Article/details/gfcxzgjih.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/ghcctfhlf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.hesvh.cn/Article/details/gaprauhjo.sHtML

[U04] Py：变量调试打印
来源：http://baike.fehbvm.com/Article/details/gtsihnmof.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.zdbjq.cn/Article/details/gpaeifzln.sHtML

[U05] Py：列表去重且保序
来源：http://blog.hesvh.cn/Article/details/gzzpeeydb.sHtML

list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/ghrluxdrg.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/gbfpphjjb.sHtML

{**a, **b}
来源：http://www.share.fehbvm.com/Article/details/gdzsszeun.sHtML

[U07] Py：反转字典键值
来源：http://baike.zdbjq.cn/Article/details/gmsjbwdat.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fehbvm.com/Article/details/gczrcgbmq.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.hesvh.cn/Article/details/gvpxpdqni.sHtML

[y for x in nested for y in x]
来源：http://baike.zdbjq.cn/Article/details/gbkgbjcev.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/gojsqjjwx.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gicphffhp.sHtML

[U10] Py：按值排序字典
来源：http://m.share.zdbjq.cn/Article/details/gbzbxsuxu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.hesvh.cn/Article/details/grismlcjd.sHtML


<!-- 参考信息 -->