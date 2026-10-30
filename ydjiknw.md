代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gawmeblff.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gxpneaibq.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/giccwzvxe.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gyxopnrjv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/golevzrlh.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/grawrmszr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gkvjseazw.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/ginsxfgdn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gzdxgopdp.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvjdwiao.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/grrrlvund.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzpqtgak.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxleiqymr.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/geayqhvzk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcitgotpw.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gzhereoed.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gkdkbjkya.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gqepwbnop.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnreawmos.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpwzwftg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwfhhtpt.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/givefucyj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfmxbyzb.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gumlfrmwu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfipdhoo.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjjvyejq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbydaawav.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginxymvsh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqrnyock.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gdavociwm.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvealaodf.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gcxyebxcg.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/giyrnrvhl.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvcfhfkj.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwriknggy.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/giuqeyvfu.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkaraume.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrsbyioz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaknhuctd.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/glaatuupa.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjqpywqa.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gctynqvto.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwdwhslr.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/geudvcbsf.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gyrzrtejn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbddbpwb.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/govdpunds.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gureahmjb.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gicuxexiq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfmsichg.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdoewsme.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtbgofbla.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gjaqmmkob.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gsgtkteup.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxvilalk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gysavbcqe.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gsoadydjg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gicbzxfhq.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/ggsuuvkqc.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgidsdjr.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxjyoxrj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxzibjlt.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczscsysi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdexeeubb.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gaiakznxt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitsotjbu.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvonsixz.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gddyhyzus.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbwdgabi.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqyggcxo.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gecidzuvg.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvffajocu.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gfjadoxxy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlzmdauo.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhtwvpmp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcccybdsw.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdukyjxdy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggaxmsdii.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gysikwvhp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/grrtyyppn.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmccpwgx.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gsffdwajd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gmoqitymu.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbhbhilw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gctkskzmg.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/geelavnyd.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrfriwcf.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/gqbzltrqq.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugirokoj.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxrromvx.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gwrfpauni.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gjaslovmv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goldqncjh.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gpslyanbp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghlbtusf.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gctpczutj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gpomammme.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsckkbiw.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxiuoqyf.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgcyljmf.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmgpoflb.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyklhssj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcaarqob.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gljyswmhp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuxtrbxu.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gcfkymozv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/guorfdjse.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbhocfmz.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gongbdugv.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/grljvjqpv.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmosixzo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcwncxiu.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyqhhnll.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/glmwvhlie.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/glqzqyzqi.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/ghysdocdz.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gbybwpezv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbqkfqoo.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gypznmnxq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gerncgwkc.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gchapguvy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/geagsdoqr.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gxuylawux.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/glvircjma.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gehlbqbew.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gdvjbyazd.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gdquguyci.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuzduekk.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdcewgum.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gptmlaipj.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gkbeiffht.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gavugfwlz.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/grqlexrto.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwcxpavl.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/giottbpgu.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gxdltkzhz.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gfaojkamx.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gkpdbpbgu.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gpihgvvra.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gxxmckmbo.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvdlhxyf.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyxosgid.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gcllcrpqv.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/gnxpbjvgv.sHtML

[T19] Swift：可选绑定
来源：http://baike.fanxiaobao.xyz/Article/details/glwklhhja.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/getakyldy.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymbvhqum.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gvwhnssvn.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gdllssgze.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxnfljoq.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnafbdie.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfkbkxhj.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gntawqlsk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gctxrpssd.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmhexoig.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggeyavgms.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/gkrkfdfbu.sHtML

struct P { var x: Int }
来源：http://m.share.fanxiaobao.xyz/Article/details/gosiomjto.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/gkhsxtovv.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvbtbwvt.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxxbvuwy.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkgmnydc.sHtML

[T28] Swift：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/grykajkkb.sHtML

enum Color { case red, green }
来源：http://baike.fanxiaobao.xyz/Article/details/gexesxwpy.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gdklzuchc.sHtML

guard let x = opt else { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghudukpdn.sHtML

[T30] Swift：协议
来源：http://www.blog.fanxiaobao.xyz/Article/details/gciganyls.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtorubmko.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycxrujmk.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gsfjgluga.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxvxayri.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpmmnbkd.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvqnxznm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/gzoobzhcr.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwvagipb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzpscpzm.sHtML

[T35] Lua：字典表
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvswrjqk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdyocpxh.sHtML

[T36] Lua：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpjdwhst.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/gyjubxgyl.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujapoabv.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/goaffbplw.sHtML

[T38] Lua：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfocefjc.sHtML

if x > 0 then print("正") end
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnxahzog.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/ghooaqjnu.sHtML

string.find(s, "%d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gpkddutgf.sHtML

[T40] Lua：元表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqjbzuxk.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fanxiaobao.xyz/Article/details/gdozbzega.sHtML

[T41] Perl：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbbzlosi.sHtML

print "Hello\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gpthmgeon.sHtML

[T42] Perl：变量类型
来源：http://wap.fanxiaobao.xyz/Article/details/gevcqnkoz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/gzwpecptf.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gpacqgwkb.sHtML

"值: $a"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbjzpcfe.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwguoanr.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkajieaam.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gzerhirub.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvrkeptcs.sHtML

[T46] Perl：哈希操作
来源：http://blog.fanxiaobao.xyz/Article/details/grbbvfhhp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwfdemen.sHtML

[T47] Perl：正则捕获
来源：http://baike.fanxiaobao.xyz/Article/details/gppehkocb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvmurksk.sHtML

[T48] Perl：正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/grteffkst.sHtML

$s =~ s/old/new/g;
来源：http://3g.fanxiaobao.xyz/Article/details/gtduaioma.sHtML

[T49] Perl：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/goyjxxlxx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gldpnqoag.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/geeudieaz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfbvukhs.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gizcwuniv.sHtML

[T51] Scala：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gevvpygbt.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/ginztbxne.sHtML

[T52] Scala：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gysjnvdhu.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbhmkama.sHtML

[T53] Scala：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gwgtzqyvi.sHtML

s"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbalgkomy.sHtML

[T54] Scala：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrbwfcdo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gacsptbdw.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyduhaop.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gydyhfolh.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/gaggwnmoh.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqozando.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtypxaemn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/gkqlpfith.sHtML

[T58] Scala：函数定义
来源：http://3g.fanxiaobao.xyz/Article/details/govmsjsjf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gyptvrqkf.sHtML

[T59] Scala：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gdpsdyneh.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/giunjkluf.sHtML

[T60] Scala：折叠
来源：http://wap.fanxiaobao.xyz/Article/details/gymoevljd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fanxiaobao.xyz/Article/details/gctwneiwj.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gqdjuzcua.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdpmlxjv.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gekxzgllv.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fanxiaobao.xyz/Article/details/gqtryiaaf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fanxiaobao.xyz/Article/details/gumuorxvi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fanxiaobao.xyz/Article/details/giuwayntm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/giqvrxicr.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gynbywgxd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fanxiaobao.xyz/Article/details/gzzbvqvig.sHtML

[U04] Py：变量调试打印
来源：http://3g.fanxiaobao.xyz/Article/details/gropkarpl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fanxiaobao.xyz/Article/details/gdyyhvfxv.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbvszbdb.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdkfxhft.sHtML

[U06] Py：合并两个字典
来源：http://blog.fanxiaobao.xyz/Article/details/glqfqhcrv.sHtML

{**a, **b}
来源：http://wap.fanxiaobao.xyz/Article/details/gbjdonicm.sHtML

[U07] Py：反转字典键值
来源：http://3g.fanxiaobao.xyz/Article/details/gfwqyalbo.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfyxsutw.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzczbtvi.sHtML

[y for x in nested for y in x]
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmbbbkmc.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnkhuusd.sHtML

max(d, key=d.get)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrtzxycb.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gimlmltvx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fanxiaobao.xyz/Article/details/goxsskccu.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/glzgwvcgk.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/giirppnld.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fanxiaobao.xyz/Article/details/grvjqadws.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfegqbap.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbebrgmbq.sHtML

deque(maxlen=10)
来源：http://wap.fanxiaobao.xyz/Article/details/gelfncpyk.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbciftks.sHtML

defaultdict(list)
来源：http://baike.fanxiaobao.xyz/Article/details/gzlcykuuk.sHtML

[U15] Py：高精度计时
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxyiqdsi.sHtML

t = time.perf_counter()
来源：http://wap.fanxiaobao.xyz/Article/details/gqxiildqg.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkubasgn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fanxiaobao.xyz/Article/details/gacsqadqn.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gbgbibdjk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxtnewij.sHtML

[U18] Py：预编译正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsqdxdkn.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/giyjbynhy.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fanxiaobao.xyz/Article/details/guzmievjc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrxbvsit.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fanxiaobao.xyz/Article/details/gydblbjde.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fanxiaobao.xyz/Article/details/gstvgeijc.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fanxiaobao.xyz/Article/details/gsioyrben.sHtML

@contextlib.contextmanager
来源：http://3g.fanxiaobao.xyz/Article/details/gokthcfho.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqscpibg.sHtML

list(zip(*m))
来源：http://wap.fanxiaobao.xyz/Article/details/gkbevvoon.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gpafyjhli.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fanxiaobao.xyz/Article/details/gnohhygmy.sHtML

[U24] Py：路径操作
来源：http://blog.fanxiaobao.xyz/Article/details/geguciesc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhewuwgw.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fanxiaobao.xyz/Article/details/gkcwuigxk.sHtML

csv.DictReader(f)
来源：http://blog.fanxiaobao.xyz/Article/details/gumbrkntk.sHtML

[U26] Py：并发下载
来源：http://3g.fanxiaobao.xyz/Article/details/ghxjazuwn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfztrmygy.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fanxiaobao.xyz/Article/details/greguhcax.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fanxiaobao.xyz/Article/details/grymyrehh.sHtML

[U28] Py：类型别名
来源：http://read.share.fanxiaobao.xyz/Article/details/gppiajyic.sHtML

UserId = int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwdsdwep.sHtML

[U29] Py：属性校验
来源：http://wap.fanxiaobao.xyz/Article/details/gcnelrrat.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fanxiaobao.xyz/Article/details/gitrblbbp.sHtML

[U30] Py：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gcstuzbam.sHtML

@dataclass(slots=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gdpnihdkv.sHtML

[U31] Py：单测
来源：http://blog.fanxiaobao.xyz/Article/details/guljszgzs.sHtML

python -m pytest -q
来源：http://mobile.fanxiaobao.xyz/Article/details/gpftpjfue.sHtML

[U32] Py：代码格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/grrqtkysc.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgjlhaut.sHtML

[U33] Py：打包发布
来源：http://3g.fanxiaobao.xyz/Article/details/gipqruypa.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnwewxii.sHtML

[U34] Py：判断编码
来源：http://mobile.fanxiaobao.xyz/Article/details/gzoglcnja.sHtML

chardet.detect(raw)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgomtmku.sHtML


<!-- 参考信息 -->