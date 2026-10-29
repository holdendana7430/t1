代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/gowmpinwf.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gidjfgjph.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gattjekas.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/gmfzaimxb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/ggcewyvkr.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/gmnottakg.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gkradzgoq.sHtML

[S11] C：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gzkakuwyj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gndddrnod.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/gbwqsufsx.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gsctglimj.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gxcsptnhj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/gqjahywye.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/gncefjehc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/gphhbzuup.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/gqvwflief.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/grsxhcnra.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gybzyhbcu.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/guplukglr.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gqguroogc.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gjnjsidzz.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gfbswkzik.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/grlodwanw.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/gwfzqtlvb.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gbmbhomlk.sHtML

[S19] C：快速排序
来源：http://mobile.hesvh.cn/Article/details/gixgcgqod.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gdzeahcfp.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gkbxjoavk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gpbaeqctn.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/gubocjoiw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gxskyakat.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gpwfrqzqz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gnwquvdjn.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/gdkswmhru.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/gfxmnmvbf.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/gdjpylyko.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/gysotsizv.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/guibiuskv.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/gunnmpxto.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/gvtfzqqmp.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/gaesnrtqb.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/gopsostkh.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gxswklbhw.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/grmruvllz.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/gqhiiwncx.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/glfykbouw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/gnwvnhhuu.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gjmdpqmhi.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/gqpyivbpn.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gesshbamm.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/ghdksposz.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gfxilfpaq.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/giqszxbjr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpsnvbaxu.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/gcvcasadx.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gxumwopat.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/gofhlujfk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/gcgkbjabb.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gpllagnvi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gtwdwxcbm.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gqeaetfxw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gapwowbww.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gwzmaqlei.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gikvpntsf.sHtML

[S37] C++：set
来源：http://www.m.share.fehbvm.com/Article/details/ghcolljhu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gdfzqmgwn.sHtML

[S38] C++：排序
来源：http://3g.zdbjq.cn/Article/details/grakjqdsq.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gxgnlnmeh.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.zdbjq.cn/Article/details/gcahaaumj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/ggmeintcc.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/glgeuyfde.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gzipkggss.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/gxhmkrzjp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gsrpqoogn.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/giqyplpsd.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gzwkqmzzw.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/gfsfczchl.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/gwqzmudqp.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gfexnqanf.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/gxiklyrfc.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gvlucfdqf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/ghxytbxgm.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gevgthxlg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/gksacracv.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/gcrznwpqz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gercoduty.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/ggtcwusnz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/gzbihduyr.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gacmvyoii.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gxsnkhrom.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/gdjrcwhmb.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/gfzhsesgc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gdhdstalv.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/gxpwzuprd.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/gmistndcp.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/gqrqmspig.sHtML

int size() const noexcept { return n_; }
来源：http://baike.hesvh.cn/Article/details/ghesvykhe.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gvhfghkal.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/gfhfkcmua.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gtwhjeasg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gicovchlo.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/gmxqtckjs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gzfbhikeg.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gzmsvvvtv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fehbvm.com/Article/details/gioiahgcq.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/gbvunhtcc.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/gqdkqvpdm.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gerewydaq.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/gbpywzwta.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/glmbciaus.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/gkreserpl.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gjugggmqh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/ggqonszwe.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyzgdwelj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gctjatbao.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqvxwvrqc.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/ggazvixed.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gpqssydzq.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/gfnnrzhci.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/gxxllhmvm.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/gitlxrruf.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/getehluvo.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gmshvuerq.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/gwziodmxi.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/gadhoxaij.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/gpnceircm.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gncwdyiby.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/gncleubcb.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gxrbvpyxp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gjkqkhyba.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gvlluursh.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gwnunwzcj.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/gfidvgjxu.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gntbacufp.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/godllzktg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/gakpwwaiv.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/gmndvbxlc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/gpaupltjz.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/guqraanfl.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gfmbtwiuy.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/gvikmnbzy.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/gtnsqyxnf.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/grldhuwyf.sHtML

for (i in 1..10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gyxxwfzod.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gzwsbayzs.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/gytiooogg.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/gxbujmfff.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gqbnopyla.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/glwnntewv.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fehbvm.com/Article/details/gxkxpwpim.sHtML

[T18] Swift：字符串插值
来源：http://blog.fehbvm.com/Article/details/gvythqlio.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/gimgdibqf.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fehbvm.com/Article/details/gyaldyhsx.sHtML

if let n = opt { print(n) }
来源：http://www.share.hesvh.cn/Article/details/gmtljydsj.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/gujppmzbh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/ggnciddcc.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/ggvxaxpmj.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/gkwptdcct.sHtML

[T22] Swift：字典
来源：http://www.blog.hesvh.cn/Article/details/gbpoagqfx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/gekesokxv.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/grngoijpc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/gxehsgubd.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/gtzybsnyv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gatbwogiu.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/gbxhcfqdo.sHtML

struct P { var x: Int }
来源：http://www.share.zdbjq.cn/Article/details/gqxxxmccw.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gtiniiaec.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/gbootkxpd.sHtML

[T27] Swift：错误处理
来源：http://baike.zdbjq.cn/Article/details/goozzudbt.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fehbvm.com/Article/details/gysmxnorv.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gqcwdrydp.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gchmxpsvv.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.zdbjq.cn/Article/details/gectertda.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/ghdtrelgx.sHtML

[T30] Swift：协议
来源：http://www.share.fehbvm.com/Article/details/gzxptqrjk.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/gnnqqilyl.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gragwatbb.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/glewzrzea.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/gxmcmabuy.sHtML

local a = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gwldjfibu.sHtML

[T33] Lua：表（数组）
来源：http://baike.zdbjq.cn/Article/details/gdfouvjvp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/goqiefyfb.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/gungpmbdc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.zdbjq.cn/Article/details/gkgrgryzq.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/gsfppxfhl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gkjebhreh.sHtML

[T36] Lua：函数
来源：http://www.share.fehbvm.com/Article/details/gwqxhyhct.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/gvwwuktbn.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/glgyvwomm.sHtML

"a" .. "b"
来源：http://m.share.hesvh.cn/Article/details/gqjzjnzal.sHtML

[T38] Lua：条件
来源：http://wap.zdbjq.cn/Article/details/gvfuxawwk.sHtML

if x > 0 then print("正") end
来源：http://baike.hesvh.cn/Article/details/ghokysrig.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gacudhywv.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/gfjgnbzeg.sHtML

[T40] Lua：元表
来源：http://www.blog.hesvh.cn/Article/details/gjaiwfnqc.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/guviseqkl.sHtML

[T41] Perl：Hello World
来源：http://wap.zdbjq.cn/Article/details/gtbjuqzfb.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gpldwwnxs.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gplbghokj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.hesvh.cn/Article/details/gkkaiwwec.sHtML

[T43] Perl：字符串插值
来源：http://baike.fehbvm.com/Article/details/gscsrnrmw.sHtML

"值: $a"
来源：http://read.share.zdbjq.cn/Article/details/gruhukjor.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/gvdbtcvsx.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fehbvm.com/Article/details/gyawyprus.sHtML

[T45] Perl：数组遍历
来源：http://3g.fehbvm.com/Article/details/gqpgwzdhc.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fehbvm.com/Article/details/ggbgvoqmd.sHtML

[T46] Perl：哈希操作
来源：http://www.share.hesvh.cn/Article/details/grodufrhh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.hesvh.cn/Article/details/grszvmora.sHtML

[T47] Perl：正则捕获
来源：http://m.share.hesvh.cn/Article/details/gmbbhsxbr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/gzahyxcnb.sHtML

[T48] Perl：正则替换
来源：http://baike.zdbjq.cn/Article/details/glqjmnali.sHtML

$s =~ s/old/new/g;
来源：http://baike.fehbvm.com/Article/details/guagxgypr.sHtML

[T49] Perl：函数
来源：http://3g.fehbvm.com/Article/details/gnujpyqvc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gcakqrqmr.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gomohjeat.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/grqmwunhq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fehbvm.com/Article/details/gbpghzkal.sHtML

[T51] Scala：Hello World
来源：http://read.share.fehbvm.com/Article/details/gpglqnncg.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gbfrjmire.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/gaxngqyfe.sHtML

val a = 1;  var b = 2
来源：http://mobile.hesvh.cn/Article/details/gccudcfxe.sHtML

[T53] Scala：字符串插值
来源：http://wap.fehbvm.com/Article/details/ghvnrbbyl.sHtML

s"值: $b"
来源：http://wap.fehbvm.com/Article/details/gtzbunhjg.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/garfhvrsn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/gmvsgskib.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gxbufidui.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/gmpgwrsrb.sHtML

[T56] Scala：样例类
来源：http://www.share.fehbvm.com/Article/details/ggzokfygg.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/gcudimvns.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gmqngawqq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gdhxfuzdx.sHtML

[T58] Scala：函数定义
来源：http://3g.hesvh.cn/Article/details/gaxcyohgp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.zdbjq.cn/Article/details/gudyogyke.sHtML

[T59] Scala：循环
来源：http://www.blog.hesvh.cn/Article/details/gxytqrkus.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gesdthbch.sHtML

[T60] Scala：折叠
来源：http://mobile.zdbjq.cn/Article/details/gwosokcxy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fehbvm.com/Article/details/gexhzxeud.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkphinojz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/gplaqajrc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvbaaznjx.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.hesvh.cn/Article/details/gejdsoxdo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/gutxfkkae.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.zdbjq.cn/Article/details/gbugpljhs.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.hesvh.cn/Article/details/ggsqvzbjh.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/gytskwpfg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.zdbjq.cn/Article/details/gcejnnidx.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/gxxsgofrl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fehbvm.com/Article/details/gggndrfjq.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/gpcrfvldf.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gdltaxkgj.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/gxirawklr.sHtML

{**a, **b}
来源：http://blog.fehbvm.com/Article/details/ggwryvfvt.sHtML

[U07] Py：反转字典键值
来源：http://baike.hesvh.cn/Article/details/glfyoppes.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.zdbjq.cn/Article/details/golttsgwj.sHtML

[U08] Py：展平二维列表
来源：http://baike.zdbjq.cn/Article/details/ghjvcqhnn.sHtML

[y for x in nested for y in x]
来源：http://baike.fehbvm.com/Article/details/gqhhnqzha.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fehbvm.com/Article/details/gdcruqhgj.sHtML

max(d, key=d.get)
来源：http://www.blog.fehbvm.com/Article/details/gvgonxkzg.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fehbvm.com/Article/details/ggewfcfex.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.hesvh.cn/Article/details/guemlkryl.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/ggucfcxee.sHtML

(x * 2 for x in arr)
来源：http://baike.zdbjq.cn/Article/details/gocbjiisr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/gblbngyng.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fehbvm.com/Article/details/gbbnqjdzr.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/gxdzywimm.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/gjqsaxdro.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.hesvh.cn/Article/details/getbpkusk.sHtML

defaultdict(list)
来源：http://read.share.fehbvm.com/Article/details/gagbifier.sHtML

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/gktnolqse.sHtML

t = time.perf_counter()
来源：http://mobile.zdbjq.cn/Article/details/gdphbjnex.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.hesvh.cn/Article/details/gleqcqyez.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gvebyrcze.sHtML

[U17] Py：初始化日志
来源：http://baike.hesvh.cn/Article/details/grzgiillf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.hesvh.cn/Article/details/gxzzxliql.sHtML

[U18] Py：预编译正则
来源：http://3g.fehbvm.com/Article/details/goylrjapd.sHtML

pat = re.compile(r"\d+")
来源：http://blog.zdbjq.cn/Article/details/gsixfffjm.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fehbvm.com/Article/details/garmirfum.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/ggoskchdf.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/gmoqvygal.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.hesvh.cn/Article/details/gruavjyza.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.zdbjq.cn/Article/details/gkbuudpul.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/gpgszlcxo.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/gwxrimptu.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/gutzmmodz.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.hesvh.cn/Article/details/gbfsbpuhp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/gmrdfpgtg.sHtML

[U24] Py：路径操作
来源：http://wap.fehbvm.com/Article/details/gqmpbtszq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gtzlosrhu.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/gianzlfde.sHtML

csv.DictReader(f)
来源：http://baike.hesvh.cn/Article/details/gqkcbossj.sHtML

[U26] Py：并发下载
来源：http://mobile.zdbjq.cn/Article/details/gmtalqoag.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.hesvh.cn/Article/details/genokknnu.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.zdbjq.cn/Article/details/gwqbszekq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.hesvh.cn/Article/details/gppjxyszq.sHtML

[U28] Py：类型别名
来源：http://m.share.zdbjq.cn/Article/details/gqdyfifwc.sHtML

UserId = int
来源：http://www.blog.zdbjq.cn/Article/details/gowosyehj.sHtML

[U29] Py：属性校验
来源：http://3g.hesvh.cn/Article/details/gyvsfzdmo.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/gstcbpawi.sHtML

[U30] Py：数据类
来源：http://wap.fehbvm.com/Article/details/grzrddode.sHtML

@dataclass(slots=True)
来源：http://blog.zdbjq.cn/Article/details/ggxupsdja.sHtML


<!-- 参考信息 -->