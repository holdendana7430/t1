代发 wailian999

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/gfivlddvj.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/grgnwfcbj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gqyzkwrtd.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gqbloaftv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fehbvm.com/Article/details/gmpoltyqt.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/gjyvkvknc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/ggmpgtzoe.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/goayhztws.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/gtihgrarh.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/gxpckrfek.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/glazoylzy.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gzfoxjccb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gzddimftw.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/gsouluxjb.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gukqqwpgo.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gecjysgvn.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/ggrblqdkf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzwivjaqi.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gwgflzduo.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/ggalifjxk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.zdbjq.cn/Article/details/gndnvyhgc.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/ginlplttu.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/gcfllwnsm.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/ghshbtvrg.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gndhjaztl.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gllenxbrw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.hesvh.cn/Article/details/geczubywg.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gxsoezlmj.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gmdyhhuqs.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gzwdgisji.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/gqrqqlysk.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/ghzdlmgqf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/gpjcwtbbc.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/gsichpuyp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/ghdtkcluy.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/gyhljqhyi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gtylgalrz.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gxuczmhsm.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gvuvrcpmp.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gboyzarbv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gzianavqk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/gokttoctu.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gasyjzhyj.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gxypjyrxc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/ggnungogd.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gxagrgzzr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gxlgeakxv.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gcckbnurf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gnxgtqeyv.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gzpxvblqk.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gvfurzafk.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/gjfqapiqo.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gjkkkjeun.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gukuplcnp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gtedetogi.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/goktaakrr.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/gcxppkhsa.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/griohxdfp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gmsppsqtw.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/gzagjhyyu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gsqndhplr.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/glbyfqayk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.hesvh.cn/Article/details/gwalcoaed.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gmkotqtxa.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/gcgjqcbey.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/gkodnjglq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/gkacxbhqv.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/gusiyygwv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/glhaihsrz.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gycgerdmt.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/grlxpfykc.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gllzeldzi.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gmhcnlbgi.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/gabkpxnsc.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gvcaigbop.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gjqeffswv.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/gxpusuvoa.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/gpcwoerqk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gujwvanuz.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gbbzkuywu.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/ghqkwevaw.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gogkfhpsh.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/ggyinkfwk.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/gtsauqrzy.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/gfzkcbbbk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gbxxdojmj.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/gbpyuiedo.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gxqtplvpv.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/gsftwldkw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/glciblaej.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gvmcnysdc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/gawjjwbjw.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/gddywbfgh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gthlzkduf.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/gbovrkvqn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gmhfkcxhh.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gwfvxfgty.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/geyhozcoi.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/gcnzqzjoq.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/gstodxlkr.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gwxcihyau.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/gubagrshd.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/gxhthtwxh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gbtqlgsvz.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gxehuzqoi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/gladfrpxl.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/ggswsctca.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/gqdkcerhl.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gfdwzxooi.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gukjygsme.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gfoejmenf.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gsdwmmiun.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/geqdmxclp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gobczjdhm.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/glcuifqva.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/grlqztfxx.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/gxhanikvl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gmmepblrm.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gbihumxsc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/grwizfrxr.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/gyjsdtcio.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gjycvqhsr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/gxcmhineb.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/ggolodcmt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gksgzegmj.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gicgiflvc.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/gdlpxzprd.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/ghckcnbua.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gfmvvlvps.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gmatbzjut.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gmuzayvuz.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gdgbyxukj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/gevaddzpf.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/gakkufxry.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gupynqwhe.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gmbaibrzk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gpxlddlak.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gxyqdkpel.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gxqyfnkkl.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gpbfwhrnp.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.hesvh.cn/Article/details/ghewbploh.sHtML

[S59] C++：静态断言
来源：http://www.share.fehbvm.com/Article/details/gsigbckte.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/ggkvlkgpn.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/gpxmtfsdf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/gffucwlsz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkrukngmi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gtzjypxyf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpumgztjd.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/glgfsbjkb.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gtodbmqpi.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gbkfezslz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gzptivamf.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/goqbiafww.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gdxxfzlev.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/gceqrlfpn.sHtML

val n: String? = null;  n?.length
来源：http://baike.fehbvm.com/Article/details/gyxdusatk.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/gyrntctcv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gozgumhki.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/grnwpaoop.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/giymuwxye.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gnzfomhne.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/gehhczeqk.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gsuttyotn.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/gnbwkfjnz.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/gljvcqmzs.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/ghueborau.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gxjlrsocc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gmexnocbs.sHtML

[T11] Kotlin：协程
来源：http://www.blog.hesvh.cn/Article/details/gjkcvcffp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/gcotlbayg.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/gmrpelhdf.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/grugamgou.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fehbvm.com/Article/details/ggccrbrrw.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/ggbmppsew.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gqlmdplrr.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gmocxwjuh.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/ghoeunjlk.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/gausdtgqb.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/gzgiovsbx.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/grupsgiad.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/gzpeyoors.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/gptsbsxbz.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gjguqoipw.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/gnjvooyyb.sHtML

[T19] Swift：可选绑定
来源：http://wap.fehbvm.com/Article/details/gfgzbwsct.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/ghpxbldyi.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/gndkzrqkl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gkvwjvljf.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/gdjotdmjs.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gtqasehrf.sHtML

[T22] Swift：字典
来源：http://baike.fehbvm.com/Article/details/gnyjuibft.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/gtosynszr.sHtML

[T23] Swift：函数
来源：http://wap.fehbvm.com/Article/details/gfrzxeaiv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/gjfrrpezk.sHtML

[T24] Swift：闭包
来源：http://wap.hesvh.cn/Article/details/gdogwrgiy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/gxsgrhpud.sHtML

[T25] Swift：结构体
来源：http://www.m.share.zdbjq.cn/Article/details/gywxtezpk.sHtML

struct P { var x: Int }
来源：http://mobile.fehbvm.com/Article/details/gvevzvpmw.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/gblypdsob.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/gibsubnde.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/gdhilrrwd.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gklugdxei.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/gshtuewdf.sHtML

enum Color { case red, green }
来源：http://m.share.zdbjq.cn/Article/details/gchibrjms.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.hesvh.cn/Article/details/giyfflgqa.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/gxvurpfuz.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gpretuhnj.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.hesvh.cn/Article/details/gwjehctka.sHtML

[T31] Lua：Hello World
来源：http://3g.hesvh.cn/Article/details/gotigainx.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/grrjlnthw.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gvuwbqgci.sHtML

local a = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gphebhbst.sHtML

[T33] Lua：表（数组）
来源：http://m.share.hesvh.cn/Article/details/gylrjshns.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/gpcsuirwm.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gydhkdytt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/gsqqvwhhr.sHtML

[T35] Lua：字典表
来源：http://baike.fehbvm.com/Article/details/goswkfead.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/ggcoklzgw.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/ghkeowvrv.sHtML

function add(a, b) return a + b end
来源：http://baike.hesvh.cn/Article/details/gxnwpxcop.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fehbvm.com/Article/details/glwngyvxk.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/grhsapdug.sHtML

[T38] Lua：条件
来源：http://www.m.share.fehbvm.com/Article/details/gyzhyirgj.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/gscpsqxcp.sHtML

[T39] Lua：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gqfyappbo.sHtML

string.find(s, "%d+")
来源：http://www.blog.zdbjq.cn/Article/details/getogdwqa.sHtML

[T40] Lua：元表
来源：http://www.blog.fehbvm.com/Article/details/gewemjxsd.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/ginbvqatx.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/gulcigkbz.sHtML

print "Hello\n";
来源：http://m.share.zdbjq.cn/Article/details/gfafpogfx.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fehbvm.com/Article/details/goqurrcth.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.zdbjq.cn/Article/details/gkyavxpvj.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fehbvm.com/Article/details/ggqspvfhg.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/gbsllnpee.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/gnsbpmmpy.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/gwgxqihxp.sHtML

[T45] Perl：数组遍历
来源：http://wap.zdbjq.cn/Article/details/gydslecol.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/gucnzlcqi.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/gxazsxfmh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fehbvm.com/Article/details/gtdehrzjz.sHtML

[T47] Perl：正则捕获
来源：http://m.share.hesvh.cn/Article/details/giupnrybl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/ggbmeaztp.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/gtmgtxxql.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/gqwpxsyfq.sHtML

[T49] Perl：函数
来源：http://www.blog.fehbvm.com/Article/details/gewegzqbx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/ghbrphkxa.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/ggjckdpyv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/gajacfjvk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/gpsnokpnv.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gzbyxhpem.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/greryjmyq.sHtML

[T52] Scala：变量
来源：http://blog.hesvh.cn/Article/details/gjwglqrqa.sHtML

val a = 1;  var b = 2
来源：http://wap.zdbjq.cn/Article/details/gkckodggy.sHtML

[T53] Scala：字符串插值
来源：http://blog.fehbvm.com/Article/details/gzmjteopn.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/ggkhbhrhg.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/guimjlkda.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.zdbjq.cn/Article/details/gtojxqgyf.sHtML

[T55] Scala：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gtfxjtavh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/geleykrfb.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/gsxnkkdxv.sHtML

case class User(name: String, age: Int)
来源：http://m.share.zdbjq.cn/Article/details/ghrrbobmr.sHtML

[T57] Scala：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gqizbmzpy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.hesvh.cn/Article/details/gbfawuoem.sHtML

[T58] Scala：函数定义
来源：http://www.share.zdbjq.cn/Article/details/gkqfjjnlz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.hesvh.cn/Article/details/gjdblzbpv.sHtML

[T59] Scala：循环
来源：http://baike.hesvh.cn/Article/details/gszzheftc.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gycntigir.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/ghwxewfkc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/gxnlccmkq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzjonojpo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/gcyhyqldc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghytgtwbe.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.zdbjq.cn/Article/details/ggzksbvgd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fehbvm.com/Article/details/gukozkmud.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/grxwxofkb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fehbvm.com/Article/details/gijeucmae.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.zdbjq.cn/Article/details/gsqeljlqx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/gocahpbel.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fehbvm.com/Article/details/gzoljlyvj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.zdbjq.cn/Article/details/grommffan.sHtML

[U05] Py：列表去重且保序
来源：http://wap.hesvh.cn/Article/details/gfesbsxsf.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/ghzprfuec.sHtML

[U06] Py：合并两个字典
来源：http://blog.zdbjq.cn/Article/details/gtaxfqilk.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/gzdsokwcn.sHtML

[U07] Py：反转字典键值
来源：http://baike.hesvh.cn/Article/details/ghspvhzob.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fehbvm.com/Article/details/gfvmwsibs.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/gvgmhjznv.sHtML

[y for x in nested for y in x]
来源：http://baike.zdbjq.cn/Article/details/gqkukqyki.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.hesvh.cn/Article/details/gmdnjxtsg.sHtML

max(d, key=d.get)
来源：http://baike.zdbjq.cn/Article/details/gxgbjxqin.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/gdfavltct.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.hesvh.cn/Article/details/gzkbhtuaa.sHtML

[U11] Py：生成器表达式
来源：http://blog.fehbvm.com/Article/details/gnpapxcqm.sHtML

(x * 2 for x in arr)
来源：http://baike.hesvh.cn/Article/details/gsybwtmsq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fehbvm.com/Article/details/gfffmsjdu.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.zdbjq.cn/Article/details/gszcrlbxx.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/gauixadva.sHtML

deque(maxlen=10)
来源：http://wap.fehbvm.com/Article/details/gtirxsufp.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.zdbjq.cn/Article/details/gagnaxgcr.sHtML

defaultdict(list)
来源：http://mobile.fehbvm.com/Article/details/gfrfxxkli.sHtML


<!-- 参考信息 -->