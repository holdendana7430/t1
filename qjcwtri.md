代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/gyqqpcujp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/gpejwfguo.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/gnzsiltvy.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/gojlafwyj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/glrtxufgz.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/gkhydhxmr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gwqefsgzt.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/gjvhtvcrq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/guxwibtqm.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/glzexnvcs.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gjflprmom.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/glizopkul.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/gukfffmyl.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gisnwhfwc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/gnwfwkiuc.sHtML

[S18] C：命令行参数
来源：http://3g.fehbvm.com/Article/details/gwubkowir.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gvitwgtbz.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gsloaesnq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/ghojrdkme.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/gwtyotaom.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gcxcnjfsk.sHtML

[S21] C：字符类别判断
来源：http://www.blog.hesvh.cn/Article/details/gdvhcytcn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/gkazcsxik.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gvuejejmc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/gzoxornid.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gcezvgyeb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/gqckqjkbp.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/gsbmqiwuz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/gzgwlzwbz.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/gjtrkncyw.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/gufldcmyj.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gbtsctlpj.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gubkowtpu.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/glywmuhug.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gybbywsgv.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gyvaioxyd.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/grrfchgzx.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/gkmkwosuw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/guemzwckp.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/gevsgutam.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/ggthpdbfh.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gwrvsxqmw.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/gyopkldbh.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/gwzdksrro.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/gwtsipyoq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/gjaxsghda.sHtML

[S32] C++：字符串
来源：http://baike.hesvh.cn/Article/details/gvekmslbq.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/geixvsqpk.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/gotohtygf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gjdhleagz.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/gacshgclu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gkdetbxqg.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/giwtlhlos.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gdaygoefc.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gcmieznup.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gjtfxfpsl.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gnimjbhoi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/gfstibfxj.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/gpzhhiwns.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gtdtaygxe.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/gnxjqdkca.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gpzrqmqzu.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/ghjxzgble.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gycedwnvw.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gmrxvmjee.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/guaphadol.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gsdbupvsh.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gtvhmrwfz.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/gexzyivjh.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gauecsppk.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gsllbfvcc.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/gvymgppcb.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/gtvhlemvz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/ggqgczlmx.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/gbhyfxnmj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gjxbnulvk.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/gsmnipfru.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gqicasxbt.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gpwbnbqqu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/geqmdnjgn.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/gzcdzxomz.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/gucvusjeo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/gqwbdrkst.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/giutklgez.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gmzlqaqok.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/goftteznl.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/ghbflxddi.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fehbvm.com/Article/details/gxsdkmfup.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/ghsktyoor.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/gecisxouo.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/ggjhipxdi.sHtML

[S54] C++：异常处理
来源：http://baike.fehbvm.com/Article/details/ggoxxqgqu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gfblttnbi.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/gfeuhadks.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/ghhczfptp.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/gulmpmnxx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/gwwqpqsuo.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/gqoopmvle.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/gqhbslgoz.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/gsqallvrl.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/grlnqkxon.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/gmyjiiven.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/ghlirdiot.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/ggqwifnom.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fehbvm.com/Article/details/gzjoigmxk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxrtoyblx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/glvcxihhn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gaxokcbcv.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gygxnfasa.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gdxttpbis.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/ghaopdnow.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/guxklitpz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/geqbzufvq.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gwxlkeqby.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gbmtqvigc.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/goxacinlc.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gmmzjtijq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/goirpozpa.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/ggygziaip.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fehbvm.com/Article/details/gxslghvid.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gaqksmweh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/gzeqlpoah.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gihwfjboz.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gmkkpvlwy.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.hesvh.cn/Article/details/gxrjodsfp.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/gvobljkbn.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/glhomaygp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gcscoochq.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/gnhxpxdlf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gfljscsqj.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/gcosqjrkt.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gojgiczqd.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gxkqhnrdg.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/gskdpposd.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/gxdjaabfg.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/gspdjfoni.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/gtrtanqut.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/gevcxcuvv.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/ghpgneqqp.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/goglvkbwd.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/gvshrhnyx.sHtML

var a = 1;  let b = 2
来源：http://www.share.hesvh.cn/Article/details/galyxgmzt.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/glhalazpi.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/glgoimfxz.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/gbcynvwjc.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/gkpbgofxm.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/gcpeauglv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/gdzudkiai.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gpcuncvgi.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/ggvhmepyp.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/gywffvekf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fehbvm.com/Article/details/gbyusuzzd.sHtML

[T23] Swift：函数
来源：http://m.share.zdbjq.cn/Article/details/gykjkiidg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/gimlrazib.sHtML

[T24] Swift：闭包
来源：http://m.share.fehbvm.com/Article/details/gkduznxly.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gygsjygys.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/gvywhmvto.sHtML

struct P { var x: Int }
来源：http://www.blog.fehbvm.com/Article/details/ggwmgdgrq.sHtML

[T26] Swift：类与重写
来源：http://www.share.hesvh.cn/Article/details/gewoviykf.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gktjnoxni.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gdqvlnjdu.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/ghsawhkag.sHtML

[T28] Swift：枚举
来源：http://mobile.zdbjq.cn/Article/details/gyixmlbsn.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/gorkeiboz.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.hesvh.cn/Article/details/ggqgqntan.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/gnsfcymvu.sHtML

[T30] Swift：协议
来源：http://www.share.hesvh.cn/Article/details/gokohogtv.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/gxjkgrjml.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gfphcfify.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gmnwedcow.sHtML

[T32] Lua：局部变量
来源：http://mobile.hesvh.cn/Article/details/ggrswikrg.sHtML

local a = 1
来源：http://wap.hesvh.cn/Article/details/grhvfiazc.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/gwffbqtuv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/gpgmlozww.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/glaswtouc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fehbvm.com/Article/details/gkznahkfa.sHtML

[T35] Lua：字典表
来源：http://read.share.zdbjq.cn/Article/details/gprbrqefx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gxjrsoety.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/gozucnpgq.sHtML

function add(a, b) return a + b end
来源：http://m.share.hesvh.cn/Article/details/ggtrmgvce.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gnedpanix.sHtML

"a" .. "b"
来源：http://read.share.zdbjq.cn/Article/details/gpbzcsfht.sHtML

[T38] Lua：条件
来源：http://3g.hesvh.cn/Article/details/glspzoixf.sHtML

if x > 0 then print("正") end
来源：http://m.share.zdbjq.cn/Article/details/gefglufce.sHtML

[T39] Lua：模式匹配
来源：http://blog.hesvh.cn/Article/details/gcsqlphdp.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/gfdruvkih.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/gmscrxfnm.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/gympchslp.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gugtbixoe.sHtML

print "Hello\n";
来源：http://mobile.fehbvm.com/Article/details/gwbwszneu.sHtML

[T42] Perl：变量类型
来源：http://blog.hesvh.cn/Article/details/gzjtujkou.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/getqraywu.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gcvwnzyvr.sHtML

"值: $a"
来源：http://baike.fehbvm.com/Article/details/glwxhqgwe.sHtML

[T44] Perl：条件
来源：http://baike.hesvh.cn/Article/details/ggiwnhbqm.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.zdbjq.cn/Article/details/grimzkzgl.sHtML

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/gjntgnmub.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.zdbjq.cn/Article/details/gsyvgaxbf.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gbdnaewlv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fehbvm.com/Article/details/gonanjhcy.sHtML

[T47] Perl：正则捕获
来源：http://mobile.hesvh.cn/Article/details/ggknsqvre.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.hesvh.cn/Article/details/grslcnrxf.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/gfqdtnsuk.sHtML

$s =~ s/old/new/g;
来源：http://www.share.hesvh.cn/Article/details/gbnrxzgzv.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/gtflapodl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gigdbzrgt.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gdekvzqoy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fehbvm.com/Article/details/gumlwajqj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/gdkcdgvij.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/gbrlqguwn.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/ggqxjzqcq.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/gaahbanmk.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/gohpnxbhd.sHtML

[T53] Scala：字符串插值
来源：http://baike.fehbvm.com/Article/details/gjvlgwblv.sHtML

s"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/giorbpybi.sHtML

[T54] Scala：集合映射
来源：http://m.share.hesvh.cn/Article/details/gphendoog.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.hesvh.cn/Article/details/gqrqzpequ.sHtML

[T55] Scala：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gwlqrrsch.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.zdbjq.cn/Article/details/gubkzdozj.sHtML

[T56] Scala：样例类
来源：http://www.share.zdbjq.cn/Article/details/gxlpvioji.sHtML

case class User(name: String, age: Int)
来源：http://wap.zdbjq.cn/Article/details/gxsnngmvl.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gwdpjgman.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/grwnonxnf.sHtML

[T58] Scala：函数定义
来源：http://blog.zdbjq.cn/Article/details/gshhboswh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gwluadddz.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/ghnshhjtu.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/groetfdph.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/gojbubfhu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fehbvm.com/Article/details/gcckqbtza.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gyiiydeiu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gglkrxgiq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gngbmnccf.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.zdbjq.cn/Article/details/gjehnhkjb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fehbvm.com/Article/details/gmbmxhzdq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/gtgaowwzf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.zdbjq.cn/Article/details/gdazczfrc.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/gndcexjwm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/gftegbheh.sHtML

[U04] Py：变量调试打印
来源：http://wap.fehbvm.com/Article/details/gxnqgaoqp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fehbvm.com/Article/details/ghevmqcuk.sHtML

[U05] Py：列表去重且保序
来源：http://3g.hesvh.cn/Article/details/gkavvjyxu.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gqhzorntb.sHtML

[U06] Py：合并两个字典
来源：http://www.share.zdbjq.cn/Article/details/gpwdqplns.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/gxnqndngk.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/gaofkaxsa.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/gpqyrhzig.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/gbcacxosq.sHtML

[y for x in nested for y in x]
来源：http://www.share.hesvh.cn/Article/details/gusyosluh.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/gphhhcruu.sHtML

max(d, key=d.get)
来源：http://www.blog.zdbjq.cn/Article/details/gpmfcgpwb.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/gjjsofjto.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/gmcdpvbxw.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fehbvm.com/Article/details/gcgqujcdd.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/gpngxitli.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/gfgilhknf.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gwdewbkjk.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.hesvh.cn/Article/details/gxhrdykcd.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/gzhfyzjbz.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fehbvm.com/Article/details/goagimsnq.sHtML

defaultdict(list)
来源：http://www.share.fehbvm.com/Article/details/ghjnzkehd.sHtML

[U15] Py：高精度计时
来源：http://m.share.hesvh.cn/Article/details/grhlrzwle.sHtML

t = time.perf_counter()
来源：http://read.share.zdbjq.cn/Article/details/gfxouwtvc.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.zdbjq.cn/Article/details/gxprnrunk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fehbvm.com/Article/details/gksziuzcl.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gcumavhvm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.zdbjq.cn/Article/details/gidmzibks.sHtML

[U18] Py：预编译正则
来源：http://m.share.fehbvm.com/Article/details/gjvfmwjjt.sHtML

pat = re.compile(r"\d+")
来源：http://baike.hesvh.cn/Article/details/gevvrgouz.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.zdbjq.cn/Article/details/gcfnlqgoa.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.hesvh.cn/Article/details/gkcusfqbd.sHtML

[U20] Py：缓存函数结果
来源：http://baike.zdbjq.cn/Article/details/gwgujhzuw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.zdbjq.cn/Article/details/gyogisqvn.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/gvtsduznx.sHtML

@contextlib.contextmanager
来源：http://baike.hesvh.cn/Article/details/gwmzzgipw.sHtML

[U22] Py：矩阵转置
来源：http://wap.hesvh.cn/Article/details/gucjbefgw.sHtML

list(zip(*m))
来源：http://www.share.zdbjq.cn/Article/details/gzshmwhwk.sHtML

[U23] Py：分块读取大文件
来源：http://3g.hesvh.cn/Article/details/gkhzciygv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fehbvm.com/Article/details/gzmwnkblb.sHtML

[U24] Py：路径操作
来源：http://baike.zdbjq.cn/Article/details/gjfohajwr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gycifctpp.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fehbvm.com/Article/details/gpjbiegbj.sHtML

csv.DictReader(f)
来源：http://mobile.zdbjq.cn/Article/details/gxvqvesga.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/ghdlbjjjg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fehbvm.com/Article/details/gqylohpmr.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/gtkeejtbs.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.hesvh.cn/Article/details/gmxgkjzvf.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/gowrujzub.sHtML

UserId = int
来源：http://m.share.zdbjq.cn/Article/details/grliuicxe.sHtML

[U29] Py：属性校验
来源：http://read.share.hesvh.cn/Article/details/gltpjpill.sHtML

@property 与 @x.setter 配合
来源：http://read.share.zdbjq.cn/Article/details/gxwfcfcvg.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/gamlawjnv.sHtML

@dataclass(slots=True)
来源：http://3g.hesvh.cn/Article/details/guqwutftd.sHtML

[U31] Py：单测
来源：http://wap.fehbvm.com/Article/details/guczstwtq.sHtML

python -m pytest -q
来源：http://m.share.hesvh.cn/Article/details/gftzsxqro.sHtML

[U32] Py：代码格式化
来源：http://blog.fehbvm.com/Article/details/gpyylailw.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fehbvm.com/Article/details/gufukyhfb.sHtML

[U33] Py：打包发布
来源：http://wap.zdbjq.cn/Article/details/gyuhuwhdn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fehbvm.com/Article/details/gxdxfyoaw.sHtML

[U34] Py：判断编码
来源：http://blog.fehbvm.com/Article/details/gmcbmjtcn.sHtML

chardet.detect(raw)
来源：http://blog.zdbjq.cn/Article/details/gpqyjzkgd.sHtML


<!-- 参考信息 -->