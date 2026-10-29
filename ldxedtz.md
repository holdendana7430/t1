代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gvirybmxx.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/grxgtcyhp.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gxqvvbdrz.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/ghklthial.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.zdbjq.cn/Article/details/grfcpettc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gbrioqkzg.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gufdpohsg.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/gajsdjelv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gotqxphtf.sHtML

[S13] C：宏定义
来源：http://www.share.zdbjq.cn/Article/details/gqvrccgzw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gnbixkioy.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gifdfimfm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/gtowipeut.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/grnbietjq.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/guoidriwa.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/gyhkbcvvt.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gbmeelcap.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/gzyvqzpzt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gddgbhruq.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gbjmnaszm.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/gazgczgvo.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/gdgwobgoj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gkennemkb.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/ghqkuavzr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gvosirkfx.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gdhbaipaj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gqkoevweh.sHtML

[S22] C：字符串转数字
来源：http://m.share.hesvh.cn/Article/details/guqadndcf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/glymqwhle.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/ghgawucir.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gylzgpvfl.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gqltnerle.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/guzdsuaqr.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gkocxwbvh.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/gchiuduff.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/gejcgqneb.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fehbvm.com/Article/details/gacvhnoqv.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gaunopbmm.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/ggkzecovg.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gzjleglqc.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gynlmjpzs.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gdbsxitxc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gpiigwrfg.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/gdhhwjsws.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gxzgnnpon.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/ghxtvrowd.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gvuotbwrz.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gkbcwnhhr.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/gczlzzhgj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gxayjxlfd.sHtML

[S32] C++：字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gjcpaayws.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/ghayhtzdv.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gpykbtqsi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/gagnpdqmr.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gquvrwxgl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.hesvh.cn/Article/details/gweboqnrj.sHtML

[S35] C++：map
来源：http://www.share.hesvh.cn/Article/details/gmxsxvckr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gmzzepfic.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/gwowcdosb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/girobnpbr.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/giecxrdbt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/ghdxlavpf.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/guqjqyeso.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/gcrlbpilo.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gipftrmvu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gujrqcshl.sHtML

[S40] C++：查找元素
来源：http://www.blog.fehbvm.com/Article/details/gtntphpvk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/gwsascgvt.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/giukureim.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/glscywcbu.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gfncjzxnv.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/gntemhboc.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gvvtjhtow.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/ggxdreped.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gbmuyzlem.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gbfnspkpa.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/glhzjkvee.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gfzqdrnyj.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/geaijbxdx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gfowkfkev.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/gqaxczawk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/ggvbqyood.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/grkyrnedf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/gieyubnit.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/gkfscixbf.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/gbeletrqk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gwdhjystk.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gteustgdg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.hesvh.cn/Article/details/geeucjehd.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gfxgjidfk.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gxzbgnots.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/gqiznbqjb.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gnwzubrxy.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gjlfrqlxo.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/gtbxjzokw.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/glhwipyvy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/gtbeluztw.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gvrtkbbjs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gufzniuya.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/gskqwzbcf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/geskbnhst.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gqxeagzhv.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gtegtafkm.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/ggnawvaoc.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/gakjtxivf.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gzjbxnktl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gjqhrggio.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gufrnlbeo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/gmpkqfsfo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxbscasux.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gjkelpxrn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/glfzshoun.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gocyrsiqo.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gcalzmduf.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/gdmpnuhax.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/gemxthvlq.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gmzghqvsv.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/grwtrikiz.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/gzgygzgga.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/groovdmov.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/grsckmfar.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gdmuspijk.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gubxdcpiq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gwuucfyoi.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gbedwlopa.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/gzoaafcdq.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/gpuxdcsqe.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gkziamrlj.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/gtdftdijn.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gtvrqaxtu.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/gzfkakwac.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/gpthydxrh.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/gbtdfkoxr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gtismfngj.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/getsnkoxc.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gyiafnkxa.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/gqbwrejtv.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/gjvwrxqoo.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/gspvoczxt.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/gifgaubyv.sHtML

[T15] Kotlin：接口
来源：http://blog.hesvh.cn/Article/details/ghddaekek.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/ghbzwedrm.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gqfrchcao.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gnxwtavis.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.zdbjq.cn/Article/details/gcqleffcb.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/gweoketlc.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gjvfbwafl.sHtML

"值: \(b)"
来源：http://m.share.fehbvm.com/Article/details/gmnfagamc.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fehbvm.com/Article/details/gxulyankz.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/gronfmvbi.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/gntntuafi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.hesvh.cn/Article/details/gkvqtkevq.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/gvvqgzrkz.sHtML

for x in a { print(x) }
来源：http://www.m.share.zdbjq.cn/Article/details/gdisiimur.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/gjppaxvhw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/gpmqgsrqo.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/ghcqavdhd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gxxpmrjze.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/grffysdip.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.zdbjq.cn/Article/details/glnnucrcr.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/gjqwysfqj.sHtML

struct P { var x: Int }
来源：http://www.m.share.hesvh.cn/Article/details/gsbjuozgw.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gndhpotcu.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/gfclghxmv.sHtML

[T27] Swift：错误处理
来源：http://m.share.fehbvm.com/Article/details/gueqofiek.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.zdbjq.cn/Article/details/gmytkhuxq.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/gyfufhhaw.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/gflnfarrg.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gpoabuitn.sHtML

guard let x = opt else { return }
来源：http://www.blog.zdbjq.cn/Article/details/gnbvpuvdu.sHtML

[T30] Swift：协议
来源：http://mobile.zdbjq.cn/Article/details/gaptfmzfk.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.hesvh.cn/Article/details/gkhdjpjms.sHtML

[T31] Lua：Hello World
来源：http://www.share.hesvh.cn/Article/details/gxfwkyehj.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gaczhfbwq.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/ghxyhmltk.sHtML

local a = 1
来源：http://www.m.share.hesvh.cn/Article/details/gexeylpqh.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/gdymoafkd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gixrwjjlx.sHtML

[T34] Lua：遍历表
来源：http://www.blog.hesvh.cn/Article/details/grmzxibei.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/gdlpavemy.sHtML

[T35] Lua：字典表
来源：http://blog.zdbjq.cn/Article/details/gydmybpsr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.hesvh.cn/Article/details/gxllbprbm.sHtML

[T36] Lua：函数
来源：http://3g.fehbvm.com/Article/details/goafvyqkn.sHtML

function add(a, b) return a + b end
来源：http://wap.zdbjq.cn/Article/details/gguaoruer.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gfepcfzrp.sHtML

"a" .. "b"
来源：http://www.blog.zdbjq.cn/Article/details/goviybxek.sHtML

[T38] Lua：条件
来源：http://m.share.hesvh.cn/Article/details/gbimbosuj.sHtML

if x > 0 then print("正") end
来源：http://read.share.zdbjq.cn/Article/details/gcliihxjq.sHtML

[T39] Lua：模式匹配
来源：http://wap.hesvh.cn/Article/details/gwuqgnwpt.sHtML

string.find(s, "%d+")
来源：http://mobile.fehbvm.com/Article/details/ghkbcavwr.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/gsrttpkcl.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fehbvm.com/Article/details/glupczsbz.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/gffehmrqk.sHtML

print "Hello\n";
来源：http://www.share.zdbjq.cn/Article/details/giadfgdzq.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gcknqctws.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.zdbjq.cn/Article/details/gvzpghknc.sHtML

[T43] Perl：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gpstinwug.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/gqvlukuvb.sHtML

[T44] Perl：条件
来源：http://m.share.fehbvm.com/Article/details/gwbkpnjiv.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.zdbjq.cn/Article/details/gtzvkllxg.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/ggevmnror.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/gfbwsctbn.sHtML

[T46] Perl：哈希操作
来源：http://baike.hesvh.cn/Article/details/gbgypawnj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdeqaicko.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/geealgbew.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/gcvvhzmjt.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/giezwdavf.sHtML

$s =~ s/old/new/g;
来源：http://wap.hesvh.cn/Article/details/gzqfekduk.sHtML

[T49] Perl：函数
来源：http://www.share.hesvh.cn/Article/details/gtruajfsc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gmurkyzcc.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gjmjblaqe.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.hesvh.cn/Article/details/gzfnlqyha.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.zdbjq.cn/Article/details/gbcezqvva.sHtML

[T51] Scala：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gzwliwzqk.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gtzciruyr.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gmmvnrpdg.sHtML

val a = 1;  var b = 2
来源：http://baike.fehbvm.com/Article/details/ghcwmtgxk.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gqrseyykw.sHtML

s"值: $b"
来源：http://wap.fehbvm.com/Article/details/ggpsftfls.sHtML

[T54] Scala：集合映射
来源：http://3g.fehbvm.com/Article/details/gwibcyxtq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fehbvm.com/Article/details/gzctbctgu.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gozypuhub.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.hesvh.cn/Article/details/gqnmnlpjo.sHtML

[T56] Scala：样例类
来源：http://mobile.hesvh.cn/Article/details/gbxjddzxf.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fehbvm.com/Article/details/glbunlluf.sHtML

[T57] Scala：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gvwstuvjq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fehbvm.com/Article/details/gghehqpak.sHtML

[T58] Scala：函数定义
来源：http://wap.hesvh.cn/Article/details/gnadzurev.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.hesvh.cn/Article/details/goskfipwv.sHtML

[T59] Scala：循环
来源：http://www.m.share.hesvh.cn/Article/details/gnmfpdrpe.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gpradqmuc.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fehbvm.com/Article/details/gebpuhsye.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/ginhwyiuv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gslafjzcb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/gumgdtnuy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gssihtvfj.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/ggkdnioew.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/gpdvlnxuf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.hesvh.cn/Article/details/grxsmzfax.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/gbxgiwpoc.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.zdbjq.cn/Article/details/grujmeerw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fehbvm.com/Article/details/gktujgweu.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/gmdqhocby.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/gotnouknn.sHtML

[U05] Py：列表去重且保序
来源：http://wap.hesvh.cn/Article/details/gkvfafixe.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/glihjnrtn.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.zdbjq.cn/Article/details/gogglgctf.sHtML

{**a, **b}
来源：http://wap.zdbjq.cn/Article/details/gnnnwlylf.sHtML

[U07] Py：反转字典键值
来源：http://m.share.zdbjq.cn/Article/details/glgpvjhna.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gijilpatj.sHtML

[U08] Py：展平二维列表
来源：http://mobile.hesvh.cn/Article/details/gdqwmlifr.sHtML

[y for x in nested for y in x]
来源：http://wap.hesvh.cn/Article/details/ghovyzxeg.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/guwiensxe.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/glvkfqczg.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fehbvm.com/Article/details/gpguxvnyz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.hesvh.cn/Article/details/giolylznu.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/gpbulkmud.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fehbvm.com/Article/details/gxuqrmuak.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fehbvm.com/Article/details/garlxxlfy.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fehbvm.com/Article/details/grnwtbzib.sHtML

[U13] Py：固定长度队列
来源：http://www.share.zdbjq.cn/Article/details/gqtwvpopp.sHtML

deque(maxlen=10)
来源：http://wap.zdbjq.cn/Article/details/gzedonyrv.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/gllvdnhje.sHtML

defaultdict(list)
来源：http://www.m.share.fehbvm.com/Article/details/grwejeczn.sHtML

[U15] Py：高精度计时
来源：http://wap.zdbjq.cn/Article/details/ggbyjwvcq.sHtML

t = time.perf_counter()
来源：http://m.share.fehbvm.com/Article/details/gtystuijo.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.hesvh.cn/Article/details/goxtfhmfd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gsxwujmef.sHtML

[U17] Py：初始化日志
来源：http://wap.fehbvm.com/Article/details/ggmmzkpdt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/gjnkwsyok.sHtML

[U18] Py：预编译正则
来源：http://read.share.fehbvm.com/Article/details/gvtsdubji.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.hesvh.cn/Article/details/ghplbfskr.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.hesvh.cn/Article/details/ghuhngfph.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fehbvm.com/Article/details/geangrwos.sHtML

[U20] Py：缓存函数结果
来源：http://wap.hesvh.cn/Article/details/ghmbxpmyo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fehbvm.com/Article/details/gllebdofu.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/ghhvawbkh.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/gsyilmxng.sHtML

[U22] Py：矩阵转置
来源：http://3g.zdbjq.cn/Article/details/gkyqoiimt.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/gvvepstdw.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fehbvm.com/Article/details/ggsokgkfa.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.hesvh.cn/Article/details/gfqgqmlde.sHtML

[U24] Py：路径操作
来源：http://read.share.fehbvm.com/Article/details/gpmpbrqou.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/glbfpugca.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.zdbjq.cn/Article/details/ghremhdme.sHtML

csv.DictReader(f)
来源：http://blog.hesvh.cn/Article/details/gdmzwgzzb.sHtML

[U26] Py：并发下载
来源：http://baike.fehbvm.com/Article/details/ghyqkmflz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/gqfxrhczb.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/grhxpefim.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fehbvm.com/Article/details/gcuswuwmb.sHtML

[U28] Py：类型别名
来源：http://www.blog.hesvh.cn/Article/details/ggqrlqjhn.sHtML

UserId = int
来源：http://m.share.zdbjq.cn/Article/details/gqdgtehhr.sHtML

[U29] Py：属性校验
来源：http://read.share.zdbjq.cn/Article/details/gonvpvhjw.sHtML

@property 与 @x.setter 配合
来源：http://wap.fehbvm.com/Article/details/getlsgvcr.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/gunquckkl.sHtML

@dataclass(slots=True)
来源：http://baike.fehbvm.com/Article/details/gvceuzocl.sHtML

[U31] Py：单测
来源：http://m.share.fehbvm.com/Article/details/gkbdjujtn.sHtML

python -m pytest -q
来源：http://www.m.share.zdbjq.cn/Article/details/gnynbfpzo.sHtML

[U32] Py：代码格式化
来源：http://3g.hesvh.cn/Article/details/gnclorzso.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fehbvm.com/Article/details/gurdcxbvf.sHtML


<!-- 参考信息 -->