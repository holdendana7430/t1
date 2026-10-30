代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gzqhdcnjl.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gufevjtzp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gordxdcmv.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gvnntzqcx.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/ghkjhhpnp.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/ghzueovsx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gkqkhaola.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/gojkrpnxu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gpcymjkru.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gsqctrfsm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gtacfjfyt.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/ggpnothov.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/ggnwqjgmb.sHtML

[R78] 交互式菜单
来源：http://baike.fehbvm.com/Article/details/gcipdpuxj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/guvhmfllc.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/giwbvojtm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gjeauzlkl.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gmrsoddnu.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gidvfmjbr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwocqvmyu.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/gjaaulyyw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdcqtjkre.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/ggwcxjyxp.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gfoajsjps.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/gtuoycaml.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/gkgkhsfzq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/gftjhmbga.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/gaparpfvr.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/gsihxkjiu.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/gcawqbrwp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/gdsqfohtk.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gswhpenoo.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/gbzxdwjgv.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/geuirtdfr.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/ghakuklha.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gmtaigxvr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.hesvh.cn/Article/details/gqibkdpry.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/gqdfoqbsw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gxfvsnpti.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/gbrgdhffz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fehbvm.com/Article/details/gffmmmcsq.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gwlhykcyk.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/gcamktqge.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gcyxrlqpy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/gtnpjlumw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/ghskpbwjo.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gpaniahma.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gkdaniuoc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gckowbbrs.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/gfvizkjmj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gdiuzydoc.sHtML

[S14] C：枚举
来源：http://www.share.hesvh.cn/Article/details/gqwakcipy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gdqyywgwe.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gysrvccrd.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/gnmfmewwm.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/gxftfqdfa.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/gnbgelbsl.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gfsssxwdt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gfxhipkvz.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/goxneasxy.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/goerpyest.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/ggmkkwxjg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gxkdsscko.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gmwsihwti.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gsaxesfqv.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gsxkernjj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/gtfssogbb.sHtML

[S22] C：字符串转数字
来源：http://www.share.fehbvm.com/Article/details/giuqrdjmr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/gjyylioqf.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gomdfxwik.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gcpmxfqdr.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/glvditdoc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gmeyadvar.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gsppbxjei.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/gqgnckekc.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gpndguigu.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gxtegojhh.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gcjjcaumo.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gjnunzptp.sHtML

[S28] C：静态变量
来源：http://wap.hesvh.cn/Article/details/gagvnkbdc.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gezuphlja.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/gvlqipdlx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gfrshheno.sHtML

[S30] C：头文件保护
来源：http://www.m.share.zdbjq.cn/Article/details/gibfhcgup.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/gsjvarufs.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/giblbxtsl.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/gxfvbdhcx.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/glkkqjueu.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/ghzorndyd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/guksvsiil.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/gqtdvkyen.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gbchokpsb.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/gvtybdsce.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/grpobcsui.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/gjfrdcols.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/gqkfrqvqc.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gfbruksti.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gaatdtdau.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/gyrbugwuy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gskawubuv.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/golmrgpvk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/gwtywfggf.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gycdzoago.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/gofcvnbxp.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/gkmycldrv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/gbpbszysj.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gkckslwul.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.hesvh.cn/Article/details/grmfvdgoa.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/gfgmgkycq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gkhgnhszt.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gdqnncbyu.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gjjfxbzls.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/glrlhbpdu.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gsqeundtt.sHtML

[S44] C++：引用传参
来源：http://www.blog.hesvh.cn/Article/details/gtesmhpcx.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/gqerwkiyg.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/ghhlpnqqe.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gqihrzrqo.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/grzplibhe.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/gyrpjbbco.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/gkujuntqp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.hesvh.cn/Article/details/ghflnscsq.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gistdqxaj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/gqngzxanh.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/gnjpvrjud.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/giakhpxqf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/gsbozcocc.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/gtmweenzw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/gzegicrbo.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/gfptnjsfs.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/gsyxikfxg.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/ggnftpjsp.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/gdehupdmk.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gixqllvbp.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/gaphtswhv.sHtML

[S54] C++：异常处理
来源：http://wap.hesvh.cn/Article/details/gbylkqttt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gzgdtoxun.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/goygwciez.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/gosbtqkxh.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/ggxlarfpt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyrinslbr.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/gdfekmozy.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gvrfmcqko.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gpbubdlyh.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gtkcmoenn.sHtML

[S59] C++：静态断言
来源：http://www.share.fehbvm.com/Article/details/goidvmpki.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.zdbjq.cn/Article/details/gqwazdyik.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gpsfapwhp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gtqjxucqc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqviyalow.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gyqbzdofi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdckqgkbu.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gealvippe.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gonarpqvf.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/geirrrmls.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/gvkokcucd.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/goacsxdnf.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/ggtvbfilc.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gxjlygqgx.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gozcmmwkj.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/gsqvusbcl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/gpkshtczs.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gejfiztvy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gcjmgeyzc.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/gxykdawfm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/gkrjanibq.sHtML

[T08] Kotlin：数据类
来源：http://wap.fehbvm.com/Article/details/gzakvafsn.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gxpayqsxa.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gaszxawja.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/glidaurvo.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gwdvbbnox.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gzhveowuz.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/gydwmqzgl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/gjnvocyns.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/gzmbfikja.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gtnxytaid.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/gufhmrqzg.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/gryslsbzv.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/gzzkoxepr.sHtML

for (i in 1..10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gveffdrqx.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gbjdkhqyd.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/gxhtsajvt.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gsojfnmlv.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/grcnoktsc.sHtML

[T17] Swift：变量与常量
来源：http://read.share.zdbjq.cn/Article/details/gervhdfcc.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/glcpaqenr.sHtML

[T18] Swift：字符串插值
来源：http://blog.fehbvm.com/Article/details/gqrgreeox.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/gvarrbvio.sHtML

[T19] Swift：可选绑定
来源：http://3g.fehbvm.com/Article/details/gxwodyjgn.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/gzegjudgp.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/gwgxsoznw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/gmsxxpwoo.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/gmflzbmpt.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/ghxorvrgp.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/gaxzhlzbc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gkhqmtoqr.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gudqcixgy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/gxtdkayap.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/gqdnmymxq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/gnacbxxbu.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/ghlcemzuq.sHtML

struct P { var x: Int }
来源：http://www.blog.fehbvm.com/Article/details/gbnefaqbp.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/gyuqighcp.sHtML

class A: Base { override func f() {} }
来源：http://mobile.hesvh.cn/Article/details/gcdptuvae.sHtML

[T27] Swift：错误处理
来源：http://read.share.hesvh.cn/Article/details/gltfnpzue.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/gtnpqczvf.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/gqvlykxub.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/gjxlrrhjl.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/grlypypmy.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fehbvm.com/Article/details/gstqyxhqq.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/gxqpemdpg.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/gqxpieepo.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/glsacrxus.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gacuzrvfr.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/gyjfrcfdr.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/gbefmzqtf.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/gcudhdmfy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.hesvh.cn/Article/details/guqahrruv.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/gmhcelkfw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.hesvh.cn/Article/details/gjhqrxbat.sHtML

[T35] Lua：字典表
来源：http://baike.fehbvm.com/Article/details/gqwrjwxos.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gnrtgpujj.sHtML

[T36] Lua：函数
来源：http://read.share.zdbjq.cn/Article/details/gzhsggbcp.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/ghvqdyeri.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gjolrtktv.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/gyukssplv.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/glzmkhezo.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/guuemazdi.sHtML

[T39] Lua：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gpwrogimq.sHtML

string.find(s, "%d+")
来源：http://m.share.hesvh.cn/Article/details/gmietnvkl.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/gupwlvwno.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fehbvm.com/Article/details/gsughdoiy.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/glunokkzb.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/gcpwdsogt.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fehbvm.com/Article/details/grqzrsjqu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.hesvh.cn/Article/details/golcjgxyj.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gpctosued.sHtML

"值: $a"
来源：http://read.share.zdbjq.cn/Article/details/gcenustji.sHtML

[T44] Perl：条件
来源：http://www.m.share.zdbjq.cn/Article/details/glkuexhls.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/gnzcblzhs.sHtML

[T45] Perl：数组遍历
来源：http://mobile.hesvh.cn/Article/details/glketxkec.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/gtupszxif.sHtML

[T46] Perl：哈希操作
来源：http://wap.fehbvm.com/Article/details/gxczyjlvz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/guddhsbif.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/gitcfnrmk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.zdbjq.cn/Article/details/gyusxmhyr.sHtML

[T48] Perl：正则替换
来源：http://baike.zdbjq.cn/Article/details/gerevbwyi.sHtML

$s =~ s/old/new/g;
来源：http://baike.hesvh.cn/Article/details/gkzymhwwc.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/gkmpmhhvj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gnfmjqwrc.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gdglkydny.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gxiklzzuk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/grmbaloxv.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/gxqesykjy.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gyyvongfw.sHtML

[T52] Scala：变量
来源：http://baike.zdbjq.cn/Article/details/gmbdifkmo.sHtML

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/gxschjksj.sHtML

[T53] Scala：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gdszwqpsh.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/geggnqpuv.sHtML

[T54] Scala：集合映射
来源：http://mobile.hesvh.cn/Article/details/gvrtqavrj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fehbvm.com/Article/details/grutzkbta.sHtML

[T55] Scala：集合过滤
来源：http://blog.fehbvm.com/Article/details/gsblxabck.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/gimkxpbuu.sHtML

[T56] Scala：样例类
来源：http://baike.fehbvm.com/Article/details/gmeaadbjf.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gwolxxvdq.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gnnxqtvjv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fehbvm.com/Article/details/gswquejac.sHtML

[T58] Scala：函数定义
来源：http://mobile.zdbjq.cn/Article/details/ggyxkhfku.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gaqbjqiyn.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/gvqggehyv.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gcwupobsk.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/gjauitfdh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.hesvh.cn/Article/details/gsjacnpfb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gewaemgmj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/gugfiyggd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grulbqqml.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.zdbjq.cn/Article/details/gblmauunt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fehbvm.com/Article/details/gznesnjwg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.zdbjq.cn/Article/details/gpyrtzlum.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.zdbjq.cn/Article/details/grgpyvyyh.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/gwgobpifz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.zdbjq.cn/Article/details/gdwngrlwb.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/guwngbwfq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.hesvh.cn/Article/details/gdstzdedx.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.hesvh.cn/Article/details/gwswjfidz.sHtML

list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gjiulvqbw.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/gujajujgx.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gvdrtljwo.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/gwczptnqt.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.zdbjq.cn/Article/details/gnilwbwmm.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fehbvm.com/Article/details/gobdmmjyf.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/gsxwuzjor.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/gjstmbmlx.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gzwjlwjpq.sHtML

[U10] Py：按值排序字典
来源：http://mobile.zdbjq.cn/Article/details/gnceawfht.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.hesvh.cn/Article/details/ghjddbmmt.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.zdbjq.cn/Article/details/gorcjmajh.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/gxwwuydof.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.hesvh.cn/Article/details/gzdqecisa.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fehbvm.com/Article/details/gialvnfum.sHtML


<!-- 参考信息 -->