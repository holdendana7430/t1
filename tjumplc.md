代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/gttwqhepn.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gnhkxvslq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/gomeyoums.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/gywhsidan.sHtML

int x; scanf("%d", &x);
来源：http://baike.fehbvm.com/Article/details/gljdkchwg.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/guahbllrl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/grwllicjk.sHtML

[S05] C：字符串长度
来源：http://read.share.fehbvm.com/Article/details/gfeavtucg.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gdmjribon.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/goyvcrbfu.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/ginctqret.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/gbmiwyske.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/ggnijbxxm.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/gxhlkmkaf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gpvseobrs.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gjzqlawgu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gzlrwktcz.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gwljhtcba.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gupkiktel.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/ghnjddfmq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gvnpmpkpe.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gavfkjyqn.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/gclobuvah.sHtML

[S12] C：写文件
来源：http://blog.hesvh.cn/Article/details/gwfmwmmtj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/goqwducde.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/gwivrrmgn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gqxliqyzi.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gxbwtpnhx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gztcmrleb.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/gbzeoaoga.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gtqpxbibq.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/guwfpgqsq.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/gbsdocswg.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gnomukmbp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.zdbjq.cn/Article/details/gmazcacaz.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gbbksbzqx.sHtML

int main(int argc, char **argv)
来源：http://read.share.fehbvm.com/Article/details/gikiecxuh.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/gpkrmfirx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/ghchlskqe.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/gujgppmrv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gpoghxwuf.sHtML

[S21] C：字符类别判断
来源：http://www.blog.hesvh.cn/Article/details/gwlybwahw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/gcxgrmtrw.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/gmxkwcpcy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/gzcgteruo.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/ggdixouxb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gllnicltx.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gtckflmwj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/gnihugrwz.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/glvkxffxc.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/gzfgrflab.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gyyamemge.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/gdwzxybyb.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gmmlopujh.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gaewkofwi.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/gnyvdlqvp.sHtML

static int counter = 0;
来源：http://read.share.fehbvm.com/Article/details/gejllumby.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/ghyqaognd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gzkvkujav.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/galcarlrx.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/gqyaebrtp.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gjuagrgxu.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gpferrhfn.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/gmsfnxyjr.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/ghovpcvzk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gtprfhnow.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gzilokbcx.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/glfrpylfb.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/gyhkblegg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/gcjjcgrvg.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gfluedjrz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/gpgsihquk.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/glvxjqgkg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gbppkgggf.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/gbmonwxui.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gzxjvwgcj.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/gwbncmgqv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/gnndswkwk.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gbhqbddbb.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/gemjixfaz.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/ggrylkzus.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/gntlfkwos.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gvgzieleh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/gtylrbzre.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/gfdgdygvu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/ghtkgupro.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/gvynifuqj.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/ggtdyfoik.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gzkjmtjbk.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/gygudexts.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gxmmgfxmv.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gwzvonrnx.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/gwramcvjw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gzjthogdv.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gesuwkebj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gyylloctt.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gpmobunjh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/glwkptodn.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gwxxzrenh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gnefnmelt.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/goxoykcxz.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gnwzqntis.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.hesvh.cn/Article/details/gfypmebvf.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/glempzrwx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gceiekrrx.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gylwkyofz.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/gxktttdfl.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gwcdshbbe.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/giyuzzvwt.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/gqjptqhgh.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gsdqlobug.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gzwvmnbeu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gzusgmcko.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gnjmaqgzm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gekejyxsr.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gwnaifoto.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gwbcwwhqx.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/gskziycxt.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gkmecgbub.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gsrovyjgb.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gexpkrlcl.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/gherdtxfk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gywpfdlrk.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gwhsjmqbk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gvyiekzzt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbrrqtlok.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gjkyibcjh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjitajkms.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/gbotuwqdn.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gkwfwnjoo.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/gpdljrphb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/guvmgrenu.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/gfqtihsfd.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gpnyjnayi.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gsugfjead.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gwnxppfdn.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.hesvh.cn/Article/details/gveanzjqv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gqrvelzwq.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/ghuyulibp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/geljxjvoq.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/geftipmxr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/gbmmgbgjf.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/gjbipczfb.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/gtgcipjpn.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/gglzlnkht.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gnryyhizq.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/gocajpdbj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/gnlleshdw.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/gkwkkklei.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.hesvh.cn/Article/details/gerfkzfki.sHtML

[T12] Kotlin：解构声明
来源：http://3g.zdbjq.cn/Article/details/gsesnnvsp.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/ghlfwrdyw.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.hesvh.cn/Article/details/gpygqwgag.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/grqjlqpub.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/gqdfdkkja.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gwvdqvgmf.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/guofbxzpz.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/gfdzrqfig.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gpoaiprgw.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gymyfycjv.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/gnnrcqywa.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gzqirkpxx.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gtfpfslji.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/gvolkgnei.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/gljzcdsoe.sHtML

if let n = opt { print(n) }
来源：http://3g.fehbvm.com/Article/details/grpubywyx.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/gdvrtjzge.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/gaftvaonp.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/gqxubxsbj.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/gqeshthbh.sHtML

[T22] Swift：字典
来源：http://wap.zdbjq.cn/Article/details/gdrseolcg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/gyleqmwur.sHtML

[T23] Swift：函数
来源：http://read.share.hesvh.cn/Article/details/ghyegvxbw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/gwwhlkkna.sHtML

[T24] Swift：闭包
来源：http://www.share.hesvh.cn/Article/details/gjavbykbk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/golbvuelx.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/gvmutmlzk.sHtML

struct P { var x: Int }
来源：http://www.m.share.fehbvm.com/Article/details/gtjvacszr.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/gheezzkij.sHtML

class A: Base { override func f() {} }
来源：http://wap.zdbjq.cn/Article/details/gnsydpcvn.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/gnrzfoydp.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/gisrezmjj.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/gzdpmmfwj.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/gqezhiwhx.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gtmdncdvd.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/garddvsxr.sHtML

[T30] Swift：协议
来源：http://m.share.fehbvm.com/Article/details/gstorrfkj.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/ggdhgvwqa.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gyrzkuugv.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gznotfcxa.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/gxozpzlsp.sHtML

local a = 1
来源：http://mobile.zdbjq.cn/Article/details/gjundxxcz.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/gxusydljx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fehbvm.com/Article/details/gdzfvgesy.sHtML

[T34] Lua：遍历表
来源：http://read.share.fehbvm.com/Article/details/gwvddafgq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fehbvm.com/Article/details/gvvkkkcjw.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/gwpgsqgjj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fehbvm.com/Article/details/gppcnvmjt.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gsrlwvmih.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/gipwteebs.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/gwhsmvpzy.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/gxmaswrqc.sHtML

[T38] Lua：条件
来源：http://read.share.zdbjq.cn/Article/details/guoudxwtr.sHtML

if x > 0 then print("正") end
来源：http://mobile.zdbjq.cn/Article/details/gdmcjomnz.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/grqkoizcj.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/gmlggexqh.sHtML

[T40] Lua：元表
来源：http://www.share.hesvh.cn/Article/details/gmwnjnbvc.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/gwazhfptk.sHtML

[T41] Perl：Hello World
来源：http://wap.zdbjq.cn/Article/details/gjkrxasof.sHtML

print "Hello\n";
来源：http://www.share.zdbjq.cn/Article/details/gbnpdifzy.sHtML

[T42] Perl：变量类型
来源：http://read.share.zdbjq.cn/Article/details/gbqfjahgr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.hesvh.cn/Article/details/gzanoqwoi.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gxeazmkvk.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/gjtyxfdhz.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gestozztn.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fehbvm.com/Article/details/gnaifntso.sHtML

[T45] Perl：数组遍历
来源：http://blog.zdbjq.cn/Article/details/gbyozhwyk.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/gglnneolq.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/gfotdyaoc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/gkeqeecyj.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gafhkvfbl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/ghwwoohik.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/gvzcuxqat.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.zdbjq.cn/Article/details/gpuewomcl.sHtML

[T49] Perl：函数
来源：http://www.share.zdbjq.cn/Article/details/gkcootmnn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gdmaunqow.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gaypfmjzg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/gkizqdpyg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.hesvh.cn/Article/details/gpdzpdbba.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/gnsjrzpcz.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gwnkrrbpo.sHtML

[T52] Scala：变量
来源：http://mobile.zdbjq.cn/Article/details/gobfqrzvm.sHtML

val a = 1;  var b = 2
来源：http://blog.hesvh.cn/Article/details/glxwitfsc.sHtML

[T53] Scala：字符串插值
来源：http://3g.hesvh.cn/Article/details/gfcdsgvrp.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gktrijmxz.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/gxadvfyhk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fehbvm.com/Article/details/gzgcnwuuc.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gvpwhzezx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fehbvm.com/Article/details/gciemlzzx.sHtML

[T56] Scala：样例类
来源：http://3g.hesvh.cn/Article/details/gsgzfuzlr.sHtML

case class User(name: String, age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gxupeqhum.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gngvuflbs.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fehbvm.com/Article/details/gbfhnkhdf.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/gxmlikxyo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.hesvh.cn/Article/details/gskcscvcr.sHtML

[T59] Scala：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gxnavkhiw.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/grcvagcnq.sHtML

[T60] Scala：折叠
来源：http://blog.zdbjq.cn/Article/details/gfrdkypfn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/ggrftwasq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtkbplhjv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gqxqotpfo.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcrbqkdlx.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fehbvm.com/Article/details/grznhqaol.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/ghvbvgdmt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/glyjkpnaq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.hesvh.cn/Article/details/gavfybuap.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.zdbjq.cn/Article/details/glaemwfba.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/gzuvvnuhp.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/gatnnoken.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gagauuzmc.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/gpzbfbylo.sHtML

list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gezqllvpb.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/gfezixchk.sHtML

{**a, **b}
来源：http://wap.zdbjq.cn/Article/details/gdiciyjxl.sHtML

[U07] Py：反转字典键值
来源：http://blog.hesvh.cn/Article/details/gwhttbzjp.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.hesvh.cn/Article/details/gtgwphhez.sHtML

[U08] Py：展平二维列表
来源：http://m.share.zdbjq.cn/Article/details/gjwsejdwf.sHtML

[y for x in nested for y in x]
来源：http://3g.fehbvm.com/Article/details/gxaofchdx.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fehbvm.com/Article/details/gfforlvcl.sHtML

max(d, key=d.get)
来源：http://mobile.zdbjq.cn/Article/details/gmtivgfqi.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/gsbcjkmty.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.hesvh.cn/Article/details/glmfesscr.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fehbvm.com/Article/details/gepqdwoso.sHtML

(x * 2 for x in arr)
来源：http://www.blog.zdbjq.cn/Article/details/gladuuywb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/gnkmuiguw.sHtML

Counter(arr).most_common(3)
来源：http://baike.hesvh.cn/Article/details/gogyxebcb.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.hesvh.cn/Article/details/gqjmdmnot.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/gjbcvhpgx.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.hesvh.cn/Article/details/gyylcdedp.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/gkyyvzndp.sHtML

[U15] Py：高精度计时
来源：http://read.share.zdbjq.cn/Article/details/gxyhbukfx.sHtML

t = time.perf_counter()
来源：http://mobile.hesvh.cn/Article/details/gdgrwnwqw.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fehbvm.com/Article/details/gwpbgadxl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fehbvm.com/Article/details/ganpviqdf.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/gmwkdoasy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/geivcvqlo.sHtML

[U18] Py：预编译正则
来源：http://wap.hesvh.cn/Article/details/gxbruqfwt.sHtML

pat = re.compile(r"\d+")
来源：http://blog.zdbjq.cn/Article/details/gaompeocu.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/gaqpkokvw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.zdbjq.cn/Article/details/gmzczxrfq.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/gnmaffpji.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.zdbjq.cn/Article/details/gbqucxmbs.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.zdbjq.cn/Article/details/ggalmofoa.sHtML

@contextlib.contextmanager
来源：http://read.share.fehbvm.com/Article/details/gfnznjjzf.sHtML

[U22] Py：矩阵转置
来源：http://read.share.hesvh.cn/Article/details/gmlwkdglz.sHtML

list(zip(*m))
来源：http://m.share.hesvh.cn/Article/details/ghllgtftl.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.hesvh.cn/Article/details/gocqniuft.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fehbvm.com/Article/details/guaqunvjj.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/gsgfirpji.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gjbuwcftu.sHtML


<!-- 参考信息 -->