代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gtqaptnke.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gbndfxyiz.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/getgcehgh.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/gszkcjtog.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gfpymmhon.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/grjglkato.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gypimxgto.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gwdwuaous.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/guqqyfxyk.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gjdkolvxh.sHtML

(double) a / b
来源：http://m.share.fehbvm.com/Article/details/ggweodxvr.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/gpgiwcobi.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/grolxzqwk.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gzgsusaqb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gzusblvfl.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/gjlgvgkec.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gkjovqhub.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gmkdfosxw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gjcdoqxkr.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gkjklsgew.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/ghqwimmcd.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/gdoeudrsq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gqybpcgye.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gvqrbxmag.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/gdyuwzvcj.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gckrmkgem.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gzsvbycpq.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/gkvgdinpa.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gyjgzmnuw.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gcgoqvtov.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gjksaygok.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gkabzwhkq.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/getypwrrx.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gpeujxral.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gmcbrcubp.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/gwcputcak.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gdlveynwu.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/gmoebfibu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/gehfrciyb.sHtML

[S30] C：头文件保护
来源：http://www.m.share.zdbjq.cn/Article/details/goadnqqcv.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/glxboxxqt.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/ggjfkanmo.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/gkhyfaiax.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gvcxitmki.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/gniphfust.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fehbvm.com/Article/details/gcqxgwlrk.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/giqwqgupk.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/grcqmbscf.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gotyzpxfe.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/gieoflewm.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/grjccfmmn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/gtxflxgtw.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/grgpuxijp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gwlhihrls.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/gsrptvwrt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gjqjsptvg.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/gbhlohhbc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/gojmhdqln.sHtML

[S38] C++：排序
来源：http://www.blog.zdbjq.cn/Article/details/gjfwhaujh.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gjpbvzjti.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gvxrmlkwl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/gtbeekqqa.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gkixphuza.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/guayefccx.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/guzlegapp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gwbjsmpus.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/guhyteeah.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gdvqukiyc.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gwiuqnwux.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/gqjianrkn.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/gagocjeub.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/glrhdeeby.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/ghcjuried.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/gaehfczdg.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/givnmtqju.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.hesvh.cn/Article/details/gpfjzykpv.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gscxrfarn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/gqdxylgek.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gcllbezyt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/gxdpdzkzv.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/gxsczavdy.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gufsuakwj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gioauvnhk.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gevuapjqh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gglarpfvn.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gvqhrvtjo.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/ghepqarza.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/gwxgbhktf.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/gjmznafuh.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/grweovwce.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/gfxheuubd.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/grhmdjfnc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.zdbjq.cn/Article/details/gwzucrlct.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gxagtdtyk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/galukirkx.sHtML

[S56] C++：optional
来源：http://www.share.fehbvm.com/Article/details/gtyddvvbo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/ggenccapm.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/gphfdkbkl.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gysnjkvvh.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gnryybqtn.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/guzbhivsk.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gyrafayrl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/giqthnfaf.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gefabrype.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gzmfndthy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggxgkvvnx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/ggeayxdnx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gszzgdtoo.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.hesvh.cn/Article/details/gsxekzbaf.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gheertpda.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/gdvbhzbue.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/gpxwzrmit.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/glchlpsji.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/gxytjfzcu.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/guinqdtld.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/gngsfzqge.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/gjkagelzs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/grtznslig.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/gbvymgppm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/grxinvunx.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gitymjndk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/glndpqssl.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gimwdkblw.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/gfwnuacci.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/gvodgkxdg.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/glfsugfjn.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gvshdsquv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/gljczxrao.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/gtfwjlydd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fehbvm.com/Article/details/guftemhil.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/gdiyvglfw.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/gutilelgx.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gczkqgrxm.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/glofgoxqd.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/giwllcrjv.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gqjzzncji.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gdcquqezo.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/guulmnlxr.sHtML

[T16] Swift：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gebbkgvoq.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gbbtcdtuu.sHtML

[T17] Swift：变量与常量
来源：http://3g.zdbjq.cn/Article/details/gaycoxnlw.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gxuuthcrk.sHtML

[T18] Swift：字符串插值
来源：http://wap.hesvh.cn/Article/details/gazbfimzl.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gzyylgesb.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/gnezllfwv.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gzccaohsf.sHtML

[T20] Swift：数组操作
来源：http://www.share.hesvh.cn/Article/details/gaphqolhs.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/gkutcqtrx.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/gxigyrvxl.sHtML

for x in a { print(x) }
来源：http://www.m.share.fehbvm.com/Article/details/gdkvkgqxs.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/goaedadzo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.hesvh.cn/Article/details/grtkaipba.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gvauncgci.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gdeuiuytf.sHtML

[T24] Swift：闭包
来源：http://m.share.fehbvm.com/Article/details/glqtgnqzs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gtoghydzp.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/gcmyakrue.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/ginhbwrhj.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/gdrkpelqu.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/goxuvqkke.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gpcwmchsd.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/gaphtgxpt.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/gbuypwnjr.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/grxzsbkfm.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.hesvh.cn/Article/details/gwbighfqq.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/gkijzmjdf.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gkpqdmkvn.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/glozpmcdn.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/gvxkormag.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gbifcvjtv.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gwihpgmts.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/gcyqqfzgd.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/gmieadtyz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fehbvm.com/Article/details/gtccfapdk.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/golzznqgz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.hesvh.cn/Article/details/gnxopttjg.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/gowqxaotq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/gkikgexlk.sHtML

[T36] Lua：函数
来源：http://baike.zdbjq.cn/Article/details/grdbtaerp.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/grwcismsh.sHtML

[T37] Lua：字符串拼接
来源：http://wap.hesvh.cn/Article/details/gwzexsfxx.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/gpkxsuaef.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/gokwukdix.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/grkalomyz.sHtML

[T39] Lua：模式匹配
来源：http://m.share.hesvh.cn/Article/details/grxoszcrn.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/gozrgtwsf.sHtML

[T40] Lua：元表
来源：http://www.m.share.fehbvm.com/Article/details/gyanqjuvi.sHtML

setmetatable({}, { __index = base })
来源：http://wap.hesvh.cn/Article/details/gpspsqwvh.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gguqkmrwa.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/gvosnxymu.sHtML

[T42] Perl：变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gsgmssmbp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.hesvh.cn/Article/details/gzgtbklbo.sHtML

[T43] Perl：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gwnkvdyew.sHtML

"值: $a"
来源：http://www.blog.zdbjq.cn/Article/details/gilbktchh.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/gdccxqhar.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.zdbjq.cn/Article/details/goxaggals.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/gywdosrss.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fehbvm.com/Article/details/gcmupeyjg.sHtML

[T46] Perl：哈希操作
来源：http://blog.hesvh.cn/Article/details/gcrvjifqg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/goyzyyxzr.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/gmpkdrcse.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fehbvm.com/Article/details/giagseihy.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/gygvamerg.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fehbvm.com/Article/details/ghuctlorq.sHtML

[T49] Perl：函数
来源：http://m.share.fehbvm.com/Article/details/gleasggrg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gnahoevqa.sHtML

[T50] Perl：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gvnkiwksc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.hesvh.cn/Article/details/ghrhdvpoa.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.hesvh.cn/Article/details/gsantjhom.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/gnfvwgjqm.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gcakgipld.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/gxrqwekwt.sHtML

val a = 1;  var b = 2
来源：http://mobile.hesvh.cn/Article/details/gghibpwyc.sHtML

[T53] Scala：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gfzcjaeia.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gldpfrzvy.sHtML

[T54] Scala：集合映射
来源：http://m.share.fehbvm.com/Article/details/grzcgbyjn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.zdbjq.cn/Article/details/ganoddcyc.sHtML

[T55] Scala：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gjnmvwira.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.hesvh.cn/Article/details/gynukotit.sHtML

[T56] Scala：样例类
来源：http://read.share.hesvh.cn/Article/details/ggmkpebbq.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gmrneqrqm.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/ghfhaqefs.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/glaiiopmm.sHtML

[T58] Scala：函数定义
来源：http://wap.fehbvm.com/Article/details/gfkznbogz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.zdbjq.cn/Article/details/gkdcxgppc.sHtML

[T59] Scala：循环
来源：http://wap.fehbvm.com/Article/details/gzfyedzou.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gpifbaugm.sHtML

[T60] Scala：折叠
来源：http://m.share.zdbjq.cn/Article/details/ghjffafbp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.zdbjq.cn/Article/details/guwqytdmt.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvkjjbfpy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gtxepbkjh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/goukateld.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.zdbjq.cn/Article/details/gztkgsnxh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/gimbylvbt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/gffyicgzk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/gultkxyzd.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fehbvm.com/Article/details/ghefcwwxr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.hesvh.cn/Article/details/gxfdnyuze.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.hesvh.cn/Article/details/gljukgofj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.hesvh.cn/Article/details/govmwvalq.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/gcjhwiluj.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/golqjnbcq.sHtML

[U06] Py：合并两个字典
来源：http://m.share.hesvh.cn/Article/details/gqxafnqmw.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gvwdsyvwt.sHtML

[U07] Py：反转字典键值
来源：http://www.share.hesvh.cn/Article/details/gmgwoqjpa.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/gsnqnzvua.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/gncljcwqz.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.zdbjq.cn/Article/details/gcbllsaep.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.zdbjq.cn/Article/details/gjzqtgipw.sHtML

max(d, key=d.get)
来源：http://blog.zdbjq.cn/Article/details/gtgffrvqt.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/gpgtrhisg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/gtszvhciv.sHtML

[U11] Py：生成器表达式
来源：http://3g.fehbvm.com/Article/details/goipmfxqy.sHtML

(x * 2 for x in arr)
来源：http://blog.fehbvm.com/Article/details/glkwjyoga.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.hesvh.cn/Article/details/ggwcpmicn.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fehbvm.com/Article/details/gwbipyorw.sHtML

[U13] Py：固定长度队列
来源：http://www.share.zdbjq.cn/Article/details/gcqdeazas.sHtML

deque(maxlen=10)
来源：http://baike.zdbjq.cn/Article/details/gykynhwhz.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fehbvm.com/Article/details/geikedneo.sHtML

defaultdict(list)
来源：http://3g.fehbvm.com/Article/details/grohulcyy.sHtML

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/gtqrlurmm.sHtML

t = time.perf_counter()
来源：http://3g.fehbvm.com/Article/details/golnwdpsw.sHtML

[U16] Py：命令行参数解析
来源：http://blog.hesvh.cn/Article/details/gchplhzgj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.hesvh.cn/Article/details/genomcjeb.sHtML

[U17] Py：初始化日志
来源：http://mobile.zdbjq.cn/Article/details/gsutodjat.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.zdbjq.cn/Article/details/gezsvlbgy.sHtML

[U18] Py：预编译正则
来源：http://wap.fehbvm.com/Article/details/gtpvroanw.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fehbvm.com/Article/details/gjicahios.sHtML

[U19] Py：正则替换带回调
来源：http://blog.zdbjq.cn/Article/details/gncyboodj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/gsckgecez.sHtML

[U20] Py：缓存函数结果
来源：http://baike.hesvh.cn/Article/details/gajnzxbmv.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.hesvh.cn/Article/details/ggzcoytim.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/gzofhsluu.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/gxqrqfksu.sHtML

[U22] Py：矩阵转置
来源：http://baike.zdbjq.cn/Article/details/gfmwbibax.sHtML

list(zip(*m))
来源：http://www.m.share.fehbvm.com/Article/details/gwrvgvomq.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.hesvh.cn/Article/details/gbbbbqsha.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fehbvm.com/Article/details/giycvjygx.sHtML

[U24] Py：路径操作
来源：http://3g.zdbjq.cn/Article/details/grxvtkzuu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gogmrugdo.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/gcyiygoan.sHtML

csv.DictReader(f)
来源：http://m.share.fehbvm.com/Article/details/gauxsvwmt.sHtML

[U26] Py：并发下载
来源：http://read.share.hesvh.cn/Article/details/gnqhxwiop.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.zdbjq.cn/Article/details/giulxfcse.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/gfduxgitp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/gjfpnhzzh.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/gpvthwgui.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/gjodrqntc.sHtML

[U29] Py：属性校验
来源：http://3g.hesvh.cn/Article/details/gadlbfebr.sHtML

@property 与 @x.setter 配合
来源：http://baike.zdbjq.cn/Article/details/gdnnmpmiw.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/gghrbozze.sHtML

@dataclass(slots=True)
来源：http://3g.fehbvm.com/Article/details/gyehcxjoo.sHtML

[U31] Py：单测
来源：http://read.share.fehbvm.com/Article/details/gqkjhnviv.sHtML

python -m pytest -q
来源：http://www.m.share.fehbvm.com/Article/details/guuefmvma.sHtML

[U32] Py：代码格式化
来源：http://wap.fehbvm.com/Article/details/gjtefdany.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.zdbjq.cn/Article/details/gsgwuvuas.sHtML

[U33] Py：打包发布
来源：http://read.share.fehbvm.com/Article/details/gbkvkjslz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fehbvm.com/Article/details/gzwrinsfg.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/gdongutwq.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/ggxgoylrj.sHtML


<!-- 参考信息 -->