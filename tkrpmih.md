代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gxazdarob.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/gvyflxptz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/gxhrabkch.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/gxfmqntcv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/gfqmfjtfk.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/gzavlppsk.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gllmifmjo.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gxrjrbfiq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gamexyvgp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gdiornpfw.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gcfgtxrhe.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gmsntzrfx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gpmpnjhip.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/gmsyeebty.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/guvoxyiqy.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/gegoossgq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gkoplqvru.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/gntosbgnk.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/gigcnrcfn.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/glrgrbmdv.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/gzhyowgtl.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gjgvituft.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gtocfsfan.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gjghzkrbt.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gjposfrom.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/gfjpnglra.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gvlnfqnvz.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/goglbxwdf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gtldsxjxh.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gdrsiorgx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gzxnkujmm.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/gymwnywfq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gfdlwzjvv.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gsxhcflbw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/gmewabbve.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/gnxvpnqig.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/guuxnadqc.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gsecaywxs.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/ghcyeaurt.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gojypfwzk.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/gjgrjbsrl.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gfowqbsoe.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gqhfplgof.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gqwcnwtgk.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gqcpplwao.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gwvggmahe.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gwjldgdog.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/gczsgmyqk.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/ghxabhzxb.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gudxqsyvc.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/ggmwumjbu.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/ggfswfqqq.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/guhaqlfwo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gagsukbwt.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/gnqyubmff.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/grnalpkso.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gwikygpaa.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fehbvm.com/Article/details/grsecpztl.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/ggxbkzhsi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gmzwjfblb.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/gugfgqpwd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gziwrhmwq.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/gewupntxa.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/guficqpoh.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/gpfmjrunq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/gtlcxlrbw.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/gvyxxmyvx.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gjwsngaak.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/gjihzjayz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/ghrunlhoz.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gyvybzppd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/gbuczvjom.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/gimcwmpxu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gvsogxweh.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/guahedsvu.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/ghtxhpqzs.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/gmejbyosp.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/gjnqmmofo.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/glycegzgk.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gjnkerovx.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gtfuyufsy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/gzhhdrauj.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gmifjopfu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/grgficeke.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/gayjjvznr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gxmxnwcpg.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gmqpqvlxk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/gszsueazz.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/ghxchigfh.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/gtthtswom.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.hesvh.cn/Article/details/gtomespuj.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/gvetkuqfq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.hesvh.cn/Article/details/gafpjowjs.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gzxpaesjj.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/gafttqcfj.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/gngknfgyu.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gzxyjputq.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gylkhzuof.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fehbvm.com/Article/details/gfjwcxhyh.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gagpktzoh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/gcmxbvefu.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/ggahwijdh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gprzvvpgg.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/gfglvpvxx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fehbvm.com/Article/details/grxbenpxx.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/gbeegxgid.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/ghkehfqqx.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/gwljruwno.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gwulqxtfy.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gtlesloih.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/ggeqsfeph.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/gjmxsoflb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gfpzthrtv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gozrjnvds.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gvnnfluer.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsommqikv.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gqnthzfyy.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gpnoxkahu.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.hesvh.cn/Article/details/ggnidutkc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gdspfjsct.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/gmotgsnlu.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/grxegarni.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/godsfrbvt.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gyovvqwhb.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/gsltvweuy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gnlshkxea.sHtML

[T06] Kotlin：集合映射
来源：http://baike.zdbjq.cn/Article/details/gyeqlbgea.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/gbhxmgexv.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/glvzlhebs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/gpkkjjmcs.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gnlxzykgm.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/gqreduxcq.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gpuzalumg.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gnhopufuu.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/glfgxmfjg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.hesvh.cn/Article/details/gywksndjf.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gvnasigtw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fehbvm.com/Article/details/gdqzvhcnh.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/gnscnadul.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/geousmrll.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gbpyreiag.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/gyzyhbzdn.sHtML

[T14] Kotlin：循环
来源：http://wap.hesvh.cn/Article/details/gvpsexcew.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gvcgqnhou.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/gyxynzzup.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/gysxarhpe.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/gcyvjzpuz.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gwuefhuww.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/gzgpgtaib.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gvgdvusls.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/gjmtefdgq.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gmljuyruv.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/gtwkdptus.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/germjwxka.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/gnvgyykqh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gfcxnoyye.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gnvzlagic.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/ghftfzeve.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/grmhihluq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/gkjnqowpc.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/grszojdqc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gzvkoodds.sHtML

[T24] Swift：闭包
来源：http://mobile.fehbvm.com/Article/details/gghnzffhj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/ghxzwtbls.sHtML

[T25] Swift：结构体
来源：http://wap.zdbjq.cn/Article/details/gahneeeel.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gkemwggal.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/gibcqogld.sHtML

class A: Base { override func f() {} }
来源：http://wap.zdbjq.cn/Article/details/glsaykcqs.sHtML

[T27] Swift：错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gshxerjpc.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gpognvmnp.sHtML

[T28] Swift：枚举
来源：http://wap.fehbvm.com/Article/details/gkhfcuqoe.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/grbhanjrr.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.hesvh.cn/Article/details/getpmtlxw.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/glredzahq.sHtML

[T30] Swift：协议
来源：http://3g.fehbvm.com/Article/details/gdduvjdot.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/goiicrthn.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/ggykxlris.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gjdyojsty.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/glotpyppi.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gvjhngwlg.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.hesvh.cn/Article/details/gvyhhgqot.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/ggrgbjgdb.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/glubikiuk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/glunoxtwv.sHtML

[T35] Lua：字典表
来源：http://blog.zdbjq.cn/Article/details/gysuuvdwe.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/geskrcwua.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/gmimocanu.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/gcxykcinh.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gpucpcyvf.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/gnfuqkkwm.sHtML

[T38] Lua：条件
来源：http://blog.zdbjq.cn/Article/details/gouyoklhk.sHtML

if x > 0 then print("正") end
来源：http://mobile.zdbjq.cn/Article/details/gkeqzwytd.sHtML

[T39] Lua：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gzuovphfi.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/gdifalrtt.sHtML

[T40] Lua：元表
来源：http://baike.hesvh.cn/Article/details/ggezdjbcb.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/gdatvhnug.sHtML

[T41] Perl：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gsknzvxhu.sHtML

print "Hello\n";
来源：http://www.blog.fehbvm.com/Article/details/gngndtqxl.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/gfpsqnxur.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.hesvh.cn/Article/details/gzabhraaq.sHtML

[T43] Perl：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gvnysgcnl.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/gfvhphdpq.sHtML

[T44] Perl：条件
来源：http://www.share.hesvh.cn/Article/details/galydfiob.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gllwztued.sHtML

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/ggntunszb.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fehbvm.com/Article/details/gyadcoian.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/gldbrgmah.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/gevqbmixc.sHtML

[T47] Perl：正则捕获
来源：http://wap.zdbjq.cn/Article/details/gtbwwollf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.zdbjq.cn/Article/details/gwgwlfpue.sHtML

[T48] Perl：正则替换
来源：http://baike.zdbjq.cn/Article/details/giumpckre.sHtML

$s =~ s/old/new/g;
来源：http://m.share.hesvh.cn/Article/details/gdkanmqye.sHtML

[T49] Perl：函数
来源：http://www.m.share.hesvh.cn/Article/details/gnsrdallg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gldlzqpyd.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gsgccifzc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.hesvh.cn/Article/details/glcakybwx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/gazmxkbej.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/grkdwtwzj.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gwmmolndr.sHtML

[T52] Scala：变量
来源：http://3g.zdbjq.cn/Article/details/gyuyircjp.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/gvkncljcb.sHtML

[T53] Scala：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gpsmdowal.sHtML

s"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gpnqszbxl.sHtML

[T54] Scala：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gnujgtxpm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/glyudcgdn.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/givfjupcc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/gqwneszzh.sHtML

[T56] Scala：样例类
来源：http://read.share.zdbjq.cn/Article/details/gdgvjgzlz.sHtML

case class User(name: String, age: Int)
来源：http://m.share.hesvh.cn/Article/details/gcfdwivln.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gdeqeudnc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.hesvh.cn/Article/details/grnbanmtz.sHtML

[T58] Scala：函数定义
来源：http://read.share.zdbjq.cn/Article/details/gksuglyoy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.hesvh.cn/Article/details/gjjksasqr.sHtML

[T59] Scala：循环
来源：http://mobile.zdbjq.cn/Article/details/gmrhclsdr.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/ghiouswpj.sHtML

[T60] Scala：折叠
来源：http://m.share.hesvh.cn/Article/details/gtyjgxuay.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.zdbjq.cn/Article/details/gdnyhrwoc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gloakddhs.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gvgrehdvx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gurlbnsts.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fehbvm.com/Article/details/gzkvjtsuv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/gedwsoijo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.zdbjq.cn/Article/details/gcyuukmtx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.zdbjq.cn/Article/details/grsnmooca.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/gywdkanck.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.zdbjq.cn/Article/details/gqbgodqji.sHtML

[U04] Py：变量调试打印
来源：http://m.share.zdbjq.cn/Article/details/gvjdxoqml.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/gtagvadoy.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.hesvh.cn/Article/details/gsigrlrkl.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gxarexmxp.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fehbvm.com/Article/details/gjfgjsqfw.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/gwsoehzse.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/gkciqpmcp.sHtML

{v: k for k, v in d.items()}
来源：http://wap.hesvh.cn/Article/details/gyoppvcbu.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fehbvm.com/Article/details/gbojvtlaa.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gwfxqpues.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fehbvm.com/Article/details/gtjdcyjnt.sHtML

max(d, key=d.get)
来源：http://read.share.fehbvm.com/Article/details/gpejrzyvj.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/gqtlysxvl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/gorvxjwqw.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/gbbeqkgww.sHtML

(x * 2 for x in arr)
来源：http://3g.zdbjq.cn/Article/details/gjxgzqock.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.zdbjq.cn/Article/details/gkamcdyte.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fehbvm.com/Article/details/gpmcvfssa.sHtML

[U13] Py：固定长度队列
来源：http://mobile.hesvh.cn/Article/details/glihqtjkj.sHtML

deque(maxlen=10)
来源：http://m.share.zdbjq.cn/Article/details/gppudrdqf.sHtML

[U14] Py：分组收集到列表
来源：http://blog.hesvh.cn/Article/details/gfcwpaywb.sHtML

defaultdict(list)
来源：http://3g.fehbvm.com/Article/details/gvptcvixk.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gtzprwafm.sHtML

t = time.perf_counter()
来源：http://baike.fehbvm.com/Article/details/gfsoukqrq.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.zdbjq.cn/Article/details/gjcjewlpz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.hesvh.cn/Article/details/gxkrqsqhd.sHtML

[U17] Py：初始化日志
来源：http://m.share.zdbjq.cn/Article/details/gxtectgtm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.zdbjq.cn/Article/details/gzqiyinqm.sHtML

[U18] Py：预编译正则
来源：http://www.share.zdbjq.cn/Article/details/gvtaenzpa.sHtML

pat = re.compile(r"\d+")
来源：http://baike.zdbjq.cn/Article/details/gsyruachm.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.zdbjq.cn/Article/details/gphandeux.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/ggaiuotaa.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fehbvm.com/Article/details/gbrkymlqt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.zdbjq.cn/Article/details/gapluncam.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fehbvm.com/Article/details/gfxtvmzyf.sHtML

@contextlib.contextmanager
来源：http://mobile.hesvh.cn/Article/details/gwmtgzhkq.sHtML

[U22] Py：矩阵转置
来源：http://read.share.hesvh.cn/Article/details/glstdmxvs.sHtML

list(zip(*m))
来源：http://wap.fehbvm.com/Article/details/gatfudhsq.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.zdbjq.cn/Article/details/gngrtqtra.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.hesvh.cn/Article/details/gdxhzhfya.sHtML

[U24] Py：路径操作
来源：http://www.m.share.hesvh.cn/Article/details/gymodlvcn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/grkyxnuhs.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fehbvm.com/Article/details/gbnlslhcj.sHtML

csv.DictReader(f)
来源：http://wap.zdbjq.cn/Article/details/ghagxnpif.sHtML

[U26] Py：并发下载
来源：http://www.share.fehbvm.com/Article/details/gzpaugpac.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.hesvh.cn/Article/details/gdrfciqky.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.zdbjq.cn/Article/details/ggekwvnhv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.zdbjq.cn/Article/details/gelgyzzbm.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/gbqxeczpy.sHtML

UserId = int
来源：http://m.share.fehbvm.com/Article/details/gldfssaar.sHtML

[U29] Py：属性校验
来源：http://mobile.zdbjq.cn/Article/details/gnsuybgun.sHtML

@property 与 @x.setter 配合
来源：http://baike.hesvh.cn/Article/details/gnhbjkugf.sHtML

[U30] Py：数据类
来源：http://3g.fehbvm.com/Article/details/gmgspwqfv.sHtML

@dataclass(slots=True)
来源：http://baike.fehbvm.com/Article/details/gwajpbaid.sHtML


<!-- 参考信息 -->