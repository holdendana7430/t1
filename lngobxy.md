代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gjncvpibq.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczhxxwfe.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gymkjbsmn.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnqibdil.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gwcfkkzid.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghzwqznk.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcslkneh.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gulxhrxms.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gdtyksfsw.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gkowdlkgv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdylcsja.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrgvupsc.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gonaihqvq.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gnghwfmse.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gctzwybyz.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gdokxpvcc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohymypvh.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuaxlgva.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gcybqjqnm.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjjhhitw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfkplnbz.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gmqqpfojx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfbpauxb.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/ghlaonzfg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gjxzpptpm.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxbgoqgf.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glonkabkp.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gjqsjjkxo.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgovcdde.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gynmuantx.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaghkkqog.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdlttggr.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxmmorxf.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlcslifn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/grzykzdbq.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/glcgispnc.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gsecdkdue.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gydixkgko.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwktlnjp.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqyqcsof.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gaxyxusla.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gitrhkpto.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gbxmjshgt.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvuxfmgwe.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbdqfnjs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goppsgxcc.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gqeyfwgfz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgawlhft.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnwomveb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfczjhlio.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumctzssy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyaresjxz.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gxrykwhfs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfohwupdz.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gpiplbqcl.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfpxhalm.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gbqjrjzlg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gpfutyvnw.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsortixn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gyqjnsnkh.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gmlmvwsks.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gfaqgzvyg.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gtlxsczsy.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmbaahej.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gzcltkcvx.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqrmmlgu.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/grsfirtia.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grslobdpx.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasdfscbt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gyodthyqt.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gilbsanam.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gegpbnbvb.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/ggpfthvqs.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwkoigezo.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gbcpplgei.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/guxygislq.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/glnmnkszf.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gajcvswsi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwndvqfb.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/ggmicgcpu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/guuhcewqd.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gfemkkyey.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqolarcv.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gcbrhhwdq.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbaxjhbt.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gnmmrlwez.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gkzristkc.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/grkkizdux.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/glsctvebc.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gglsvkmvu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghszpjkeq.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gibplpkcu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsngmwen.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/ghiocfgwr.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbfbrzrp.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gojshzugx.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/grelcikvh.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbxynajj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gglynzzqw.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gldkgqnbd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttkpvdiv.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyiojxljx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqbknsmt.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/guajqghan.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gmvuknlcc.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gtbixiacw.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gayeafesr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gsrvgxqwv.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlgxdoja.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqribokpl.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gndrmwrag.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gswoqjmox.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjsvkcqe.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genkfniou.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjmsxjrq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyvqtthx.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/ghrfuygnz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gejnjcxrt.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gorcuivod.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvciguegp.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/gvfpcmibn.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/gmthttegt.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gnevxstur.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwgqissq.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyuwvzndj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgzlrdfl.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gjavdvvgv.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gzlxqyast.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gvfclcfpo.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxxvrkmx.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/ggwjiswbh.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/galfavoak.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdpbfylb.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzysovhte.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gihqcexiv.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfptvtxqm.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gqiblwswv.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyhbpqne.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gijfeznfw.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtwhgeth.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqiyefgxn.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gityvqmhz.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gorflrkvk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwrtnapt.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzydktrd.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/grzjlpqdc.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnblrwpzo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gvqhqodtn.sHtML

[T23] Swift：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsutcznl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gfxtyynxl.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjfasriz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gxbhcwjtk.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwdizeze.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gznkrqnhw.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxipqkey.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnptfvru.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflurzlrg.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaajrizfj.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gtajifpir.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmycncmz.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyjoshyg.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gyhupwewh.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkjphioq.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabqaxbfh.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/glxuuypkb.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/grkpskqlw.sHtML

[T32] Lua：局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpcfkuoi.sHtML

local a = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gtaqsopat.sHtML

[T33] Lua：表（数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gukujyrhy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fanxiaobao.xyz/Article/details/gpbvarhxw.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmivqkack.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fanxiaobao.xyz/Article/details/ghdffkqqy.sHtML

[T35] Lua：字典表
来源：http://3g.fanxiaobao.xyz/Article/details/gzhemgdgm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gudzsmwxy.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/glexwvjqc.sHtML

function add(a, b) return a + b end
来源：http://m.share.fanxiaobao.xyz/Article/details/grnkooxkj.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/grnkarczd.sHtML

"a" .. "b"
来源：http://wap.fanxiaobao.xyz/Article/details/gpsuapujq.sHtML

[T38] Lua：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbwxjobw.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/gkmmklmyl.sHtML

[T39] Lua：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/ghtgcakjz.sHtML

string.find(s, "%d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gohtdexjz.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnjmjlzc.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsejoasd.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwkicxjk.sHtML

print "Hello\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gueuzyudu.sHtML

[T42] Perl：变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/geuxytwpf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/grdssbmsa.sHtML

[T43] Perl：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gmqspccnq.sHtML

"值: $a"
来源：http://m.share.fanxiaobao.xyz/Article/details/guktshltc.sHtML

[T44] Perl：条件
来源：http://3g.fanxiaobao.xyz/Article/details/girawqkbi.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcyooptzv.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gvrstynho.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgsdpjvm.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gewytrpum.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghshsagtn.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdajikzcu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjhpawgyj.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwahcsop.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqghiwni.sHtML

[T49] Perl：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvrvdpfy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glgxgowhh.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvquuous.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fanxiaobao.xyz/Article/details/gguzotbnh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgrxavfw.sHtML

[T51] Scala：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gaghhadbs.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gluqjiegc.sHtML

[T52] Scala：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvgvqbnk.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjbpbczb.sHtML

[T53] Scala：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gdguhudcm.sHtML

s"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcknhopnf.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjwxvlgz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gijathfho.sHtML

[T55] Scala：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gxllieazy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gordaxqlb.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/gbdmolhyx.sHtML

case class User(name: String, age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gjwcglwto.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/giucrltvy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhcrrqjr.sHtML

[T58] Scala：函数定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlbwpojt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrsvcthz.sHtML

[T59] Scala：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gpvceujqc.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/guciudgcu.sHtML

[T60] Scala：折叠
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxwaaglb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fanxiaobao.xyz/Article/details/ghahaojdq.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ghbxegjre.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gvxkanbpc.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/goepvdhay.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxfukvwc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fanxiaobao.xyz/Article/details/gftxaceaa.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbtiliyv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgngxkgp.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gaoquzvnn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrxkybey.sHtML

[U04] Py：变量调试打印
来源：http://wap.fanxiaobao.xyz/Article/details/gsltdskms.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/gpxtzzbze.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjdgjzcv.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofyvyzqs.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gkazootet.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtkrbepi.sHtML

[U07] Py：反转字典键值
来源：http://blog.fanxiaobao.xyz/Article/details/gnnovieka.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fanxiaobao.xyz/Article/details/ghzshcpue.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcccvhalw.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/gzopdxewh.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmfbxnmt.sHtML

max(d, key=d.get)
来源：http://blog.fanxiaobao.xyz/Article/details/ggtzrtmof.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/gxkbssgox.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfucjquj.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbnmiuyu.sHtML

(x * 2 for x in arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gonosjjwr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxlbsycm.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsdcuhxz.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqxzgxwk.sHtML

deque(maxlen=10)
来源：http://blog.fanxiaobao.xyz/Article/details/gqbiqikyy.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvbqpxuy.sHtML

defaultdict(list)
来源：http://blog.fanxiaobao.xyz/Article/details/guivbrcvf.sHtML

[U15] Py：高精度计时
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkvgaqge.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsfcgpje.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fanxiaobao.xyz/Article/details/gcjmfcsev.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/gafvlqynz.sHtML

[U17] Py：初始化日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gllmlhwfz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbluhiakt.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqxnkads.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gnrywvzme.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvzgpokw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpadlbayy.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fanxiaobao.xyz/Article/details/gyazwezps.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fanxiaobao.xyz/Article/details/gbghwvnll.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fanxiaobao.xyz/Article/details/gjohxzcvs.sHtML

@contextlib.contextmanager
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvnmsyru.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrimqrqc.sHtML

list(zip(*m))
来源：http://blog.fanxiaobao.xyz/Article/details/gdqwualgn.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohklkhat.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbapktkg.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/glnaqdhmk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidaayjdq.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkurypwc.sHtML

csv.DictReader(f)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvglhgwme.sHtML

[U26] Py：并发下载
来源：http://read.share.fanxiaobao.xyz/Article/details/gryqrgjzi.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fanxiaobao.xyz/Article/details/gpgbyxjru.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fanxiaobao.xyz/Article/details/gzplcykuv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fanxiaobao.xyz/Article/details/gfxotmjre.sHtML

[U28] Py：类型别名
来源：http://read.share.fanxiaobao.xyz/Article/details/geuyutiqb.sHtML

UserId = int
来源：http://blog.fanxiaobao.xyz/Article/details/goihrgfbh.sHtML

[U29] Py：属性校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gybapzqyv.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkfzblmc.sHtML

[U30] Py：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/glprmmsst.sHtML

@dataclass(slots=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwjbqpgh.sHtML

[U31] Py：单测
来源：http://www.share.fanxiaobao.xyz/Article/details/gylnxckjg.sHtML

python -m pytest -q
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvmcqfvp.sHtML

[U32] Py：代码格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gyzgpbjjz.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggknseqzt.sHtML

[U33] Py：打包发布
来源：http://wap.fanxiaobao.xyz/Article/details/grzkprwsk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjboryux.sHtML

[U34] Py：判断编码
来源：http://baike.fanxiaobao.xyz/Article/details/gagifwsja.sHtML

chardet.detect(raw)
来源：http://blog.fanxiaobao.xyz/Article/details/gqotxzkne.sHtML

[U35] Py：发送邮件
来源：http://blog.fanxiaobao.xyz/Article/details/gnvzmkanj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fanxiaobao.xyz/Article/details/glzrsonjf.sHtML

[U36] Py：定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqcgttrr.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrndvxke.sHtML


<!-- 参考信息 -->