代发 wailian999

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gpryrtdad.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/gegjmhaxq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gyepumixk.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gjqceqhlg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gotocwmdq.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/ghxqklhns.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gyhhvrjsh.sHtML

[R77] 读取用户输入
来源：http://blog.fehbvm.com/Article/details/gvpjxurjy.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gkvxbnpde.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gxmenrfgs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/gxibfhtlp.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gmfsiewgy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/gvcwynkqa.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/gwkolqsnw.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/gjdaouhmu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqiyvyqth.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gvlmklafp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwbyqjmix.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/guwtelozy.sHtML

#include <stdio.h>
来源：http://m.share.hesvh.cn/Article/details/gmlwhwofp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gdmmgtqhk.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/grmypjebb.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gkrpvdnzu.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/gdgzkzptr.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/ghbmpjhpw.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/gpuhxfqca.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gnsircvky.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/goetgwpql.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/geyrsldqh.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gtshmrbqg.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gexbwpzbv.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gbevjgrtn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/gegwapbdy.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gecyjnlja.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/gvengaszx.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/gyhxcofjx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/ggretttmg.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gwvstqlsx.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gqjihkyjt.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gwtgzjnzu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gsqwdjiqi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/gplapjdgo.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gklfocxyi.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gphuowinu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gtwtvltwv.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gifdgnqqw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/glaptguby.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gewcjsvyt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/gzohyjtdy.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/guqlilqyg.sHtML

(double) a / b
来源：http://m.share.fehbvm.com/Article/details/gwrlxlvzp.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/gabevknxc.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/gieajtgao.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gsqfmckhk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/ggvyndltl.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gsdkdgbik.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gefoeykiq.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gnombhxud.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/guricefsy.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/gdzipuetw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gwqvgphmu.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/gxwvtsagf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gutnfwuvt.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gxnrrqtja.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/ghigrrizh.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gatklagfx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gygjuqlzi.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/gawhkzcqn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/gcidoutrk.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/grnetgmio.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/ggmetmmao.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/goehcpuqy.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/grgnmzdzt.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gookujxae.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gbfzlacql.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gfybptqmo.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gujdzeudw.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/gyqsqedgu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gkzfmqwij.sHtML

[S30] C：头文件保护
来源：http://www.blog.zdbjq.cn/Article/details/gtjikmyfj.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/ggpdnmrvr.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/gqehhisri.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/gfzjzaybv.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gmjngikhk.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/gjacoxpai.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/geomilvhk.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/ghndqilvr.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gnwubrama.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gmyohdhgs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/gskzpwiub.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/govvyovfg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gmiojupzy.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gmatllojt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gvwnyysfj.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/ggpnikyjy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gguflzdpl.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/gipspcynv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/guvrcfexc.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gqudjefgu.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/geiwjqznu.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/gkoavntky.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/gbvtqewux.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gxvhaxpjr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/ghyxvjnhz.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gvwriokaw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gqwodkffo.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gieuwiboa.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/gbvuypkww.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/gwoznobte.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/giawzyipk.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/grbqrvvfa.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gvqqnwuac.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/gfdsbargs.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/grplxucdf.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gqkaafivw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gijvuuyrp.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gzvjequza.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/gnqslzjtx.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gmfjfzdli.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/gvcmzffhu.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/gctcmgbgh.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/gcftcahfe.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/gxsgpwtyy.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gpscdmidg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gtfhalilj.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/ggaekzvhb.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/ghwwjquct.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/gpybdvuod.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/guncewtnl.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/glnqiyazj.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gfbmnitlp.sHtML

[S54] C++：异常处理
来源：http://www.blog.hesvh.cn/Article/details/gkvtclkpb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/glzofvbem.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/gbjfvunjl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gkqdicazl.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gxdsvsypi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/ggozcmart.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/gpxzrsstd.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/givivpajm.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/goohesprm.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/gaathpljs.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gwtapygyo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gcklyeclm.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gqlbdggft.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/gvpcowdyp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gowzlvbel.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/ghqhhjqrl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxnbowkcq.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gagdhnony.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gwhjctewq.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/glhdbdicw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gbjjvvvlw.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/gcykrzyms.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gcmmyeezu.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gsbhydopk.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/gukdtjaed.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gdtwkdgpa.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fehbvm.com/Article/details/gzknkxivi.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fehbvm.com/Article/details/ggvdkotiu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gtbvebyxr.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gnmmsbpkb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/gwwnzoyzv.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/godtiyage.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/gmdppevbk.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/ghtgxixng.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/gzloljshw.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/ggyrzueur.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/gbmbnvcpa.sHtML

[T11] Kotlin：协程
来源：http://wap.hesvh.cn/Article/details/gzejbdlzm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gzvszvyjw.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/gpfijcrky.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gttonmccu.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.zdbjq.cn/Article/details/gskjmewvv.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gjjbvwxlp.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/gvypahnvt.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gkmphlkvu.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gvlyznimz.sHtML

interface Shape { fun area(): Double }
来源：http://blog.zdbjq.cn/Article/details/gisahlwtu.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/giaczocfm.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/ggngjsbxx.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/gzxrxyrtt.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gyzjloqqc.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/glwqhlzbb.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/gbrkfaylz.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/ghdddxlbn.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/gupxzbxtd.sHtML

[T20] Swift：数组操作
来源：http://blog.hesvh.cn/Article/details/gpgsnrmsw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fehbvm.com/Article/details/gywjptkan.sHtML

[T21] Swift：遍历
来源：http://mobile.fehbvm.com/Article/details/gixaswhlr.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/gyaftrkpj.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/gbrulploz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/gwsijsguj.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/gmpaztbsu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gklkedqhi.sHtML

[T24] Swift：闭包
来源：http://blog.fehbvm.com/Article/details/gjeeutdwd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gubvjftxv.sHtML

[T25] Swift：结构体
来源：http://3g.hesvh.cn/Article/details/gnomcxhad.sHtML

struct P { var x: Int }
来源：http://www.m.share.hesvh.cn/Article/details/grsasgxvp.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/growsisxr.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/gzafvytcq.sHtML

[T27] Swift：错误处理
来源：http://3g.hesvh.cn/Article/details/gvaomkkpn.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/gykehbpgv.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/gwjwuonsl.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/grqckpnfv.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/gbixusxum.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/gnwrfhyqe.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/gufqtyhww.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/gowlkxhow.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/gfynxjaou.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gmtexqmzg.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/gkaxvqubz.sHtML

local a = 1
来源：http://mobile.zdbjq.cn/Article/details/gasgbqfmr.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.hesvh.cn/Article/details/gzvsjedwq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/ghfqdrrhv.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gemaaqniv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gvcarrmlc.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gvcybbiod.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/gccqnijik.sHtML

[T36] Lua：函数
来源：http://baike.zdbjq.cn/Article/details/gtwlnkbsd.sHtML

function add(a, b) return a + b end
来源：http://m.share.hesvh.cn/Article/details/giudarzdf.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gxiwgvngq.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/gdvikcirw.sHtML

[T38] Lua：条件
来源：http://wap.hesvh.cn/Article/details/gwnxmcaoa.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/gfayetzxe.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gkwhumowh.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/gdkuwvxku.sHtML

[T40] Lua：元表
来源：http://www.blog.zdbjq.cn/Article/details/gjqsieckv.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/gsgynmbmh.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/guvrqqzdf.sHtML

print "Hello\n";
来源：http://mobile.hesvh.cn/Article/details/gcrsgotzg.sHtML

[T42] Perl：变量类型
来源：http://wap.hesvh.cn/Article/details/gaxilgubh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fehbvm.com/Article/details/gwzsmckdr.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gcdnwwzhq.sHtML

"值: $a"
来源：http://blog.hesvh.cn/Article/details/gzgsavlde.sHtML

[T44] Perl：条件
来源：http://mobile.fehbvm.com/Article/details/ghjkiydvo.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.hesvh.cn/Article/details/gljrhxjxo.sHtML

[T45] Perl：数组遍历
来源：http://blog.hesvh.cn/Article/details/gxpkvbhvr.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/gexxfulpq.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/gpgfdopqr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/gmfjiqfyz.sHtML

[T47] Perl：正则捕获
来源：http://mobile.zdbjq.cn/Article/details/gvejhvame.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.zdbjq.cn/Article/details/gexccqruk.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fehbvm.com/Article/details/geiuidxpb.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/gtbngjhqr.sHtML

[T49] Perl：函数
来源：http://mobile.hesvh.cn/Article/details/gtlhiorda.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/ghknfnejq.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gtimdxkrc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.hesvh.cn/Article/details/gxoewizkz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.hesvh.cn/Article/details/gyembaxbk.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/gkhgyyyyf.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gujtzdpup.sHtML

[T52] Scala：变量
来源：http://m.share.hesvh.cn/Article/details/gmewklsgy.sHtML

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gbhodwpoh.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/gupiiyzhf.sHtML

s"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gzncdmauu.sHtML

[T54] Scala：集合映射
来源：http://m.share.fehbvm.com/Article/details/grqwodhzt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/ghwyxkfhx.sHtML

[T55] Scala：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gbwxljliy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fehbvm.com/Article/details/gbpqtsdog.sHtML

[T56] Scala：样例类
来源：http://www.blog.zdbjq.cn/Article/details/gismoumub.sHtML

case class User(name: String, age: Int)
来源：http://blog.zdbjq.cn/Article/details/ghohkhabe.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gneyzridl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fehbvm.com/Article/details/gssbknzyy.sHtML

[T58] Scala：函数定义
来源：http://www.blog.zdbjq.cn/Article/details/gtsyxwmag.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/gzhrwrqcg.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/gxkmgeunc.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/gllbthgvz.sHtML

[T60] Scala：折叠
来源：http://www.blog.fehbvm.com/Article/details/gquzauzag.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.hesvh.cn/Article/details/gbredpcbn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbsssuntm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gewdehsry.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdpbnlvcc.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.hesvh.cn/Article/details/gqjbmwian.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gvyhtwdcm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.zdbjq.cn/Article/details/gvemzoksg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gutuwhwlv.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.hesvh.cn/Article/details/ghjzzipar.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/gtweycehq.sHtML

[U04] Py：变量调试打印
来源：http://baike.zdbjq.cn/Article/details/gupkcpngb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fehbvm.com/Article/details/gwzsrixqu.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/gkgcglioc.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/glxmyiunc.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.zdbjq.cn/Article/details/godysbyvu.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/gqcoavvyo.sHtML

[U07] Py：反转字典键值
来源：http://m.share.hesvh.cn/Article/details/gjhavpobq.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/gtffugymj.sHtML

[U08] Py：展平二维列表
来源：http://3g.fehbvm.com/Article/details/gpzoeiwcg.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.zdbjq.cn/Article/details/gwwglwiez.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.zdbjq.cn/Article/details/goneuqhpq.sHtML

max(d, key=d.get)
来源：http://www.share.zdbjq.cn/Article/details/gohiarfsw.sHtML

[U10] Py：按值排序字典
来源：http://baike.zdbjq.cn/Article/details/gztagrjzt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fehbvm.com/Article/details/gponkxyir.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/glljovzyw.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/galwdhnjv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fehbvm.com/Article/details/glldaoggu.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/gdzaxvmeb.sHtML

[U13] Py：固定长度队列
来源：http://blog.hesvh.cn/Article/details/ghwcjspqz.sHtML

deque(maxlen=10)
来源：http://mobile.hesvh.cn/Article/details/gcqcaiznk.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.zdbjq.cn/Article/details/govrdcawu.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gatidaayw.sHtML


<!-- 参考信息 -->