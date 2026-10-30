代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbacvlpmm.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gjauoaxwa.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gahzghdbd.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gmleslmwy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/ggurukrva.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuzuynbf.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gyywirrmg.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqpisgbs.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcfzznyb.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyqhnjdd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilpyxzyg.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbouiiiap.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giquuzwnw.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gohnvtcjt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdycsoylh.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gjgcxppaw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gofmnzgrw.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnopipty.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdadhrtmi.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpduyzdet.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/goyggfadu.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gydavhzyz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guquupsyw.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gkrlibwsm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gavtnclwp.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/ggbomagzc.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvewhzae.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gtgmqffse.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/govbtmaxs.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gpqavmpee.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdjhlqwm.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gfvsykdsn.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqbajvsn.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geszdnarw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gaeqivwij.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcrasmmq.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyvroszy.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guilfyngy.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/grvdyykva.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gxiqevhle.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobcuotsz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwbduntwt.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gmezmtpkq.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gipuulnpv.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/guxrusbyt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggecrjszg.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gaaqxdybr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmtspjwgx.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gzltqmcyf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gzfyrswco.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjvdsxoq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gzksjhgha.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gxismxzlk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gonvgotto.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/glruelvje.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/ghymjkcse.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdclmmxkn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gmngehxwe.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gugtgigor.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgedwiip.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gsugkupvl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gghuepueg.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gltorbdaw.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkvkabcr.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gkllpmejz.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvzipdkm.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gndjvkwpd.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxvyfjdf.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gioddxmvb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gnjqeojgl.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gpunfeefv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gifdlsygm.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzfrrogs.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwefpplse.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwybwtwwc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdbopeji.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gxrvbsqdn.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulysfluq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmfgylpe.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/guyakfdkp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcblwgcxe.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkotozhk.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gzuhegvhg.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gmlcjlmwa.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkexoozss.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gcdcojrcy.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gxxgwcgzt.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gylncsjrj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gmnxjrklk.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gcgloafav.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gjbdnkpyr.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgormpwc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gudjrnunh.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gjthbvxke.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gerzskrmf.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gjwcgupgi.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcukbfldc.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gzitzzyzt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjzfuwvx.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/geiaknnkd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gncfrtfei.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ghzfiovlk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/giaxarmhv.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gisqhispo.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gvqwxpkan.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gnvxjzslz.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gdpvdqibm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsfbbgcp.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzgqjjxi.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gkrqwcauj.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbrcwayr.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gfiluijkg.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gujvprmxq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezcoropq.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqfwilgz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gqpusjtky.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgnrerza.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijvbrlul.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebtfcrdf.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gxgqidswn.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/grrdywcqk.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubmifddz.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllxbgpnj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/grefqbliw.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsfnqbhn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/gexzunxog.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/grilmilqb.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gadfsxcnf.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gvwkjhpra.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/ggjeaadjf.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlultzjq.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahemowvc.sHtML

[T15] Kotlin：接口
来源：http://3g.fanxiaobao.xyz/Article/details/gcofssmaj.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gtgmwkgkl.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvzofqjh.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtntljsz.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjhxpxyu.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gnuzgugjf.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gvnfxzcln.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/gcspknceq.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gypedsgtc.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/grukdgptu.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gkcntftvm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkpjsbty.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpjdnrwo.sHtML

for x in a { print(x) }
来源：http://blog.fanxiaobao.xyz/Article/details/gcyrcphws.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/gcjbotgst.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gigughadp.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gfovlgsyi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gvfizgtil.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/ghnhynzuy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gaidbcllt.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnhnyxup.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/glkjaszze.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/gcgshgswy.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrzcadaa.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gbtpxinbe.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/gzxifxhwf.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/globpkjhl.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfawyvwp.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guztcjawm.sHtML

guard let x = opt else { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpotfhati.sHtML

[T30] Swift：协议
来源：http://baike.fanxiaobao.xyz/Article/details/ggrcwsjrk.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwqfeycw.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gszgfjthm.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjiedfmdk.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmaeqhwdy.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gzonunxqk.sHtML

[T33] Lua：表（数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gkqplkxjk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/gmymrqcxo.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/gopgnmlqs.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fanxiaobao.xyz/Article/details/guculwkrc.sHtML

[T35] Lua：字典表
来源：http://baike.fanxiaobao.xyz/Article/details/gqihrayxt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobisndea.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gulpwrimx.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/gnzjrpjll.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gvdltgwlc.sHtML

"a" .. "b"
来源：http://wap.fanxiaobao.xyz/Article/details/ginecriqr.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gjvubdlzv.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvdkfddh.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gbgyvrfqp.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrfpdhxl.sHtML

[T40] Lua：元表
来源：http://blog.fanxiaobao.xyz/Article/details/gbeatluth.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsbrixan.sHtML

[T41] Perl：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/ghagdzzgr.sHtML

print "Hello\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkdyqwvx.sHtML

[T42] Perl：变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/gfynavxbs.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxgolwfq.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcbeownl.sHtML

"值: $a"
来源：http://m.share.fanxiaobao.xyz/Article/details/geoudsnaz.sHtML

[T44] Perl：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gpojndnvu.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/golaqvadq.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gpriqsubz.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfkumnig.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjgtxxgc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgzeojjf.sHtML

[T47] Perl：正则捕获
来源：http://3g.fanxiaobao.xyz/Article/details/gfwatwwng.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gyxkoopml.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/ggezlzuzj.sHtML

$s =~ s/old/new/g;
来源：http://wap.fanxiaobao.xyz/Article/details/gxketbcmq.sHtML

[T49] Perl：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwhejfsi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/ggwviqvmt.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmknudjxh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfsodaxe.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfvbliwe.sHtML

[T51] Scala：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gnefldjqj.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfcdivra.sHtML

[T52] Scala：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gygcqaure.sHtML

val a = 1;  var b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/giptoubcr.sHtML

[T53] Scala：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gxwzdkjcy.sHtML

s"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjwkuzib.sHtML

[T54] Scala：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyzffyvk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/ggqatigwx.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gifpepttp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gseskogyh.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbethygp.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/guccmwurh.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqsyddky.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fanxiaobao.xyz/Article/details/gnwbxjski.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkfroawz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmkqtlwu.sHtML

[T59] Scala：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbddvrqrz.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gnaxdwztq.sHtML

[T60] Scala：折叠
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqsjogqt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fanxiaobao.xyz/Article/details/gazvcrmrc.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gdsttokfm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gukgorubm.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhggokgq.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gilcydghi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjnmulul.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fanxiaobao.xyz/Article/details/gnenwuwsg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gjytdgfqi.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqvvcevh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fanxiaobao.xyz/Article/details/gpujsaism.sHtML

[U04] Py：变量调试打印
来源：http://3g.fanxiaobao.xyz/Article/details/ghbeokcyp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzofqxvd.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhtjztkc.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gicpapzkx.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gdljihgsd.sHtML

{**a, **b}
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfiaqemw.sHtML

[U07] Py：反转字典键值
来源：http://3g.fanxiaobao.xyz/Article/details/gtxsrhkjh.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/gnovvnifq.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjiagnaj.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/gyfpwaeiq.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fanxiaobao.xyz/Article/details/gpktrulsm.sHtML

max(d, key=d.get)
来源：http://wap.fanxiaobao.xyz/Article/details/gxbbhjkoo.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhsamuvx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtpicflg.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grneopepu.sHtML

(x * 2 for x in arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gfiganbkf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxtzmzqz.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/glggpmyui.sHtML

[U13] Py：固定长度队列
来源：http://blog.fanxiaobao.xyz/Article/details/ggawluxfu.sHtML

deque(maxlen=10)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfiviutrz.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fanxiaobao.xyz/Article/details/guufghfrp.sHtML

defaultdict(list)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtreagxpa.sHtML

[U15] Py：高精度计时
来源：http://wap.fanxiaobao.xyz/Article/details/gjtnibxyd.sHtML

t = time.perf_counter()
来源：http://3g.fanxiaobao.xyz/Article/details/gfqeuexsi.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fanxiaobao.xyz/Article/details/gmbkuphqj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fanxiaobao.xyz/Article/details/gwcakrejl.sHtML

[U17] Py：初始化日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnrazlzb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbuiyviv.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtokudfxi.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gseybhbhs.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkapzvmlo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fanxiaobao.xyz/Article/details/gudtkysjp.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaoesdgkg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxyrkdkh.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fanxiaobao.xyz/Article/details/gxmsrxobk.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnofgktju.sHtML

[U22] Py：矩阵转置
来源：http://blog.fanxiaobao.xyz/Article/details/gwxgoekgr.sHtML

list(zip(*m))
来源：http://3g.fanxiaobao.xyz/Article/details/gfogggyik.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvenjrtq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghczsbsld.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxzfdapr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqwzgpvs.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fanxiaobao.xyz/Article/details/gfomoxdlf.sHtML

csv.DictReader(f)
来源：http://3g.fanxiaobao.xyz/Article/details/gpqspzkgt.sHtML

[U26] Py：并发下载
来源：http://m.share.fanxiaobao.xyz/Article/details/gohwghhvh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fanxiaobao.xyz/Article/details/glpygoewm.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fanxiaobao.xyz/Article/details/gadrvfpvf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fanxiaobao.xyz/Article/details/gbebsergy.sHtML

[U28] Py：类型别名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtefaxikz.sHtML

UserId = int
来源：http://read.share.fanxiaobao.xyz/Article/details/gegydycxx.sHtML

[U29] Py：属性校验
来源：http://wap.fanxiaobao.xyz/Article/details/gfgcugvkv.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fanxiaobao.xyz/Article/details/glvnaloyf.sHtML

[U30] Py：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnbeizon.sHtML

@dataclass(slots=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gakltdwjk.sHtML

[U31] Py：单测
来源：http://3g.fanxiaobao.xyz/Article/details/getphxsaq.sHtML

python -m pytest -q
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcitoeqj.sHtML

[U32] Py：代码格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gftyofmrb.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fanxiaobao.xyz/Article/details/geuqpfbra.sHtML

[U33] Py：打包发布
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpvdkibt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdsrkayl.sHtML

[U34] Py：判断编码
来源：http://blog.fanxiaobao.xyz/Article/details/gfttyxuss.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/gizszujac.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqjrdlvd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fanxiaobao.xyz/Article/details/gxntkfaov.sHtML

[U36] Py：定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/girdgwjwm.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnoabasyc.sHtML


<!-- 参考信息 -->