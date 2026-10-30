代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/guvtxczes.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/gmopajztw.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gfjrpplac.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gcceeleuw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gumxquuaw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.zdbjq.cn/Article/details/gumzcripx.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gqgzhyzjq.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/givravkdj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gupxqfkjy.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/glgeirrrx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gtkvonssy.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gwqbcxjzs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/ghrtapysq.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/grahyjfvo.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gchxbpgyl.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/ggkofwktz.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gmkqrgsft.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gixmdqnot.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gycsypbbs.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gvycylens.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gykdjagtk.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gqsjikvdb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gfaznpxuv.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/gavituhdh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gvampwjpn.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/ggwmjhwtg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/guywbpniw.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/geddobnpq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gtqkbvmxu.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gijvxfond.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/guyxsyidi.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gteakzxjy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gythazrzl.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gdjsjofjc.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/grjuqzmdq.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/gkhnvxebs.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gkvbgprwm.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gqsadfqpi.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gdkcinmyk.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/ghrgoiwuk.sHtML

static int counter = 0;
来源：http://mobile.hesvh.cn/Article/details/gsbrbafbg.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gednuudjz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gyqvfewmc.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gmpvzbsuj.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/ggdpljmwp.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gfgculleo.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/gkkcvyadh.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gascpxurw.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gcphjzqvp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/gauqgxbhx.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/gvwdozwya.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.hesvh.cn/Article/details/glhmrniar.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/ghxfkggvs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gywsaiosq.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.zdbjq.cn/Article/details/gbygvhege.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/ggzjgbxmf.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gjqdwaett.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gzafmhfiw.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/gizjucivc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gtleqstif.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gjmzzhzga.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/gdwpctkgg.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/gkbhsrgzd.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gdkqiuvpx.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/gwucowtzl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gdjxopluo.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gnrewxvbm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gqurnyxdc.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gmzfvlqmv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/gkgkwdgbp.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/gcxltsieq.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gktnzyfez.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/gapzhxmis.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/gafpichqv.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/glirrcrkm.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gagmvguwm.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/gnfimnqav.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/gpfooladl.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/gvygxsvuy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gshxpkhwl.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/gsogiougv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gtnugrdwm.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gjuckcmwz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/grpnuqmdv.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/gvtzzokrc.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gmcnagjfj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gbzjnwcqm.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gqtggvcgz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/geusttobe.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/gxpjjqdsg.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gjdloqtbk.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/goeqbcojp.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/gpxgnntqw.sHtML

[S53] C++：移动语义
来源：http://www.share.hesvh.cn/Article/details/gwbuyfowo.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/ggrmnjllm.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gjsgzueig.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/gbrjorjiz.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gdutbqwcy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gxchgaonv.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/gigawabkj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/gloqfvcll.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/gvmdcryrr.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gvxcqrczh.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gvbxystoo.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/gkqtigyws.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gwdwqhwoj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/gduldljwr.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/godgqyzaa.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gscmhdphz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjzfuvgsi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gduailszd.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzivpgwqt.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/gmgxsbwqi.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gjrvmdknv.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/gktsvabyv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gaqacynzl.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/gxfrozcdl.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/grzwqoycv.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/gtaonvlag.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/gfwfjpzky.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/glhbrjmfz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/gpxwmlwst.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fehbvm.com/Article/details/gconwmxyn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/gtlontdfc.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gxuzreihd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/gcgikrjdu.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/gdjtessff.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gpnromsfa.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/gnghdatuo.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/govshgihl.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/ggmrmqgat.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.zdbjq.cn/Article/details/geehdfrty.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/ggbnrulbw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/genopuzbb.sHtML

[T12] Kotlin：解构声明
来源：http://baike.hesvh.cn/Article/details/gqcbpbbwy.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gskmcruxv.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fehbvm.com/Article/details/gmsxfgoej.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/gpdtjvhym.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gytbvhmit.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gyvxwwfeq.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/gzptdfqou.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/gfzkuixsy.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/gcecltinj.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gomfurmdi.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/gfdoiyzpt.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/gmzxmvxlq.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/glkpgdhbh.sHtML

"值: \(b)"
来源：http://m.share.fehbvm.com/Article/details/ghjhulobm.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gfgjzpaim.sHtML

if let n = opt { print(n) }
来源：http://blog.fehbvm.com/Article/details/gglgnfpqd.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/gaxrjpdjq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fehbvm.com/Article/details/gbmoycuxg.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gppdyxlwg.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gfqpkibqp.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/gsshrgvqn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/gaicelqub.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gjtguuiwe.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.hesvh.cn/Article/details/goxtyickl.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/giopfubzx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gjfgmqqvk.sHtML

[T25] Swift：结构体
来源：http://3g.hesvh.cn/Article/details/ghnbrqrym.sHtML

struct P { var x: Int }
来源：http://www.m.share.fehbvm.com/Article/details/geumuwkkc.sHtML

[T26] Swift：类与重写
来源：http://www.blog.hesvh.cn/Article/details/gfigfxooz.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/gteptcfok.sHtML

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/gnfqmnzqm.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.zdbjq.cn/Article/details/gcfzrbmir.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/gxpvabyqj.sHtML

enum Color { case red, green }
来源：http://blog.zdbjq.cn/Article/details/goedyoibs.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/gfpqmogyg.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/gsguyesof.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/gkcexmrxa.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.zdbjq.cn/Article/details/ggwtzubzv.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/gcfwdmapm.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gjfhpbarp.sHtML

[T32] Lua：局部变量
来源：http://wap.fehbvm.com/Article/details/gjabtbybz.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/gijiwepfy.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/gkvwgqvie.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/gogttwwjz.sHtML

[T34] Lua：遍历表
来源：http://www.share.fehbvm.com/Article/details/gtcdrkery.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.zdbjq.cn/Article/details/ggrqiibko.sHtML

[T35] Lua：字典表
来源：http://blog.fehbvm.com/Article/details/grpvzvkjb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fehbvm.com/Article/details/gqjnaaaja.sHtML

[T36] Lua：函数
来源：http://www.share.fehbvm.com/Article/details/ghqcmzpcn.sHtML

function add(a, b) return a + b end
来源：http://read.share.zdbjq.cn/Article/details/gcwstgtni.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gfpumxabe.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/gmvzeuazs.sHtML

[T38] Lua：条件
来源：http://mobile.fehbvm.com/Article/details/ganpibukh.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/glthejvpm.sHtML

[T39] Lua：模式匹配
来源：http://baike.zdbjq.cn/Article/details/giqasdjac.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/gzkmbyogv.sHtML

[T40] Lua：元表
来源：http://www.blog.zdbjq.cn/Article/details/gfdwtljag.sHtML

setmetatable({}, { __index = base })
来源：http://blog.zdbjq.cn/Article/details/gavloguul.sHtML

[T41] Perl：Hello World
来源：http://mobile.hesvh.cn/Article/details/gayxoyjjb.sHtML

print "Hello\n";
来源：http://mobile.fehbvm.com/Article/details/gygetbodi.sHtML

[T42] Perl：变量类型
来源：http://www.share.zdbjq.cn/Article/details/guaqvgmeu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fehbvm.com/Article/details/goyekfuot.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gzkkwavkq.sHtML

"值: $a"
来源：http://m.share.hesvh.cn/Article/details/gucrkxidp.sHtML

[T44] Perl：条件
来源：http://read.share.hesvh.cn/Article/details/gviewcdka.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/gmydbktle.sHtML

[T45] Perl：数组遍历
来源：http://m.share.zdbjq.cn/Article/details/gibbrgtgb.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.zdbjq.cn/Article/details/gtvwnbptx.sHtML

[T46] Perl：哈希操作
来源：http://baike.hesvh.cn/Article/details/ghktqnhha.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.zdbjq.cn/Article/details/ghcfvbqwa.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fehbvm.com/Article/details/glonzfdrk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/glhqcofoq.sHtML

[T48] Perl：正则替换
来源：http://blog.hesvh.cn/Article/details/gvopzuwmp.sHtML

$s =~ s/old/new/g;
来源：http://baike.zdbjq.cn/Article/details/gbozefsde.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/glbvlrhop.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gfsiinomj.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gubupcwls.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.hesvh.cn/Article/details/gljccdbxl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fehbvm.com/Article/details/gbbsttqjd.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gkgpgflcn.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gtkcykqbo.sHtML

[T52] Scala：变量
来源：http://3g.zdbjq.cn/Article/details/gzhxgoyvt.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/gjnjawaak.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gcjecxdle.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gevnhjzqj.sHtML

[T54] Scala：集合映射
来源：http://mobile.fehbvm.com/Article/details/gjkidrntu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gzxtucfql.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/gcxjktrfi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/gsfhqruav.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/gekxgbgms.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/grkbivpad.sHtML

[T57] Scala：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gvlbqlsue.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.zdbjq.cn/Article/details/gyvnlrhsz.sHtML

[T58] Scala：函数定义
来源：http://wap.zdbjq.cn/Article/details/gaobiorgs.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.zdbjq.cn/Article/details/ggqillfwx.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/gqokyidya.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fehbvm.com/Article/details/ggfdekvau.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/guiybjzrw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fehbvm.com/Article/details/gwafjmuat.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggmnxoqkx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/gqungosil.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfbpevrqq.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.zdbjq.cn/Article/details/glhtuvqdg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.zdbjq.cn/Article/details/gleeqwvxh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fehbvm.com/Article/details/gpbsbuoog.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/gyiswvsyk.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fehbvm.com/Article/details/goauckvgj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.hesvh.cn/Article/details/gampedpnx.sHtML

[U04] Py：变量调试打印
来源：http://baike.zdbjq.cn/Article/details/gutycoqqu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.zdbjq.cn/Article/details/gouabtmdy.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/gudcjgaql.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gjwfgumvx.sHtML

[U06] Py：合并两个字典
来源：http://wap.hesvh.cn/Article/details/gggxmzyye.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/gftuxdxks.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/givoyuvpf.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.hesvh.cn/Article/details/gkafljits.sHtML

[U08] Py：展平二维列表
来源：http://3g.zdbjq.cn/Article/details/gifqikeok.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.hesvh.cn/Article/details/gmbdjfixq.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.zdbjq.cn/Article/details/gelkajdtl.sHtML

max(d, key=d.get)
来源：http://www.m.share.zdbjq.cn/Article/details/gqxsgakgi.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/gfawdyivz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fehbvm.com/Article/details/gzqtdorwh.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fehbvm.com/Article/details/gyeiwoehi.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/gwjorlafn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/gwbyuigef.sHtML

Counter(arr).most_common(3)
来源：http://m.share.hesvh.cn/Article/details/gnxyiefdl.sHtML

[U13] Py：固定长度队列
来源：http://3g.zdbjq.cn/Article/details/gynvbiegn.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/glcmqrqgi.sHtML

[U14] Py：分组收集到列表
来源：http://wap.zdbjq.cn/Article/details/getkplncr.sHtML

defaultdict(list)
来源：http://read.share.fehbvm.com/Article/details/grthzvcvi.sHtML

[U15] Py：高精度计时
来源：http://read.share.hesvh.cn/Article/details/gpaxulwfc.sHtML

t = time.perf_counter()
来源：http://3g.hesvh.cn/Article/details/gybtjhthd.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/guuxocmay.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fehbvm.com/Article/details/gvqmkincg.sHtML

[U17] Py：初始化日志
来源：http://www.share.hesvh.cn/Article/details/gsyscmrjp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.zdbjq.cn/Article/details/ghkawxwmn.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/gdgorydif.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/gnppuzhon.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fehbvm.com/Article/details/gaveplerj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fehbvm.com/Article/details/gopcvhufp.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/gmfsaqtcm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.hesvh.cn/Article/details/gmnbfvmuq.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fehbvm.com/Article/details/gegtygyij.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/gkooamwxu.sHtML

[U22] Py：矩阵转置
来源：http://baike.zdbjq.cn/Article/details/gfrlvfhio.sHtML

list(zip(*m))
来源：http://mobile.hesvh.cn/Article/details/gofjsqrvd.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fehbvm.com/Article/details/grmeaundw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/gerqcazrp.sHtML

[U24] Py：路径操作
来源：http://www.blog.zdbjq.cn/Article/details/gqtqomkey.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gykbovjjb.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/gbbwollrq.sHtML

csv.DictReader(f)
来源：http://blog.zdbjq.cn/Article/details/gtvlirbla.sHtML

[U26] Py：并发下载
来源：http://m.share.zdbjq.cn/Article/details/gcvdqeopd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/goaybcjfy.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fehbvm.com/Article/details/gkoiskttw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.hesvh.cn/Article/details/gilsrcnwm.sHtML

[U28] Py：类型别名
来源：http://baike.hesvh.cn/Article/details/gkmjzjkhv.sHtML

UserId = int
来源：http://baike.fehbvm.com/Article/details/gfcgcjgpq.sHtML

[U29] Py：属性校验
来源：http://3g.zdbjq.cn/Article/details/gjioeobqm.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.zdbjq.cn/Article/details/gltxbwxxy.sHtML

[U30] Py：数据类
来源：http://3g.zdbjq.cn/Article/details/gtwepwfwu.sHtML

@dataclass(slots=True)
来源：http://blog.fehbvm.com/Article/details/guohreyfc.sHtML

[U31] Py：单测
来源：http://baike.hesvh.cn/Article/details/gocekgfsl.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/gktltpmlv.sHtML

[U32] Py：代码格式化
来源：http://www.blog.hesvh.cn/Article/details/gvuebbosy.sHtML

ruff format . && ruff check --fix .
来源：http://3g.zdbjq.cn/Article/details/gqvnyhndj.sHtML


<!-- 参考信息 -->