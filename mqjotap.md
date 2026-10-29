代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/glaewnusz.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gnnhlrtsp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/gmsozazsy.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/gqpcqixwx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/goexlofzx.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gjeknrshs.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gghmkmlgf.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gezpqovor.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/gksoiysgn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/gyltylbgx.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gyxfdbyhw.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gezfifmqe.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gxpcbkxtp.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/goecrvuis.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/goqqpbfvm.sHtML

[S14] C：枚举
来源：http://m.share.zdbjq.cn/Article/details/gwontvjzr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.hesvh.cn/Article/details/giotpthen.sHtML

[S15] C：类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gcvpyqmup.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gzdhyowzz.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gqrtpbcpg.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/gcsqjetvd.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gcdcvlaey.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gczeoyuwh.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gzraufxjs.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gxjnzypwg.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/gertqyjtx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gglmqwiwh.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/grtsdvrrc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gesmuqalk.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/ggcvgvqaj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/gotmdqkxc.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gvchgrvpe.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/ggyjbnkja.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gqvltqeny.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/glzsxlqum.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/gyjlnwtln.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gpifswctm.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/gxvczehgp.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/gapizjtui.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/gzmitsnwo.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/gretwizpr.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gvpgqnouv.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gbtpztmzy.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/glztvxyfy.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gmlkcgwsz.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gwuigyhmt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/gnyaarrqf.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/gdwnmrxkz.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gfqeniyrw.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/gbzvremcz.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/gzxcewtzl.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/gqhrnqubm.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/guauetyty.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gjuhkfljp.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gkalsrxds.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gcrkyowpq.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/gdamgdwcq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gxghwnjyq.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/gckoxxlbe.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gmwzvwskj.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gdqhpiowo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gihukqqxr.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/gnofjdcyo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gxrphoigw.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gixkoflot.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gxbanfwde.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gmlumbhjv.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/gxdmosqzi.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/gtdglunps.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/ghtnfycwk.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/gcnavizik.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/gpivonthk.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gkhoypbjp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gekzfizqo.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/gqelhdmue.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/grnroyqnf.sHtML

[S43] C++：智能指针
来源：http://3g.fehbvm.com/Article/details/gjrfdoanl.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gllybulgh.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gtkyauatp.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/glmpxueez.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gcbjwmyxg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/gxgbzomcw.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gtzkodcxx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/gpaqdtoyu.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/ghvzitute.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/gjyuotkhm.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gmqseiukl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/goqsdrtqx.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/grpjngvtw.sHtML

[S49] C++：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gyxcydeql.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/gupvleezz.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/gthxhdlos.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gomfuejwc.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/ghwcoyqlo.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/gmxqafejn.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/gwmkyhjyz.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/giesqgzni.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/gtcefzbce.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gjimspoxt.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gptxmorme.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/ghvogbttb.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/gqwzgwjxq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/gwbqyeimx.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/gyiqihjla.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gsooalgfj.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/grznrnsdt.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gxobbthpa.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gkptnppdl.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/gdwdlxixy.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gzmhcklir.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gkyeezias.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gmcakydjo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/gwusolrku.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkaswfiya.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/gycbwqzpm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gepuduzhr.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/goregcplj.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gnobyeucp.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/geauzclgk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.zdbjq.cn/Article/details/gxhxhwxkz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/glaucfxvi.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gaauubphd.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/gogvujsvo.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gkcnlboga.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/gzbiohlgq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.zdbjq.cn/Article/details/gonvnnqgz.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gsenzzlis.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/ggokzgvch.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gpyxteqki.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/gzsioggaw.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gbtvidesw.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gnsyxjysn.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/glfipmoyu.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.zdbjq.cn/Article/details/gvyqkexyb.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/givouchpi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gzeedqlet.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/gorhnxeim.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/gipzicpww.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/gjwiftoxg.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/gauztdrfd.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gxhqolorn.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gycbadgwc.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/gwovnzduo.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gwikglsnt.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/gilbvxers.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/grdvcybon.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/gxcogskes.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/glwqsxkfc.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/glepnicgh.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gjrnloubf.sHtML

[T18] Swift：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gqcohftlg.sHtML

"值: \(b)"
来源：http://www.blog.hesvh.cn/Article/details/gqzoulegc.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/gxmoonxbm.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gpeuktgpm.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/gkkjnfher.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/gdzjswqib.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/gtttgpuhe.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/gwhfzjjgp.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/gbxwxqhhc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/gpamzpngd.sHtML

[T23] Swift：函数
来源：http://3g.hesvh.cn/Article/details/gfvnscsgh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.hesvh.cn/Article/details/gdgnxxorx.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/gpzqteuug.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/guznjpzsq.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/goqjmcaqx.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/ggfmtjfnl.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/gndetiisy.sHtML

class A: Base { override func f() {} }
来源：http://wap.fehbvm.com/Article/details/gdjhtmgmw.sHtML

[T27] Swift：错误处理
来源：http://baike.hesvh.cn/Article/details/gznbdeypq.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/gvmppegve.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/gcfvjqfgw.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gdsclawtk.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.zdbjq.cn/Article/details/gpdhovyhc.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gsbgundgn.sHtML

[T30] Swift：协议
来源：http://3g.hesvh.cn/Article/details/gwwajjyxu.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/gaxxebyky.sHtML

[T31] Lua：Hello World
来源：http://blog.fehbvm.com/Article/details/gahyinaeg.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gwugnynak.sHtML

[T32] Lua：局部变量
来源：http://mobile.hesvh.cn/Article/details/gqvaicjdy.sHtML

local a = 1
来源：http://blog.hesvh.cn/Article/details/gtubtgxdq.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/gjxoqnxpe.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.hesvh.cn/Article/details/gochxllls.sHtML

[T34] Lua：遍历表
来源：http://3g.hesvh.cn/Article/details/geegkzisl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/gucqrnqer.sHtML

[T35] Lua：字典表
来源：http://m.share.zdbjq.cn/Article/details/ghutbmzwf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fehbvm.com/Article/details/gwrclkpdd.sHtML

[T36] Lua：函数
来源：http://wap.fehbvm.com/Article/details/gshhthlgy.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/gaaxakxih.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gwtwhhpzw.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/gshcxckte.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/gwhyhdhxp.sHtML

if x > 0 then print("正") end
来源：http://www.blog.hesvh.cn/Article/details/gffmwkmxa.sHtML

[T39] Lua：模式匹配
来源：http://baike.fehbvm.com/Article/details/gofbxsqrm.sHtML

string.find(s, "%d+")
来源：http://3g.fehbvm.com/Article/details/gwkjwhnio.sHtML

[T40] Lua：元表
来源：http://baike.hesvh.cn/Article/details/gelpusmjp.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fehbvm.com/Article/details/gdejhgrfb.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gxanfhowb.sHtML

print "Hello\n";
来源：http://blog.zdbjq.cn/Article/details/gfagvfljh.sHtML

[T42] Perl：变量类型
来源：http://mobile.hesvh.cn/Article/details/gjpmxkipl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/grbnhitpp.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/ggjebkpqs.sHtML

"值: $a"
来源：http://www.blog.zdbjq.cn/Article/details/gntgmhcna.sHtML

[T44] Perl：条件
来源：http://baike.hesvh.cn/Article/details/glhxzzgwx.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.zdbjq.cn/Article/details/gpxzqzmgb.sHtML

[T45] Perl：数组遍历
来源：http://baike.hesvh.cn/Article/details/ghndoovlq.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fehbvm.com/Article/details/ggtlkcwnw.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gxpactxdy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.hesvh.cn/Article/details/gdzvmpsho.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/ggtgcchai.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/gbnrjixbr.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/gygitdnme.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/gqqlurkyy.sHtML

[T49] Perl：函数
来源：http://m.share.hesvh.cn/Article/details/gnxfryfnr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gnhgslwlv.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gesaxuqfi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/guxauxrld.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.zdbjq.cn/Article/details/gagsfrlac.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gnxjuhdii.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/ghdepypol.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/gkxgrkgej.sHtML

val a = 1;  var b = 2
来源：http://read.share.hesvh.cn/Article/details/gymzbelge.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gwbbhghvf.sHtML

s"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gczezucby.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gamqdcpcv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/gdvedqhcb.sHtML

[T55] Scala：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gettewqdb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.hesvh.cn/Article/details/gpsencijq.sHtML

[T56] Scala：样例类
来源：http://read.share.fehbvm.com/Article/details/gtjhvthau.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gymmxkypz.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gkgqciouy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.zdbjq.cn/Article/details/gominvbvf.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/gmnzdzmrw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.hesvh.cn/Article/details/gusgbzxho.sHtML

[T59] Scala：循环
来源：http://mobile.hesvh.cn/Article/details/gvanrdcef.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gypaffnsr.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/gtrcqjtej.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/glciledpx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkonfmczl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gvdladflv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghjyvztff.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fehbvm.com/Article/details/glzsphnhk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/grxlvjdpe.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.hesvh.cn/Article/details/gitecarwk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gopwfixes.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/giglqpdvz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.zdbjq.cn/Article/details/gaeonieot.sHtML

[U04] Py：变量调试打印
来源：http://3g.zdbjq.cn/Article/details/gcutfjqdd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.zdbjq.cn/Article/details/gjtriueqw.sHtML

[U05] Py：列表去重且保序
来源：http://blog.hesvh.cn/Article/details/gdbsckgcv.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gwnapelsk.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.zdbjq.cn/Article/details/gldgafjwu.sHtML

{**a, **b}
来源：http://www.m.share.hesvh.cn/Article/details/gtdoovdkx.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/gkrwnubbn.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/gxdgcoltt.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/gjvzlneqt.sHtML

[y for x in nested for y in x]
来源：http://baike.zdbjq.cn/Article/details/giwufnaxf.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/gkgfbicor.sHtML

max(d, key=d.get)
来源：http://baike.fehbvm.com/Article/details/gpvafccxr.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fehbvm.com/Article/details/gnpirqmtd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.hesvh.cn/Article/details/gycitssun.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fehbvm.com/Article/details/gscbexszy.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/guekcznkd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.zdbjq.cn/Article/details/ghbozpcnm.sHtML

Counter(arr).most_common(3)
来源：http://blog.fehbvm.com/Article/details/gyvohrpks.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fehbvm.com/Article/details/gxvhvrugb.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/goauvgxpv.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/gagcaesqr.sHtML

defaultdict(list)
来源：http://www.blog.zdbjq.cn/Article/details/gvwnpeqvp.sHtML

[U15] Py：高精度计时
来源：http://blog.hesvh.cn/Article/details/gdtsegsrc.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/gqwvkpyvo.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fehbvm.com/Article/details/gmouoyjym.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fehbvm.com/Article/details/gfczsmtvt.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.zdbjq.cn/Article/details/guzkbufub.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.hesvh.cn/Article/details/guzsszgdg.sHtML

[U18] Py：预编译正则
来源：http://www.blog.zdbjq.cn/Article/details/ggccnxshw.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.hesvh.cn/Article/details/gugauziil.sHtML

[U19] Py：正则替换带回调
来源：http://wap.zdbjq.cn/Article/details/geeascvem.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.zdbjq.cn/Article/details/gjbrlkcsc.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/gtxrzhzia.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.zdbjq.cn/Article/details/gykjfqqat.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fehbvm.com/Article/details/guigmvyos.sHtML

@contextlib.contextmanager
来源：http://blog.zdbjq.cn/Article/details/gefmwvxyi.sHtML

[U22] Py：矩阵转置
来源：http://baike.hesvh.cn/Article/details/gphuovagh.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/gnjwbriyi.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.hesvh.cn/Article/details/glqgggflw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.hesvh.cn/Article/details/ghcfdcfuw.sHtML

[U24] Py：路径操作
来源：http://wap.fehbvm.com/Article/details/gcjynjftw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gootjoxaq.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fehbvm.com/Article/details/giuphxxlb.sHtML

csv.DictReader(f)
来源：http://read.share.fehbvm.com/Article/details/gkalajrsx.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/gttzhakgt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fehbvm.com/Article/details/gjizrfipl.sHtML

[U27] Py：异步 HTTP
来源：http://blog.zdbjq.cn/Article/details/geivmnrhf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.zdbjq.cn/Article/details/gytoarldr.sHtML

[U28] Py：类型别名
来源：http://read.share.hesvh.cn/Article/details/gnagnxtet.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/glbxhohqn.sHtML

[U29] Py：属性校验
来源：http://mobile.fehbvm.com/Article/details/garylmpml.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fehbvm.com/Article/details/gwhagcwiu.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/gjykqombf.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/gyzwwnpxm.sHtML


<!-- 参考信息 -->