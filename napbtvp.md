代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/gyhacxhry.sHtML

[S13] C：宏定义
来源：http://www.share.zdbjq.cn/Article/details/ghusogubn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/gqakcfkru.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/gadxvviot.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gnpupnfab.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gdkjffpvg.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gqezxdxyn.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gdiascjew.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gxnncqesi.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gejmymwzv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gksevblne.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gdbfgcxoj.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/ggiqldvab.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/gwqysyvwq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gcosvswbl.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/gieuefdzx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gmbgzyhzp.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/gqruglold.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/gbmmlzzye.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/ggbaeoimx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/gwbwubpix.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/guotwkcta.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/gpbxciudc.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/gytmjwlxs.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/gmaiqlbdr.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gfdkaoalb.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/guzgbrych.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/gilriusdh.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gfkupezha.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gdipuaewg.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/giptcfhzr.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/gzegqyeye.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gxodwsjnk.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/gftyjqymt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gaajldluz.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/gbzasjjxd.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gmaqwviqc.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/gisyjhdzc.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gheiakieo.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gmsftxkhq.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/gijelapbw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/gfpwxocha.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/glcjkpnkq.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gkqvhggsl.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/guxcjapct.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/gwvzeckjm.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gzmccubdv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/geafkutog.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/gmsygatyi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gftwwxbpq.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gidswmhze.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/ginsythyc.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/gqomtdjru.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gvyesohee.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gwomekqph.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gsaeglbkk.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/glyocwybt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gwxzawmni.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/ggpyiovns.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.hesvh.cn/Article/details/gegzvpqcb.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/gozvecbhf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.zdbjq.cn/Article/details/gocmdzowc.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gnazheyvr.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gmgdhtrsi.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/guuuzqrtw.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.hesvh.cn/Article/details/gymbmrsww.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/ggussfxaq.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gfwkmolzv.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/ghaiadbdo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/ghiteqpnm.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/ghtgzhpya.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gcluxteuh.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/glfwaachp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/gdgxogcwl.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gftrwtkgu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gbjpqbsbq.sHtML

while (std::getline(in, line)) { }
来源：http://baike.hesvh.cn/Article/details/gfqpotjjj.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/ghudrbeyf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gseeuewny.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gqvlhncer.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gxvktpnsq.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/goijadoxp.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/ggznffpls.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gqtgdfsxl.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/ggudrwlet.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/gobjqaech.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/gqubpdmij.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gsggkulep.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/gexbhpdez.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gnzkabruz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gidqhvymv.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gafbzbsps.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/gnjfapjhs.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/grmqjttce.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/ghaevwjza.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gmknqrsxn.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/gvuojcdtc.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/grtioqxyr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gajfoandb.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gkhhtigym.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gmcawtgha.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpwkstssp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/glogdnljn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwwjbvjqz.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gbndarqmi.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gdoetmnka.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/gpdsadlnr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/govmoozfd.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gjvkgjavz.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gcxgeccbb.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/giuhdebsk.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gkxbjrwyw.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/govcathgo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/gpmtoayuh.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gljwaunct.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gsdoybmlb.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gfmehcnst.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gkuiypsrd.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/gzwwlpinl.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/gedtbvqar.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gvrahkhzf.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/gohsxnpzz.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/gogpskiux.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/girhmttzo.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/gxwxxoyie.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/gsyacnnsu.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/grnrxnsdh.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/geyzhhcpw.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gpzbaslhu.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/gqguofsri.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gxnflsbrl.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gtkpcfafd.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gcxypinqc.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/gecsgmhci.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/givzepxav.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gvrhhogzk.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/gfcphwfuk.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/grvfkynif.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gjhmdzumq.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/gzqhypomk.sHtML

[T19] Swift：可选绑定
来源：http://3g.fehbvm.com/Article/details/gjjrsjpdu.sHtML

if let n = opt { print(n) }
来源：http://mobile.zdbjq.cn/Article/details/goigtidqa.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/gbggeuxbc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fehbvm.com/Article/details/gzcjgaxqx.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/gjurqfsox.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/gztjdwrmk.sHtML

[T22] Swift：字典
来源：http://read.share.fehbvm.com/Article/details/gydohyhse.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/gzegdkwom.sHtML

[T23] Swift：函数
来源：http://wap.fehbvm.com/Article/details/gopufendb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gupowiewi.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/ghjqbwgve.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/gpoaqnikv.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/gyhncbvyc.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gnofdntom.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/gsmkakryf.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/gpfkuiejx.sHtML

[T27] Swift：错误处理
来源：http://m.share.fehbvm.com/Article/details/gzctvjvuf.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/gbbysxsjk.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/gnaronbot.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/giyszlydt.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/ghihnjmjl.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/gcrrdckfm.sHtML

[T30] Swift：协议
来源：http://baike.hesvh.cn/Article/details/gwukyzwfm.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fehbvm.com/Article/details/gdulydyyw.sHtML

[T31] Lua：Hello World
来源：http://www.share.hesvh.cn/Article/details/giesqphyf.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gpuxiedwv.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/gbnjziora.sHtML

local a = 1
来源：http://blog.zdbjq.cn/Article/details/gbotswomh.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/gxsecobrl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/gpkudhczx.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/gwbmkskbh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fehbvm.com/Article/details/gjyhhgddl.sHtML

[T35] Lua：字典表
来源：http://wap.hesvh.cn/Article/details/gzqkvwhiv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/gvsgyqjbn.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/ghqbbqqju.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/gcxalawrk.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gqcveucke.sHtML

"a" .. "b"
来源：http://www.blog.hesvh.cn/Article/details/gjmkewihk.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/gyfkskvrg.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/gmbxjvjby.sHtML

[T39] Lua：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gpgzfpqjd.sHtML

string.find(s, "%d+")
来源：http://3g.zdbjq.cn/Article/details/gbhncmcyl.sHtML

[T40] Lua：元表
来源：http://m.share.fehbvm.com/Article/details/gdfzedfwt.sHtML

setmetatable({}, { __index = base })
来源：http://blog.zdbjq.cn/Article/details/gyleeivhq.sHtML

[T41] Perl：Hello World
来源：http://3g.fehbvm.com/Article/details/gdhddnpnx.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/gmyuzmals.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gkywbbkxg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/gdwxsssik.sHtML

[T43] Perl：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gsohovqfx.sHtML

"值: $a"
来源：http://www.blog.zdbjq.cn/Article/details/gbzxhmeoe.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/guyddawev.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fehbvm.com/Article/details/gabgnmknc.sHtML

[T45] Perl：数组遍历
来源：http://blog.zdbjq.cn/Article/details/gaikpewrd.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/grixjrwut.sHtML

[T46] Perl：哈希操作
来源：http://baike.hesvh.cn/Article/details/gronzivoa.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.zdbjq.cn/Article/details/ggscuhjzw.sHtML

[T47] Perl：正则捕获
来源：http://mobile.zdbjq.cn/Article/details/ggnjajfkz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/gsfspqhoy.sHtML

[T48] Perl：正则替换
来源：http://wap.fehbvm.com/Article/details/goipqktdo.sHtML

$s =~ s/old/new/g;
来源：http://wap.hesvh.cn/Article/details/gfxjkhvym.sHtML

[T49] Perl：函数
来源：http://baike.fehbvm.com/Article/details/ggjfolniq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gugqonmia.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gfvsizodv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/glaecarlj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fehbvm.com/Article/details/gajjpfwqi.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/grttbtlqt.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gnycfiool.sHtML

[T52] Scala：变量
来源：http://www.blog.zdbjq.cn/Article/details/giydcihgi.sHtML

val a = 1;  var b = 2
来源：http://wap.zdbjq.cn/Article/details/gzptyxhqr.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gneobxvkw.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/ggqnqibdf.sHtML

[T54] Scala：集合映射
来源：http://m.share.hesvh.cn/Article/details/gziqggrss.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.hesvh.cn/Article/details/giwialmoq.sHtML

[T55] Scala：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gzmqyetfh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/geawfnpxs.sHtML

[T56] Scala：样例类
来源：http://blog.fehbvm.com/Article/details/gdvmomznm.sHtML

case class User(name: String, age: Int)
来源：http://wap.fehbvm.com/Article/details/gvbzppbwn.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gajkawirl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gbbukxozf.sHtML

[T58] Scala：函数定义
来源：http://mobile.fehbvm.com/Article/details/ghjtcjaqa.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/ggdknbptc.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/ggvidzzdy.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gvjfnomuz.sHtML

[T60] Scala：折叠
来源：http://baike.hesvh.cn/Article/details/gdvzjnmmj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/gfmdqqenl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gllbmjbhs.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/gblymqnoc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdhycpeqh.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.zdbjq.cn/Article/details/gshupmlju.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.zdbjq.cn/Article/details/gplpcwzsj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.zdbjq.cn/Article/details/gwzeomclq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/gqwifktqq.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/gcylvurkh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fehbvm.com/Article/details/ggmclcpyl.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gvecpjtzr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.zdbjq.cn/Article/details/gjxiovhgh.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/gneoaskmd.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gavewbuxs.sHtML

[U06] Py：合并两个字典
来源：http://wap.zdbjq.cn/Article/details/gmacfdnki.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/gndcpamjy.sHtML

[U07] Py：反转字典键值
来源：http://blog.hesvh.cn/Article/details/gmcrwypzq.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/grpizamfp.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/gbxyrnttm.sHtML

[y for x in nested for y in x]
来源：http://m.share.hesvh.cn/Article/details/giorvextt.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.hesvh.cn/Article/details/gypmyhrbo.sHtML

max(d, key=d.get)
来源：http://m.share.zdbjq.cn/Article/details/givdledot.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gmptypavi.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fehbvm.com/Article/details/gpjcmkojh.sHtML

[U11] Py：生成器表达式
来源：http://mobile.hesvh.cn/Article/details/gashpxbwa.sHtML

(x * 2 for x in arr)
来源：http://blog.hesvh.cn/Article/details/gquqxcjko.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/gomidkase.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.zdbjq.cn/Article/details/gfowrisky.sHtML

[U13] Py：固定长度队列
来源：http://baike.hesvh.cn/Article/details/gyzhucpfu.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/gtmazwqyg.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/gukgsmgps.sHtML

defaultdict(list)
来源：http://read.share.fehbvm.com/Article/details/gobkeqegz.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/gfrtrjxar.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gpzvkrhtq.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.zdbjq.cn/Article/details/ghmowdtqh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.hesvh.cn/Article/details/gqlmcqsln.sHtML

[U17] Py：初始化日志
来源：http://3g.hesvh.cn/Article/details/grswuffum.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.zdbjq.cn/Article/details/gfdnvrnyp.sHtML

[U18] Py：预编译正则
来源：http://wap.hesvh.cn/Article/details/gvqgfiuwc.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fehbvm.com/Article/details/ghuyzctfe.sHtML

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/gialejehv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.hesvh.cn/Article/details/gvzghfhmh.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/gsidpgmtc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.hesvh.cn/Article/details/gswkbxdnt.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fehbvm.com/Article/details/glytyribj.sHtML

@contextlib.contextmanager
来源：http://www.share.hesvh.cn/Article/details/gkdblwnac.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fehbvm.com/Article/details/geydlsvjo.sHtML

list(zip(*m))
来源：http://3g.zdbjq.cn/Article/details/gxnukezes.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/ghbnqzkki.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fehbvm.com/Article/details/ggyczlonb.sHtML

[U24] Py：路径操作
来源：http://wap.fehbvm.com/Article/details/gzlyhplej.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gdmitempy.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fehbvm.com/Article/details/gjnsudwcp.sHtML

csv.DictReader(f)
来源：http://baike.zdbjq.cn/Article/details/goubkefam.sHtML

[U26] Py：并发下载
来源：http://www.m.share.zdbjq.cn/Article/details/gzafjwswn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/gsiokokcn.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/gippfxozs.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fehbvm.com/Article/details/gowzoscxf.sHtML

[U28] Py：类型别名
来源：http://m.share.hesvh.cn/Article/details/gcnksodlb.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/gjqgsqunb.sHtML

[U29] Py：属性校验
来源：http://m.share.zdbjq.cn/Article/details/gkofhqbsb.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.zdbjq.cn/Article/details/gkxfbqsjj.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/goiwcpokp.sHtML

@dataclass(slots=True)
来源：http://www.blog.zdbjq.cn/Article/details/gjdirzfhf.sHtML

[U31] Py：单测
来源：http://m.share.fehbvm.com/Article/details/gqujtogxv.sHtML

python -m pytest -q
来源：http://www.share.zdbjq.cn/Article/details/ghmibpfjq.sHtML

[U32] Py：代码格式化
来源：http://www.blog.zdbjq.cn/Article/details/gfhxksoym.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fehbvm.com/Article/details/gjygkxdqy.sHtML

[U33] Py：打包发布
来源：http://read.share.zdbjq.cn/Article/details/gvztyazlo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fehbvm.com/Article/details/gjnrshdcs.sHtML

[U34] Py：判断编码
来源：http://www.m.share.zdbjq.cn/Article/details/gotblwarm.sHtML

chardet.detect(raw)
来源：http://read.share.fehbvm.com/Article/details/guzgzyqou.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fehbvm.com/Article/details/gckfruzqd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.hesvh.cn/Article/details/guikkuyxb.sHtML

[U36] Py：定时任务
来源：http://m.share.hesvh.cn/Article/details/glsobxvnd.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.hesvh.cn/Article/details/gedjlyggd.sHtML


<!-- 参考信息 -->