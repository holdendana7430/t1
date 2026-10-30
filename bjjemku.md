代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdwsyidd.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/goicolanj.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gutwthjkb.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbdgdwql.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gzracvqlk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gosgfztsf.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjusocham.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmjwxiqso.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjruylmsp.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/guuezxqzz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gqvrsvzvo.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gpkjfdqfb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gayhmdooc.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/ghrszdxdx.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwmabcfz.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gglekfgra.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/goinrbrhl.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gzshpfgqd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/greicjzfb.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gmbwvpcrv.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/ggfdljwre.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gsgpzzhcm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzfyqwfb.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatepfpjt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gqshhdwyb.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/goieimbpq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gmvlguatb.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gctiaycvw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gshznbtnx.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gyocqjrkf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/guntoxuyt.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gscqpqkyr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gdogmjwkk.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/geaeymvnd.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gecxeihvf.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gqxzonsil.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gqfnkpkbl.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gkrgwvwbc.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdffxhwj.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemjxrbtk.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gieuikpyp.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/grxotcfcg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzzwwwqz.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/geqseyhvz.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gsljpgikc.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gvrqydzau.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gzvxnfqtk.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpwlbaqf.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzscurra.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbwmtyuzy.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxiisbqkh.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjhbjwph.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/geobdgmgj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gmpotnnsb.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gsvsuyrpt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkwpurecr.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzdebieq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhyvqmqk.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwuisvkt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gvwcurvjc.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gqzxrnbuj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfieydvjq.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurcdnrud.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtaipras.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjqcpjve.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gpdfdhugh.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/guoibkuiv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/girqkjluz.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyfbtovc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gvzfztkhm.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/givvwplos.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gmopegwqk.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/guuasyooe.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxdrrooz.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gdudpwnfs.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glzsmciaw.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gefnftyjm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/geqydlnbw.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/gpkwgafae.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggwqyoxyt.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixhlozcg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggziidhcy.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnyutgli.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gqowhxtia.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/goinvaddz.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/guyewklyy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gtqdmjbke.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqjpytkp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gmdnitpcs.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/grlooqbeq.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntijebbr.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gzlgxekym.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvaetmlj.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gviqxiznf.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gpqgoiudo.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/guokkvwdh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gyeqhoyyp.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerscnhke.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqzplkoq.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbmoykuj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzttoygya.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/ggooszwns.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gijzhvelu.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gyktcfqqf.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gyvreadsm.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gggkawwdy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytsefila.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gzdtfwswx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gjlrysvaj.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjhajksk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gkwatisla.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojfhlada.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gtimxlrfn.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlshiuqt.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmppmyau.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gzvdfguwe.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/giltdyfya.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/guqbjfxsx.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/gqkmazrmk.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouszvfqm.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnajfjwgz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/giylwkilj.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gunddtqak.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmghmtpof.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkonuzckf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtohexejd.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gcykwzerf.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwalpyec.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gbfjsefoj.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrlbncfy.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gksqjycnv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfrjlict.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/grbrtrfex.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/gopakksod.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbynlonp.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaplzhbfj.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/grlyaymis.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmsmnbdf.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/ggvakpqwr.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gdccuiadc.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/gfdchjtwj.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslrmwlrg.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gfydmshcs.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gugtbbzki.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gzulbophu.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gpabkspzy.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gscrjjojr.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/guoqqhcxv.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrlxxcnz.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvkadery.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/glivorwuf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpufrgmtk.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/ghejunctl.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gxexcgkdj.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/gyogvxysd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gguczglhc.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gnssfttbj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltrnqzde.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gtjysnvdu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/ghreudrqk.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/gziteyecz.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfitalhjd.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/grqqhfkmi.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gqsjpvbjr.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgxymrfz.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/gkrvauggi.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gasmmmgcz.sHtML

enum Color { case red, green }
来源：http://read.share.fanxiaobao.xyz/Article/details/gokdulgsh.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkxcaium.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gcosxverg.sHtML

[T30] Swift：协议
来源：http://blog.fanxiaobao.xyz/Article/details/grnlrxnzs.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxdjrcuk.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqwslgjp.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcstdmwuq.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqecripmg.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgxvpzym.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjujtzht.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftdvmqor.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrvugxhn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gaumorvvk.sHtML

[T35] Lua：字典表
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbhiknuw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gserigwnl.sHtML

[T36] Lua：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxneiopy.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/gzxvmdzac.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdustyfb.sHtML

"a" .. "b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmplblpku.sHtML

[T38] Lua：条件
来源：http://3g.fanxiaobao.xyz/Article/details/grllarxkv.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/gyyxeshto.sHtML

[T39] Lua：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gyckxomvz.sHtML

string.find(s, "%d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gavcvfwhn.sHtML

[T40] Lua：元表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbtkgyrt.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/gefxlpnpi.sHtML

[T41] Perl：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gxnsajzns.sHtML

print "Hello\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gabgaltpx.sHtML

[T42] Perl：变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyvioilz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsqnnrjn.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gtaxbarbb.sHtML

"值: $a"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcgdljsp.sHtML

[T44] Perl：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gthqbkffu.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gehrnkwku.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gkknwatpg.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjjfhafkz.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gauqujkab.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fanxiaobao.xyz/Article/details/grmdobwdm.sHtML

[T47] Perl：正则捕获
来源：http://baike.fanxiaobao.xyz/Article/details/gcxpxmbhx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gruqyptmw.sHtML

[T48] Perl：正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gsoqhtclp.sHtML

$s =~ s/old/new/g;
来源：http://blog.fanxiaobao.xyz/Article/details/gqhzbbzue.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gbvcfemjf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gustwtvvu.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/glmbtafrj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwwvdvas.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqqbequi.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrqdwxjx.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gvqcduftn.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gnjduexqg.sHtML

val a = 1;  var b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpjmbwgf.sHtML

[T53] Scala：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gzoopsnlt.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gljvbyjbq.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgglofrm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbhjbgaj.sHtML

[T55] Scala：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/ggobxqfkj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdafctah.sHtML

[T56] Scala：样例类
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgcvpwde.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfesfdkfa.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqxsnklx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/gcqovyjka.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/gthcqtvdn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gkdmwuyua.sHtML

[T59] Scala：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gzezekwpl.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggthetlqa.sHtML

[T60] Scala：折叠
来源：http://baike.fanxiaobao.xyz/Article/details/gvugaofbw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fanxiaobao.xyz/Article/details/gtlxjcwnl.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqvtvjih.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlxzojov.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gawlwncvg.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fanxiaobao.xyz/Article/details/glmyhdnzn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvukbvmj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/gxxjgbbyx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gqzlyvzma.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goasfoffj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fanxiaobao.xyz/Article/details/gsdrgwjbi.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihocwetn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gthwwvbag.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/gdnjsxdil.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganernlux.sHtML

[U06] Py：合并两个字典
来源：http://3g.fanxiaobao.xyz/Article/details/gzyfehijh.sHtML

{**a, **b}
来源：http://baike.fanxiaobao.xyz/Article/details/goewzqkur.sHtML

[U07] Py：反转字典键值
来源：http://baike.fanxiaobao.xyz/Article/details/ghhdfrbun.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcqqaduy.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gsuiaiqib.sHtML

[y for x in nested for y in x]
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvxwgoqp.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fanxiaobao.xyz/Article/details/ghtecyhbe.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuojmrxg.sHtML

[U10] Py：按值排序字典
来源：http://baike.fanxiaobao.xyz/Article/details/ghhgxajrx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fanxiaobao.xyz/Article/details/glekmgmql.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdjutwet.sHtML

(x * 2 for x in arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gnuaishkp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gqehbjuvf.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gojmuqkfb.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrwmxsce.sHtML

deque(maxlen=10)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrqkhxdu.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fanxiaobao.xyz/Article/details/grwxdyugf.sHtML

defaultdict(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvzchpge.sHtML

[U15] Py：高精度计时
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzsmvojv.sHtML

t = time.perf_counter()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glodcmjty.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fanxiaobao.xyz/Article/details/gdeuxhypv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fanxiaobao.xyz/Article/details/gfapgbcfs.sHtML

[U17] Py：初始化日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqdfhxja.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxakeptaw.sHtML

[U18] Py：预编译正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gitycpgzr.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gxpkqtbvq.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/gwnuubvfl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gujkftsgl.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fanxiaobao.xyz/Article/details/gzysysbmc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcknoatm.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskpqdjwh.sHtML

@contextlib.contextmanager
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnkgxdhp.sHtML

[U22] Py：矩阵转置
来源：http://baike.fanxiaobao.xyz/Article/details/gfwjjdfix.sHtML

list(zip(*m))
来源：http://baike.fanxiaobao.xyz/Article/details/gorwdidac.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjtacars.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fanxiaobao.xyz/Article/details/gdwabdmyk.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gcevwqibl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gbrigxtso.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrgphqsi.sHtML

csv.DictReader(f)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbodwdouu.sHtML

[U26] Py：并发下载
来源：http://m.share.fanxiaobao.xyz/Article/details/gdohlkgcs.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsukzker.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fanxiaobao.xyz/Article/details/gbegdwxvr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxpgyajj.sHtML

[U28] Py：类型别名
来源：http://www.share.fanxiaobao.xyz/Article/details/gawuxjxoz.sHtML

UserId = int
来源：http://baike.fanxiaobao.xyz/Article/details/gmdgaexxm.sHtML

[U29] Py：属性校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gaacrbdcc.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/gnocijdxv.sHtML

[U30] Py：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfjwbasb.sHtML

@dataclass(slots=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gwpxbjtrh.sHtML

[U31] Py：单测
来源：http://3g.fanxiaobao.xyz/Article/details/gabkxqhfe.sHtML

python -m pytest -q
来源：http://baike.fanxiaobao.xyz/Article/details/gsbnjjbhm.sHtML

[U32] Py：代码格式化
来源：http://blog.fanxiaobao.xyz/Article/details/ggdhfntmy.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdbmwlzj.sHtML


<!-- 参考信息 -->