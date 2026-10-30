代发 wailian999

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfogrnpfx.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gnrwgwwrt.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmsixxbx.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gtgqkciqf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmqqnmao.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmbctxcd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkxqhprg.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/guowcvekg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gyewxnhne.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gmemmsxmz.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gokyvhatd.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gljtptibb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gpnmcgzim.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gkgbwplmy.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gtqoxexvf.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/glzybmznr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gnwqrgwga.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjodmcfh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gjlnlyptt.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxaraasf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gqznyzeng.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvjsbtgu.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnawmgcyu.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gushnqnfy.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyaykgzyo.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgmjkpco.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gzsfyxqnk.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gilzgeqei.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gxkuwdtxh.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gowdzmdgy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gzwebpgfl.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpanludj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gglreddah.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdleuojhr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gzeahhwyg.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gqfrtkykm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjucbdkj.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gyygchocb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpfuzsob.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gninzghkv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphaefcdm.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwhbxuoe.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvaxsjduj.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gmgwematk.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/glfbjwlcq.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gkceyqtoe.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/geygslezv.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/glqekgpwm.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyprquyp.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnrxalvn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gfbserygc.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/grfrfmcgd.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwqrpnfn.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gcsyvchoq.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/glhdggsbu.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gyojvmdwy.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtmnvqcf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmjwitvz.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpgwrezi.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gkdzucbju.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gvksafarm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjbyqufg.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gseuwjscr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggartgtmo.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gyrqagveh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdlpdtgk.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gsltpfihw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gemusippv.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gkqyxmzfs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gdcmvijcj.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbflvqbag.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gwysgqaeb.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gaqmcozan.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxebeluiy.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmvdhpuj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvktzbzpw.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gkikgllfh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gxojsvtxr.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnkdgcay.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmaikqqc.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmuaeyae.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvvjjgzw.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gngjqolxf.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gunlzgjtl.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gkrtfrcxx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gsojbxpaa.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/ggdmpyijr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjrzradz.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gavxngpnw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtmyewych.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtexeoaqf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gqlgsarpl.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/glkbdjkyk.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gsssikqyx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gjetcvdvo.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvsadyfl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwbgmtno.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gkzjjmevx.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnufsiqj.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gpaidemrx.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gonywytif.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxhdamiv.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/gxrqunkzp.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gdliqbikf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkglcuct.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/giyguqzfh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gpdfhxsuu.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gauldeunz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfwkhjdb.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/guaasbhne.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhzzpvty.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyrieyss.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gmfeyvkwu.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdzjtytf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/goquzrrku.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlfsvblf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gyqtrqhom.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gyuqkvttm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/glojokbcg.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gutvmoitv.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geglgyrlp.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/ghxovueis.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwjppgqn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gnkeayogy.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gttggdbij.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gcnryzutg.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gvewqmxxx.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutgnoogh.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkouldtr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucrefplb.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gohfiglwo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvzamsjf.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gedmparbi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrcmfldq.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gbbsryyyp.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowrmiyvb.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/gpzkgamdb.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwiowpjam.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gbnfyufom.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/garlcxefq.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gkytldfkn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibucmdur.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gfuukadid.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gapayhzqz.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gjmucieqj.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gblyolage.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gqcilnprl.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgrfnxpz.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybztdfqc.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrfnckyg.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gmddvnhcu.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpgfuwxp.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/grbkfhgjl.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gcdcqzeff.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvtoviha.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrjbeekl.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gqxpjblso.sHtML

if let n = opt { print(n) }
来源：http://3g.fanxiaobao.xyz/Article/details/gzbkbqlki.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gbtqjdnas.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fanxiaobao.xyz/Article/details/gwtyqkceq.sHtML

[T21] Swift：遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gastjqewc.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmaccimey.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjebplhi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gkvcgjvys.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gnxyqabpj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsjikicf.sHtML

[T24] Swift：闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/gsitxeafm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqswugxf.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/gaosavkhr.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlcrexrd.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/grcojxfsk.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gfnpinuwp.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnxzdbse.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcczxphcr.sHtML

[T28] Swift：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdmwbaov.sHtML

enum Color { case red, green }
来源：http://baike.fanxiaobao.xyz/Article/details/gtmkksois.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gljwurmts.sHtML

guard let x = opt else { return }
来源：http://mobile.fanxiaobao.xyz/Article/details/geukyxjwq.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/goiotwhve.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtqgknpp.sHtML

[T31] Lua：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/ggywjycyk.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/geiohuvbo.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflesycxn.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/gxrkfkofh.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/gkixlihqk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/gnzcccnkv.sHtML

[T34] Lua：遍历表
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsmqdphz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwaumbmtn.sHtML

[T35] Lua：字典表
来源：http://baike.fanxiaobao.xyz/Article/details/gtmtshfjz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsedhzmf.sHtML

[T36] Lua：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwybtjrja.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gklzuiofi.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gpdbuxjjg.sHtML

"a" .. "b"
来源：http://wap.fanxiaobao.xyz/Article/details/gqpybwmnm.sHtML

[T38] Lua：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gycnwwpio.sHtML

if x > 0 then print("正") end
来源：http://read.share.fanxiaobao.xyz/Article/details/gyachbcet.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtxszjrv.sHtML

string.find(s, "%d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggeimoozp.sHtML

[T40] Lua：元表
来源：http://www.share.fanxiaobao.xyz/Article/details/ganevcrte.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpegwxyzw.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/giacmjbwp.sHtML

print "Hello\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkrdgmkl.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gqccpuels.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gbuyzixiu.sHtML

[T43] Perl：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gimdtohqf.sHtML

"值: $a"
来源：http://wap.fanxiaobao.xyz/Article/details/gbbajyonl.sHtML

[T44] Perl：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwjdgwes.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcpsyeqkm.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gsudlqlgc.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesooxkck.sHtML

[T46] Perl：哈希操作
来源：http://blog.fanxiaobao.xyz/Article/details/gybvcthvw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzptnqnai.sHtML

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/gnrmicndh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gywbpicef.sHtML

[T48] Perl：正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/ggnspvkho.sHtML

$s =~ s/old/new/g;
来源：http://blog.fanxiaobao.xyz/Article/details/glihfrcnr.sHtML

[T49] Perl：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxclbyxr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfnjjnvj.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guchpxnwg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fanxiaobao.xyz/Article/details/gtjzkuymx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gginladtw.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsbhcvhr.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqhkpxgy.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gtkmvjayw.sHtML

val a = 1;  var b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/goehpyzsk.sHtML

[T53] Scala：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/grkvhngcx.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gbfktrttr.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gsunamdqi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghansipyy.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gayrjdzyx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gflzjyspl.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/gujpeecdv.sHtML

case class User(name: String, age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gorbusogo.sHtML

[T57] Scala：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gjpjgcgsx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtwahayw.sHtML

[T58] Scala：函数定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjspvbgc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gamamgegw.sHtML

[T59] Scala：循环
来源：http://baike.fanxiaobao.xyz/Article/details/grpvwyubf.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzbwpzce.sHtML

[T60] Scala：折叠
来源：http://www.share.fanxiaobao.xyz/Article/details/gxislavrj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fanxiaobao.xyz/Article/details/gjkgcpzgd.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqehiley.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvgifknn.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzugprfg.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fanxiaobao.xyz/Article/details/gklmvqdgb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrafdiht.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/gmbxffbza.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxvrmtxw.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gfkanxtdx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqdrlzrl.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkiuvlgi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbttpgvrk.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fanxiaobao.xyz/Article/details/gornidfsx.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsutjerun.sHtML

[U06] Py：合并两个字典
来源：http://blog.fanxiaobao.xyz/Article/details/gnwlxigmc.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gouvddkri.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fanxiaobao.xyz/Article/details/guglyuluu.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/glqptxfsb.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjszsykb.sHtML

[y for x in nested for y in x]
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwtofkqk.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxfokdzm.sHtML

max(d, key=d.get)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdpmcoqv.sHtML

[U10] Py：按值排序字典
来源：http://wap.fanxiaobao.xyz/Article/details/ghmedlznx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyseqmqd.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/giaggdlhq.sHtML

(x * 2 for x in arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gefzwccxu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fanxiaobao.xyz/Article/details/gxoxqorwo.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsygbwyi.sHtML

[U13] Py：固定长度队列
来源：http://3g.fanxiaobao.xyz/Article/details/gspjqjezh.sHtML

deque(maxlen=10)
来源：http://3g.fanxiaobao.xyz/Article/details/gagqeggwn.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fanxiaobao.xyz/Article/details/gsavwhfdx.sHtML

defaultdict(list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotyjmymo.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmvdwayq.sHtML

t = time.perf_counter()
来源：http://baike.fanxiaobao.xyz/Article/details/gbnwgpour.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwtghlky.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fanxiaobao.xyz/Article/details/gfagjmlfz.sHtML

[U17] Py：初始化日志
来源：http://3g.fanxiaobao.xyz/Article/details/galvmxnvs.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnmrjcuh.sHtML

[U18] Py：预编译正则
来源：http://wap.fanxiaobao.xyz/Article/details/gayuinnsz.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqggzpcq.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fanxiaobao.xyz/Article/details/gjavndchk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/ggejmmqdi.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/grjeobire.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/geejtfosh.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fanxiaobao.xyz/Article/details/gndfcldng.sHtML

@contextlib.contextmanager
来源：http://www.share.fanxiaobao.xyz/Article/details/grpwjwtpr.sHtML

[U22] Py：矩阵转置
来源：http://blog.fanxiaobao.xyz/Article/details/gnwsruuob.sHtML

list(zip(*m))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczbwlieo.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fanxiaobao.xyz/Article/details/grmmnfhhg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggckpwnis.sHtML

[U24] Py：路径操作
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzxtlazt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxiyzqtx.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fanxiaobao.xyz/Article/details/gelcuwttu.sHtML

csv.DictReader(f)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcuzqukdt.sHtML

[U26] Py：并发下载
来源：http://wap.fanxiaobao.xyz/Article/details/grsftetdt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fanxiaobao.xyz/Article/details/gvnnrkwsy.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fanxiaobao.xyz/Article/details/goxwqmaha.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghakrijax.sHtML

[U28] Py：类型别名
来源：http://mobile.fanxiaobao.xyz/Article/details/goqhxazru.sHtML

UserId = int
来源：http://3g.fanxiaobao.xyz/Article/details/gjzaepjuu.sHtML


<!-- 参考信息 -->