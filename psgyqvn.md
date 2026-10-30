代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gedlpmxxl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/gjnsgtzrb.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/griahsvdi.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/gqyugputj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gtbwiumee.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gcbhirhix.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gmcbffgux.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/gouadtpce.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/gwcswdlgf.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/gmpkjuezl.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/grxvralgw.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/gedosgwvd.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/ghrdilcym.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gnbthtcdj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gnnuxcfbl.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/gavsvairr.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gkyrxayxu.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gftruvtqs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gbqvgctdl.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gezguydvt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gyfrethpo.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gbhzfxcnw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gayyjaiik.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gmanptrci.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gwrfsdpvx.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gpybkaqbb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/gqqfyumez.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gwrsukvmt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/gbiptbswj.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gqtopooka.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/gkecsogvd.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/gjisuofem.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/glqpmsnjv.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/gfsuuwshg.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gonxteuwy.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/ggpbbcuko.sHtML

static int counter = 0;
来源：http://read.share.fehbvm.com/Article/details/gonrljins.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/grbavhwen.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/gyjxvrjwg.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/gyhzyvxvw.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/ggvfdpyle.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/gkipskkvp.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gghnsicku.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/gullhtrcx.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gbqwudtji.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/gaiydtail.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/gwspvqyja.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gkkmthdar.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/gtbtulgxf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/gzngygtus.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/gjjxicfbx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gvsenjvtg.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gywnhcjjy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/glcfzlfml.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/gmepzuoqm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/guxpxjvxi.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/gsjdyejxj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/giduskhsu.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gqubecnzv.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gztuhobmk.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/gomcvywoa.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gntnfertg.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/gfznivmdr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/gizrtujvp.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/grtlvncog.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/gntrusilb.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/gulsasifu.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/gwkgiqfwr.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/giuagkjiv.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/gioojtckt.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/gslwsniar.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gnabdgdvh.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gpeygrzdp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gdvsnsxep.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/ghaowifxx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gpyvwyplh.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gagriugmc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.hesvh.cn/Article/details/ghwxnsyxw.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gqforlfll.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/gitvfrqtg.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/gwirauesy.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gwedmxjtz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/gnxmqxwsq.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/gbvliwpbf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gjookdang.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/gyfzowpyq.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gombzgpft.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/gexkefgyx.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/gwozpttxi.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gpxmzbgwe.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gdoneoonk.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/gvulajttj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/goguupcep.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gcgwizafg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gfvzclypx.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/gdqesbtva.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gtdmecqfy.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/gdhcinfeb.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/gwvrhxyru.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/goewyphcj.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/gyykxegbw.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/gytpxaaho.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gsrpumdjc.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/gfzdfszbz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gbmgxrcbb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqplpkecx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/golhaaiml.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmdhuqvdi.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gpoxezwjj.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gtgellgpi.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/giodohdag.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gllleugnv.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gtebviozt.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gpfrjaqpc.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/gbpudljcm.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/gwyzzvpwq.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/gfbmsglxq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gfmfmywco.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gfbkwttpu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gpozyfara.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/gaktmyrkt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/gjofwclwx.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/grdtjslmo.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gvcubnjde.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/ghgdbdsce.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gkxokitxc.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/gtwvjcwyb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/glyqqvwzt.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/gjnvakijz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gjfxkczap.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/gwjahczzt.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gmvszcxjz.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gxyvpicat.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gvhfeupya.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gbnehjedj.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gynvlszvl.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gpfoqwvvx.sHtML

interface Shape { fun area(): Double }
来源：http://blog.hesvh.cn/Article/details/gxcqmbtgu.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/gluoekitm.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gfuovniek.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gijuniapz.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/ggpvqhlnw.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/gfsmbjaom.sHtML

"值: \(b)"
来源：http://www.blog.hesvh.cn/Article/details/gryuormlg.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/gwoklpvcf.sHtML

if let n = opt { print(n) }
来源：http://read.share.hesvh.cn/Article/details/gfecdvenz.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gwznveeep.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gpctrclql.sHtML

[T21] Swift：遍历
来源：http://www.blog.fehbvm.com/Article/details/gjifhpemh.sHtML

for x in a { print(x) }
来源：http://www.m.share.hesvh.cn/Article/details/gryrudkyr.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gkqsqpfcy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/gzpaxsswi.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/gpmfrzbmi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/gjiexpnvh.sHtML

[T24] Swift：闭包
来源：http://www.blog.fehbvm.com/Article/details/gidxmokdd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gqazucwrn.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/gzpocheoi.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gejqsgiqv.sHtML

[T26] Swift：类与重写
来源：http://www.blog.zdbjq.cn/Article/details/gevrbnzni.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/ghlgqbupx.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/gneqeggcu.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/gsnuwttvf.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gdflfbawx.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/geyvjfjxe.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.hesvh.cn/Article/details/gtffjjxsv.sHtML

guard let x = opt else { return }
来源：http://www.blog.fehbvm.com/Article/details/ghefdgzch.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/gqdntgjdm.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/gudycmtyj.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/grpxzyxzi.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gwfltxkdz.sHtML

[T32] Lua：局部变量
来源：http://www.share.fehbvm.com/Article/details/gpyrbvmve.sHtML

local a = 1
来源：http://read.share.hesvh.cn/Article/details/gdrigpakl.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gyoxjvuaz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gyepkpjee.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/gwypgsoqv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.hesvh.cn/Article/details/gpqthjhwb.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/grppameqb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/grixmmcox.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/gnmdldbkx.sHtML

function add(a, b) return a + b end
来源：http://mobile.hesvh.cn/Article/details/gswtrlxgk.sHtML

[T37] Lua：字符串拼接
来源：http://wap.hesvh.cn/Article/details/gbjxgoaic.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/gtcznbsfo.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/gcgywpjfw.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/gyvpnmbpl.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gbfyuhxqj.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/gvkksannr.sHtML

[T40] Lua：元表
来源：http://www.share.hesvh.cn/Article/details/gsefkepmd.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fehbvm.com/Article/details/gvblpvnqt.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/ggvhkloww.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/gybfbbcfh.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/ggmkorpzy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fehbvm.com/Article/details/gbmmasana.sHtML

[T43] Perl：字符串插值
来源：http://baike.fehbvm.com/Article/details/gkgbtbokp.sHtML

"值: $a"
来源：http://read.share.zdbjq.cn/Article/details/gpchkgrfw.sHtML

[T44] Perl：条件
来源：http://mobile.hesvh.cn/Article/details/guklaninn.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.hesvh.cn/Article/details/gnonsunqj.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/gwygfyuqv.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.zdbjq.cn/Article/details/gcklnhxpr.sHtML

[T46] Perl：哈希操作
来源：http://wap.hesvh.cn/Article/details/gtkuushto.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fehbvm.com/Article/details/gvekjsnut.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/glhinzhds.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fehbvm.com/Article/details/gszyvkkty.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gtxysorow.sHtML

$s =~ s/old/new/g;
来源：http://www.share.hesvh.cn/Article/details/gsndvaqjn.sHtML

[T49] Perl：函数
来源：http://www.blog.zdbjq.cn/Article/details/gtyqaejll.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gberyrpyu.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gdfswbvey.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.zdbjq.cn/Article/details/gdargjndb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/gwxwpjbpx.sHtML

[T51] Scala：Hello World
来源：http://read.share.fehbvm.com/Article/details/gardxcuns.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gabtxamky.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/grwcfqjta.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/gevfvftxp.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fehbvm.com/Article/details/ggqgqgmvj.sHtML

s"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gvksbatzs.sHtML

[T54] Scala：集合映射
来源：http://mobile.hesvh.cn/Article/details/ghnitacxd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/grpzlgyyj.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/gvctukeed.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.zdbjq.cn/Article/details/goeyfuedb.sHtML

[T56] Scala：样例类
来源：http://wap.fehbvm.com/Article/details/gipkpvzyq.sHtML

case class User(name: String, age: Int)
来源：http://m.share.hesvh.cn/Article/details/gbxfwwqri.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gyyxyhisk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.hesvh.cn/Article/details/gzbquypfq.sHtML

[T58] Scala：函数定义
来源：http://read.share.zdbjq.cn/Article/details/gqclzzawn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gqewezaeo.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gzgeoxhww.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/gvscuyryk.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/gcyiqdimt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fehbvm.com/Article/details/gjtczcfem.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/goyrpxomt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/ghwxyqvrg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grjympjet.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/gwgtsufut.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fehbvm.com/Article/details/grfiplwtu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/gdsrqchic.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.hesvh.cn/Article/details/guteqetfv.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.zdbjq.cn/Article/details/gtlizmpvv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fehbvm.com/Article/details/gubsykfhh.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fehbvm.com/Article/details/gdvecnmxe.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.hesvh.cn/Article/details/gdayzelcs.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fehbvm.com/Article/details/gqrbutwjj.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gsrpwpipf.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fehbvm.com/Article/details/gmdjkhvmf.sHtML

{**a, **b}
来源：http://baike.fehbvm.com/Article/details/gtulqaeqg.sHtML

[U07] Py：反转字典键值
来源：http://3g.hesvh.cn/Article/details/gheccmzoo.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fehbvm.com/Article/details/gbijnmhor.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/glkftsqjh.sHtML

[y for x in nested for y in x]
来源：http://baike.zdbjq.cn/Article/details/glrqcuzho.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/gvulglkwx.sHtML

max(d, key=d.get)
来源：http://read.share.zdbjq.cn/Article/details/gximfoypy.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fehbvm.com/Article/details/glwuajycd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/gapolzovi.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/gtumxugud.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fehbvm.com/Article/details/guxhawunp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/glukyveym.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/gzosbqhnl.sHtML

[U13] Py：固定长度队列
来源：http://3g.zdbjq.cn/Article/details/gndornxlc.sHtML

deque(maxlen=10)
来源：http://read.share.fehbvm.com/Article/details/gpsupeajr.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.zdbjq.cn/Article/details/gmmlgkkck.sHtML

defaultdict(list)
来源：http://www.share.fehbvm.com/Article/details/gjlvozjkt.sHtML

[U15] Py：高精度计时
来源：http://m.share.zdbjq.cn/Article/details/gfqttiqra.sHtML

t = time.perf_counter()
来源：http://wap.hesvh.cn/Article/details/gdpwilcra.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/givqvdhhw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.hesvh.cn/Article/details/gowzicopj.sHtML

[U17] Py：初始化日志
来源：http://m.share.fehbvm.com/Article/details/grolaokyq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.hesvh.cn/Article/details/ggeglfazn.sHtML

[U18] Py：预编译正则
来源：http://m.share.zdbjq.cn/Article/details/gdznxshyv.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gfwxvkioq.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.hesvh.cn/Article/details/ghlfvxjdm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/geeosdmau.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fehbvm.com/Article/details/gykfzunfg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.zdbjq.cn/Article/details/gvumhwpcj.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.zdbjq.cn/Article/details/goudbdati.sHtML

@contextlib.contextmanager
来源：http://www.blog.zdbjq.cn/Article/details/gjffvykrq.sHtML

[U22] Py：矩阵转置
来源：http://m.share.hesvh.cn/Article/details/gkhqwirqo.sHtML

list(zip(*m))
来源：http://3g.zdbjq.cn/Article/details/gjrsygtyd.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.zdbjq.cn/Article/details/gnlplggju.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/gpywgbbby.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/ggngobsrk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gjuxguktb.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.zdbjq.cn/Article/details/gpgdwoemh.sHtML

csv.DictReader(f)
来源：http://www.share.zdbjq.cn/Article/details/gbqjfvizg.sHtML

[U26] Py：并发下载
来源：http://mobile.zdbjq.cn/Article/details/gbsnjtzvj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/gmyqhxems.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.zdbjq.cn/Article/details/gawpwshyn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.zdbjq.cn/Article/details/gggwurwqd.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/gmvcuizwk.sHtML

UserId = int
来源：http://wap.fehbvm.com/Article/details/gaqocexkh.sHtML

[U29] Py：属性校验
来源：http://www.m.share.zdbjq.cn/Article/details/gkiohbvde.sHtML

@property 与 @x.setter 配合
来源：http://3g.zdbjq.cn/Article/details/ggmnswgzp.sHtML

[U30] Py：数据类
来源：http://blog.fehbvm.com/Article/details/gjwuypxfv.sHtML

@dataclass(slots=True)
来源：http://www.blog.hesvh.cn/Article/details/gtgcqkjly.sHtML

[U31] Py：单测
来源：http://www.m.share.fehbvm.com/Article/details/gjxmyeglw.sHtML

python -m pytest -q
来源：http://www.blog.fehbvm.com/Article/details/gxzkkstep.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/gbgowkdaq.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.hesvh.cn/Article/details/glnohdhyr.sHtML

[U33] Py：打包发布
来源：http://baike.hesvh.cn/Article/details/gefcbziel.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/ggjbzsjyi.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/gxatbsxqq.sHtML

chardet.detect(raw)
来源：http://mobile.hesvh.cn/Article/details/gaztywtek.sHtML


<!-- 参考信息 -->