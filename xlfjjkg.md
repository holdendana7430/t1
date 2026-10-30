代发 wailian999

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gnhtzwreb.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gzplwmesy.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gborlrbho.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gqhavkzoi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gjyibfdcq.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gevastsin.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/gwxsxzdxj.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/gfreqwptk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/giisjswce.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/glsnevnfv.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/gbefplacs.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gqfpxhncw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/glzhgokom.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gnajlwxrd.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/golmpmrfs.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gruedmlhr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gekznlzuj.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/gerpdbphl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/gwvldblts.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gkjvbqnii.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gulrtqfoe.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/guwbeozjs.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/ghlkmqbwx.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gvjzduhqb.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gpwaakboq.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/gpgqjkhin.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/guhhlwwpm.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/gklbaayvh.sHtML

int main(int argc, char **argv)
来源：http://read.share.fehbvm.com/Article/details/gwbzksgrt.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/glskqfgsh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gskbnihcx.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gzeoxebtc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gmdgqngqt.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/ggdzgnxjl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/gykepurmn.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gdcyfbytz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/gmzmvoihk.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gjunqmzow.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/gybhosrli.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/guozlwnif.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/gulyjcfyx.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gesmkbvtc.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gaedkfjya.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gjpobynwz.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gaqqnkzhu.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/gstwwdblm.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gfayrpfqe.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/guvchfxuq.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gugigbbrz.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/gryfvadfs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/gvbaibdox.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gtcyfozgo.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gfnhhzuld.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gtdlfmpik.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/gmpvnzrlc.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/gslispiwr.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/gavnewosg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gecitbyzn.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/gtmefqyez.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.hesvh.cn/Article/details/gdibkxclw.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gkciautto.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/glsyjsrfm.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/gpyzfkrxg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.zdbjq.cn/Article/details/gczyqtgkf.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/guhteqywu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gzemtohra.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/ggmhskesi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gsuwslrca.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gnqkxdzod.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/gpblfxrwt.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/gfbrdocns.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gxxawtokb.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gmlkhpeku.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gfdfwlsjm.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/ghazmfnui.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gfhttsfux.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/gryauhunw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.zdbjq.cn/Article/details/gseqwbpjy.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gtgedeqvj.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/gxehfxeiq.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gffszjjfn.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/ghzpuobdx.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/guykyftxf.sHtML

void inc(int &x) { ++x; }
来源：http://wap.zdbjq.cn/Article/details/guxixgqgf.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/gfesixewg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gocboximp.sHtML

[S46] C++：函数模板
来源：http://www.share.fehbvm.com/Article/details/gyqdjlhfb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gfbifntsl.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/glpesnofv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/glgppsjcp.sHtML

[S48] C++：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gbceoibmu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.zdbjq.cn/Article/details/gdfktkdhd.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/gyoiuzdgw.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gmqxtyqqf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/gueddiimu.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/gvntraulk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gbbcblwbc.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/gonwgdjbv.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/grduvpvky.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/goflzzjtz.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/ghrnasidj.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/ghsmmdhva.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/gtgbatlsd.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/gmfepqvry.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gtrmxnydu.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/gsbgczktf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gkqsqocit.sHtML

[S56] C++：optional
来源：http://www.share.fehbvm.com/Article/details/gczetodtq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gmeymyaqr.sHtML

[S57] C++：编译期常量
来源：http://blog.hesvh.cn/Article/details/gdmxbwdux.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gwdtlpwyp.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/ghkhxpdhc.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gvlykmvqq.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/gmebzamzh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/gtoeqdyyy.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/gcmseiwfp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gwgqkbwsv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfapkteox.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/grpzyzeau.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnncuklik.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gqkvmuogm.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/guwbsntpl.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/gzbvdlblc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/gqulbvcpm.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/girclrslt.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gsgwxqdye.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gvjxtfvct.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/guifehcyy.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/gixyqliaf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gyefqslix.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/gxcsotvvl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gactsgpqa.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gudtsxgac.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gjhpqhnwo.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gorkqkpfq.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/gmohgaqqr.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/gchtyuhen.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gzgvkkqgn.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gejjbgfrv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.hesvh.cn/Article/details/gcllesnjf.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/gomkiytnq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/gllathcaf.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.hesvh.cn/Article/details/gcikofwpw.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gfohdvieb.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gdqidshyx.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/ggwixpral.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/gfzqyctmn.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gwapvdslb.sHtML

[T15] Kotlin：接口
来源：http://wap.fehbvm.com/Article/details/gxayqijkr.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/gtdlghouu.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gnrjkcpeg.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gexoxwipl.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/gteqszind.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/gekzlpcjh.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/geyprauss.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/genocogau.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gakocnikh.sHtML

if let n = opt { print(n) }
来源：http://baike.zdbjq.cn/Article/details/gfvurmhuq.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/gbehofsbm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gvpuwmknt.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/giucqmioz.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/gzioiebyo.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gksdhugfu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/gkcvaxezj.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/grplidmdg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/gtakcdfbo.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gurghdoyp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/ginazyxfq.sHtML

[T25] Swift：结构体
来源：http://mobile.zdbjq.cn/Article/details/gjfagxzjw.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gexxnrrfr.sHtML

[T26] Swift：类与重写
来源：http://read.share.hesvh.cn/Article/details/gtozyiuva.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/gisiksxmo.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/gwnooxack.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fehbvm.com/Article/details/gfgmeicug.sHtML

[T28] Swift：枚举
来源：http://3g.fehbvm.com/Article/details/gbnkwnxls.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/guzpovnyu.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.zdbjq.cn/Article/details/gyudifimy.sHtML

guard let x = opt else { return }
来源：http://www.blog.zdbjq.cn/Article/details/gzfxigbwn.sHtML

[T30] Swift：协议
来源：http://baike.zdbjq.cn/Article/details/gkwjkgkhf.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.zdbjq.cn/Article/details/ghpzqkesz.sHtML

[T31] Lua：Hello World
来源：http://3g.hesvh.cn/Article/details/gecjxhtkm.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gnvmbmeeu.sHtML

[T32] Lua：局部变量
来源：http://www.blog.hesvh.cn/Article/details/gmfvsxmsq.sHtML

local a = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gceaxqkfi.sHtML

[T33] Lua：表（数组）
来源：http://www.share.zdbjq.cn/Article/details/glbnexvis.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/gzyaytnez.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/grfjkszdm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/grofvmzut.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gtnfznxuk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.zdbjq.cn/Article/details/gfjxneifi.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/gptirjnvq.sHtML

function add(a, b) return a + b end
来源：http://read.share.fehbvm.com/Article/details/gbtanrnix.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gxdulqwhx.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/gorqjzewa.sHtML

[T38] Lua：条件
来源：http://www.m.share.fehbvm.com/Article/details/grfkcmcpx.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/gubrsoerr.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gltpkjuje.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/gebhsxqlg.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/glyudxpvp.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/gnsgivacs.sHtML

[T41] Perl：Hello World
来源：http://baike.fehbvm.com/Article/details/glcfcotnw.sHtML

print "Hello\n";
来源：http://www.share.zdbjq.cn/Article/details/gfexshian.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/gnegjzthi.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/gxmrefxja.sHtML

[T43] Perl：字符串插值
来源：http://m.share.hesvh.cn/Article/details/glphjblyv.sHtML

"值: $a"
来源：http://www.m.share.hesvh.cn/Article/details/gkbbednfv.sHtML

[T44] Perl：条件
来源：http://mobile.zdbjq.cn/Article/details/gdjwracxh.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.zdbjq.cn/Article/details/gxvxbskmp.sHtML

[T45] Perl：数组遍历
来源：http://baike.hesvh.cn/Article/details/gbcedqzbd.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/goybecque.sHtML

[T46] Perl：哈希操作
来源：http://baike.zdbjq.cn/Article/details/gkgmehkap.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fehbvm.com/Article/details/gsmupnsrf.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.hesvh.cn/Article/details/gqqgofjep.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.hesvh.cn/Article/details/gihdledqn.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.hesvh.cn/Article/details/gdhhgbmvy.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/gywmgtgvq.sHtML

[T49] Perl：函数
来源：http://3g.hesvh.cn/Article/details/guutjentj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gomodznjy.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gvymrmxez.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/ghjbvpbpb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/grsmcpwst.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/gwgpmwypx.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gabodpxqq.sHtML

[T52] Scala：变量
来源：http://m.share.zdbjq.cn/Article/details/gkzmatvpw.sHtML

val a = 1;  var b = 2
来源：http://read.share.hesvh.cn/Article/details/gkopylrcd.sHtML

[T53] Scala：字符串插值
来源：http://wap.fehbvm.com/Article/details/glwkmzesy.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gqqagppdu.sHtML

[T54] Scala：集合映射
来源：http://mobile.fehbvm.com/Article/details/gghithycb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.hesvh.cn/Article/details/gcbyhdykt.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gjxiedbwo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.zdbjq.cn/Article/details/gkcwduozz.sHtML

[T56] Scala：样例类
来源：http://baike.hesvh.cn/Article/details/ghaozefyw.sHtML

case class User(name: String, age: Int)
来源：http://3g.fehbvm.com/Article/details/ggyfjgnxk.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/gdhcfsetm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.zdbjq.cn/Article/details/geueimysn.sHtML

[T58] Scala：函数定义
来源：http://read.share.fehbvm.com/Article/details/gvgwzjgbh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.hesvh.cn/Article/details/gvmdnplmr.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/gozcymwlu.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fehbvm.com/Article/details/gshahqvjw.sHtML

[T60] Scala：折叠
来源：http://www.share.fehbvm.com/Article/details/gfvtdrdvx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fehbvm.com/Article/details/guiraqmmb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdhfiszjn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gtqtsacbw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmrnsokda.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/giujtxmja.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/gfuljfcpc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.hesvh.cn/Article/details/graetlote.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.zdbjq.cn/Article/details/gxcfzlzuk.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gczxbnwxj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/gnjtmsiub.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.zdbjq.cn/Article/details/gdcxwysrp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.zdbjq.cn/Article/details/gyeepewct.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fehbvm.com/Article/details/gmzizqpkm.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gpvnibpee.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/gglttzhqk.sHtML

{**a, **b}
来源：http://wap.zdbjq.cn/Article/details/gcvswkxoh.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/gysmgyvvr.sHtML

{v: k for k, v in d.items()}
来源：http://baike.hesvh.cn/Article/details/gcwikjxfx.sHtML

[U08] Py：展平二维列表
来源：http://blog.zdbjq.cn/Article/details/goxvbyaei.sHtML

[y for x in nested for y in x]
来源：http://www.share.fehbvm.com/Article/details/gkrwvcetd.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.hesvh.cn/Article/details/gtwgxffgj.sHtML

max(d, key=d.get)
来源：http://www.share.hesvh.cn/Article/details/gmnprlozk.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/gttaqnnxe.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/gonesfuiy.sHtML

[U11] Py：生成器表达式
来源：http://blog.hesvh.cn/Article/details/gefcyrbgn.sHtML

(x * 2 for x in arr)
来源：http://wap.fehbvm.com/Article/details/gmfbhsfuf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fehbvm.com/Article/details/gmvsmrqvt.sHtML

Counter(arr).most_common(3)
来源：http://blog.zdbjq.cn/Article/details/giszkgnlk.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fehbvm.com/Article/details/gcujrykwh.sHtML

deque(maxlen=10)
来源：http://mobile.hesvh.cn/Article/details/gggppwuxx.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/gyaxvtjlm.sHtML

defaultdict(list)
来源：http://www.m.share.fehbvm.com/Article/details/gneyljzvg.sHtML

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/gshfjqbhp.sHtML

t = time.perf_counter()
来源：http://m.share.zdbjq.cn/Article/details/gqgzepdpv.sHtML

[U16] Py：命令行参数解析
来源：http://baike.zdbjq.cn/Article/details/gtfjzfgfk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gtteeqrjs.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/gsuqlnbkj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.hesvh.cn/Article/details/gcrohswih.sHtML

[U18] Py：预编译正则
来源：http://www.share.hesvh.cn/Article/details/gnbruacxo.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/gbivfiztx.sHtML

[U19] Py：正则替换带回调
来源：http://baike.zdbjq.cn/Article/details/gacxwddju.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fehbvm.com/Article/details/giyoaixyg.sHtML

[U20] Py：缓存函数结果
来源：http://3g.zdbjq.cn/Article/details/gkhntmncd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.hesvh.cn/Article/details/gkjskulcw.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/gbibyjvwu.sHtML

@contextlib.contextmanager
来源：http://www.blog.hesvh.cn/Article/details/gnvlqglvk.sHtML

[U22] Py：矩阵转置
来源：http://m.share.zdbjq.cn/Article/details/ggmrqkwdt.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/gvrxkcmdr.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/gtfioxdpb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fehbvm.com/Article/details/gdvqccllp.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/gblrontzb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gwxyeqvig.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fehbvm.com/Article/details/gdeslhekd.sHtML

csv.DictReader(f)
来源：http://m.share.fehbvm.com/Article/details/gofyjkidk.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/gymbwssae.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.zdbjq.cn/Article/details/gzpelpbvy.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fehbvm.com/Article/details/gexdxwnbr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fehbvm.com/Article/details/ghebvccpn.sHtML

[U28] Py：类型别名
来源：http://www.share.fehbvm.com/Article/details/gqttcedzi.sHtML

UserId = int
来源：http://www.share.fehbvm.com/Article/details/ggcuyimnf.sHtML


<!-- 参考信息 -->