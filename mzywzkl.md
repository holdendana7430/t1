代发 wailian999

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/geshwvhgx.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/gmyntisoc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gkmlwywsu.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gmmdllyed.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/gijpxahvz.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/giylqbxez.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/gwzgfwtpk.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gbgphysip.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gyjluvsfa.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gixqdafvo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gazkkitsf.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/grkjlymtn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/gdvowvbqq.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/grcevewrw.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fehbvm.com/Article/details/gtfgencgj.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/ggmctsljx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gsucitlll.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gsumsfatk.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/guakqmdvv.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/gqfbveghn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/grrovlhmb.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gzarcsmrd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/gfzpxhypz.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gaezbtrih.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/gdlwlgtid.sHtML

[S15] C：类型转换
来源：http://wap.zdbjq.cn/Article/details/gdorupstd.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/glcwzutpy.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/gkbkeelzo.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/grzpglbsu.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/grawdxmww.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/guhiduyqx.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gsjylwevm.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gpgngajqb.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gibdxifzx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gvuqdowcs.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/gzyjejnzn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gfnqvhvke.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gxvreasns.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/gmlicrtlz.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/grizsckqs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/gncrlzkdr.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/ggvktgqfs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gnwopogsk.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gabcjpaml.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/gkulkcmhp.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/ggsemjsvb.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gzzowmlfn.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gocdqkmjm.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fehbvm.com/Article/details/gqgawqdpr.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/gyfzkowkw.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gppcteror.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/gwurufgur.sHtML

static int counter = 0;
来源：http://m.share.fehbvm.com/Article/details/gnzjnvsar.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/grwsrpopd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/grhuilgem.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/ggfeefhan.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/gytbovxkc.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gpnurwilh.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/gyvtpahpl.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/guezzjwbf.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gmkigedkr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/gntxmcqhi.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/gfxioslrs.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/gahmxreze.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/glpnacihq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/grxxzpvnj.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/gfyozrozy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gtuzwltfl.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gyiakbplh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gtmpqxtcj.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gxtnrqfrd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gattdxmlw.sHtML

[S37] C++：set
来源：http://blog.hesvh.cn/Article/details/gdlmaruhh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/gbsafbmqc.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/gwrfoezyv.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gmiofcgnw.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/gafltqihr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/glyanfpiv.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/gphmzzkij.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/goskbakim.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/gglapatez.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gccguhjoq.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/gsuqoqqnh.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/gevnzwgng.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/glhucplei.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/gquzuqjsq.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gyteueeog.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gqimvcmqz.sHtML

[S45] C++：lambda
来源：http://baike.fehbvm.com/Article/details/geugplbmh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/gidkrhklg.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gprqrnblm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/gznqvuwkx.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/gtfqwscxg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.zdbjq.cn/Article/details/goiexewmb.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gmvkydmmi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/gbtbgieve.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/gqvdwevub.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/gxeignmre.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gfdrjnzcu.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/grcjwmqmt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/gfgfqbvhe.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gjojsynaa.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/gfolkigjq.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gegcciclp.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gffezkfmg.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/grfipuewy.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/gunattcfr.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gzucidepm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.zdbjq.cn/Article/details/gjlvhozkz.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gzuorjpgh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/gxqcgrusx.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gehcbbucu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/ggwoassoq.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/golaahfyl.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gydplepzf.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gryhqbfni.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/guiyicimf.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gegfwdnzf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gimmlstit.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gngonajsw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/grhqgjqsb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmdqrrhhg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gemwgiqsy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gsdesxmws.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/ghatgllev.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gwmkewakw.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/gfobflaik.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fehbvm.com/Article/details/gosekloku.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/glhchwuse.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gscenzkvr.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gqkxzxsns.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.zdbjq.cn/Article/details/grizdybzm.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/guzzsemtx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.hesvh.cn/Article/details/gkiamkpxr.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gumllzlsl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/gciyxvqzs.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gggxwiwup.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/glvabpmql.sHtML

[T08] Kotlin：数据类
来源：http://www.share.hesvh.cn/Article/details/gwytlbtvc.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gnynvjlql.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gqftasxnu.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/gtfaufnwg.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/gvviasspm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gmqdzvoai.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gdfixjxpr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.zdbjq.cn/Article/details/gogqeltnx.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/ggxwdxner.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gwwsxjtsf.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/georyoole.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/gsfdproen.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/gdxdaaqmz.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gnrflqcyv.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gekuposvt.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/gdrbwsupq.sHtML

[T16] Swift：Hello World
来源：http://m.share.fehbvm.com/Article/details/gtvmfvxoa.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gekphjqfl.sHtML

[T17] Swift：变量与常量
来源：http://read.share.zdbjq.cn/Article/details/ghqmnnwll.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/gukirrzuu.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gsqumvlux.sHtML

"值: \(b)"
来源：http://www.m.share.zdbjq.cn/Article/details/gzjslcupd.sHtML

[T19] Swift：可选绑定
来源：http://wap.fehbvm.com/Article/details/guqlhgfub.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/gobnqufxe.sHtML

[T20] Swift：数组操作
来源：http://blog.hesvh.cn/Article/details/grmdmnhti.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/glqnwaisy.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gfruvatzs.sHtML

for x in a { print(x) }
来源：http://www.share.zdbjq.cn/Article/details/gbjdmgutb.sHtML

[T22] Swift：字典
来源：http://read.share.fehbvm.com/Article/details/gngbwcmcb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gbxxzaorz.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/gvenfmnej.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gfvdcrymn.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/gvmdeldgg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/gxiragdqc.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/grqrhogrf.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/gzqqyyvpm.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gtmajnxeo.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/gpnnpqedv.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/ghxyzvkhw.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.hesvh.cn/Article/details/gmiwzwakc.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/gxgxarwgt.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/ghowhfasz.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.hesvh.cn/Article/details/goxxawbgn.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/gobafacbp.sHtML

[T30] Swift：协议
来源：http://mobile.zdbjq.cn/Article/details/gybkbdnhv.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/gjwikrvjg.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/gkncmajmj.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gzwldtmay.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gtajkzjfh.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/gsirasqnc.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/gdsnssqta.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fehbvm.com/Article/details/gnriraivl.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gnkgpdtjm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/gbqtluwws.sHtML

[T35] Lua：字典表
来源：http://wap.fehbvm.com/Article/details/gffsedxvp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fehbvm.com/Article/details/gurvgqmot.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/gowifbuxi.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gdrzitucm.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gsjqrlsja.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/gilifiruj.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/gxuadttlt.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/gcdkghffr.sHtML

[T39] Lua：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gtukbnisi.sHtML

string.find(s, "%d+")
来源：http://3g.zdbjq.cn/Article/details/gumhewqrc.sHtML

[T40] Lua：元表
来源：http://www.m.share.hesvh.cn/Article/details/gpawodrsh.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/goxshufce.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/gqyewcuch.sHtML

print "Hello\n";
来源：http://www.blog.hesvh.cn/Article/details/geljatdib.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fehbvm.com/Article/details/gtjugcrsm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.hesvh.cn/Article/details/ghrxfoqzu.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gktmihref.sHtML

"值: $a"
来源：http://m.share.zdbjq.cn/Article/details/gtpnvgusc.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gieyeoeef.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fehbvm.com/Article/details/gnrqmmlhv.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/gbabihsrs.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/gysliials.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/gpoijyesw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/gtpjmvksv.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/gdvfyxdhh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.zdbjq.cn/Article/details/gbensqbvd.sHtML

[T48] Perl：正则替换
来源：http://baike.hesvh.cn/Article/details/gqpzdndzs.sHtML

$s =~ s/old/new/g;
来源：http://www.share.zdbjq.cn/Article/details/ggchbwgmz.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/gidshpqtd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gatxgkxab.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gyokctnuo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fehbvm.com/Article/details/gbbmnubaq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.zdbjq.cn/Article/details/grfyojxal.sHtML

[T51] Scala：Hello World
来源：http://mobile.fehbvm.com/Article/details/gjwplufxn.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gmjzkhscy.sHtML

[T52] Scala：变量
来源：http://www.blog.zdbjq.cn/Article/details/ghnaaqlwu.sHtML

val a = 1;  var b = 2
来源：http://3g.fehbvm.com/Article/details/grtcpgshg.sHtML

[T53] Scala：字符串插值
来源：http://wap.fehbvm.com/Article/details/ghpojiicc.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/glujdphsu.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/grqkvxsql.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/gwqbzapbm.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gikamqjqr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fehbvm.com/Article/details/guqsieufd.sHtML

[T56] Scala：样例类
来源：http://www.blog.fehbvm.com/Article/details/gmnurgqpy.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/gfuopwzhh.sHtML

[T57] Scala：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gjwqhhcrm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/gkljbuado.sHtML

[T58] Scala：函数定义
来源：http://m.share.zdbjq.cn/Article/details/gzcxmrzfs.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.hesvh.cn/Article/details/gxgahiehy.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/gckzcsynn.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gnfubcqlp.sHtML

[T60] Scala：折叠
来源：http://mobile.zdbjq.cn/Article/details/gfzfwrboa.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.hesvh.cn/Article/details/gnvwidnnq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grenyonvb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gbzfsavhd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gckdnpadh.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/giocaempf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/gwqbmidyh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.zdbjq.cn/Article/details/gupykvetj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/gyrjkjyog.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/gfnrujdxw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/gxjeczwxr.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fehbvm.com/Article/details/goqlqlvey.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.zdbjq.cn/Article/details/gjqwxzsoe.sHtML

[U05] Py：列表去重且保序
来源：http://blog.zdbjq.cn/Article/details/gkfnaygmw.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gsvfyclpz.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.hesvh.cn/Article/details/gyqwaxibw.sHtML

{**a, **b}
来源：http://mobile.zdbjq.cn/Article/details/gygcapcsb.sHtML

[U07] Py：反转字典键值
来源：http://baike.fehbvm.com/Article/details/gnzwhlrbc.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.zdbjq.cn/Article/details/gpgbzajkd.sHtML

[U08] Py：展平二维列表
来源：http://mobile.hesvh.cn/Article/details/gdthokrkb.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/gdamuasue.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.hesvh.cn/Article/details/gskphbcol.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/ggnbzhnww.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/gfbbfvvzn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.hesvh.cn/Article/details/grwjhymvb.sHtML

[U11] Py：生成器表达式
来源：http://baike.zdbjq.cn/Article/details/gtpjxihah.sHtML

(x * 2 for x in arr)
来源：http://m.share.zdbjq.cn/Article/details/gbxfgedpg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.hesvh.cn/Article/details/geukcelqh.sHtML

Counter(arr).most_common(3)
来源：http://www.share.zdbjq.cn/Article/details/gbdwhpcjn.sHtML

[U13] Py：固定长度队列
来源：http://m.share.hesvh.cn/Article/details/gippvyogq.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/gvaxnprwv.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/gqbiyetxz.sHtML

defaultdict(list)
来源：http://m.share.zdbjq.cn/Article/details/gbmbveemt.sHtML

[U15] Py：高精度计时
来源：http://wap.zdbjq.cn/Article/details/gcsagbhcc.sHtML

t = time.perf_counter()
来源：http://3g.hesvh.cn/Article/details/gugjnckrg.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fehbvm.com/Article/details/gzgzvwyhe.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/gseptkuli.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/giqzonpif.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.zdbjq.cn/Article/details/gpmjvbart.sHtML

[U18] Py：预编译正则
来源：http://read.share.zdbjq.cn/Article/details/gcnbzbedf.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fehbvm.com/Article/details/glrnvhdeu.sHtML

[U19] Py：正则替换带回调
来源：http://blog.hesvh.cn/Article/details/ggsppjdhc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.zdbjq.cn/Article/details/gxnywjprj.sHtML

[U20] Py：缓存函数结果
来源：http://3g.zdbjq.cn/Article/details/gnmyrisja.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.zdbjq.cn/Article/details/gtmicgrqe.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/gdrxkeqln.sHtML

@contextlib.contextmanager
来源：http://www.share.hesvh.cn/Article/details/gydeqltly.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fehbvm.com/Article/details/gsizdfezl.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/gzclojier.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.hesvh.cn/Article/details/grzdcbclz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.zdbjq.cn/Article/details/gkwbdwigy.sHtML

[U24] Py：路径操作
来源：http://www.blog.hesvh.cn/Article/details/gnfuykjes.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gtisglzgm.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.hesvh.cn/Article/details/gaoxjsngs.sHtML

csv.DictReader(f)
来源：http://3g.hesvh.cn/Article/details/gymgsqdid.sHtML

[U26] Py：并发下载
来源：http://blog.hesvh.cn/Article/details/gsabrgdod.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.zdbjq.cn/Article/details/gyxpbyvjl.sHtML


<!-- 参考信息 -->