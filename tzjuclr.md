代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbgklafv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmfzgmff.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/ggcckhrqt.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzievnur.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/glteiskef.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gztoxjuys.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gdbkycupq.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gybprfied.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gyynrknay.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrosfinm.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/glarnwdlu.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gyulyamxp.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gehnxdjlz.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/graljvzim.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnchqdbkj.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/goqettoox.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gzaevcllu.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvuxaaom.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvetnitp.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/giowgxjpa.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcmzhwze.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gvmtleitr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gyburjxxs.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gzpaxobxe.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsdifpre.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gstksgrsu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/guveyimvc.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gnlhwivpp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtvjzvyi.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gnubymazq.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/glhbhxfiv.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gtmagbiwe.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/geyzvbaog.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayqzdvwh.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfckborg.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gayobktup.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gkwiconvt.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gksbjglpa.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gsnuaocxm.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gxybjaxsy.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/guqyuvhtv.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmjaphkz.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gyoqbkvxb.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmooxspi.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdkvtnru.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gagmdbqhp.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdgkfqhs.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gcthtzteq.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/greomskvr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/ghkkkumxd.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/grrgtzjdu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqihkzxrn.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszzodmjs.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/grvgchvww.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/ggurdfkzr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/glwenyrqs.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/girvijxht.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gxlqnmlmx.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gxuassxil.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gsftwcwus.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gfbcoibnz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gelffacxv.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gqwjudewa.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gljccrbpo.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsvlvlsy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gdeizkwcc.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gbmzkuamg.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gwpncbrlt.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkuxydmb.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyeuekmrq.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzkcenms.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gezsqynbo.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gymwbxvyu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgolranb.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmqlvtpv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojtjfwem.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gwualdpkk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzweduqxi.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/giagmsmwa.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gtrrdrqwe.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gsrfkeqfe.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gicpcrzak.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gpeobommc.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhpfhcqk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gzoltdmmd.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhlviwra.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gkhlrsxux.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/ghlpxflmp.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyrcxbaf.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfqpcdlc.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gifyvpnap.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/grbcdhysk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gswchqqsw.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gsyarldku.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxgrvwbu.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnolwwqwg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/giccjemib.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/grbokbdue.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtasvbno.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyocbjfw.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggiqubrbs.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblkqyoqy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfsjcosy.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/grjiwovzp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gyoadtuty.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjhrrklb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gavfvpgzm.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gnvmdwuth.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gqddkhozu.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gomhzogmz.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxhpunzq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmikgcli.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybbqmtwj.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvtzuznu.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goujkyowj.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gcfncbcgw.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/ghtjmqhaa.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgshimbp.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/goefikbbn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpgjhblx.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gmkeksbpq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/gdhulztsd.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gzabhjymo.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmwjldkz.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyzkrccf.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsiswsjyk.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtfgvnpy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gydcuelvq.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/grzdyzezy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/gxztrmiun.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/glupjugor.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gnpzicefc.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/geqwzrmqk.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/grsfkqlaz.sHtML

[T14] Kotlin：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/geqdnlbfy.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpclrtdpx.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gjtuikquw.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbqdrkzq.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gmafnrzud.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjrqfong.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/gsoyhyqrz.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlblajhn.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/glkbwzxzu.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxqibnwd.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/glaqhxezb.sHtML

if let n = opt { print(n) }
来源：http://3g.fanxiaobao.xyz/Article/details/gpqghhiev.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/glwnqyaud.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcltvmtkl.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/ghvcsbred.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwhbkkfv.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/grzlkyecl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymjnbfke.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gwbtfbyoj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gqorxmizf.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gusbikosz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gswyrywla.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/grtweopts.sHtML

struct P { var x: Int }
来源：http://3g.fanxiaobao.xyz/Article/details/grxaocnzf.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjjhjrhj.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdifqclu.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftdmdpxq.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gedcgmiix.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqnfuuws.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/glhgcxdop.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fanxiaobao.xyz/Article/details/gyhwhaurg.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/ghvimbzlo.sHtML

[T30] Swift：协议
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvumfadx.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghivfwnnc.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gwswlblaw.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxehoifme.sHtML

[T32] Lua：局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkjmbdek.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/geipsajeb.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkkmukma.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqjwtfpi.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwcdxjqc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcntblpyi.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqitvllvg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gayswyzhz.sHtML

[T36] Lua：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmbothnn.sHtML

function add(a, b) return a + b end
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlgzrcim.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gygsendqs.sHtML

"a" .. "b"
来源：http://wap.fanxiaobao.xyz/Article/details/gsxnicask.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyhsiean.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmcfhuvk.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdfbckzp.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcsvzhym.sHtML

[T40] Lua：元表
来源：http://baike.fanxiaobao.xyz/Article/details/gqfbvoign.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/gedtvrmbv.sHtML

[T41] Perl：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/grosqfgaa.sHtML

print "Hello\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gqjkopwud.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdehpcvvj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelosfabc.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqtxvttn.sHtML

"值: $a"
来源：http://baike.fanxiaobao.xyz/Article/details/gedfoymsl.sHtML

[T44] Perl：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gkuhdpdec.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gktdqgrgu.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfdneawj.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmtrnzryv.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvijnlmb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogdtsbrx.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkwdxcxm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbnjkapt.sHtML

[T48] Perl：正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/gileymprf.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxjywacp.sHtML

[T49] Perl：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gswmgkfrg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcswtlhea.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwiuemhy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fanxiaobao.xyz/Article/details/glrarnrqf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcaxklco.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhlvntla.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfanxjlgn.sHtML

[T52] Scala：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gdawdxpsp.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisycvzbt.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnizayzx.sHtML

s"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gbtrvadua.sHtML

[T54] Scala：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gppbcyeis.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsauitaeb.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxtltabd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/grkobdiyc.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzfjjuoe.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gbirkxxnj.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gzqpfyjpm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fanxiaobao.xyz/Article/details/gcvhioxee.sHtML

[T58] Scala：函数定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gcirwtmpn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmialala.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfxycmms.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzwbxogc.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfywxutg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/gyzbkzawe.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakfzqubk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrxvvgkc.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnbyyvee.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/guuaqchqy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fanxiaobao.xyz/Article/details/gxrsswwdg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fanxiaobao.xyz/Article/details/gdciulthx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fanxiaobao.xyz/Article/details/grutdzhvk.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/goltmpwsx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fanxiaobao.xyz/Article/details/gzjzatipe.sHtML

[U04] Py：变量调试打印
来源：http://baike.fanxiaobao.xyz/Article/details/gxjmxhbpa.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fanxiaobao.xyz/Article/details/gxgksvult.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fanxiaobao.xyz/Article/details/guqrqniqz.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gqksdttkl.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gntazdvrc.sHtML

{**a, **b}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfojqmoqq.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwbgqzrw.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fanxiaobao.xyz/Article/details/gftyndrxa.sHtML

[U08] Py：展平二维列表
来源：http://blog.fanxiaobao.xyz/Article/details/gtwddlrhi.sHtML

[y for x in nested for y in x]
来源：http://www.share.fanxiaobao.xyz/Article/details/gfycoplnu.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fanxiaobao.xyz/Article/details/gweffgddc.sHtML

max(d, key=d.get)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrcjrqlm.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/gfazwkleh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gciwopzzc.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhyagjai.sHtML

(x * 2 for x in arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gjiczojyf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwkwxgdz.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/guzlhuala.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjndtymk.sHtML

deque(maxlen=10)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxalxiqgh.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fanxiaobao.xyz/Article/details/gotqzjxdu.sHtML

defaultdict(list)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcywogrec.sHtML

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/giynecwvv.sHtML

t = time.perf_counter()
来源：http://wap.fanxiaobao.xyz/Article/details/gebgzvlkq.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvnhifit.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fanxiaobao.xyz/Article/details/gouwunhho.sHtML

[U17] Py：初始化日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjesivbb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fanxiaobao.xyz/Article/details/ghmklbkns.sHtML

[U18] Py：预编译正则
来源：http://blog.fanxiaobao.xyz/Article/details/gjsnucslx.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gptkvnkwx.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcwgqewc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkogfjew.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fanxiaobao.xyz/Article/details/glopjfgjz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjqwfogo.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmyktqvy.sHtML

@contextlib.contextmanager
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfsgbhxo.sHtML

[U22] Py：矩阵转置
来源：http://baike.fanxiaobao.xyz/Article/details/gumjckuus.sHtML

list(zip(*m))
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpadjanl.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gmavwxntz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fanxiaobao.xyz/Article/details/gdlvumiil.sHtML

[U24] Py：路径操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfuubroi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqjkwgtw.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fanxiaobao.xyz/Article/details/glqpaviei.sHtML

csv.DictReader(f)
来源：http://baike.fanxiaobao.xyz/Article/details/gqccvlwxc.sHtML

[U26] Py：并发下载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpimldcov.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkdddgvb.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fanxiaobao.xyz/Article/details/gdupivcgq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fanxiaobao.xyz/Article/details/gsggfkbhj.sHtML

[U28] Py：类型别名
来源：http://read.share.fanxiaobao.xyz/Article/details/grocytwgx.sHtML

UserId = int
来源：http://mobile.fanxiaobao.xyz/Article/details/gldagjpzg.sHtML

[U29] Py：属性校验
来源：http://blog.fanxiaobao.xyz/Article/details/gtsphscnw.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzzxopey.sHtML

[U30] Py：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/guvazjjga.sHtML

@dataclass(slots=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gonafmler.sHtML

[U31] Py：单测
来源：http://3g.fanxiaobao.xyz/Article/details/glvvogmqv.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/gkojtvigx.sHtML

[U32] Py：代码格式化
来源：http://blog.fanxiaobao.xyz/Article/details/ginkdloxk.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fanxiaobao.xyz/Article/details/gnqcvcjaq.sHtML

[U33] Py：打包发布
来源：http://blog.fanxiaobao.xyz/Article/details/gcnludvaq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fanxiaobao.xyz/Article/details/gclmttolr.sHtML

[U34] Py：判断编码
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhqpbjus.sHtML

chardet.detect(raw)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxjpsgga.sHtML


<!-- 参考信息 -->