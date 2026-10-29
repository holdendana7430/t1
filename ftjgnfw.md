代发 wailian999

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gkshybidp.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/grtebesza.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gfgoodjmh.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/gtymdjbdn.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/gjsaqawxc.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/grjocsfhu.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/gfckyisrh.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/ggdvlxvsi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/gjpvgtbkw.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gktkepflb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/gphcpmtnl.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/glebtbmaz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gievuwdkd.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/gfrbazhwx.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/glnhgfhkb.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gmccxhwds.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gwnrubdyz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/gkyuvhuoo.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gqgpfdvay.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/giprncjyw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gvtxtkeau.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/ghcybgnyy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.zdbjq.cn/Article/details/glxmvjkux.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gafdvcphc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/gejcsbgbx.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/guyfacyml.sHtML

(double) a / b
来源：http://www.blog.zdbjq.cn/Article/details/gkqfjspwy.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gpupcdlin.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gdndntrqa.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gfyokacvl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fehbvm.com/Article/details/gufufwveh.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gnaqnogdr.sHtML

int main(int argc, char **argv)
来源：http://blog.hesvh.cn/Article/details/gwilfgunv.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gzhhutdgt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gxpehzdis.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gwuyhlxzg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gtwndxejc.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gkpscmfqi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.hesvh.cn/Article/details/gzpdnhfhd.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/ghboszfvd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/gbepoqvjw.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/glogimozd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/gdlcvywmx.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gfyvanbuv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/gunpuyvjc.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/gcpddiexe.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gfaxlwiyu.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gcksilses.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/gswtjvxop.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/gsywpokdq.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gvxtugcpa.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/giwcrlkga.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gcwgrwvem.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/ghkkohtic.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fehbvm.com/Article/details/gqldmeedz.sHtML

[S30] C：头文件保护
来源：http://www.blog.zdbjq.cn/Article/details/gaannbdwa.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/giqkafsdk.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gmrzxeymw.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gjeengbls.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/ggaanttmp.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gueecfbts.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gytshpupj.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gmmsrfpjy.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/glegatnjf.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/gowbtzgsk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/glfkjbjkb.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gvalwdezr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gvpqmqnyw.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gtgsyyalu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gpcqfdtsq.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/gobcspanm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gvdtalkct.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gjszssgil.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/gyduurwsp.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gsfbbglhi.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gpbtqnpek.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.zdbjq.cn/Article/details/gibmdeqes.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/gtqpikrqh.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gnuryopte.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gmgsnvtpk.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/gmkvaoveg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gkorkrhkm.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/gxtjwussv.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/gxkxfcfjt.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gpzpkwvde.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/ghqitqjqe.sHtML

[S44] C++：引用传参
来源：http://wap.fehbvm.com/Article/details/glpkmyinf.sHtML

void inc(int &x) { ++x; }
来源：http://wap.zdbjq.cn/Article/details/gfzfbvdpy.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gplwhfvig.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/gyhacwshr.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gylrwwhhc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/gfwcpzbck.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gfqwtevsl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/grrkzqshh.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/ghswoxfay.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gonifiwkn.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/glqltmrmj.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/gqgbyrila.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gkzxwowse.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gnarsdawq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gsprxlfxq.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/gjrlwycdv.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/gisdpqnwt.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gkwjzhgqt.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/gfcziclsc.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/glkmkqejt.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/gzqiufwzw.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/gkepzolqv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/glukdagmh.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gealurhsn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gumholflt.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/gqlmgtqsf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/gcwigmcmm.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gaezaveqv.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/ggycyfysd.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/ggcxclrzm.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gcnjohjwd.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/gqaknmjaj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gazxwampu.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/ghnuwqinm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/glgwnzmxy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggqvdsara.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gmqmwykpy.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdkspfeld.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/gpirzbnyu.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gnlmqynmd.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/ggilyhkyh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gjwexupim.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gezgfxenz.sHtML

"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gwnpwxrbw.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gdofpwiuo.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/ghzhccvwh.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gqcwhuixx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gsjkgpeel.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/gudnbunei.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/geqmhkrty.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.hesvh.cn/Article/details/goxirfssl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/guzpznoxm.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gfezevciz.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/gqzelgntj.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/gfjhxjrtx.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/gulurldih.sHtML

[T10] Kotlin：默认参数
来源：http://3g.zdbjq.cn/Article/details/gubjasmnm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gvhrszhmg.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/gxhremmsl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/gnajcwhkq.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/gutlvzxlb.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/giyeqsbbm.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fehbvm.com/Article/details/gxytmxuig.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/gsyoaysde.sHtML

[T14] Kotlin：循环
来源：http://blog.hesvh.cn/Article/details/gbfttrbdh.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/ggvenyxjr.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/ghdonzhcs.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/gfexedzpe.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/geulrksyf.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gynwvnuyk.sHtML

[T17] Swift：变量与常量
来源：http://blog.fehbvm.com/Article/details/gtjommqpa.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gaovjlcij.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gmdpegayd.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/gmrrncvbq.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fehbvm.com/Article/details/gnxzlhtyx.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gjrrloajb.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/gukclpevt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/gcezhmvwx.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/gyficbspe.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/gvpyxplci.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gglpxrxpf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.zdbjq.cn/Article/details/glsuhutkn.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/goozreqlx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.hesvh.cn/Article/details/gojifarrg.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/geutvfhcf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/gvpiqubcx.sHtML

[T25] Swift：结构体
来源：http://blog.fehbvm.com/Article/details/gzulvapox.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/gspzsuzia.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gpppsnndo.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/gsutxcear.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/gojdeoqbe.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/gzbdsinsv.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/geayqmenz.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/gerzmlkpr.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.hesvh.cn/Article/details/gpnalvary.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/gzcuvsrag.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/grhzibiek.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/gzpdoxfch.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/gngfjorcv.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/getyiywtp.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/geyjfmsjm.sHtML

local a = 1
来源：http://www.share.fehbvm.com/Article/details/gatsljjyn.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.hesvh.cn/Article/details/ggfukuucw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fehbvm.com/Article/details/gxfqafjct.sHtML

[T34] Lua：遍历表
来源：http://mobile.fehbvm.com/Article/details/gqhcwrqkt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/ggzrjjhje.sHtML

[T35] Lua：字典表
来源：http://m.share.hesvh.cn/Article/details/gkkromngb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gqgezkscz.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/gqrrnwtwy.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/gjktailhu.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/ghuplzxyw.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gyqcqidfc.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/geuilsfnt.sHtML

if x > 0 then print("正") end
来源：http://www.share.fehbvm.com/Article/details/gdugazkmk.sHtML

[T39] Lua：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gipzkhqle.sHtML

string.find(s, "%d+")
来源：http://3g.zdbjq.cn/Article/details/gwtkmufnp.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/gjtclhcmz.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/gdhpaalbj.sHtML

[T41] Perl：Hello World
来源：http://www.share.hesvh.cn/Article/details/gmzjugdku.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/glenmmkzs.sHtML

[T42] Perl：变量类型
来源：http://m.share.fehbvm.com/Article/details/gumvlrilg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fehbvm.com/Article/details/gfacnamky.sHtML

[T43] Perl：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gnddrzwko.sHtML

"值: $a"
来源：http://www.share.zdbjq.cn/Article/details/gtcuamkyb.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/gnoqmgyrw.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.zdbjq.cn/Article/details/gdvtcpbgc.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/gsheamlkb.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/gryhmcbap.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/gjqtszmvq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.hesvh.cn/Article/details/gvwmnhogi.sHtML

[T47] Perl：正则捕获
来源：http://baike.zdbjq.cn/Article/details/gmonhzsmf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fehbvm.com/Article/details/gyjlsmnmj.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.hesvh.cn/Article/details/gihjoljij.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fehbvm.com/Article/details/ghgtdpucp.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/gsmyamzfv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gtkdrdlze.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/grgwslfpv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/gssczzkrk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/gnbqfxrbw.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gzfirqdpg.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gzwqxqwum.sHtML

[T52] Scala：变量
来源：http://www.share.hesvh.cn/Article/details/gqizueuvn.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/giujyiqqx.sHtML

[T53] Scala：字符串插值
来源：http://3g.hesvh.cn/Article/details/gaogigefg.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gztapahwf.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gpijiizyo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gewwkywiu.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/gotmaluxy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/gvcwaiffl.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/gladuktvq.sHtML

case class User(name: String, age: Int)
来源：http://baike.hesvh.cn/Article/details/gcytieyhx.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/ggldqlxiy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fehbvm.com/Article/details/gnpwnuvpv.sHtML

[T58] Scala：函数定义
来源：http://3g.zdbjq.cn/Article/details/gfmfizgtn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.zdbjq.cn/Article/details/ghqafmdnx.sHtML

[T59] Scala：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gxjwlvzrb.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gnoyayjaz.sHtML

[T60] Scala：折叠
来源：http://m.share.zdbjq.cn/Article/details/gsvskjaio.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.zdbjq.cn/Article/details/giiafiunz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbyzeylnf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gtluusrbc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkrlmapxy.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.hesvh.cn/Article/details/glpynasby.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.zdbjq.cn/Article/details/grcuvfibg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fehbvm.com/Article/details/gsnnjxdcz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.zdbjq.cn/Article/details/gmgpuqqwa.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fehbvm.com/Article/details/gudjogjta.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fehbvm.com/Article/details/glrlsiyoi.sHtML

[U04] Py：变量调试打印
来源：http://wap.hesvh.cn/Article/details/ghyidqnwd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/gawffyapa.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fehbvm.com/Article/details/gozetgamk.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gpceogiol.sHtML

[U06] Py：合并两个字典
来源：http://blog.hesvh.cn/Article/details/gfmdwritu.sHtML

{**a, **b}
来源：http://blog.fehbvm.com/Article/details/goynptayu.sHtML

[U07] Py：反转字典键值
来源：http://www.share.zdbjq.cn/Article/details/gzulykrxq.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fehbvm.com/Article/details/gundpujcn.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/gtskfqlao.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/glcogmeaj.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.hesvh.cn/Article/details/gtcjqromw.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/gibbcjgjt.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fehbvm.com/Article/details/guwsskvpy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/gphzldzdz.sHtML

[U11] Py：生成器表达式
来源：http://www.share.zdbjq.cn/Article/details/gsumxvloq.sHtML

(x * 2 for x in arr)
来源：http://www.share.zdbjq.cn/Article/details/gmqhsukjj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.zdbjq.cn/Article/details/gkumtcvvo.sHtML

Counter(arr).most_common(3)
来源：http://blog.fehbvm.com/Article/details/gxohrwmay.sHtML

[U13] Py：固定长度队列
来源：http://mobile.hesvh.cn/Article/details/gofsvdcwa.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/ggchokhzq.sHtML

[U14] Py：分组收集到列表
来源：http://blog.hesvh.cn/Article/details/gxkeogkei.sHtML

defaultdict(list)
来源：http://3g.hesvh.cn/Article/details/gcrrvkibw.sHtML

[U15] Py：高精度计时
来源：http://wap.hesvh.cn/Article/details/gcbyxhdky.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gtgayffxt.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fehbvm.com/Article/details/geipftglh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.hesvh.cn/Article/details/gaqfzamyr.sHtML

[U17] Py：初始化日志
来源：http://read.share.hesvh.cn/Article/details/gcrdxiqek.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.hesvh.cn/Article/details/gdvaqaore.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fehbvm.com/Article/details/gtjijwauf.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fehbvm.com/Article/details/gkfafkpwy.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fehbvm.com/Article/details/gpjvhcjyt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fehbvm.com/Article/details/gyfdnxcic.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.hesvh.cn/Article/details/gjjplyhrt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fehbvm.com/Article/details/gbbqidirw.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.zdbjq.cn/Article/details/gxectricb.sHtML

@contextlib.contextmanager
来源：http://www.blog.hesvh.cn/Article/details/ghlpszvmz.sHtML

[U22] Py：矩阵转置
来源：http://baike.zdbjq.cn/Article/details/ggnkwxrwv.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/gbjlofhzh.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fehbvm.com/Article/details/ghjxunzgk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fehbvm.com/Article/details/gdrevcdlf.sHtML

[U24] Py：路径操作
来源：http://3g.zdbjq.cn/Article/details/gsolggwbs.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gvhkonjpn.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.zdbjq.cn/Article/details/gtijqldvf.sHtML

csv.DictReader(f)
来源：http://read.share.hesvh.cn/Article/details/gdciayptl.sHtML

[U26] Py：并发下载
来源：http://m.share.zdbjq.cn/Article/details/gmmehoaxs.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/ghpyenhog.sHtML


<!-- 参考信息 -->