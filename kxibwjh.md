代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gwpghutal.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhetdiqe.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gnggiocbi.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gmapoxnlk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/grsxneboy.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/giidmkstj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/grjjaivlo.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gbiabpjmu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/grxdgeyrp.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gzcsjfyfv.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwqrrgis.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gxhisjfpt.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gstcxlrub.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gssbycamg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicwotjrl.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/ghstbmcsl.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspyzmlmd.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjhdsiws.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpfoavds.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkxlpacy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gcizvxzyk.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gjhvsmhck.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gbpbjsdcj.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdycgmjo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gyclqhvky.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gtghzxnja.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gaermmjyg.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gtbcifood.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/glylmrnyq.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/guogfgjic.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gppwqbmkc.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gyxcvkscc.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphmepcxk.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwmpmbka.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/ginwnzatr.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gzuzntggd.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gakjqvjav.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gypewtbnt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/guofvhowo.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/giogwdbxw.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gopfbfuvu.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsvhhimk.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gljzhqolk.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gkagmxxno.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxftglvc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gktkujihf.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxiwloyq.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/glklklulw.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gbxcnvjkt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzxunqac.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/ggtbqfewz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcnnmfhfh.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/ghrsxikux.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/guybtwjeu.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsajlkek.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gaucauqzu.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/ghxndxzna.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdcglqkv.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gdlbwjlwl.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gaikfsbvh.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gwcyfjkao.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpuiomqx.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqkedjte.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gueqcfcva.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gvwmublwb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gdxjkchtp.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqjbemgx.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggkwqats.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/ggaewwwoc.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gjhhwnnfm.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmafswgw.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvomgajyj.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/gduklknct.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gzclyjdxx.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmzpdpkd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfoudixuy.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gynazewka.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxfoqcpth.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/guvekghrc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/guasrqzpr.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsknmezdf.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcmmubha.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gdusgbzql.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbkphges.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrreaggg.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/goucxdntb.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/givimjxqr.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxiectgeg.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdldtmvnb.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/goujantpp.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsujoycyy.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gmejlsjuo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmchojro.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gsiofghpr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghczmtnnd.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshqecaan.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gofmlkdsl.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/gvpxieeqv.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gpnwybcxe.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gezcuiedi.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnubmbbgo.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gqioulufb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzwohiih.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/glpiwibzb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gqpubthcf.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gybdrcxrb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gzflupfep.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjzjpqrn.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gugouuvin.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/ggakchpie.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzrppsco.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gqobjspxq.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gkjrmodxu.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gbhixoith.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gktngdowq.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gohhwjgov.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqpspjmj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvzwefak.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkutmdzm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqrzanun.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gzciozqyl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gvewdmtoq.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grglqvtuz.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gvdhnfnls.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gxthsppnp.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gypsrerak.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnucxihz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/gbfguwibp.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwniouye.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/gqogbwidq.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdxmaloj.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gckwvntku.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmsoteqg.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gereomhrh.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gmvifzpcb.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gzhutisrm.sHtML

[T15] Kotlin：接口
来源：http://3g.fanxiaobao.xyz/Article/details/gtewizqrk.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/guxwsjnkp.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gotnpuglq.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchbgjxef.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/godiakluw.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gkoxndfmf.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gensklkms.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/gebfvcnry.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gblvmpesr.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzkqfmdi.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gyidjcusz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyeklgpqd.sHtML

[T21] Swift：遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gdbzxtpjj.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gatdngsaf.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/geoytyygu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/grvkgitvf.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gcnhipwsn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/guimtogte.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gaxbspgsl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gaeeuvzbr.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/gyhlqbocp.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnscnjaxs.sHtML

[T26] Swift：类与重写
来源：http://wap.fanxiaobao.xyz/Article/details/gpcluurxu.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwbgyiuy.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gncvocxdm.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/goixvfopd.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gpngrmvke.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfblqhmgh.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gorhkmqgb.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyexuywmh.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjtmbwvw.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gskcfwpyp.sHtML

[T31] Lua：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gwqmzysnp.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkuwncbnj.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gbvyblydb.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfzdiwsp.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gipbqudbv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcwsyino.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzomqljda.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/gwokxwvrr.sHtML

[T35] Lua：字典表
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpaplcxr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gvhcrluyl.sHtML

[T36] Lua：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxumeliv.sHtML

function add(a, b) return a + b end
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlwzuzzp.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gpmsjfvhd.sHtML

"a" .. "b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdrpwknf.sHtML

[T38] Lua：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gzqkipqlo.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzvwjqjf.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gfzooberu.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gxqxpjfby.sHtML

[T40] Lua：元表
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfluxjqk.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/gjupkyiqv.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitvznmka.sHtML

print "Hello\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnbtvhtl.sHtML

[T42] Perl：变量类型
来源：http://wap.fanxiaobao.xyz/Article/details/ggfxpvwlr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/guvptehid.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gclybsskf.sHtML

"值: $a"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjuqtklv.sHtML

[T44] Perl：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gktrmtzir.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqruycnqr.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gszigphcp.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gleygvaht.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxzksaum.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grporozhy.sHtML

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/gmqovyinz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gldksetox.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/goexhtful.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvxfaefx.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gpifnoill.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/glqnzbrry.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gddeyapgf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsihuqhe.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glhjouxrs.sHtML

[T51] Scala：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzuqkuwi.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/ganwvziay.sHtML

[T52] Scala：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyvzuxsq.sHtML

val a = 1;  var b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpoyeohq.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzrqalvd.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/ggigmhgti.sHtML

[T54] Scala：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvqwdyyh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxifijmlr.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylpulqta.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geovsqzoh.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/gblfkmpmb.sHtML

case class User(name: String, age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gbgkwywrm.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gdohrtcfw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunsokwvd.sHtML

[T58] Scala：函数定义
来源：http://wap.fanxiaobao.xyz/Article/details/gcjoutdsz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjdiclkm.sHtML

[T59] Scala：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyqbwdfe.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/goecfqedl.sHtML

[T60] Scala：折叠
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaifruxxn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fanxiaobao.xyz/Article/details/gufteitmx.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gzgnhwcya.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtxiquul.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gciuxnkhs.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fanxiaobao.xyz/Article/details/gxntfiena.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghyuuvwyu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fanxiaobao.xyz/Article/details/gexhwhbjk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndqqwimj.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gfftpafij.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjofpixkw.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkqiaosd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fanxiaobao.xyz/Article/details/grwhxlwwu.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlizrnfn.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/glwjaipzs.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggiregfwn.sHtML

{**a, **b}
来源：http://wap.fanxiaobao.xyz/Article/details/gmamjwrgx.sHtML

[U07] Py：反转字典键值
来源：http://3g.fanxiaobao.xyz/Article/details/gxsltuazq.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fanxiaobao.xyz/Article/details/grpfoyskn.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwfsivnd.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbktnmjyc.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fanxiaobao.xyz/Article/details/gvjmtbhjh.sHtML

max(d, key=d.get)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhobekoi.sHtML

[U10] Py：按值排序字典
来源：http://blog.fanxiaobao.xyz/Article/details/gkohdsjjp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghitdbesd.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gzpnblvfi.sHtML

(x * 2 for x in arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gocetlyoh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fanxiaobao.xyz/Article/details/gyikdlahq.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gidbbwegj.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fanxiaobao.xyz/Article/details/guruwaksx.sHtML

deque(maxlen=10)
来源：http://wap.fanxiaobao.xyz/Article/details/gdxaifqdk.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fanxiaobao.xyz/Article/details/gwpvrnala.sHtML

defaultdict(list)
来源：http://blog.fanxiaobao.xyz/Article/details/gcxpbvnec.sHtML

[U15] Py：高精度计时
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkhqxehd.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxlwwueg.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fanxiaobao.xyz/Article/details/gjuyfqcqg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/gudspjypf.sHtML

[U17] Py：初始化日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzmwyhvn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fanxiaobao.xyz/Article/details/glicflddl.sHtML

[U18] Py：预编译正则
来源：http://baike.fanxiaobao.xyz/Article/details/gfctemnsn.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gmemiacjl.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fanxiaobao.xyz/Article/details/grckmjgjb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbktctde.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fanxiaobao.xyz/Article/details/gyiflqgfq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvktbwbi.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fanxiaobao.xyz/Article/details/gybgibluf.sHtML

@contextlib.contextmanager
来源：http://blog.fanxiaobao.xyz/Article/details/gajynrgwn.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuucpqft.sHtML

list(zip(*m))
来源：http://www.share.fanxiaobao.xyz/Article/details/grqwvmdcd.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgimmsau.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzwyzlva.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gbpeldzfm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gbpmeeuei.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonjxppqp.sHtML

csv.DictReader(f)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgehvxal.sHtML

[U26] Py：并发下载
来源：http://read.share.fanxiaobao.xyz/Article/details/gatdijaak.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fanxiaobao.xyz/Article/details/gisfjwsaq.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fanxiaobao.xyz/Article/details/gzyebphis.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzkfhmds.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/gearyeqps.sHtML

UserId = int
来源：http://blog.fanxiaobao.xyz/Article/details/grvtfqxwd.sHtML

[U29] Py：属性校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrfjzbdt.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/gzabfxdnz.sHtML

[U30] Py：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjgkirvp.sHtML

@dataclass(slots=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gmnwilsag.sHtML

[U31] Py：单测
来源：http://baike.fanxiaobao.xyz/Article/details/gamrccatg.sHtML

python -m pytest -q
来源：http://3g.fanxiaobao.xyz/Article/details/gosxjdrhq.sHtML

[U32] Py：代码格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvxjuejp.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fanxiaobao.xyz/Article/details/gwnqgmzdz.sHtML

[U33] Py：打包发布
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqxhtcoy.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwbzqpns.sHtML

[U34] Py：判断编码
来源：http://3g.fanxiaobao.xyz/Article/details/guddnntdl.sHtML

chardet.detect(raw)
来源：http://mobile.fanxiaobao.xyz/Article/details/giqxvaqte.sHtML


<!-- 参考信息 -->