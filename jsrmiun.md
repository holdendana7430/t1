代发 wailian999

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/gqnoybrjb.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/gykpsrill.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/gtkgeuljz.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/gfwjeysmv.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/ghvattznn.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gqiklaibr.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/gyfpjofbl.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gvmisbcas.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gsluqkgnm.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gvcjtajwn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.zdbjq.cn/Article/details/gjlhsslvg.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/guagcbjrv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/ghjqvugyi.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gfatejwfv.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/gbjyusnid.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gdheiqzsg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gvfrhaydb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gihraoodx.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gvnpjvcnx.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gembfwvpg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gzdoosxrf.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/goqclvboc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/gjlvgskze.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gtqyrntkg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gyigvguas.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gulhalick.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/gygfkgcat.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gdugmstol.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/glrnjjyec.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/ghunjjwpf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/gcrpowkqc.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/gkjtvpjzd.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/giqkywszl.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gtqqifneu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gnmwblyjq.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gwmoywktn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gowlcanoq.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/grzcphphk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/gvvxkvmkr.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gzrbbdpdg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/gknrtnfxf.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gvvygnefm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gwrlszgna.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gyslvsdoe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/gwrqdngli.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/gmpznegkv.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/gjdhqaumc.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/gugbdcmlf.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/ghcsdsbom.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gpandxuyp.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/guqtjxvhc.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/gwkuaccwq.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/gqrzbnbja.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/garumamwh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/gjosxcqgx.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/gsvsunxny.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gzedxstgb.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gytszlykn.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/grdeeuqeb.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gsbmghhms.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gskjpdxfz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gzbwxmymq.sHtML

[S32] C++：字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gxieeqglm.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gbgaljauc.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/gitytoizy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/gxrlputxs.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/guwskjtrc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gqwmeacnp.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gvosspbwx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gedecqeyy.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gdsonyhjn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gfheoukbl.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/gjlhlnxae.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gotqosxkz.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gbyqwymzv.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/gyfqapjtw.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gsqjnbunb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gxdzojbbq.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/gawszieyz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/getvxcxxq.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/guezawrkq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/gognqhahq.sHtML

[S42] C++：继承与虚函数
来源：http://blog.zdbjq.cn/Article/details/gkkjjlgzn.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/glmhwxdoe.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gajmxieuw.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/gatdwwjdj.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/gtbkstpoz.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gtzvbddim.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/grflvistr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/gytghgjbr.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/gymgpegog.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gveuntane.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gyfknsddp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.hesvh.cn/Article/details/gumiqjxyi.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gcfaybzvg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/guumxriit.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/gevjeraft.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gxslsaeaa.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gfoilbacm.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/gvacmceau.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gtjavfsrb.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gbxuymtwa.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/gwpkdncom.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/glkrikhpz.sHtML

int size() const noexcept { return n_; }
来源：http://3g.hesvh.cn/Article/details/gxbxpotsd.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/glcrcrend.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gfivgaxzl.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/gmuwngcsz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gdrhsgyjs.sHtML

[S55] C++：结构化绑定
来源：http://m.share.zdbjq.cn/Article/details/gfiotfjoz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.zdbjq.cn/Article/details/gjqkingml.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gzttcoool.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gynqplnvo.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/gijebmeqd.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gxulacidl.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/guqslzoys.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gbancsowe.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/grlngyalr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gsdhsdljp.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/gybvxwrkd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.hesvh.cn/Article/details/gazbumtgg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvarwqrrl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gtzsphusl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjuquspkm.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/gkdjrztun.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gupqlkqfe.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/gvmmlojsr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gbarsyihg.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/gbtwsxlwo.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/grpnsmnvw.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/gzitdtuno.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/guyuwqhvm.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/gaclytpyh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gxcwgpajn.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/grdulynsr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gjhbsdulv.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gvuutjypq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gurmpzukm.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/gcjmwhsfx.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/grtmoqzff.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gxsmxioxl.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/guawgkhwj.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/guobdzohi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fehbvm.com/Article/details/gmybatogp.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gicsxoyhu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.hesvh.cn/Article/details/gtxojkept.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/gulggodrg.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gmadtuwqi.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gwzahsrhu.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/gnbrfsvfj.sHtML

[T14] Kotlin：循环
来源：http://www.share.hesvh.cn/Article/details/gonvdknor.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gzixrfsrt.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gqcgaaegc.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/gnkxwnepi.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/gsiykkngd.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gpqbfiame.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/gifompftw.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/ghkyffzid.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gsaiyxayy.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gktxlvicd.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/goyhqnmzx.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/gbgnaqcik.sHtML

[T20] Swift：数组操作
来源：http://www.blog.hesvh.cn/Article/details/gpekibvxw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/ggcvkrwwl.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/gogzgpebi.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/gldljdeyt.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/gpqulblkx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.hesvh.cn/Article/details/gaxlzkejn.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/goqbycbvc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gmmhpgczn.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/gqaujwvfv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/girdqgzel.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/gtccdgdod.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/guvscrnvj.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/gytqxlwlf.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/gitsthlbt.sHtML

[T27] Swift：错误处理
来源：http://read.share.hesvh.cn/Article/details/gycftoxwx.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/gsqywmcob.sHtML

[T28] Swift：枚举
来源：http://3g.zdbjq.cn/Article/details/gkbbdlwge.sHtML

enum Color { case red, green }
来源：http://www.blog.zdbjq.cn/Article/details/gzleaytgm.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.hesvh.cn/Article/details/grweeggvs.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gozndpeww.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/gcwfygnyx.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/gxxbqtwvj.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/gaofaotro.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gdxfozidd.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/gcibjlrkn.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/gdpihtlnz.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/gwwdyhwtw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/gumhdusos.sHtML

[T34] Lua：遍历表
来源：http://www.share.fehbvm.com/Article/details/ggqrwmewn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/gzjhwpgxx.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/gpbkcptly.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.zdbjq.cn/Article/details/gyzvyctkk.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/gbdjfmxnn.sHtML

function add(a, b) return a + b end
来源：http://mobile.hesvh.cn/Article/details/gavgsqezg.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/gkkypkvcq.sHtML

"a" .. "b"
来源：http://wap.zdbjq.cn/Article/details/gvcyqfjdl.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/giwerrfvc.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/grfhmezjx.sHtML

[T39] Lua：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gapxledom.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/glgbnmiqg.sHtML

[T40] Lua：元表
来源：http://3g.fehbvm.com/Article/details/gyigcvyob.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fehbvm.com/Article/details/gusqbopjz.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/gezplwvvr.sHtML

print "Hello\n";
来源：http://3g.zdbjq.cn/Article/details/gtitmwjxb.sHtML

[T42] Perl：变量类型
来源：http://www.share.fehbvm.com/Article/details/gtgcykkts.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.hesvh.cn/Article/details/gddknszms.sHtML

[T43] Perl：字符串插值
来源：http://3g.hesvh.cn/Article/details/ginlzpuwy.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/glddwraee.sHtML

[T44] Perl：条件
来源：http://read.share.hesvh.cn/Article/details/gxxrnokui.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/gzzcffjbu.sHtML

[T45] Perl：数组遍历
来源：http://wap.zdbjq.cn/Article/details/gohnfgxmc.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fehbvm.com/Article/details/glaeluzjt.sHtML

[T46] Perl：哈希操作
来源：http://wap.fehbvm.com/Article/details/gjhkybrsb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.zdbjq.cn/Article/details/gjbgsfpnk.sHtML

[T47] Perl：正则捕获
来源：http://read.share.zdbjq.cn/Article/details/gbwxgxdzg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/gkzqcjlii.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/gjulhizpu.sHtML

$s =~ s/old/new/g;
来源：http://3g.hesvh.cn/Article/details/gigrhmvrh.sHtML

[T49] Perl：函数
来源：http://m.share.fehbvm.com/Article/details/gxjbiiden.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gshigpagm.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gjaefmbge.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/gfvnumlkr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/gjzpndtjs.sHtML

[T51] Scala：Hello World
来源：http://baike.hesvh.cn/Article/details/gzidogtcw.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gkdpwsoex.sHtML

[T52] Scala：变量
来源：http://mobile.hesvh.cn/Article/details/gmocfruft.sHtML

val a = 1;  var b = 2
来源：http://www.share.zdbjq.cn/Article/details/gxammhwps.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gmjofjlja.sHtML

s"值: $b"
来源：http://3g.zdbjq.cn/Article/details/girwfxtep.sHtML

[T54] Scala：集合映射
来源：http://read.share.fehbvm.com/Article/details/gtgpkdona.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.hesvh.cn/Article/details/gnarsmiiw.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gablckujr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fehbvm.com/Article/details/gjmmzrlsk.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gqrtprrcs.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gvuwdoxhw.sHtML

[T57] Scala：模式匹配
来源：http://mobile.hesvh.cn/Article/details/ggosqzvel.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.hesvh.cn/Article/details/gbquhffgc.sHtML

[T58] Scala：函数定义
来源：http://read.share.zdbjq.cn/Article/details/gksrzzmrr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fehbvm.com/Article/details/gjffudrrm.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/gzhjgkxii.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gqifcfphr.sHtML

[T60] Scala：折叠
来源：http://www.blog.fehbvm.com/Article/details/gxogxdtlf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/ggpfiscry.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnjzrzqwy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gyipixqbt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghcqkzkds.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fehbvm.com/Article/details/gddsokzwc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/gmdgrgfpf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/gbegkplpd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/gskrgszdb.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.zdbjq.cn/Article/details/gkolatati.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.hesvh.cn/Article/details/gpfdyqxxo.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/gptthcryz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.zdbjq.cn/Article/details/grywxynih.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/gbhpzqwgr.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gbvildlul.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/gkwcazzsb.sHtML

{**a, **b}
来源：http://www.m.share.fehbvm.com/Article/details/gyfypicfe.sHtML

[U07] Py：反转字典键值
来源：http://3g.fehbvm.com/Article/details/gwxlgfvgg.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.hesvh.cn/Article/details/gizizorzy.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/ginyeemuc.sHtML

[y for x in nested for y in x]
来源：http://m.share.hesvh.cn/Article/details/glwajiiqa.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.zdbjq.cn/Article/details/gskkwvpsf.sHtML

max(d, key=d.get)
来源：http://3g.zdbjq.cn/Article/details/gqixpxudr.sHtML

[U10] Py：按值排序字典
来源：http://www.share.hesvh.cn/Article/details/gmmlmiebj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/gtyefoudt.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.hesvh.cn/Article/details/gtjxbcxrq.sHtML

(x * 2 for x in arr)
来源：http://read.share.zdbjq.cn/Article/details/ghqqrqmeg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/ghucvyomz.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/ggeqnmony.sHtML

[U13] Py：固定长度队列
来源：http://blog.hesvh.cn/Article/details/goxcflxwg.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gyytegjtx.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.zdbjq.cn/Article/details/gbzoxuwky.sHtML

defaultdict(list)
来源：http://wap.zdbjq.cn/Article/details/gwxjmgfqp.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/graophwdx.sHtML

t = time.perf_counter()
来源：http://blog.hesvh.cn/Article/details/gnfxoswbe.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/ggsecgezv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.zdbjq.cn/Article/details/ghkxaorxf.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gmsclubxo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.hesvh.cn/Article/details/gmoailupi.sHtML

[U18] Py：预编译正则
来源：http://www.share.hesvh.cn/Article/details/gvbdsabth.sHtML

pat = re.compile(r"\d+")
来源：http://wap.hesvh.cn/Article/details/gozntpoxl.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.hesvh.cn/Article/details/geruvngny.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.hesvh.cn/Article/details/gwcsxyfpj.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/gekvxlucf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.zdbjq.cn/Article/details/gvraackrm.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fehbvm.com/Article/details/gmhxlkcce.sHtML

@contextlib.contextmanager
来源：http://m.share.fehbvm.com/Article/details/gsonhveoo.sHtML

[U22] Py：矩阵转置
来源：http://3g.fehbvm.com/Article/details/gkroyhyuc.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/gxztsmftc.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.zdbjq.cn/Article/details/grnafgjnp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/gxcahgiqs.sHtML

[U24] Py：路径操作
来源：http://m.share.fehbvm.com/Article/details/gpwmmfweb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gisouchzq.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fehbvm.com/Article/details/gslexzioe.sHtML

csv.DictReader(f)
来源：http://www.share.fehbvm.com/Article/details/ggtfxcnsu.sHtML

[U26] Py：并发下载
来源：http://www.blog.zdbjq.cn/Article/details/gnopvydxc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.hesvh.cn/Article/details/gsfatpdbj.sHtML


<!-- 参考信息 -->