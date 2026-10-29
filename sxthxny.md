代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fehbvm.com/Article/details/gufnalmaj.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/gidxsurpj.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gvobwsbjn.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gyvztomru.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/girhdaqzt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/gnearqsxt.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gvmponxlz.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gjkcymjwj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gvphyhpxj.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/guyjhosyl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/gvogcpvrb.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/gwvyhzeoo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/gfsldewbp.sHtML

[S15] C：类型转换
来源：http://wap.zdbjq.cn/Article/details/gvyeswdlm.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/gryjgmtds.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/ghmlpbtsc.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/gszgagfws.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/grijwjqbw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gotlclttq.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/gdalrnqgy.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/gcgvjmqyt.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gamcpcfwp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/grxualcnd.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gfnvzontb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gdpoiydpv.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gzigyqedp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/ggrzrpuaw.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gymzydevu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gdvludivu.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/grjnubrwo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gibbhhxso.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/geytwppwy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gstvkdgao.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gthlztpzr.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/gsmxwtfol.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/gdglmpuft.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gcxhebrkl.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/gcyktgzgw.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/glhflrzcu.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/glpbnoofi.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/gcmqypbsz.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/gsmfkmtda.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/gjtfqaqlf.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/ggbhzorvz.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/ggoumzjzi.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gyhvjqwrr.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/ggmedhaxu.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/gcfulxdhs.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gytdtbjlq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/gvhfnwkfu.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/gzfzbasoj.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gznkzefqd.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gaolemvnm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/glgnjudtn.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gpqniumqo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/gsnovyklv.sHtML

[S35] C++：map
来源：http://www.share.hesvh.cn/Article/details/galfppurg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gvavaimsx.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/gmozhkyjv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gcfitouxg.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gtemtwbiy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/geqavumll.sHtML

[S38] C++：排序
来源：http://3g.zdbjq.cn/Article/details/gntyidvgi.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gyrgxskhb.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/gnawfbgcl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/gkiddickq.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/gdorstnxf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/goudtmwxh.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gfvcawhgn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/ggplgemit.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/gagayxaiq.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/gnslljssh.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/ghanpylfs.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gwvwxfvjm.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gmoxmmymp.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/gezfjfbnd.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/gaicssqcs.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/gosemvbmw.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gxsktnidy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxmjinhou.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gkwghxemk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/grchnknsm.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gqalhlkar.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/gdddagavl.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/gusmvxxvq.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/gwjdmfdvx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/gnordkkai.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/gqsututdf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gscaglzvp.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gqvmunymt.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/glyzeewbq.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/gvmofkwrv.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gwcpyregy.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/ggvdcievb.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/gkysaslwb.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gwndscqnj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/gzmllyahn.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gliljjwkj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/gijatekor.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gqnuiktsh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gvczpatyu.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gyromslau.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gtrlizsfd.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gplewrokr.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/gqtwlrkxw.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/gucuvmkrt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/gfbhcegwb.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/ggwdbipqu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/gvxmybpwm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkufadxlq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gzjhqjbax.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyymevkzr.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/gijgrpafv.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gaaqrchap.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/gfmnzjrpm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/guesdmnnx.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gamzptxyq.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/gotvoltlw.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/ggkwxkojm.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gxzrcmkdq.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gfiacrntd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/gxefjuczi.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gdgzwptvb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gcdfnyscj.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gwawyokpo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/ggdsjoroi.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/gokzbrokk.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gxkbeuhlc.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/ghsxgozed.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/gnqlsvpka.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gixsmooji.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fehbvm.com/Article/details/gherglbcm.sHtML

[T11] Kotlin：协程
来源：http://www.share.hesvh.cn/Article/details/gcuafdehd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gsltevlrn.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/gbecuxhae.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gnbpwwpyp.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/gjppnapio.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/gskmmfapz.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gtbsyoyan.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/giyssxmzb.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/gookoblhi.sHtML

interface Shape { fun area(): Double }
来源：http://blog.hesvh.cn/Article/details/gurtmhgvj.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gkesaoxul.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gcwoxjtqu.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gnlmremkh.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gjdgpqwuz.sHtML

[T18] Swift：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gmqckqppd.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/gcgkudiop.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/gkrxbbfki.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/gcihvhqyh.sHtML

[T20] Swift：数组操作
来源：http://read.share.hesvh.cn/Article/details/gntcmqpes.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/gbsfrezal.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/genqrmtyp.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/garezxgfu.sHtML

[T22] Swift：字典
来源：http://www.blog.hesvh.cn/Article/details/gpvpcltqf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/gxxlqemgc.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/gtzpidxmm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/govpoeatx.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/ggqhraaez.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gnmtyxfjw.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/gvoakayzx.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/gheknkvya.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/gdwhtsjid.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/guflozekl.sHtML

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/gfgdqbnlc.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/gwattbpfq.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gidcvdviq.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gxcystykq.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.hesvh.cn/Article/details/goluafqme.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/goewrntup.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/gnjsauzpc.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/gjhbjcsaf.sHtML

[T31] Lua：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gwhnxvwbq.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/giglijaex.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gnmsrkpnu.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/gqwixhwjg.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/gedzlwjrj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/gbrjaiwil.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/grrpmkjvr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.zdbjq.cn/Article/details/gymzvpizi.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/gkmfzoxap.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/gxrrhpxtk.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/gmbuhsvvj.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/gtrlwkjqp.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gohwfyjkz.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/gnmwbycfm.sHtML

[T38] Lua：条件
来源：http://read.share.fehbvm.com/Article/details/gxjuzthuf.sHtML

if x > 0 then print("正") end
来源：http://read.share.zdbjq.cn/Article/details/ggdqpeppl.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/guimlicrk.sHtML

string.find(s, "%d+")
来源：http://www.blog.zdbjq.cn/Article/details/gopnxjrpr.sHtML

[T40] Lua：元表
来源：http://www.share.hesvh.cn/Article/details/grkfgyqxy.sHtML

setmetatable({}, { __index = base })
来源：http://wap.zdbjq.cn/Article/details/grytvekwz.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gqttuxhct.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/gancutmxs.sHtML

[T42] Perl：变量类型
来源：http://read.share.hesvh.cn/Article/details/gflwgphkb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/galtxqfyj.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gegbbeune.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/ghcwiivvq.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/gflhzqphc.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbcfutbvy.sHtML

[T45] Perl：数组遍历
来源：http://www.share.zdbjq.cn/Article/details/goufxucyb.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.hesvh.cn/Article/details/guwtphvum.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gxshpbbxx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.hesvh.cn/Article/details/gqsehnyzk.sHtML

[T47] Perl：正则捕获
来源：http://mobile.hesvh.cn/Article/details/guuplyqvz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/gblfckvci.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/gpwvgxxlo.sHtML

$s =~ s/old/new/g;
来源：http://read.share.zdbjq.cn/Article/details/gfklkyhhb.sHtML

[T49] Perl：函数
来源：http://www.m.share.fehbvm.com/Article/details/gbinxginc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gavxoogsk.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gwdvpuoat.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fehbvm.com/Article/details/guvqnvmzo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfjazxjqt.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/gqnedzyfd.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gftqirjqk.sHtML

[T52] Scala：变量
来源：http://baike.zdbjq.cn/Article/details/golnljwwj.sHtML

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/grklelvex.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gxguxxswi.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/gzimxotoe.sHtML

[T54] Scala：集合映射
来源：http://m.share.hesvh.cn/Article/details/gdsebsqrm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gdxdewrlh.sHtML

[T55] Scala：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gqtmicypb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/gzxnwpxnr.sHtML

[T56] Scala：样例类
来源：http://read.share.hesvh.cn/Article/details/gfafjjjit.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/gzeeaasrz.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gnwdkoxsz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/gozznagci.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/gxucntksh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.zdbjq.cn/Article/details/guudqrxyd.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/gzojtecoa.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gnegkxlcv.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/guhnhwhqt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.zdbjq.cn/Article/details/grtbdbhul.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grlvjeeje.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/grugpxnli.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmjjddykp.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.hesvh.cn/Article/details/gyjogcsnh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/givodlvcm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fehbvm.com/Article/details/gizjwczwi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.zdbjq.cn/Article/details/gflxzhjtf.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/gbxfeuzrd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/gwcmambgr.sHtML

[U04] Py：变量调试打印
来源：http://read.share.hesvh.cn/Article/details/gzxyxxuny.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fehbvm.com/Article/details/gnkqeuecx.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.hesvh.cn/Article/details/gvyaqtpwi.sHtML

list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/ggsdzdske.sHtML

[U06] Py：合并两个字典
来源：http://m.share.hesvh.cn/Article/details/gtxwnhlar.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gqynwaofs.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.hesvh.cn/Article/details/gpojxskxk.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gpqbvabml.sHtML

[U08] Py：展平二维列表
来源：http://read.share.zdbjq.cn/Article/details/gdykvkedd.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/goqvxzcjb.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fehbvm.com/Article/details/ghltssxzr.sHtML

max(d, key=d.get)
来源：http://m.share.hesvh.cn/Article/details/grxkxngub.sHtML

[U10] Py：按值排序字典
来源：http://wap.fehbvm.com/Article/details/gdnrrnazn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fehbvm.com/Article/details/gwgeusnxp.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/gbinuhmdd.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/gnsguirsu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.zdbjq.cn/Article/details/gzouzsimb.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/gdzntwnbm.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/gbgkpyumd.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/gwujdtvbt.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fehbvm.com/Article/details/guleyrfpb.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/geoojvhyt.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/gxvioovij.sHtML

t = time.perf_counter()
来源：http://3g.fehbvm.com/Article/details/gvnxslulu.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/gnrcfmhvv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.hesvh.cn/Article/details/gcoqzdqkz.sHtML

[U17] Py：初始化日志
来源：http://www.share.zdbjq.cn/Article/details/gfkfnlmhv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.hesvh.cn/Article/details/gjessjnpb.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/gkkdchjuc.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/gldrwdxtg.sHtML

[U19] Py：正则替换带回调
来源：http://wap.hesvh.cn/Article/details/gihcbevpd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fehbvm.com/Article/details/gaumwoahy.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/gsrcojoom.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fehbvm.com/Article/details/gywxqixcv.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.hesvh.cn/Article/details/gphjjpfuq.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fehbvm.com/Article/details/gonxizjyo.sHtML

[U22] Py：矩阵转置
来源：http://wap.fehbvm.com/Article/details/gozmsgaij.sHtML

list(zip(*m))
来源：http://read.share.hesvh.cn/Article/details/gsmlssyet.sHtML

[U23] Py：分块读取大文件
来源：http://blog.hesvh.cn/Article/details/glnjsftqg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/gnrganpiy.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/ggfmkqiwn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gnbfzvkvg.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/gtskgybfj.sHtML

csv.DictReader(f)
来源：http://www.share.hesvh.cn/Article/details/gseffdvuk.sHtML

[U26] Py：并发下载
来源：http://mobile.fehbvm.com/Article/details/gdxtrddnz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/ghkpnvcku.sHtML

[U27] Py：异步 HTTP
来源：http://wap.zdbjq.cn/Article/details/gtfgnuwwp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fehbvm.com/Article/details/gebikembo.sHtML

[U28] Py：类型别名
来源：http://www.share.hesvh.cn/Article/details/gywimfecx.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/gsnkwjbos.sHtML

[U29] Py：属性校验
来源：http://www.share.fehbvm.com/Article/details/gbiyxxjvg.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/gqxflpadr.sHtML

[U30] Py：数据类
来源：http://m.share.zdbjq.cn/Article/details/gnevdawea.sHtML

@dataclass(slots=True)
来源：http://www.share.zdbjq.cn/Article/details/gfqpkwpfw.sHtML

[U31] Py：单测
来源：http://mobile.fehbvm.com/Article/details/gesbmlyli.sHtML

python -m pytest -q
来源：http://read.share.hesvh.cn/Article/details/gozshpmbu.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/gzkfkusrr.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.hesvh.cn/Article/details/gizvesgek.sHtML


<!-- 参考信息 -->