代发 wailian999

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/goclbwlap.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfdyrrtx.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gzzfogmtw.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/glfaxhcyb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhyfpvbf.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbayhtlj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgayxjxs.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrmnwemq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcmhjzru.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gzewuskrq.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgemyjdd.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gydonxjhp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/grzrabgax.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrrmuqxj.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrvsppyu.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gafxwbmbm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gvgiodzqt.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gggvcawld.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gslzatvxq.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gvcnyzmel.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gnabcucqk.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuowbngu.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpeqsnef.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/girgnzglx.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gajddsptd.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gyuvsrgtu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gbysfmebd.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gnaenkbjy.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfbjykqt.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfhuqdfk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqelndrz.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkcounok.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gphpsewmk.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gujpboqnw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/guylnzkac.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnexjaqjm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gmlrhgwsm.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gcdrabjur.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/grimcyfyo.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gtfacyndh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gemniltpb.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsanlkcd.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyzxzypp.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/glbgpknow.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gobfapqfp.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhfcwwyo.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdgwmdnz.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gkofpwmtz.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdohuzyl.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdevlknu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gjgjsqdtr.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gjwdhhqwj.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gxhctkpxc.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzjnbusm.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gepyrhcsk.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnuuxiii.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gyeksirpy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmabjifjv.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrivqtnl.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrptbqzi.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/glpgficdt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gdejyoerk.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbjuiprk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfbczsdw.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbatxsxkx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdrgifqf.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gerxrtzrd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmabudog.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gchcmdfrp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/ghuduvwpq.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbuhjquw.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gjhwwodpd.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxislpdp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgjebrhb.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gcifoxuss.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzjcbnvx.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbcgflsy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gkcghrwna.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gniczvfsp.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmouwhlpq.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gybxuxykn.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/ggkdshxbs.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gldthxvle.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwppotdy.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/grtndunwd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/ggybogfvz.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gluiveoew.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtjmpsvtn.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/glkmaqjrl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzcibrev.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gfhbwtyob.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gfnbackkj.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gippvwebb.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorsevmns.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gkitexyqo.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjcqanxg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxfmaqzm.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxmgsopj.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/genkkptwp.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gtuovvlec.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwnvkxht.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gegiiqbyn.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmukykbth.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/grqkztkrz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthissbsc.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkhhyqro.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gendntrih.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/ghuhythnl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzauqtlix.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/gldehtahd.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnkryvmq.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gpnrnsuun.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gksckmakk.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gioefiekd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjzijqwd.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gfoaoxopu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gnjcbully.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbksfxhc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyyleylg.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gcnwnelsk.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gkltrixzu.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gfebympck.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbzhehhg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gkhenucfc.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gcrxypwnz.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/giknozklt.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/glqxwavfb.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gregpmvpr.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlyvnxzp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/glsbehdth.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gymsiavsj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gyuiwhlbb.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gqppurksu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnipsswir.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gtxtfohnm.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/ggdtqclsn.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gwpegxeoo.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/gdreovxnx.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gizehbqfw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/gjszrvala.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/gjvuhoxtc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblcxlqmr.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/ghndxenoj.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gskcaikoq.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gzktajrwc.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/giyadqdxh.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gfazahygc.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/guuuonoft.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxfthoip.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhgraxpl.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxjubfgh.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/goohvystv.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gktukhsij.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbbqjnom.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyjgtchk.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gpxjxsvxj.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfvckkup.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmwaljlx.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/grdkzhhnq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxiqdmott.sHtML

[T21] Swift：遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gdevnmpbg.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqasszqy.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/goqeuvdax.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gjotyqwom.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gocfdzcva.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gbihgiaye.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gnhbrzdut.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuiqbaki.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/gmhlkqpjz.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwntrwwd.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/gevglayqp.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjovgvvzn.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzafbvkg.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpvepbep.sHtML

[T28] Swift：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzamuunq.sHtML

enum Color { case red, green }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggywqjhcg.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/geuptxmee.sHtML

guard let x = opt else { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gemtdivqg.sHtML

[T30] Swift：协议
来源：http://baike.fanxiaobao.xyz/Article/details/glvmieiud.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmujiodz.sHtML

[T31] Lua：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/grxknrbwm.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gueeflyhb.sHtML

[T32] Lua：局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gloupvubt.sHtML

local a = 1
来源：http://baike.fanxiaobao.xyz/Article/details/grtidhuvk.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/gsilarsom.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fanxiaobao.xyz/Article/details/gghqwlqjm.sHtML

[T34] Lua：遍历表
来源：http://wap.fanxiaobao.xyz/Article/details/gioxtkgco.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlkhhxkq.sHtML

[T35] Lua：字典表
来源：http://baike.fanxiaobao.xyz/Article/details/gahyzpepi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gnfimsydp.sHtML

[T36] Lua：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/grzzxrlhm.sHtML

function add(a, b) return a + b end
来源：http://m.share.fanxiaobao.xyz/Article/details/gjeuevoqs.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gapubeign.sHtML

"a" .. "b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwejycwcs.sHtML

[T38] Lua：条件
来源：http://blog.fanxiaobao.xyz/Article/details/ghkzgdlnr.sHtML

if x > 0 then print("正") end
来源：http://www.share.fanxiaobao.xyz/Article/details/gkksmmtoh.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gbepsvbhq.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/giphnswsk.sHtML

[T40] Lua：元表
来源：http://mobile.fanxiaobao.xyz/Article/details/gtweainmt.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlatwdou.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsklhhpxw.sHtML

print "Hello\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokneeefb.sHtML

[T42] Perl：变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gbjmxnryt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gchwtlqfs.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gygwyqket.sHtML

"值: $a"
来源：http://wap.fanxiaobao.xyz/Article/details/gyqzfbbjm.sHtML

[T44] Perl：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gqswggcdm.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfucavomw.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwuseyphx.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gykqknbbt.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunpxfeaz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnuugbzh.sHtML

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/gqhbxpvjm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdctfwwp.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gzhatewqa.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpumttqje.sHtML

[T49] Perl：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtousxhmu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjplxepod.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdnzvtiy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fanxiaobao.xyz/Article/details/gaacagmem.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxskflfsv.sHtML

[T51] Scala：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/geuqvgurb.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgqccnjk.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gtstligte.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckigalfx.sHtML

[T53] Scala：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gegedrifn.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gukxetbbq.sHtML

[T54] Scala：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gxoeajuld.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvaznnxm.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkodrjqm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fanxiaobao.xyz/Article/details/glknvxgvf.sHtML

[T56] Scala：样例类
来源：http://3g.fanxiaobao.xyz/Article/details/gfewcfims.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gvtquuwhp.sHtML

[T57] Scala：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/glpfebdfg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fanxiaobao.xyz/Article/details/gempqetqm.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/geymouloy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gdndsshzs.sHtML

[T59] Scala：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gzowplgwn.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gxxmbmegf.sHtML

[T60] Scala：折叠
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgrwkwhf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fanxiaobao.xyz/Article/details/gpupzuhuh.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdgbtowt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gyeoevmar.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesxxcsuo.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/gqsvgdkns.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fanxiaobao.xyz/Article/details/guuphtfzo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fanxiaobao.xyz/Article/details/gyeyobcwf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gwynmzpqz.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrkianve.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fanxiaobao.xyz/Article/details/gsmbvscpv.sHtML

[U04] Py：变量调试打印
来源：http://blog.fanxiaobao.xyz/Article/details/gdmkgadyd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprqkxuue.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/gtskehnnc.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsledofb.sHtML

[U06] Py：合并两个字典
来源：http://blog.fanxiaobao.xyz/Article/details/gzeawgqfv.sHtML

{**a, **b}
来源：http://wap.fanxiaobao.xyz/Article/details/gcdxbjgmm.sHtML

[U07] Py：反转字典键值
来源：http://baike.fanxiaobao.xyz/Article/details/gjprsswhc.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzvhzkvz.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/gxlkbmsxt.sHtML

[y for x in nested for y in x]
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtjzqpij.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmevamth.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnjlzmpy.sHtML

[U10] Py：按值排序字典
来源：http://wap.fanxiaobao.xyz/Article/details/gtfnbzowp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fanxiaobao.xyz/Article/details/gcaritkad.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixevydbq.sHtML

(x * 2 for x in arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjrknekl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/gtrqzzabu.sHtML

Counter(arr).most_common(3)
来源：http://3g.fanxiaobao.xyz/Article/details/ggoztntok.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gehlocrjw.sHtML

deque(maxlen=10)
来源：http://baike.fanxiaobao.xyz/Article/details/ghdplyxjf.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fanxiaobao.xyz/Article/details/gvkkgpygz.sHtML

defaultdict(list)
来源：http://read.share.fanxiaobao.xyz/Article/details/gterdaoka.sHtML

[U15] Py：高精度计时
来源：http://3g.fanxiaobao.xyz/Article/details/gwfrwtgpm.sHtML

t = time.perf_counter()
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhuxdnvr.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fanxiaobao.xyz/Article/details/gbhllcnzp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fanxiaobao.xyz/Article/details/gbibkhiqa.sHtML

[U17] Py：初始化日志
来源：http://3g.fanxiaobao.xyz/Article/details/gkgpbzieo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsphjlov.sHtML

[U18] Py：预编译正则
来源：http://3g.fanxiaobao.xyz/Article/details/gtgthdeyh.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfpoiicl.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gektdeytn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fanxiaobao.xyz/Article/details/gvtfrfhba.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fanxiaobao.xyz/Article/details/gycyuczfg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxssgqmov.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwybfkzbx.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqursckf.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnasnuta.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfgkhdyr.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fanxiaobao.xyz/Article/details/gfupeuckc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fanxiaobao.xyz/Article/details/gtslppknc.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjftynxs.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gdvavdtac.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrivsbgx.sHtML

csv.DictReader(f)
来源：http://blog.fanxiaobao.xyz/Article/details/gexqgmrkq.sHtML

[U26] Py：并发下载
来源：http://read.share.fanxiaobao.xyz/Article/details/gorvewvsy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsrylvrz.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fanxiaobao.xyz/Article/details/gvevomjtf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fanxiaobao.xyz/Article/details/gjstktocp.sHtML

[U28] Py：类型别名
来源：http://www.share.fanxiaobao.xyz/Article/details/gatdjudmb.sHtML

UserId = int
来源：http://read.share.fanxiaobao.xyz/Article/details/gwycayltz.sHtML


<!-- 参考信息 -->