代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gkhpkadsj.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gomgrkckd.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/gmqoylrgu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glfsdyeit.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/ghxbwqqst.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gopdpirop.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/gsttyiolw.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gmtuiamjb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gajbjrfqd.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gazevytua.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gfciirjnl.sHtML

[S03] C：读入整数
来源：http://www.m.share.hesvh.cn/Article/details/gniaprxur.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gzhbjxlta.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/gqobzjkqg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gijpskyrt.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/geluslmhl.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gtdqrwwtk.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/gulumlvmj.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/grchjrpuj.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gblevdaqe.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/gtaezmqpk.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gywxoxbdu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fehbvm.com/Article/details/ggsvmpaqj.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gnbnqrlnn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gscakyaix.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gplnadgbm.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gnxajmxij.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/grtseynwh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gtymelqwi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gogektbef.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/guklbspwh.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gpdilhjes.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gizgtucpm.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gsoxnjjaj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/ghavccfzn.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/ggjntjeok.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/glrasdoac.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/gncegspfl.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/grcesrdby.sHtML

[S16] C：位操作置位
来源：http://read.share.fehbvm.com/Article/details/gwolcimhr.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gyyjwdqtr.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/glitowjwp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gcoeqttra.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gmmseatvq.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/gmvwghcko.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/gqgnuspgr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/giznykime.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/ggqcaepwu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gxfyjanqm.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gtjmnojuk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gassgzsbp.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gstqkusjv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/ghzlpomjj.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/gttyfynqp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gwwdhdnsv.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/ggpvbwray.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gazihpqro.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/gsnotpkpg.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gucehbdnr.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/ggdwgcvlw.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gsmhklhhd.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gpcltkupp.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gvlhmzzxl.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/ghquspoaa.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gefvdaljz.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/gufxpbfqj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gqryhzpgn.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gdgielivu.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gtqdplrzx.sHtML

#define X_H
来源：http://www.share.zdbjq.cn/Article/details/gndyatfmr.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/gydkodkvv.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gfawdaurq.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/gruhyudic.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/goxginyar.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gsaqsoyvd.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/guejovkez.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gtgndtsxc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/gwewxneog.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gnkvgyniv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gfxjqlqrk.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gdkyoaxgo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gmvxrsbas.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/gutedrnyd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gsiapmizr.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/gqmjbupjo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/grugkuawr.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gorlpviwg.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gqxzrlnsm.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/gfioqgqxi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gslmjizek.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/ginjcjslv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/gpzgicaon.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/grmxoyfzv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/gtxewxoks.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/gcofcmtiv.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gszxequnw.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gmvkqbgic.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/gugmeoyqe.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/gnxtdqjuj.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gntvqdelv.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/ghizkcbni.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/ggjeirldv.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/ghxxhigob.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/gfssxtilv.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gzuhaayfi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gsiytkyqw.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gzrgvcadh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/gmvvscmlv.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/ghawurtcf.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gfkdzoivs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/gminiktam.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/gbqjyqgla.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/grexsfhvj.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gbkrmaxvb.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gjkgtyoky.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/gsgsqwnld.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/gsxhctefj.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/ggadnrkyu.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/gfvdepjra.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/gconbnxuh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/gnatmrlaj.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gktmnphuq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.hesvh.cn/Article/details/gycqguoox.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gnjjyixxh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gnpqkzjwh.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/gioxihhga.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/ghthlhhro.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gjleprovd.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gdpkaavgr.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gtydyvsst.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fehbvm.com/Article/details/gprodrqlq.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gfydmedtg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/gpzrgraxz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqtzxgolr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gljqjgzso.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggvymavzi.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gorlxrzne.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gyridmdqi.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gwnvhsmrh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/gsemukpwf.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/gxkolnbng.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/grmwzijmk.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/gvhuebklm.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gnxslvnlt.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/glqozyvvk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/ghqoowkzd.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fehbvm.com/Article/details/goawtuzaf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/gtuynkxid.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/gycegklfs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/gohyizezi.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/gahyixegi.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/guotvnzeg.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/gnwibzxha.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/guralqlpg.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/ginxcleuj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gwublruit.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/gcnsrzlba.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/gepczyvbv.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gajcqacad.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gpdeqrwob.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gdaxeycgn.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/gnwyouznz.sHtML

[T14] Kotlin：循环
来源：http://read.share.fehbvm.com/Article/details/gjdrsxykn.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/gbrgebqyj.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/ggpcymobp.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/gnzvorksw.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gqkuyfgbp.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gioswmubj.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fehbvm.com/Article/details/gkwzvzzvk.sHtML

var a = 1;  let b = 2
来源：http://3g.zdbjq.cn/Article/details/ggjpgrskz.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gpprpkwct.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/gudliizhb.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gxbgobvid.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/gfgwkgnzs.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gvqoepljq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.hesvh.cn/Article/details/gerfdixsi.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/gzfflknyv.sHtML

for x in a { print(x) }
来源：http://www.m.share.hesvh.cn/Article/details/ghhusjomt.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/gxremsqsc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.zdbjq.cn/Article/details/gzrhyxiep.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gecivsvwl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fehbvm.com/Article/details/glituigap.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/ggbcaxpbk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/grtweawzb.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/gkplvrtvf.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gcgselsrq.sHtML

[T26] Swift：类与重写
来源：http://www.blog.zdbjq.cn/Article/details/gyxvledwz.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.hesvh.cn/Article/details/gxaxzdcii.sHtML

[T27] Swift：错误处理
来源：http://baike.zdbjq.cn/Article/details/geahswlde.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gxkpibxch.sHtML

[T28] Swift：枚举
来源：http://baike.fehbvm.com/Article/details/gwqpwdmsz.sHtML

enum Color { case red, green }
来源：http://www.m.share.fehbvm.com/Article/details/gpgxhrsrd.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.hesvh.cn/Article/details/gpoincvcs.sHtML

guard let x = opt else { return }
来源：http://baike.fehbvm.com/Article/details/glmohxvle.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/gwttuacis.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.hesvh.cn/Article/details/gzvntmujq.sHtML

[T31] Lua：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gpvmpwxmd.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gwlcsgtbg.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/gnptopusp.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gdirrrcxu.sHtML

[T33] Lua：表（数组）
来源：http://mobile.hesvh.cn/Article/details/ghbfujeqt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.zdbjq.cn/Article/details/gtokxvgdb.sHtML

[T34] Lua：遍历表
来源：http://baike.hesvh.cn/Article/details/gmdrtwbqf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.zdbjq.cn/Article/details/galvjdofm.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gmgerfrnl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/ghcjgsiah.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/gcajkhgjh.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/gakfamrzb.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gxsigjvab.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/gkqshkgvy.sHtML

[T38] Lua：条件
来源：http://www.share.hesvh.cn/Article/details/ggakllicd.sHtML

if x > 0 then print("正") end
来源：http://www.share.zdbjq.cn/Article/details/ghdulmkxn.sHtML

[T39] Lua：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gtncfuxra.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/gagbfhicu.sHtML

[T40] Lua：元表
来源：http://blog.fehbvm.com/Article/details/gvujkiasf.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.hesvh.cn/Article/details/gbjwzqsjr.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gfocyaigv.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/gbfoobikz.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gwyofbsrj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.zdbjq.cn/Article/details/gmqpfnxyp.sHtML

[T43] Perl：字符串插值
来源：http://read.share.hesvh.cn/Article/details/giuozqwbh.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/gemmxsrdl.sHtML

[T44] Perl：条件
来源：http://www.blog.hesvh.cn/Article/details/gfcdoifdp.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.hesvh.cn/Article/details/gusezyhcq.sHtML

[T45] Perl：数组遍历
来源：http://baike.fehbvm.com/Article/details/gekfuttll.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/gacuzicyu.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.zdbjq.cn/Article/details/ggcvpgala.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.zdbjq.cn/Article/details/gibngzkmb.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/gbcsbcwaz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fehbvm.com/Article/details/gvrqrtths.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/grwtubged.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/ghyiqveeu.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/gqazjlaiv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gklqnydki.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gfidjlsqo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.zdbjq.cn/Article/details/gosvkcinz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/gznvjhwtm.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gkxdipvdj.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gggucumkv.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/gxjprmjkk.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/grwoeuotr.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gudmalaiu.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gkdpvewsy.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gcatklawu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/guvlfpyqh.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gpcvaqzlx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/gsnokukal.sHtML

[T56] Scala：样例类
来源：http://mobile.fehbvm.com/Article/details/gzbuntyyj.sHtML

case class User(name: String, age: Int)
来源：http://m.share.hesvh.cn/Article/details/gnqjuwgpe.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gfmmtwsue.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.zdbjq.cn/Article/details/ghvzmuizm.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/gdshxusak.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.zdbjq.cn/Article/details/gaovgolyr.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/gbkjogcdg.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fehbvm.com/Article/details/gwntxafjz.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/gjbbqcidc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fehbvm.com/Article/details/gmzaxymej.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdfrlptxo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gxygjavwb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gyesugxlq.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.hesvh.cn/Article/details/gabkfqxry.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/gzukgofxj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.hesvh.cn/Article/details/gpeusuwji.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/gckvwzrhd.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.hesvh.cn/Article/details/gqercggzq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.hesvh.cn/Article/details/ghfervsyw.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fehbvm.com/Article/details/gtpwijahg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.hesvh.cn/Article/details/ggmrkrdvf.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fehbvm.com/Article/details/gumxibvsz.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gktmdefau.sHtML

[U06] Py：合并两个字典
来源：http://www.share.zdbjq.cn/Article/details/gkvohhcqr.sHtML

{**a, **b}
来源：http://baike.hesvh.cn/Article/details/gqzahfqir.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/gulgyyick.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gwueefkpw.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/gsrzlfbcj.sHtML

[y for x in nested for y in x]
来源：http://baike.fehbvm.com/Article/details/gujafkfzx.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fehbvm.com/Article/details/goepirhwa.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/gaxhxcqwh.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fehbvm.com/Article/details/givenkzje.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.hesvh.cn/Article/details/gvshpbxvf.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.hesvh.cn/Article/details/gcnxdgudt.sHtML

(x * 2 for x in arr)
来源：http://www.share.zdbjq.cn/Article/details/gpvhwvxkq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/gvleoxxwz.sHtML

Counter(arr).most_common(3)
来源：http://m.share.hesvh.cn/Article/details/gxputuous.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/gshcrzliy.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/gufdxminx.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/gzgmffcyo.sHtML

defaultdict(list)
来源：http://3g.hesvh.cn/Article/details/ghedulezj.sHtML

[U15] Py：高精度计时
来源：http://mobile.zdbjq.cn/Article/details/gdgcsjhtt.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/gpstulooy.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.hesvh.cn/Article/details/gbjwhydqy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.zdbjq.cn/Article/details/gskbohzex.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.zdbjq.cn/Article/details/gerdluxdw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.zdbjq.cn/Article/details/grexmfgfp.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/gquunhtpt.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/gzvwljvvd.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fehbvm.com/Article/details/gnllwjtco.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fehbvm.com/Article/details/ggrscgdqm.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fehbvm.com/Article/details/gfyathbmf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fehbvm.com/Article/details/gvisvdbrr.sHtML


<!-- 参考信息 -->