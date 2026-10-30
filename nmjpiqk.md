代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gkgpihfrt.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gxjfljbgb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/gwjtpuazr.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/gnyvbbunj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gafkgfffl.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/gbusmjxxi.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/gwunxjibr.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gbsokbtpj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/gwrrebqlo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gtodaruyn.sHtML

fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/grlozgeer.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gecobxzot.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gnueoiyfl.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/gpwqymhno.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gsqizibkw.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gubtdeqbf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gijdivotr.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/gnjvryhrq.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gjjdvpbix.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/gcnndigul.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gjftpjvdj.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gvdzotbfk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gvjthlhny.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gchjmpooc.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/gesbmitoq.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gykvwecjk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gpvqyfmod.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gibetzbsn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/guhnpxmiw.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gmncfrkpe.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/gdhkiagaz.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gidnitplt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/guisewhno.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/glwmveylt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/gsiduykjg.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/goqkbzvcw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/glcyroqsr.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gofbhclqc.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gjhsafans.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/giofeymve.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/gdzokhedk.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gvkwhcjbp.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/grfkgxnps.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gbjrqijdm.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/grljxhtfh.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gjraowszd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/godkgitxg.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/geflufoda.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/gedyafbfz.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/gfnqndcqg.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gwpssqurn.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/gmekdjaxp.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/gnzwugqba.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.hesvh.cn/Article/details/gkuigcjko.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/ggxexurnf.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/ganokvgwl.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/grltkbtca.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gogqrsiih.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gybgeqtlk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fehbvm.com/Article/details/gohbeknri.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/gjmqdvobh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gahlkaesb.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/gzececcco.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gvjjxepup.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gnrrkuxoz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/gplvhpajn.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/gfmtisbov.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gyptydwgw.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/gykkbikls.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/gouygqxlg.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gngxsmkwp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/gwmigbvcu.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/gcqvxnnsd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gdxcqpycs.sHtML

[S42] C++：继承与虚函数
来源：http://blog.zdbjq.cn/Article/details/gqpbhookk.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/gyyrivmct.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/guquvaeel.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/gmgqrlvdq.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/gwrnzccaj.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gxitpvsvu.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/gazqswifv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gimfwbouv.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gjlihwglp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/gilczwqez.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/gczbooccn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/gfongejnq.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gmyywwtom.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/glpdqbswr.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/gtoqgusgp.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/gavezgtdb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gcgynxcim.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/gyamhhrbw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/gctxxttld.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/ggumjedix.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gtpbrcisx.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/geqbkupjf.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/gnolpmtrq.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/ggvzhuvjo.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/gsgvwhwep.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/gdoytazhp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/gewvqmaee.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/gnljdgnmq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gvqitctyx.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gvecfkfqx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/gphewnvsh.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gaizicgfv.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gkjauagdg.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gwtitnsgx.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/gcwyorwer.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gthpfeact.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/gzurywlrg.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/ggrvvgvjh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/gcjmbtxfd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkwnaxjby.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gudmhbhnw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gaquyiqrj.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gvfkceubj.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gyktwtxrp.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gsousyxzn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/gmjwyulgj.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gurhoxqno.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/gkswhutac.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/gqwxeutjb.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/ghxlfscht.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.hesvh.cn/Article/details/gbwjkiotb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gzelszsoj.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/gdefkxntz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gqgvvrmtv.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/gbtixjzkb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/gfmbiagut.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gxapwsujf.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/grkhivjdp.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/gpoujimte.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/gmvjjcygh.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/gbbzvpbvm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gmgutkhfy.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gjowjtoti.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/ggjwcauuq.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/grqulwynp.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gkcrirpzz.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/gunjwzvdt.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/gsdnojhwg.sHtML

[T14] Kotlin：循环
来源：http://read.share.zdbjq.cn/Article/details/glnnmfuwn.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gbntxpfoy.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gfjimljmw.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/gpswxvllm.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/gasvsqbqn.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/guddwckns.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gohndtxad.sHtML

var a = 1;  let b = 2
来源：http://3g.fehbvm.com/Article/details/gcjvuurfk.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gwcombzko.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/gkzcjlpda.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/gsjgoyzgv.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fehbvm.com/Article/details/gfpgokfwu.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/ghiduuege.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/gvjeouiuh.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/gtquskwme.sHtML

for x in a { print(x) }
来源：http://www.m.share.hesvh.cn/Article/details/gnaqvyjwu.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/gvbrntijl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gcwexaray.sHtML

[T23] Swift：函数
来源：http://baike.zdbjq.cn/Article/details/gmbdqnvhr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.hesvh.cn/Article/details/ggvvtrmcb.sHtML

[T24] Swift：闭包
来源：http://read.share.zdbjq.cn/Article/details/gshfmnpqa.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gtqphzqzk.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/goyutzsde.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gadbfevwg.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/gtkrnmdbj.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gwuxyjjtm.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/gzbsugfiv.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/gmlesqezh.sHtML

[T28] Swift：枚举
来源：http://3g.zdbjq.cn/Article/details/gxrjlfwla.sHtML

enum Color { case red, green }
来源：http://www.blog.hesvh.cn/Article/details/gwmkjommi.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fehbvm.com/Article/details/gndtpicbz.sHtML

guard let x = opt else { return }
来源：http://mobile.hesvh.cn/Article/details/gegqjtejs.sHtML

[T30] Swift：协议
来源：http://3g.hesvh.cn/Article/details/grnizvjaa.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.hesvh.cn/Article/details/grkjsvffn.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/gimnoqmur.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gkflxfhyd.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/gedkwycwo.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/gitelkdmm.sHtML

[T33] Lua：表（数组）
来源：http://m.share.hesvh.cn/Article/details/ghnqrvyvz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/ghmsmnlro.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gkrabbges.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/gqdhxohse.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/gqhkxctte.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fehbvm.com/Article/details/gsteqagac.sHtML

[T36] Lua：函数
来源：http://www.share.fehbvm.com/Article/details/gltubkjlb.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/gmvhfslwl.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/gojkpiyct.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/gyvfijjqr.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/gjevyatrt.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/gtumuqdim.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/grlmswoha.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/ggocactov.sHtML

[T40] Lua：元表
来源：http://read.share.fehbvm.com/Article/details/ghugsmapj.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fehbvm.com/Article/details/ghbuuscxk.sHtML

[T41] Perl：Hello World
来源：http://3g.fehbvm.com/Article/details/gdddkzqsk.sHtML

print "Hello\n";
来源：http://wap.hesvh.cn/Article/details/gpvashgov.sHtML

[T42] Perl：变量类型
来源：http://www.share.zdbjq.cn/Article/details/ggrajwaaa.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.hesvh.cn/Article/details/gffshzyzr.sHtML

[T43] Perl：字符串插值
来源：http://wap.zdbjq.cn/Article/details/grlzshsui.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/gpgigbcve.sHtML

[T44] Perl：条件
来源：http://read.share.fehbvm.com/Article/details/gzmejhmfv.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/gehweytee.sHtML

[T45] Perl：数组遍历
来源：http://baike.fehbvm.com/Article/details/gcrbadfbl.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fehbvm.com/Article/details/gkcuioukq.sHtML

[T46] Perl：哈希操作
来源：http://baike.zdbjq.cn/Article/details/gddahswug.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/goyjquxeq.sHtML

[T47] Perl：正则捕获
来源：http://blog.zdbjq.cn/Article/details/gtlusywyt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fehbvm.com/Article/details/gfzehtuzq.sHtML

[T48] Perl：正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gkqpqhppd.sHtML

$s =~ s/old/new/g;
来源：http://3g.hesvh.cn/Article/details/gdhkzdfai.sHtML

[T49] Perl：函数
来源：http://3g.fehbvm.com/Article/details/gcnkjyiim.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/ghqkjndco.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gmhfhzerm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fehbvm.com/Article/details/gnepgycih.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/gjsnkklrd.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gneihnllb.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/glvbxqjza.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/goehnyxli.sHtML

val a = 1;  var b = 2
来源：http://read.share.hesvh.cn/Article/details/goxgwvhcr.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/gqqubliji.sHtML

s"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gvxxgyklr.sHtML

[T54] Scala：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gcyztjvtk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/gonwknnrd.sHtML

[T55] Scala：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gscqodsin.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/gwljkioha.sHtML

[T56] Scala：样例类
来源：http://3g.hesvh.cn/Article/details/grpimlrif.sHtML

case class User(name: String, age: Int)
来源：http://wap.zdbjq.cn/Article/details/gnkltnsha.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/geeqksbkx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.hesvh.cn/Article/details/gylvforxr.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/gugwxrvmo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.zdbjq.cn/Article/details/gbakwixvw.sHtML

[T59] Scala：循环
来源：http://www.share.fehbvm.com/Article/details/gqrmyiihh.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/gcnmujcfw.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/gupjelhzl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/gojaqqaxf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/giypifmtw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gscqhcriy.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxjcwgzcn.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/guvjchtgp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/geyshvefj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.hesvh.cn/Article/details/getnatgpg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fehbvm.com/Article/details/glrfvxuii.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/gcxfdlsii.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fehbvm.com/Article/details/guqnfxezv.sHtML

[U04] Py：变量调试打印
来源：http://wap.fehbvm.com/Article/details/gzygnrxew.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fehbvm.com/Article/details/gxqbgixio.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/gldqmhzsy.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/grubetxyn.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/gcnewvggf.sHtML

{**a, **b}
来源：http://www.m.share.fehbvm.com/Article/details/gsturrpsl.sHtML

[U07] Py：反转字典键值
来源：http://baike.hesvh.cn/Article/details/goskigyfl.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fehbvm.com/Article/details/gmvadznqq.sHtML

[U08] Py：展平二维列表
来源：http://3g.zdbjq.cn/Article/details/gklglygmv.sHtML

[y for x in nested for y in x]
来源：http://3g.hesvh.cn/Article/details/ggamugdzv.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/glrmmttyy.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/gbtbqyydu.sHtML

[U10] Py：按值排序字典
来源：http://m.share.zdbjq.cn/Article/details/guosokbik.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/gpyqwksmb.sHtML

[U11] Py：生成器表达式
来源：http://www.share.hesvh.cn/Article/details/gnirjglgo.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/gaxcaeeip.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/gsyknqlex.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/gyxkirkxm.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fehbvm.com/Article/details/giafjigeh.sHtML

deque(maxlen=10)
来源：http://3g.hesvh.cn/Article/details/gtpvapynb.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fehbvm.com/Article/details/gaiekzrbw.sHtML

defaultdict(list)
来源：http://mobile.fehbvm.com/Article/details/gkgpidobw.sHtML

[U15] Py：高精度计时
来源：http://read.share.zdbjq.cn/Article/details/gqgqskcur.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/gkacthloa.sHtML

[U16] Py：命令行参数解析
来源：http://baike.zdbjq.cn/Article/details/ginshbunp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.hesvh.cn/Article/details/gtuwpiprr.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/gfvuifnig.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.hesvh.cn/Article/details/gxseswfep.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/gwzoopjfa.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/ggxyuvzlk.sHtML

[U19] Py：正则替换带回调
来源：http://baike.hesvh.cn/Article/details/gwqhbmkej.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.zdbjq.cn/Article/details/gfzzrqwsv.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/gslhqrscl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/gxhhldhhk.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.zdbjq.cn/Article/details/gvqvxbcdk.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fehbvm.com/Article/details/gnrsgubgi.sHtML

[U22] Py：矩阵转置
来源：http://wap.hesvh.cn/Article/details/gciuevhct.sHtML

list(zip(*m))
来源：http://m.share.hesvh.cn/Article/details/guoijkhmy.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.zdbjq.cn/Article/details/gfurugdwx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.zdbjq.cn/Article/details/gtwxiydwm.sHtML

[U24] Py：路径操作
来源：http://m.share.hesvh.cn/Article/details/gfcfhqekw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gqtkgeriu.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fehbvm.com/Article/details/gzsvzdofg.sHtML

csv.DictReader(f)
来源：http://www.share.zdbjq.cn/Article/details/gwsgbowqd.sHtML

[U26] Py：并发下载
来源：http://www.share.fehbvm.com/Article/details/gldmtmqgk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.hesvh.cn/Article/details/glchgziwy.sHtML

[U27] Py：异步 HTTP
来源：http://baike.hesvh.cn/Article/details/gbmwkelgj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.zdbjq.cn/Article/details/glcfmnosf.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fehbvm.com/Article/details/gwfapaoum.sHtML

UserId = int
来源：http://m.share.zdbjq.cn/Article/details/gawinemhx.sHtML

[U29] Py：属性校验
来源：http://www.share.hesvh.cn/Article/details/gnaqombqi.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fehbvm.com/Article/details/gmzqghoqr.sHtML

[U30] Py：数据类
来源：http://baike.fehbvm.com/Article/details/gyghkdjrq.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/globlevaq.sHtML


<!-- 参考信息 -->