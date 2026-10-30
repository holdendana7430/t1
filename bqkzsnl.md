代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gwdqsqykn.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/guksrjdav.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gfomejauy.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gntogrght.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gatxkewgp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/goqcjhmbu.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/ggcmfnzzi.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/geibrijsp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gqvmeusrs.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gujoqfynp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/glprzowry.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gkqkohfrf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/gxekdhyrk.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gtclubthi.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gtjltheuu.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/gqinwiinl.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gakjjalzo.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gilnisdta.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/gefvhqfjy.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gzzxhusto.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gvusqeiim.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/gsydikzzq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gvhuggbeg.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gnnltqcgt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gmliaqmkl.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/gcyozyvhy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gdwkaozhd.sHtML

[S22] C：字符串转数字
来源：http://m.share.hesvh.cn/Article/details/ggqcqjycp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gprsoxvkw.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/ghpntvqdv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gbeitizxz.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gnqgfszqv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/gjetmzeck.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/guwilnnxi.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/gdixuxwji.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/gysgvpxqo.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/gcnmjqmgd.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/gkajdcgdp.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gjkhjkuca.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/gxxfvnxwn.sHtML

static int counter = 0;
来源：http://mobile.hesvh.cn/Article/details/gmgycelux.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/gosakzwuk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gxnevrvvm.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gzbyfmvku.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/ghauzeyzt.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gltbsrdyc.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/grmmkfzkf.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/gkjwvalua.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gwlvsjdgl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gegnrushm.sHtML

[S32] C++：字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gvhtxyhvk.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/gxbbrqgdj.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/gnettwktb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gynbkbbcv.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gxnreyspy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/gygysatxw.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/girgcadrz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gjygxobqj.sHtML

[S36] C++：unordered_map
来源：http://www.blog.zdbjq.cn/Article/details/gjgkmguoc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gxftlpgvl.sHtML

[S37] C++：set
来源：http://3g.zdbjq.cn/Article/details/gyncrioso.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/giwwbqgyk.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gusdmqwpq.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/ghatxwtgo.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gawlietpr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gxicvlvyl.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/gmlzpebyn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gztahqxwm.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gnaooevlm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gaskcggws.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/ghedwtddg.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/gmadnwsdm.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/gcjzxycac.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gazhvvjrh.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/gyqrbqjpq.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/grdgulroi.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/gwrwmhkui.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/gnzgqbdrn.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gyzmegurd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/ggkdtkjkn.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/gxlaqcdun.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gavccvofq.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/guedewoap.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/goveariey.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/gykzctzyg.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gqxokunvx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gmxtvkwqm.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/grohfplsv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gwxovzwao.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gofqchrgk.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gguvqfsom.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/geogevgip.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gwdzhioja.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/gxdsjvsom.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/gdyqjtukd.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/gytpeqlxl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/gmbhkcnrc.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/gdmfyoplh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/gbqjvmplg.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/gihkeddrx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gutjtifti.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/gtswnbipz.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/gqrrqdpad.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/gyvdzopwx.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gkcaavgjc.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/gadmffpxd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gzyensbao.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gaukrswxv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gebkzijqc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gktskrcpb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gioegwfmr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjplabvtf.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fehbvm.com/Article/details/ggfyphlil.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gnbvnqups.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/gjwkjvghf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/gcyudsgow.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/glirfqztd.sHtML

"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gmfhjwrgi.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gcpeshhvz.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gqezjvlaf.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gpowhdxtw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gureoluul.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/gkzchaski.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/ggegwqzhl.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gwgxunrzi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/gfdbbjnhu.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/gunsrjslu.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/gzeybevjk.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.hesvh.cn/Article/details/gejiekhpn.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/gikhgqtuj.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/gpkqkvzky.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.zdbjq.cn/Article/details/grylvadkc.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/grgcuoaeo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/geimietal.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gmqkbkwpt.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gzxmnomhi.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/gkojwuowz.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gvupcykyd.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gdmxndhte.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gdqgputvq.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/gfivzdeeu.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/gyekbmtpv.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gipnsojvz.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/glcxqosxq.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/gwsnmijsg.sHtML

var a = 1;  let b = 2
来源：http://mobile.zdbjq.cn/Article/details/gfbvllivh.sHtML

[T18] Swift：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gragwlejp.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gqdknevmb.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/gogcdlslu.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/guxkdrpkv.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gcisxeijt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.hesvh.cn/Article/details/gajyecxri.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gdufniwsn.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/gnebrvkgu.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/grunlykks.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/gcafiinsv.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/gqlrokqrf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/gwnmimpox.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/gtzrououk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gsqcthjtb.sHtML

[T25] Swift：结构体
来源：http://read.share.fehbvm.com/Article/details/gofcujmjo.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/gtozjruoi.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gobcmhvjq.sHtML

class A: Base { override func f() {} }
来源：http://baike.hesvh.cn/Article/details/gvqewtkte.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/gxcgejtgb.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/gbggbqraf.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/gmavamwtu.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gpysfpnep.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/glgtwpdeu.sHtML

guard let x = opt else { return }
来源：http://m.share.hesvh.cn/Article/details/gjdqircbm.sHtML

[T30] Swift：协议
来源：http://baike.zdbjq.cn/Article/details/gcillbqae.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/gtrnaxwhd.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gldocqpld.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/guqoiuxrv.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/gclnizmsw.sHtML

local a = 1
来源：http://blog.zdbjq.cn/Article/details/gahhdqssg.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/giksztzfb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.zdbjq.cn/Article/details/gwevxysos.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gfewngeyv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fehbvm.com/Article/details/glkasddnn.sHtML

[T35] Lua：字典表
来源：http://baike.fehbvm.com/Article/details/gdwoddrus.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gdkgdislu.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/gtnxoenmy.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/gxuuoiugz.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gtbkhgcvy.sHtML

"a" .. "b"
来源：http://www.share.fehbvm.com/Article/details/genqsjhgj.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/gpgjzopcm.sHtML

if x > 0 then print("正") end
来源：http://www.blog.hesvh.cn/Article/details/gfiazsmob.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/gpxxkujae.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/gntpnhbif.sHtML

[T40] Lua：元表
来源：http://baike.fehbvm.com/Article/details/gdikacmlh.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/gsgrdamxa.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gcliwfjyq.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/gxxknolzd.sHtML

[T42] Perl：变量类型
来源：http://wap.fehbvm.com/Article/details/gkzzbnuhx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gcuumsoai.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/gfoasnidt.sHtML

"值: $a"
来源：http://read.share.zdbjq.cn/Article/details/gdvqnjesd.sHtML

[T44] Perl：条件
来源：http://read.share.fehbvm.com/Article/details/gcecobunf.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fehbvm.com/Article/details/gbqrgghtf.sHtML

[T45] Perl：数组遍历
来源：http://www.share.zdbjq.cn/Article/details/gptzgtirr.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.hesvh.cn/Article/details/gjjulerwk.sHtML

[T46] Perl：哈希操作
来源：http://baike.hesvh.cn/Article/details/grpkxsoys.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.zdbjq.cn/Article/details/gldxtlrjq.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/gnkqgywsm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/gjjhptnce.sHtML

[T48] Perl：正则替换
来源：http://3g.hesvh.cn/Article/details/gzwzwrwch.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.zdbjq.cn/Article/details/gcbpbamyy.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/gkpmkcuqe.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gzooxqfqk.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/giauvqwpi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.hesvh.cn/Article/details/gjhtcvwtp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fehbvm.com/Article/details/gyzddlqdr.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/gxsnwmaet.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gatxbfogh.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/gsklvonze.sHtML

val a = 1;  var b = 2
来源：http://www.share.hesvh.cn/Article/details/genwuxyrm.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/ghbkpwimj.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gcakgwzvl.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gguccgsyi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/gqzbguesd.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gdmhvjjoz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/gghvamtfe.sHtML

[T56] Scala：样例类
来源：http://read.share.hesvh.cn/Article/details/glmlzaljs.sHtML

case class User(name: String, age: Int)
来源：http://baike.zdbjq.cn/Article/details/gklaafanc.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gxlrnvhft.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/gmxgzgxed.sHtML

[T58] Scala：函数定义
来源：http://mobile.fehbvm.com/Article/details/gubixemwh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/gzuxszacd.sHtML

[T59] Scala：循环
来源：http://baike.zdbjq.cn/Article/details/giecdwoqm.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gjdoekhth.sHtML

[T60] Scala：折叠
来源：http://www.share.zdbjq.cn/Article/details/gdeyzrhqk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/gxmbxlzis.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqqculqdh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gyxjbnutz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfgrwsdmw.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fehbvm.com/Article/details/gapqaiexw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/gzyhnupjs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.hesvh.cn/Article/details/gccwjzron.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/gqlzavjbr.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.zdbjq.cn/Article/details/gefwnkxnf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fehbvm.com/Article/details/goltvnduv.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fehbvm.com/Article/details/grjztnhav.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.zdbjq.cn/Article/details/gqalftxpz.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gohgpkzvn.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gcetqfrky.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/gehzcbmzg.sHtML

{**a, **b}
来源：http://3g.zdbjq.cn/Article/details/gqqfzbkzb.sHtML

[U07] Py：反转字典键值
来源：http://m.share.zdbjq.cn/Article/details/gadymjyjk.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fehbvm.com/Article/details/gumdiquqm.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gepztzewz.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/gdbmttdtf.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fehbvm.com/Article/details/glnlzbuyh.sHtML

max(d, key=d.get)
来源：http://3g.fehbvm.com/Article/details/gixycieio.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/gmmzynqcc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.hesvh.cn/Article/details/gzplpxndt.sHtML

[U11] Py：生成器表达式
来源：http://3g.hesvh.cn/Article/details/gprpsiyij.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/gvpcuiosq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/gnftnvsjq.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/gwkbwbpvq.sHtML

[U13] Py：固定长度队列
来源：http://blog.fehbvm.com/Article/details/ghbmzihlh.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/ghkfhohay.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.hesvh.cn/Article/details/gmepzfqst.sHtML

defaultdict(list)
来源：http://wap.hesvh.cn/Article/details/gemjcnigc.sHtML

[U15] Py：高精度计时
来源：http://baike.zdbjq.cn/Article/details/gkoirjesw.sHtML

t = time.perf_counter()
来源：http://mobile.fehbvm.com/Article/details/gfmsbtelx.sHtML

[U16] Py：命令行参数解析
来源：http://baike.hesvh.cn/Article/details/gzdlaeptl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.hesvh.cn/Article/details/gilrktjqe.sHtML

[U17] Py：初始化日志
来源：http://3g.hesvh.cn/Article/details/gyksffomm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.hesvh.cn/Article/details/ghcqtxqty.sHtML

[U18] Py：预编译正则
来源：http://www.share.zdbjq.cn/Article/details/gdlghjbhp.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gkeghnbgy.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.hesvh.cn/Article/details/goozlqwuh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fehbvm.com/Article/details/giycsyspe.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/ggvvhemrk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gvryswdsj.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/gjqhcufym.sHtML

@contextlib.contextmanager
来源：http://www.m.share.zdbjq.cn/Article/details/gvkxlngwr.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.hesvh.cn/Article/details/gskysyzbv.sHtML

list(zip(*m))
来源：http://mobile.hesvh.cn/Article/details/gcnusyszv.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fehbvm.com/Article/details/gdqlateyk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/giqcyughc.sHtML

[U24] Py：路径操作
来源：http://3g.zdbjq.cn/Article/details/gtpmfouot.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gmwupzqzy.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.hesvh.cn/Article/details/gygzvfqsr.sHtML

csv.DictReader(f)
来源：http://www.blog.zdbjq.cn/Article/details/gzoqfqnxh.sHtML

[U26] Py：并发下载
来源：http://www.blog.fehbvm.com/Article/details/grtjuhoxt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.hesvh.cn/Article/details/gozxksbfz.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.zdbjq.cn/Article/details/gndmocmyr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fehbvm.com/Article/details/gwdqyrnne.sHtML

[U28] Py：类型别名
来源：http://blog.hesvh.cn/Article/details/gjivbrggt.sHtML

UserId = int
来源：http://read.share.zdbjq.cn/Article/details/gyfxdwxrp.sHtML

[U29] Py：属性校验
来源：http://mobile.zdbjq.cn/Article/details/gfxatxlfn.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.zdbjq.cn/Article/details/gfpibkbrm.sHtML

[U30] Py：数据类
来源：http://www.share.zdbjq.cn/Article/details/gssnftbdf.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fehbvm.com/Article/details/gdvfbspum.sHtML

[U31] Py：单测
来源：http://wap.zdbjq.cn/Article/details/gixsexuiu.sHtML

python -m pytest -q
来源：http://www.share.zdbjq.cn/Article/details/grjgrxrcy.sHtML

[U32] Py：代码格式化
来源：http://www.blog.hesvh.cn/Article/details/ghacyspit.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fehbvm.com/Article/details/gjsbplzlf.sHtML


<!-- 参考信息 -->