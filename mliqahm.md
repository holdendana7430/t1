代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gtukcptpt.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gefickyrd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gxotqyvac.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcigyxfj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/ggmxprhto.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gydxsowbt.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/gsezbdfsk.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gqyetxzab.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gejfsglxl.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gbldlogiv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjjkenib.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gsybouxbx.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwaywpop.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gcoxzhscx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzpwmpan.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gujlgwsjm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gdaidlisa.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcnbfbpp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrnesljm.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gvwbqezpm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gdwfnqizt.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gpqmfkppk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbauvbdx.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/glekncdrf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwyycmco.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gsolmluiz.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzscbkoys.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gcaqqmxll.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gjugkqivj.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gsixbcahh.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfwyrjeo.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvjmqmhf.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gleaygwae.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxzogqiu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gejpqxkyl.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gqldltjoc.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gcgpuvxok.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gbepbcyoj.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gamhrewqc.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmnoyaej.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gseajqklo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gathgvrzr.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gnwxyerzq.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfvqpzuy.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfuqvhwy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gybmbschk.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gocertbyz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvjrmpeva.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gyasalovw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsmryilc.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gmghxtily.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslisjkbm.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzftiqir.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/guqzdtcir.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpmajlej.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gnvxbpdju.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gktfamznl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gzwyqujri.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/ggnmndjbt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gdcazpxxy.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbamsfvx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/guuqqmjnj.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbavsmnf.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczfvzklq.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/giytavwjt.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/giyteyngl.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcedqxsor.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gujjxfizu.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gktyrfmyp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/guheegdph.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/guquftkwn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggirbqzik.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gvooogevw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzobwpbcq.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/grygarzah.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gowwopbqr.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzssqvsnz.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxivswriy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gvynlpozd.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gioufvrzj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/geezrdyiz.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gbrcgoerm.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdtdwwrv.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnicnxwj.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gunnjntee.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gpztyjwez.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqpkxhrc.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpjgfwei.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gipbecwkc.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjpjefpg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gejqlbrwl.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gkwhhlnpv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkqjdthm.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmpydgrj.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxarysgl.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gkupieihs.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gzlmnkofd.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuhotamv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gfdaakoza.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrlqyyfo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfnknlaa.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gytlfghfe.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnyyocaq.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gywqcqtav.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljhhbzga.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcqbpkeb.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxinniazv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbhazasp.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejsyjtvv.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwobedao.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gyuwfqqmq.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/ghctddlrq.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gloeecdzr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/gddjgmvwp.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gtacmhckv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/ghhclhzdq.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gjejznjvo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gklceooav.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/grlujivyn.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geoxcmoxj.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrxljfym.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/ggoesyemw.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gemqefgrh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/gxyzqhvbi.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/goymbggxi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/grtkwkpaa.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpofqzrdy.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusggbhzb.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbctwlwg.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gscgzxlve.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gzggmcyad.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmmjmawa.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gxyxokgal.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdqwtcbj.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gemmvilvx.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gsciwyzfd.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/gbapefemo.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gjbzpkopq.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gezvfoblo.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/gmkfnomgk.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gjtifcktr.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gvsqjknzx.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gaoobnnjz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fanxiaobao.xyz/Article/details/gsweyonvp.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitdpgnql.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/godhlqomb.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemqhkkqh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefbyojjf.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/ghdgfjzby.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmelziffc.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/glyqistby.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gurbtjhhg.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwyqkivoa.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gneamivgj.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/guywpuvje.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvurcaixi.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/geidnmdhy.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/gsjodecok.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdzewkoh.sHtML

enum Color { case red, green }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqufbwgl.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqguymcvd.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfkyxdga.sHtML

[T30] Swift：协议
来源：http://baike.fanxiaobao.xyz/Article/details/gvzbvqvou.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gxrfncxiv.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gqxeyygww.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gyrqoemqw.sHtML

[T32] Lua：局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gokxpdjuo.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnkwebxi.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/gepareija.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/gizebxtcc.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/ghthujwdf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gboiaiurn.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabmiyccd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gdbjuwtkg.sHtML

[T36] Lua：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghgxtblg.sHtML

function add(a, b) return a + b end
来源：http://m.share.fanxiaobao.xyz/Article/details/gofeeagbh.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gmoymzjpb.sHtML

"a" .. "b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsszegulp.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gravzyhvm.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/gugomyias.sHtML

[T39] Lua：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gahcnugkm.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvndaqed.sHtML

[T40] Lua：元表
来源：http://read.share.fanxiaobao.xyz/Article/details/gkutmqysr.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/gkpufrjbw.sHtML

[T41] Perl：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gfwrnrmtc.sHtML

print "Hello\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gjmpnagcx.sHtML

[T42] Perl：变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcdwrkkp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gqaoobepw.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gekkkxuoc.sHtML

"值: $a"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxdjaqub.sHtML

[T44] Perl：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gkiwskews.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvyglmos.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggryqlzeu.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gatkpaxer.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgyhnzmg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbwznblgb.sHtML

[T47] Perl：正则捕获
来源：http://3g.fanxiaobao.xyz/Article/details/gtvytmleh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdxwvoii.sHtML

[T48] Perl：正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/grrauafou.sHtML

$s =~ s/old/new/g;
来源：http://wap.fanxiaobao.xyz/Article/details/goyhxpnnc.sHtML

[T49] Perl：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkheyavn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grfyflgcb.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gdvxcnadt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fanxiaobao.xyz/Article/details/gqjwuspqz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/gojteqyre.sHtML

[T51] Scala：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gzukfxftz.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gawpddomn.sHtML

[T52] Scala：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gcyhudekq.sHtML

val a = 1;  var b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gxcauoocm.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfiaeegsj.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdssqpsmd.sHtML

[T54] Scala：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gfwjnkxwo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gcymtkvvx.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxftcwkb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gblsimezo.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/gqpvavwym.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gwpvxrepp.sHtML

[T57] Scala：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/ggbsjmujf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcftgdzc.sHtML

[T58] Scala：函数定义
来源：http://3g.fanxiaobao.xyz/Article/details/ghpgzbxpq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gyolbjqyx.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/glpgxqgho.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxhfpgjb.sHtML

[T60] Scala：折叠
来源：http://read.share.fanxiaobao.xyz/Article/details/gszzgtqle.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fanxiaobao.xyz/Article/details/gerkflhgn.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gpsvpyqzg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcgdbfkc.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gbniswhov.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/goyxcjddm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fanxiaobao.xyz/Article/details/gvscvjqsd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fanxiaobao.xyz/Article/details/gxujmwzpv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gapwnrauw.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fanxiaobao.xyz/Article/details/grsalkrht.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkkjoodh.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhzxfqlw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fanxiaobao.xyz/Article/details/gqaajprku.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/glpylsdya.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gupcrkbxa.sHtML

[U06] Py：合并两个字典
来源：http://blog.fanxiaobao.xyz/Article/details/gtrbhmwub.sHtML

{**a, **b}
来源：http://baike.fanxiaobao.xyz/Article/details/gnbfinxhm.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfoxsesxf.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwrhkigv.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fanxiaobao.xyz/Article/details/glvzwwnnz.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlkuzoes.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/gnhlznbup.sHtML

max(d, key=d.get)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmnpbiwe.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gdintbpwg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fanxiaobao.xyz/Article/details/gioukmzbx.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlgzyvim.sHtML

(x * 2 for x in arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuixktls.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fanxiaobao.xyz/Article/details/greznylxe.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxuogqyh.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjaukuuz.sHtML

deque(maxlen=10)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnacdnmco.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gqezlnoyg.sHtML

defaultdict(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpajnlycf.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/gmkkokmkk.sHtML

t = time.perf_counter()
来源：http://blog.fanxiaobao.xyz/Article/details/gqtfhilsg.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdbhxgat.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fanxiaobao.xyz/Article/details/gimdshcgo.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaobftuqp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowzpgrpe.sHtML

[U18] Py：预编译正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmhnzsal.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtlpqkhs.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fanxiaobao.xyz/Article/details/gdsshlhrr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gimfdutvv.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrhqqwyh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxusvlyfw.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fanxiaobao.xyz/Article/details/gvqvpwtbp.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gweszawld.sHtML

[U22] Py：矩阵转置
来源：http://wap.fanxiaobao.xyz/Article/details/glsxmdyhd.sHtML

list(zip(*m))
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzuldzjl.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/gnsiviabi.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fanxiaobao.xyz/Article/details/ghkrmvvhx.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gsgeqitfm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gycqpvxdc.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcblnavw.sHtML

csv.DictReader(f)
来源：http://baike.fanxiaobao.xyz/Article/details/getbmydrl.sHtML

[U26] Py：并发下载
来源：http://mobile.fanxiaobao.xyz/Article/details/gftzotslr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fanxiaobao.xyz/Article/details/gmgjicnrm.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfnrulqw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscizchpz.sHtML

[U28] Py：类型别名
来源：http://m.share.fanxiaobao.xyz/Article/details/glskjqcrj.sHtML

UserId = int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwrwehan.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grghmqrpy.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fanxiaobao.xyz/Article/details/gblbetvcx.sHtML

[U30] Py：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gxvkohmdl.sHtML

@dataclass(slots=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gyeftxbhy.sHtML

[U31] Py：单测
来源：http://blog.fanxiaobao.xyz/Article/details/gvzdccrfc.sHtML

python -m pytest -q
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxcuqmky.sHtML

[U32] Py：代码格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzhalvkh.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndxbedaj.sHtML

[U33] Py：打包发布
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqeohmws.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsuslrdd.sHtML

[U34] Py：判断编码
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzglxyus.sHtML

chardet.detect(raw)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnrzwghp.sHtML

[U35] Py：发送邮件
来源：http://wap.fanxiaobao.xyz/Article/details/gmhwrrjeu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fanxiaobao.xyz/Article/details/gpdtyjuxe.sHtML

[U36] Py：定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgkybisy.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fanxiaobao.xyz/Article/details/gkmtgrepz.sHtML


<!-- 参考信息 -->