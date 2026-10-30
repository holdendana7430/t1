代发 wailian999

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/gknmftmbn.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gxkdhjwlp.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/gzecwctck.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gazdjrddl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/gkurxkmzc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/gpucackqr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/gjztflpnn.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/grwrtdovm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gtbhdvjxk.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gwbplxfkl.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/grbhhsdsx.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gsmbwtkyk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/garvfawmq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/gxksdpzum.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/grxzewcsn.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gkouljarv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/gdtupkqom.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gynisdgqk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gzkzqrlst.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gboimqnzz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/gtcbazkla.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gzfnemcom.sHtML

(double) a / b
来源：http://www.m.share.hesvh.cn/Article/details/gbhttqsor.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gazohksjt.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/gbubrzcnu.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gccpftqcu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gkntiqkbz.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gfzrrarsd.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/gqknavhjd.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gjttijcrv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gcvzawwel.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/gjkuomqyg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gqdzmttrn.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/giducsjvf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/gsotlyuwl.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/guzeljmef.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gxafjjcig.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/gtztlwpdh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fehbvm.com/Article/details/gudphrjog.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/gcybuiotn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/gdpihfhvv.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/gqntkjrlq.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/ggndveegd.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/ghwsrmcna.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/gdzkixuhf.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/ghsrzhdfh.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gpjnlbhrj.sHtML

[S28] C：静态变量
来源：http://wap.hesvh.cn/Article/details/gfmzzuiyj.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gzbsiovmp.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/gkureuuyw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/gfrwxaufu.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gtisdntvi.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/gyukbotpf.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/gcmotvkzx.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/gepotdceo.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/gljybdpar.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/gqdrzfkuq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gdvhctukj.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gketcmrmj.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gcnnyumla.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gxrepjxph.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/goaokxemg.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/gfrzgdobi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gbqwihaui.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gwaneyiff.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/guqryckbm.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/gatnbvavo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gkcqraioq.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gcnjuwoww.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/gawnheqgp.sHtML

[S38] C++：排序
来源：http://3g.zdbjq.cn/Article/details/gukiyceiw.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/gufxfmcpw.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gmlelmmjl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gzhygeick.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/gogjogatx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gjqulfelg.sHtML

[S41] C++：类与构造函数
来源：http://www.share.zdbjq.cn/Article/details/gcqkcdlip.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/gfbxknpxz.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/gblfvfsrv.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/gckseohkw.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/ggyeoanlf.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/ggscoczij.sHtML

[S44] C++：引用传参
来源：http://read.share.zdbjq.cn/Article/details/gijmynwrv.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/gjekiincj.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/gmbhtlzvw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/gmrapznno.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/gsjftjzcl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gyouyqqzp.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gfzukyjzb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/geimrmkke.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gsgyxtizm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gvaqzhlqw.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/gretgwyfo.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/ghcgdihib.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gzmnozfod.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/gfmufydwy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gegrwaehy.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/gaylhryla.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gcfazwbik.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gpnduvaew.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gcjrryqgy.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/gfotpgwmc.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/ggoeovgix.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/grrfhtyrk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/gprhtyoeo.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/ghmkywtru.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gjrehvqwi.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/grwkvqrhl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/gnhvuatvv.sHtML

[S57] C++：编译期常量
来源：http://mobile.fehbvm.com/Article/details/gcprfhamw.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gecqarnqv.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gyzaqdbkh.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/guiyinzsx.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/gvlzrezcy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gbdtitbht.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/ghpovsznr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/gmuyfqxxi.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gsrfkepyo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gowidoixs.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glasbisar.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/grjqbttxo.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gjlwwppiw.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gzdthmgal.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/ggchkebkj.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gnuecubwf.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/gbdnvqmgw.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/gfdmtbogv.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gvmtiphlw.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/garzlcgen.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/ggbjilvxr.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/gsbacrmsy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gznnflnqr.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/grrfsikin.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/gasucedps.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gjocmiktw.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gbljjsqkv.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gzsjerwuu.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gkjxkgdal.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gqepygnrf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gparuihun.sHtML

[T11] Kotlin：协程
来源：http://3g.hesvh.cn/Article/details/gjtfecprb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/grfjwmbuw.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gragpyloy.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gwuddrxlc.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fehbvm.com/Article/details/gkyncrmuv.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/gjilzchok.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/gcjplasrj.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gkwcjpodu.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gyvrmwrde.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/gqwtqcwbm.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gwzkvrkgp.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gfdirftvj.sHtML

[T17] Swift：变量与常量
来源：http://3g.zdbjq.cn/Article/details/gtwmyogig.sHtML

var a = 1;  let b = 2
来源：http://read.share.hesvh.cn/Article/details/gqsfyhddv.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gxmnupmdq.sHtML

"值: \(b)"
来源：http://m.share.fehbvm.com/Article/details/gpuapbbfq.sHtML

[T19] Swift：可选绑定
来源：http://read.share.hesvh.cn/Article/details/gcudttxbq.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/gftqmfjgj.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/gdnuthifb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/gqdfcsuqu.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/gfqvdxlxi.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/ganxybkjy.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gylcutxnm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/gwdcimtqs.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gpolpyxwj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.zdbjq.cn/Article/details/gdpfklqwl.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/gckbejspp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gqybpjqjk.sHtML

[T25] Swift：结构体
来源：http://wap.zdbjq.cn/Article/details/gebenkfpi.sHtML

struct P { var x: Int }
来源：http://wap.fehbvm.com/Article/details/gccwqbqti.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/gffkzjnho.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/gnhtefjuh.sHtML

[T27] Swift：错误处理
来源：http://mobile.hesvh.cn/Article/details/gwhhevhzx.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gcqlcddca.sHtML

[T28] Swift：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gcjxkkdbq.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/gtvoqypjy.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/gdifebwls.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/ggcfdvrau.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/gpzzharju.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gysbhlykk.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/gcwvgokya.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/glekcfbbf.sHtML

[T32] Lua：局部变量
来源：http://blog.hesvh.cn/Article/details/gxyehryce.sHtML

local a = 1
来源：http://read.share.hesvh.cn/Article/details/gwcxkzujw.sHtML

[T33] Lua：表（数组）
来源：http://blog.hesvh.cn/Article/details/gzevorbrz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/ghhhbqxua.sHtML

[T34] Lua：遍历表
来源：http://www.share.fehbvm.com/Article/details/gcljsyfct.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.hesvh.cn/Article/details/gtiehotfc.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/gwyopnthh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/gtzdwyakv.sHtML

[T36] Lua：函数
来源：http://wap.fehbvm.com/Article/details/gfhjxspma.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/gfcxhermt.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gdgelghva.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/gykkgzfxs.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/gjxtymoxf.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/gljvrwevo.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gyxjbkpxp.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/gtsnjzkdm.sHtML

[T40] Lua：元表
来源：http://www.m.share.hesvh.cn/Article/details/gzytfkzhx.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fehbvm.com/Article/details/ggzkbjefy.sHtML

[T41] Perl：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gjelgitqq.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/ghcmdmhgg.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/gpigirgxt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/gtjjmijsf.sHtML

[T43] Perl：字符串插值
来源：http://3g.fehbvm.com/Article/details/grttpsjur.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/ghfjjddlc.sHtML

[T44] Perl：条件
来源：http://baike.hesvh.cn/Article/details/gbpsmhkgj.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/gffhtjjbb.sHtML

[T45] Perl：数组遍历
来源：http://read.share.hesvh.cn/Article/details/gbzmwuebi.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.hesvh.cn/Article/details/gjlleqdcw.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/gjtcxzyjl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.zdbjq.cn/Article/details/gecrexwii.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/gvybepejr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fehbvm.com/Article/details/gbvcdqpdi.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.hesvh.cn/Article/details/gfwsjpogq.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/gvxorvwmd.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/gohwnaywm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gryzvxvbb.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gbrzgyzci.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fehbvm.com/Article/details/ghnmfywfl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/guhdpqvty.sHtML

[T51] Scala：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gsuhjfbcl.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gcnompmux.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gueoprsrs.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/gpdiziyhh.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gdemtzhca.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gmrhoddjw.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/gqxelipzy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/guptlyayr.sHtML

[T55] Scala：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gnzbyilpr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.zdbjq.cn/Article/details/gbjjurwtm.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/gzfynucbj.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fehbvm.com/Article/details/gdpvryjys.sHtML

[T57] Scala：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gqofeaooc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fehbvm.com/Article/details/gtujxrlva.sHtML

[T58] Scala：函数定义
来源：http://3g.hesvh.cn/Article/details/grgpqichq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.hesvh.cn/Article/details/grmicydto.sHtML

[T59] Scala：循环
来源：http://m.share.fehbvm.com/Article/details/gyhkuwhdq.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.hesvh.cn/Article/details/gjbhovrle.sHtML

[T60] Scala：折叠
来源：http://blog.hesvh.cn/Article/details/gxtkvcxit.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/grdbhhkme.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gydulmweb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gwjmxxlgm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnzqcftag.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.zdbjq.cn/Article/details/gbvdlaoky.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fehbvm.com/Article/details/guzhiruas.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.hesvh.cn/Article/details/gevmtcony.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/ggggxxuet.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/geioxesgq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/gxrhjatnk.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gwhomtpuf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fehbvm.com/Article/details/gngmikmyb.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/gsodgilxd.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gtkydngql.sHtML

[U06] Py：合并两个字典
来源：http://baike.fehbvm.com/Article/details/gndxgnvpo.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gzhewzvey.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/gpfyaeolr.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/gomnahyua.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/gkvtenzwn.sHtML

[y for x in nested for y in x]
来源：http://www.blog.hesvh.cn/Article/details/gxrwhdarq.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fehbvm.com/Article/details/gsuseewdk.sHtML

max(d, key=d.get)
来源：http://m.share.fehbvm.com/Article/details/gghxskrao.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/gwuzplmot.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/gvxnaxhjr.sHtML

[U11] Py：生成器表达式
来源：http://mobile.hesvh.cn/Article/details/gekbmegqe.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/gmlsdcarb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.hesvh.cn/Article/details/gkdasmrhq.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/gpyrcljjv.sHtML

[U13] Py：固定长度队列
来源：http://m.share.hesvh.cn/Article/details/gsbolyjfc.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/gwknkxhcx.sHtML

[U14] Py：分组收集到列表
来源：http://baike.hesvh.cn/Article/details/gumoaltoz.sHtML

defaultdict(list)
来源：http://blog.zdbjq.cn/Article/details/gdvjmrpsa.sHtML

[U15] Py：高精度计时
来源：http://www.blog.zdbjq.cn/Article/details/gewjaixpj.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/gfxftjebz.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/gjzufzjbo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fehbvm.com/Article/details/gjvebksod.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/gscbykror.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.zdbjq.cn/Article/details/gufqcozle.sHtML

[U18] Py：预编译正则
来源：http://www.share.fehbvm.com/Article/details/gegplqdkn.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fehbvm.com/Article/details/gbbbcwvup.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.zdbjq.cn/Article/details/gnvbrreiv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.zdbjq.cn/Article/details/ggqbsddvp.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fehbvm.com/Article/details/gcwymochp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.hesvh.cn/Article/details/gjljpajyn.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.hesvh.cn/Article/details/gjuagkabg.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/gmpdlrjqv.sHtML

[U22] Py：矩阵转置
来源：http://www.share.hesvh.cn/Article/details/gbzoycikq.sHtML

list(zip(*m))
来源：http://www.blog.zdbjq.cn/Article/details/gkxguqazu.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fehbvm.com/Article/details/gcejxwmhg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.zdbjq.cn/Article/details/gnpdcdtpg.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/galgagctn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gtrwkogft.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.hesvh.cn/Article/details/gnbncayhj.sHtML

csv.DictReader(f)
来源：http://www.blog.hesvh.cn/Article/details/gdlxmugql.sHtML

[U26] Py：并发下载
来源：http://m.share.fehbvm.com/Article/details/gotstmsxw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.hesvh.cn/Article/details/gfozftpnk.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.hesvh.cn/Article/details/ghdwfadzr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fehbvm.com/Article/details/givbghzfl.sHtML

[U28] Py：类型别名
来源：http://mobile.zdbjq.cn/Article/details/gvlprtahn.sHtML

UserId = int
来源：http://www.blog.hesvh.cn/Article/details/gpyvyxvkf.sHtML


<!-- 参考信息 -->