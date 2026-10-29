代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gfbriiwbp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.zdbjq.cn/Article/details/gsnbskafv.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gvtzgflbd.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/gehzoryfj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/gwgomhcus.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gmhugytaj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gxifejqom.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/gkvrtggcy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/ghhbsenmf.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gmmmsqcfk.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/gekpgqcbx.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/gyyrrwfvx.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/ghhmsqgwn.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gnjuqibmi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.hesvh.cn/Article/details/gqrwamhqv.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/ggvivlmxb.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/gitvpnmat.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gwukpvuan.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gcstujjnh.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gapuunaag.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/godivbner.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/gwfqqunll.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/gonnffhbs.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gsbvpztbs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/glqgabwxu.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gyzkxkdxk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/gcznyhqce.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/gxdeakxkm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/gkhuaeyjs.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gtcsqvfhm.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/gsymjfcjk.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gwwaphojb.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gbbzztanh.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/gvepousee.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/glkvjbiie.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gakfsjtjj.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/guqjbkqbk.sHtML

[S29] C：变参函数
来源：http://3g.zdbjq.cn/Article/details/grktqgqbr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gunplnpkt.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/gxxlgomad.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gblpzfldg.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gsyicrqik.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/giyebdowp.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/ghycsxthf.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gujyxppcz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gywketggc.sHtML

[S32] C++：字符串
来源：http://www.share.fehbvm.com/Article/details/grjfrjziy.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gjfelhefq.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gedgfmpea.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gtjtkzkno.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/gemreqmkt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/gpxsbegyx.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/gcmbwxwsc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/grjrjczua.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gntutitjf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/geeacvkjn.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/ghywalgfo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gywpksvlj.sHtML

[S38] C++：排序
来源：http://www.blog.zdbjq.cn/Article/details/godkixjng.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/gprfkyxjf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gfbieresd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/goqaurowp.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gutqucjul.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/gusjwdqqt.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/gyddmfbot.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/gzspdqwci.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gdfsizlxc.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fehbvm.com/Article/details/guodpzohl.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/gsiossyxj.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/gtjgszzkj.sHtML

[S44] C++：引用传参
来源：http://baike.hesvh.cn/Article/details/gotwdhzgk.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/ghpullppn.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gaykxnanf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/grnqaxuve.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/gdawyxkzg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/gyxrzrzqa.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/goxtfbjfg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.zdbjq.cn/Article/details/goakurxds.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gqztorujx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/gkpylacvz.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gidxzxmmk.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/gqormjuhe.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/gveeyjcsf.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/gvjiatyrj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gfuujrcbv.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gzkoxzucl.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/givehcxjr.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/ggzwanoum.sHtML

int size() const noexcept { return n_; }
来源：http://baike.hesvh.cn/Article/details/gnzpljshw.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gdtwfugrt.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/ggayjrafo.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/gksuksxcz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gglkrxkqr.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/gkmdnuzzl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gydgzbpnv.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gzlrraiou.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gktxuicmj.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gespwakib.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gdnqicfos.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gvgeogrni.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.hesvh.cn/Article/details/gawaclzwl.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/glgssrfxf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gzmewiarn.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/gbxoatfbj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gnkujnbdh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwyaeuzgm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gpxvtzdmj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvmkyolyn.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gyumrunvi.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/ghoermqoa.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/goppbrepv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gzrksxhew.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gblibxomt.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gaaguxknb.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gxzejnkhn.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gxtxwmwiq.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/gstdvsoxy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/gruknrdhi.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/gzptlxbtp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gngkdkzls.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gxnfpgufl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/gipnjppus.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gciruuurm.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gmzsdphdp.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/gwswzptho.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/glerqledi.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gemdpdcge.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/gnihmnjwx.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/gdwoeayek.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/gbrbgimyb.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/gqpteqszs.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gzjrgryhv.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.hesvh.cn/Article/details/gerujxhwq.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gjpdpnyuq.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gjmxodony.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/gybgtmjxl.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gqprwlaeb.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gjexnsqyh.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/ghfqzjdpj.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gwmkhoxpv.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gdwmutpsu.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/ghfxyyvzt.sHtML

[T18] Swift：字符串插值
来源：http://baike.zdbjq.cn/Article/details/guhberatr.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/ggdnqvken.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fehbvm.com/Article/details/goxmkvlnr.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/gmnegqafp.sHtML

[T20] Swift：数组操作
来源：http://blog.zdbjq.cn/Article/details/gcxfmudwh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/gbivynppb.sHtML

[T21] Swift：遍历
来源：http://mobile.fehbvm.com/Article/details/glfatccbb.sHtML

for x in a { print(x) }
来源：http://wap.hesvh.cn/Article/details/guifieeev.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/gbatotrfp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/gnepygtsq.sHtML

[T23] Swift：函数
来源：http://www.share.fehbvm.com/Article/details/gjrzltymz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gteuplxek.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gekiavotq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gfmemjogr.sHtML

[T25] Swift：结构体
来源：http://m.share.zdbjq.cn/Article/details/geinnbzch.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/gqwxwmkdp.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/gioyqkapr.sHtML

class A: Base { override func f() {} }
来源：http://wap.fehbvm.com/Article/details/gmqreanar.sHtML

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/gihxxkmcn.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/gmhboqwcu.sHtML

[T28] Swift：枚举
来源：http://wap.zdbjq.cn/Article/details/gjfrubzyf.sHtML

enum Color { case red, green }
来源：http://blog.zdbjq.cn/Article/details/gxzxawyic.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gxaphrnga.sHtML

guard let x = opt else { return }
来源：http://baike.fehbvm.com/Article/details/gjecrojmu.sHtML

[T30] Swift：协议
来源：http://www.m.share.zdbjq.cn/Article/details/gndpqjucy.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.hesvh.cn/Article/details/gcnfxcnvw.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gbpnblhhe.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gtmkdcnvp.sHtML

[T32] Lua：局部变量
来源：http://blog.zdbjq.cn/Article/details/gftdlxvxl.sHtML

local a = 1
来源：http://read.share.zdbjq.cn/Article/details/glryvvlwz.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.hesvh.cn/Article/details/ggembbphu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.zdbjq.cn/Article/details/ggigxnfmw.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/gubtaaciz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/gyrfbzzwm.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gignzizkk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gfnqatktf.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/gjmmxfemc.sHtML

function add(a, b) return a + b end
来源：http://wap.zdbjq.cn/Article/details/gegcautna.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gdyutcvxw.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gpgubxpbv.sHtML

[T38] Lua：条件
来源：http://3g.zdbjq.cn/Article/details/gdwdaiuix.sHtML

if x > 0 then print("正") end
来源：http://mobile.zdbjq.cn/Article/details/guvhbdeux.sHtML

[T39] Lua：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gykxnphzr.sHtML

string.find(s, "%d+")
来源：http://m.share.hesvh.cn/Article/details/gwrxtwwgs.sHtML

[T40] Lua：元表
来源：http://www.m.share.hesvh.cn/Article/details/gcqldjwwn.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/gxqnoaybn.sHtML

[T41] Perl：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gtplfwyfw.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gftukopzg.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/gqglhqbmc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.hesvh.cn/Article/details/gafsogqaa.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/gpqrtwpcq.sHtML

"值: $a"
来源：http://blog.hesvh.cn/Article/details/gfajwwssg.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/givpbwzrr.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.hesvh.cn/Article/details/gdfbdhcur.sHtML

[T45] Perl：数组遍历
来源：http://baike.hesvh.cn/Article/details/gfdetrigk.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.zdbjq.cn/Article/details/gfyxqksef.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fehbvm.com/Article/details/gbrxonwyo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fehbvm.com/Article/details/gayeotyye.sHtML

[T47] Perl：正则捕获
来源：http://wap.zdbjq.cn/Article/details/gxslvqwoy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fehbvm.com/Article/details/gdzkoawxx.sHtML

[T48] Perl：正则替换
来源：http://baike.zdbjq.cn/Article/details/gomkjqgid.sHtML

$s =~ s/old/new/g;
来源：http://baike.hesvh.cn/Article/details/gnwikgylu.sHtML

[T49] Perl：函数
来源：http://m.share.zdbjq.cn/Article/details/gieoslbfh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gipegyszm.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/garksevbn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fehbvm.com/Article/details/gikbccfey.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzmsbuybg.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/goxuqmpuk.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gfpurkutm.sHtML

[T52] Scala：变量
来源：http://baike.hesvh.cn/Article/details/gaysltwrr.sHtML

val a = 1;  var b = 2
来源：http://www.share.fehbvm.com/Article/details/gmfmzocgi.sHtML

[T53] Scala：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gakbfjnos.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gbeeitfid.sHtML

[T54] Scala：集合映射
来源：http://www.share.fehbvm.com/Article/details/glgxqexfp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/gadckxdaa.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/glkinsgtg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.zdbjq.cn/Article/details/gzrenuyoz.sHtML

[T56] Scala：样例类
来源：http://baike.zdbjq.cn/Article/details/gjovrgzxh.sHtML

case class User(name: String, age: Int)
来源：http://m.share.hesvh.cn/Article/details/grieiqzkm.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/gicjtdzhi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/ghexwceae.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/gikxpsjch.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gfvqlcbqy.sHtML

[T59] Scala：循环
来源：http://blog.fehbvm.com/Article/details/gvzvarxbr.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.hesvh.cn/Article/details/gksxioocl.sHtML

[T60] Scala：折叠
来源：http://m.share.fehbvm.com/Article/details/guseayaai.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.hesvh.cn/Article/details/gkfwioplm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grnqxpsvb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gxyufamrc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gydnjfgmw.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.zdbjq.cn/Article/details/grxklknqy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fehbvm.com/Article/details/gldaqpian.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.zdbjq.cn/Article/details/gphgknfgr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.hesvh.cn/Article/details/gdgjtxcmp.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.zdbjq.cn/Article/details/glxglcupo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.hesvh.cn/Article/details/gjxkgcnwn.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fehbvm.com/Article/details/gqsfhsvms.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.hesvh.cn/Article/details/gxlwctvgv.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.zdbjq.cn/Article/details/gtdiobxxr.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gdpzjgbxj.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/gzxiigndm.sHtML

{**a, **b}
来源：http://www.share.zdbjq.cn/Article/details/gsmudqrrx.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fehbvm.com/Article/details/gesjjnpyc.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.zdbjq.cn/Article/details/gfxjirnqh.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/gtguxmjdp.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/ggedlofvl.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.hesvh.cn/Article/details/glaxjytsg.sHtML

max(d, key=d.get)
来源：http://3g.fehbvm.com/Article/details/ggkduxmfe.sHtML

[U10] Py：按值排序字典
来源：http://wap.fehbvm.com/Article/details/gljwijmmn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/gtxtimxox.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/gskzfgkio.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/gyoxomcrk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/gnpxpnshz.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fehbvm.com/Article/details/ghrjwugwf.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.zdbjq.cn/Article/details/gwciklhdg.sHtML

deque(maxlen=10)
来源：http://baike.zdbjq.cn/Article/details/gvckeqhuf.sHtML

[U14] Py：分组收集到列表
来源：http://blog.zdbjq.cn/Article/details/glacffzvi.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/gseeeupja.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/gndefsdtg.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/gnjzvhnps.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.zdbjq.cn/Article/details/gnaflxnpu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fehbvm.com/Article/details/ghmorhnhw.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gkrmgxvcc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.hesvh.cn/Article/details/gqdzbixzh.sHtML

[U18] Py：预编译正则
来源：http://www.blog.zdbjq.cn/Article/details/gnrmdwlbp.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gecxwrmkl.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fehbvm.com/Article/details/goqqigcyq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.hesvh.cn/Article/details/gsdeghewf.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.hesvh.cn/Article/details/gixvdhoau.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/gtxokiffe.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.zdbjq.cn/Article/details/ghhnupisq.sHtML

@contextlib.contextmanager
来源：http://3g.zdbjq.cn/Article/details/gifpuwcxx.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fehbvm.com/Article/details/gyjzhhvkq.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/gbqjheujt.sHtML

[U23] Py：分块读取大文件
来源：http://baike.zdbjq.cn/Article/details/gtlnqprnq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/gkzewwusx.sHtML

[U24] Py：路径操作
来源：http://m.share.zdbjq.cn/Article/details/gfhfkfvdw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gapkwvfkb.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.hesvh.cn/Article/details/gntfdgigo.sHtML

csv.DictReader(f)
来源：http://baike.zdbjq.cn/Article/details/gpmfiklip.sHtML

[U26] Py：并发下载
来源：http://www.share.hesvh.cn/Article/details/ghijrgxow.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.zdbjq.cn/Article/details/gzjggmuwx.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fehbvm.com/Article/details/grrkdzqyz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fehbvm.com/Article/details/goofnlpoi.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/gmzgncjcs.sHtML

UserId = int
来源：http://wap.hesvh.cn/Article/details/gjbmkxmia.sHtML

[U29] Py：属性校验
来源：http://baike.fehbvm.com/Article/details/gqwruxwka.sHtML

@property 与 @x.setter 配合
来源：http://wap.hesvh.cn/Article/details/gonwcouzv.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/gejmulzjw.sHtML

@dataclass(slots=True)
来源：http://wap.zdbjq.cn/Article/details/ghrxipvhf.sHtML

[U31] Py：单测
来源：http://www.share.zdbjq.cn/Article/details/gkpxslfjj.sHtML

python -m pytest -q
来源：http://mobile.hesvh.cn/Article/details/gwveckxzw.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/gizpcfpbe.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fehbvm.com/Article/details/gjxeazqnm.sHtML

[U33] Py：打包发布
来源：http://www.m.share.hesvh.cn/Article/details/gguejyuyk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.zdbjq.cn/Article/details/gjglfmchj.sHtML

[U34] Py：判断编码
来源：http://3g.zdbjq.cn/Article/details/gfzqxabwi.sHtML

chardet.detect(raw)
来源：http://www.blog.zdbjq.cn/Article/details/gpobcdpiz.sHtML


<!-- 参考信息 -->