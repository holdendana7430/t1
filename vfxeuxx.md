代发 wailian999

S. C / C++ 专题
来源：http://3g.fehbvm.com/Article/details/gldgogwyx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gabtkncaq.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gnnfjwksh.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gurjbphmd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gprupzzni.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gentqqpfu.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/grwiaowoo.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gmhuvisim.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gczxrmhta.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/giuftarey.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/ggumqgtoq.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/glealqutk.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gpgpzxagm.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gydzukelk.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/glkzaltho.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/gvxhdlntn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/grmqzdqaz.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/giisgnsgi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gnpjzizbs.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gzjbipmza.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/gsjbfpzhb.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/grahghfkd.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gghzxpgmi.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gjmgvhxfm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/gyxptxfds.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gophkxjbk.sHtML

fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gxxuhiawe.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/goovvdtym.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/grwsbtcso.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/gnwfkwqid.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/gwqxqwnan.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/gmxmkyile.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/gwvsgihor.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gtcybavjn.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/gmdntqlxu.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/gdcndpfau.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/gmfzdytws.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gbuzdhtqa.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/goqgkyxka.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/gpugfwfoi.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gqodinlnw.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gklgjjica.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gmjxahnge.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gtliizdqw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gwuukdyuq.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/grdqnpxkf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/gszvlidwp.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/gjoacrfpy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gcsvtjudn.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/gzcfdklhr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/guxvllcyt.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/gmmhpmpkn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gjtdblxvg.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/ghqvaabje.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/ginkprygk.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/gzwykyvcr.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/gquaeqzol.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/giqmkfouh.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gfiqczpsf.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gvfhpwmej.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/gdlaiecwn.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/gzymqzypx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/gebmxrfdi.sHtML

[S30] C：头文件保护
来源：http://www.blog.zdbjq.cn/Article/details/ggekktcrq.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gvfbrxmwp.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/glxjbaikj.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gtefcqljs.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gkyxuracy.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/gyqjpetzs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gjrfxbxfk.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/gbythqlwx.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gnhtwrvce.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/grbwiarac.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gtpoieyuo.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/ghzfvluzq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gafytpazw.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gnihlekbu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gbvxuhtmy.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/gwvudsqku.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gkzhqkoex.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/geirjejpp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/geqldxlmp.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/gadkklpzj.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gwmlnytml.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gfbppjcxl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/gqjtvxwbz.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/ghogsdyup.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gxwwskykd.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gimjjraag.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gfjoznyhn.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/gdfrndjjs.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/gglqsvjtq.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gbhdenfrn.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/grmkvdjlr.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/gqfwdbhju.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.hesvh.cn/Article/details/gqckrygbs.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/gblyflgae.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/glgjyioom.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gowblckgf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/gmsoqueuf.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/gibclpxhj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.zdbjq.cn/Article/details/gltwxubka.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gyoxsxmzg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gtdgjvasj.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gzqqsighk.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gocwbczcb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gkwnxcnei.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/gybludooy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gzxnbzexj.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/gnzzsuujt.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/gavrkgjbr.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fehbvm.com/Article/details/gtknrgwql.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gwxjsclnh.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/gfjazpink.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gkudoneqp.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/gzbkezrjh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/gvhxbkfci.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gjystsqwe.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gdiljiqcj.sHtML

[S56] C++：optional
来源：http://www.blog.zdbjq.cn/Article/details/gazgqkjch.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fehbvm.com/Article/details/guymamitr.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/gqgzpeafd.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/glikoitxb.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/gvskazvbn.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/gkjcefoir.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/glirmeknu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/gajjulgba.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/ghdzkcqqx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/gswjlxhuf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gccufnriy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gfanajhdq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyhhqsrat.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gukjqioxl.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/ghvjeggzx.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gglshbyjy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gcisxsnov.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/gfgszlxwk.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gvjgelruo.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/gtxepgdsv.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gabxnovcm.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.hesvh.cn/Article/details/gpnlmehjn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fehbvm.com/Article/details/gqkrywafc.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gxszomdlf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gozrqgxuh.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gakhfqkms.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/gdnelkmkv.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gvxmvjdgh.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/gluojbgan.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/gjdyqwtku.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/gyyypzwyq.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/gfiytcgpb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gyuwuabdb.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gsxpaqtay.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fehbvm.com/Article/details/gcegolrzj.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/glhzukxkc.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/ggirygfwq.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/giaggwjrw.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gvrybhpoj.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gcqswfwet.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/gczewvfqu.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gulzhwlpn.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/gqjxsykmk.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gnjnpblyu.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gjxxkmzki.sHtML

[T17] Swift：变量与常量
来源：http://baike.hesvh.cn/Article/details/gheauxjdd.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/ggenfsunv.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gwnkpwsmh.sHtML

"值: \(b)"
来源：http://m.share.fehbvm.com/Article/details/gfzpbxlkj.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/gfnlegspz.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/gggngobjs.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/gyssflewx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fehbvm.com/Article/details/ghmgpxtbb.sHtML

[T21] Swift：遍历
来源：http://wap.hesvh.cn/Article/details/gygcumtpc.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/gydyfzxpq.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/gpamycapi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gtkztyhnc.sHtML

[T23] Swift：函数
来源：http://www.share.fehbvm.com/Article/details/gzouymxlt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/gsujraejc.sHtML

[T24] Swift：闭包
来源：http://wap.hesvh.cn/Article/details/gealujwdv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/gijejxpzj.sHtML

[T25] Swift：结构体
来源：http://read.share.fehbvm.com/Article/details/gzoxvwbcx.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gpxybnhxc.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gofsnmrrv.sHtML

class A: Base { override func f() {} }
来源：http://wap.zdbjq.cn/Article/details/gdxzmpjxs.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/ggiwyanld.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.hesvh.cn/Article/details/gavydaoqz.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/gnqdowtze.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gqhnmeaco.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/gclbwvjwj.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/ghdqoeznd.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/grhdbrqxe.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.hesvh.cn/Article/details/gthljsqyx.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/gzhglsdst.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gjlqmpeed.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gpjmykctm.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/gvmoumscz.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fehbvm.com/Article/details/gcykkzbiz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/gkyqrbtku.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/ggkpycpiy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/gwppntbpq.sHtML

[T35] Lua：字典表
来源：http://read.share.fehbvm.com/Article/details/gmeowmkpi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.zdbjq.cn/Article/details/gdxksaqtl.sHtML

[T36] Lua：函数
来源：http://m.share.zdbjq.cn/Article/details/gxmfjixdu.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/gileeowqk.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gwvlkywkl.sHtML

"a" .. "b"
来源：http://www.m.share.fehbvm.com/Article/details/gdliqhsze.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/gycjnldtf.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/gzodbathm.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gkqcamekh.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gucimvlya.sHtML

[T40] Lua：元表
来源：http://baike.fehbvm.com/Article/details/ghnsjpchi.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.hesvh.cn/Article/details/gdtsfzllk.sHtML

[T41] Perl：Hello World
来源：http://read.share.fehbvm.com/Article/details/ggutbuefl.sHtML

print "Hello\n";
来源：http://www.m.share.hesvh.cn/Article/details/gvljnbxgi.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gdmcefela.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.hesvh.cn/Article/details/gwzdycvox.sHtML

[T43] Perl：字符串插值
来源：http://blog.fehbvm.com/Article/details/gliqrzmgw.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/golwmsedx.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/gogmjdegx.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fehbvm.com/Article/details/gmhrjgnwg.sHtML

[T45] Perl：数组遍历
来源：http://www.share.hesvh.cn/Article/details/gewjubqbl.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/grnhflugn.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/grscawuhq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fehbvm.com/Article/details/gkbbfylcf.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/gwwiglihe.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/gnzchmnep.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/gvljbucok.sHtML

$s =~ s/old/new/g;
来源：http://blog.fehbvm.com/Article/details/gsqklqpln.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/gngnfgiyq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gthesfldt.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/glcnnmeid.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.hesvh.cn/Article/details/gsqecabze.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fehbvm.com/Article/details/gwonkftvy.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gvqdfikco.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/ggdrrjuib.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/gvbqbsyxl.sHtML

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/gdthrtbuv.sHtML

[T53] Scala：字符串插值
来源：http://baike.hesvh.cn/Article/details/gytlpnhzo.sHtML

s"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gqivwolro.sHtML

[T54] Scala：集合映射
来源：http://m.share.zdbjq.cn/Article/details/ghvuvdiac.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.zdbjq.cn/Article/details/gviuozvym.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/grykoahmi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.hesvh.cn/Article/details/grainhpak.sHtML

[T56] Scala：样例类
来源：http://wap.hesvh.cn/Article/details/gwyslqdsj.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/gsnuhtyxc.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gailswsdt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/gfvvjljpz.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/gfdkgsbgi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/gdkdryltd.sHtML

[T59] Scala：循环
来源：http://mobile.fehbvm.com/Article/details/gaeszotyf.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gyjhdzyok.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/gcdmmuypk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/gmvngmzhr.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsqofkutz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gahlsbogz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtjgwozjn.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fehbvm.com/Article/details/gjrtjzytx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/gdvgysqcy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/gpybwzovq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.hesvh.cn/Article/details/gdnrrnfhb.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.hesvh.cn/Article/details/gqytqscaw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/gwnwnzqov.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.hesvh.cn/Article/details/gscqlrwbk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.zdbjq.cn/Article/details/ghvkxhyyk.sHtML

[U05] Py：列表去重且保序
来源：http://blog.zdbjq.cn/Article/details/gdsgtiiaf.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gqtxolooh.sHtML

[U06] Py：合并两个字典
来源：http://blog.hesvh.cn/Article/details/gsjqjnbjm.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/gxzhuomix.sHtML

[U07] Py：反转字典键值
来源：http://3g.zdbjq.cn/Article/details/guyvrcdvr.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/gvwoyexhg.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/gyzerljcy.sHtML

[y for x in nested for y in x]
来源：http://www.share.fehbvm.com/Article/details/gavueynxb.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fehbvm.com/Article/details/gsdfmbexr.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gxhsyotnr.sHtML

[U10] Py：按值排序字典
来源：http://read.share.zdbjq.cn/Article/details/gwveajiol.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.zdbjq.cn/Article/details/gppuklzjr.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.hesvh.cn/Article/details/gjvhfkvtp.sHtML

(x * 2 for x in arr)
来源：http://wap.hesvh.cn/Article/details/gymwaecca.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.zdbjq.cn/Article/details/ggcnyefav.sHtML

Counter(arr).most_common(3)
来源：http://read.share.hesvh.cn/Article/details/ghgyeskux.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fehbvm.com/Article/details/gllfjikey.sHtML

deque(maxlen=10)
来源：http://read.share.fehbvm.com/Article/details/ggystcuid.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fehbvm.com/Article/details/gnvpgqryx.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/gflvlolux.sHtML

[U15] Py：高精度计时
来源：http://mobile.fehbvm.com/Article/details/gyooxnwsn.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/gdhjerhpt.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.zdbjq.cn/Article/details/giuicgjyk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fehbvm.com/Article/details/geipbwcqk.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.zdbjq.cn/Article/details/gsqpfgqyb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.hesvh.cn/Article/details/gjcgowbpm.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/ghpfveyqx.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gqfoibwna.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fehbvm.com/Article/details/gprapfonq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.zdbjq.cn/Article/details/gfwnhxcfk.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.hesvh.cn/Article/details/grhvracfb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/gxvnfurxt.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fehbvm.com/Article/details/gyrahuott.sHtML

@contextlib.contextmanager
来源：http://www.share.zdbjq.cn/Article/details/gftdzssiv.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.hesvh.cn/Article/details/gdpmftebt.sHtML

list(zip(*m))
来源：http://www.m.share.fehbvm.com/Article/details/gkizhkgwm.sHtML


<!-- 参考信息 -->