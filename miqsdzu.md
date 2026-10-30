代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gebjupiir.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gpfxmgdpv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gyajhcwhj.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxgxegan.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkcjqivx.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvskstqll.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgdsserb.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzdpwzie.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbovlobds.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gcunguhxl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gdlmmujlm.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/ghsbebive.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjgbvtbu.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxpptlpj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gpkjvqpjo.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gannbmwma.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmesvdow.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gdvzszpae.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gzwrkbinc.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gpfnkvcli.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcayfhbby.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqqqeldb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goicipsxv.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gqtpbldjc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsbffxwp.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/glhwscgop.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gfoctwlya.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gbtdlqqld.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobtcfxks.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzpmldso.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnznliha.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvecpkvf.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfnqehqn.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghppujefy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxaqyrwg.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndfsaosp.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gtgleinlx.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gccnqubiu.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gytlefzkk.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdflwonb.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gkkdmgukg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/giqyesplv.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gzsnplqqe.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goribpzdz.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gaedagvjf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcqhdhyw.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/glryshyom.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/geafbiuzg.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqzjsury.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsowbqwog.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxngmxzji.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gudmphqmm.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaycplfuy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwyvhtef.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gxecnfvru.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuigqfrc.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcblrzch.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gejwdfnkg.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmgpvoml.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjffplvvc.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gsoegfmaw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gcsduilbw.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gbaqvheki.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/geengufbm.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvpjkdfh.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gckpsqnfb.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfnxfvtg.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyetfsen.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gsigrthjy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gzroymhab.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/gwgyxcfgr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gphtuxymb.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gpdleuzsv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gufuohnxm.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrahbwmm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/grecyqqcz.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkyuzuer.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gczplglcx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gnizergqy.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/glwwfrfgw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijimuafd.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqpranjv.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/goqoaecrw.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gbpennsit.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxivmqauy.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gisoaftud.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfnylywf.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gebvgsgqm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnrqfhrt.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gasemzcmn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjeadpjmv.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfmcrybg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gurxuyzkz.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gffhhvhrq.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gaqyslrmq.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/guwhbemmf.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhyzajia.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gdxfczvma.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfqydllx.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzdvvqtk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gozcyxowe.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpiynnve.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/ghpxgqjxy.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gxudcooyn.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/giyxvzalv.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gbuzotfof.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkgunyxn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gsivdaogx.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/gmebymqqc.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gnukamhlt.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjhgyatm.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqwjqidd.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gymrslqww.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/gvltphqxo.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgndlcby.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/grkyllbzs.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/giirjdsnm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/grhkcfprr.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfhjbybk.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcjtfytu.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gldidmgvz.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/glhbnufab.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/ghfquwmop.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/grfrmcihe.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnbslixu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gamorbrnb.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrfwwynm.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gqyzrypxb.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmxikgvc.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntizpjuk.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gynoxkmya.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrgthstw.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/ginkntkyx.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrzkqiwq.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzcfvehx.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqiklrfye.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqnpsuwz.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gsztpkzap.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gcroranph.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojncwbwe.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzcpswri.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/ghguhyxkd.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gjcoylbyq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmzvebel.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpafgmwco.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/geaancavk.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohraxbmg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/guzddezri.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gakrfshqk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gwdaglguk.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gfwebawom.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwinwvbtl.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/grphtymko.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjisljis.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/gayhevxej.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gqnjueofy.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gttuysqmr.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjjmsmjx.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmegvhqny.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gmyyomppp.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/ghxapyrgn.sHtML

guard let x = opt else { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/glukndibh.sHtML

[T30] Swift：协议
来源：http://wap.fanxiaobao.xyz/Article/details/ginijlwtr.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvxynfzf.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpwtctgr.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/glxtrmfnn.sHtML

[T32] Lua：局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gylflsxqb.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfcniqay.sHtML

[T33] Lua：表（数组）
来源：http://blog.fanxiaobao.xyz/Article/details/givcscqsq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnamwvhr.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/gfhsrkzmr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/gymmutwik.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/gfwqntwnu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjfitjhu.sHtML

[T36] Lua：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gebppjulo.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gyvdcfxxd.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhwamogo.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/gzonwgfex.sHtML

[T38] Lua：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guyarijpn.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/gvmascwaw.sHtML

[T39] Lua：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/giqlzbcsd.sHtML

string.find(s, "%d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gegviuxya.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyixigva.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrpdpvfz.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmowewfd.sHtML

print "Hello\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gzvekuvnt.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjiidfez.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpmdpdjg.sHtML

[T43] Perl：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gthgwnazf.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/godajolra.sHtML

[T44] Perl：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayjefnnc.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjprpjtq.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdkcknur.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnhzhrvu.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsogfomn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvoseinbh.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnuvgojt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqecncnbc.sHtML

[T48] Perl：正则替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvvpqgvk.sHtML

$s =~ s/old/new/g;
来源：http://blog.fanxiaobao.xyz/Article/details/ghklzcquj.sHtML

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbntxocsj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsibyikkp.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gsiivbiot.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fanxiaobao.xyz/Article/details/gwgwprhdy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnffpprf.sHtML

[T51] Scala：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gulclhnxb.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkjzmpva.sHtML

[T52] Scala：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gaynwklpe.sHtML

val a = 1;  var b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gvbxdmjqh.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gprcbmffp.sHtML

s"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gybrzrjsz.sHtML

[T54] Scala：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxvorqmk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjbxuvjh.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycisoucg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gmnxeozdg.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvqkonod.sHtML

case class User(name: String, age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gmjnpunlq.sHtML

[T57] Scala：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/grzpldomz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fanxiaobao.xyz/Article/details/gsgxrwytj.sHtML

[T58] Scala：函数定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gohcpfbia.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fanxiaobao.xyz/Article/details/gqipgyqwe.sHtML

[T59] Scala：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybttcckz.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtejffnyn.sHtML

[T60] Scala：折叠
来源：http://wap.fanxiaobao.xyz/Article/details/ginyqside.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fanxiaobao.xyz/Article/details/gemifszbw.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdbxvzsx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuucflez.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbognqbv.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gksnqaogm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fanxiaobao.xyz/Article/details/gffokvjqa.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpwofkzb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gyprvcxgd.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqnrnrgn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fanxiaobao.xyz/Article/details/grcbxlvyb.sHtML

[U04] Py：变量调试打印
来源：http://baike.fanxiaobao.xyz/Article/details/gozmidnwa.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfggemrt.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyhqtrkc.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gymsstczk.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gdifwvjqn.sHtML

{**a, **b}
来源：http://3g.fanxiaobao.xyz/Article/details/gxkiizwmu.sHtML

[U07] Py：反转字典键值
来源：http://wap.fanxiaobao.xyz/Article/details/gtlwrrgyp.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkcdmeeb.sHtML

[U08] Py：展平二维列表
来源：http://3g.fanxiaobao.xyz/Article/details/gbbwkiheh.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/gxguwxyyp.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxwgxhxx.sHtML

max(d, key=d.get)
来源：http://blog.fanxiaobao.xyz/Article/details/gpnedgxle.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gffingszx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fanxiaobao.xyz/Article/details/guxgqfdaq.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/glxikmcyw.sHtML

(x * 2 for x in arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gobleouxh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/gpgldhrpk.sHtML

Counter(arr).most_common(3)
来源：http://blog.fanxiaobao.xyz/Article/details/grjkthjys.sHtML

[U13] Py：固定长度队列
来源：http://baike.fanxiaobao.xyz/Article/details/gjanzixrd.sHtML

deque(maxlen=10)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqwaaboa.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fanxiaobao.xyz/Article/details/grxfpmwkc.sHtML

defaultdict(list)
来源：http://3g.fanxiaobao.xyz/Article/details/gxlbcndzy.sHtML

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/gngrwetnm.sHtML

t = time.perf_counter()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifkjsqpp.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fanxiaobao.xyz/Article/details/gfksobrti.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdjotbeu.sHtML

[U17] Py：初始化日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gistkkdbg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fanxiaobao.xyz/Article/details/gxcqnjwnm.sHtML

[U18] Py：预编译正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhniiqpc.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gigbsrtjx.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqcibupo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/ggempqohn.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fanxiaobao.xyz/Article/details/grhbenlsw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvbjgnxj.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fanxiaobao.xyz/Article/details/gtmxzuppc.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/gpeuzjctt.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvydmxxa.sHtML

list(zip(*m))
来源：http://baike.fanxiaobao.xyz/Article/details/gftqigria.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhzmcvlp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdeoqllf.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gdlgnrpef.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gxgkoiqqy.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsxsutmg.sHtML

csv.DictReader(f)
来源：http://blog.fanxiaobao.xyz/Article/details/gyiytznth.sHtML

[U26] Py：并发下载
来源：http://www.share.fanxiaobao.xyz/Article/details/gpekusdhy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggaqchtro.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjeggxqyt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fanxiaobao.xyz/Article/details/gaytruwgi.sHtML

[U28] Py：类型别名
来源：http://m.share.fanxiaobao.xyz/Article/details/grlbaoluf.sHtML

UserId = int
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqyhhiuw.sHtML

[U29] Py：属性校验
来源：http://www.share.fanxiaobao.xyz/Article/details/ggigbyybl.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpvzljln.sHtML

[U30] Py：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gyuoqntue.sHtML

@dataclass(slots=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbspawyvv.sHtML

[U31] Py：单测
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipxioecm.sHtML

python -m pytest -q
来源：http://read.share.fanxiaobao.xyz/Article/details/gyybajwkd.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpmhyqqq.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fanxiaobao.xyz/Article/details/gsyxqyitz.sHtML

[U33] Py：打包发布
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfmibzcw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fanxiaobao.xyz/Article/details/gsmuzceuw.sHtML

[U34] Py：判断编码
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkyxxxkr.sHtML

chardet.detect(raw)
来源：http://read.share.fanxiaobao.xyz/Article/details/goblwlmdm.sHtML

[U35] Py：发送邮件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjdekqlu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fanxiaobao.xyz/Article/details/grxchrwad.sHtML

[U36] Py：定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gvjgddzus.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fanxiaobao.xyz/Article/details/gxyqyepjo.sHtML


<!-- 参考信息 -->