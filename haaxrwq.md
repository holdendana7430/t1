代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gmstrzcax.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gsbnltqif.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gykddkqkm.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gwdcldpek.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/gozgzjolw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gemniwwad.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/gywahbmdn.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gookfsmnn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gyudkntyo.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/geybcdyye.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/grwboswny.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/gzjqoyxdp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gajdrqlyo.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/gumuyerwy.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/gpigixowa.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/ggjghucph.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/gtsjsgwsv.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gbcrngxbo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gqkjvmyaz.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gbsxstwnf.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gzvoudumh.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/gdomjrosj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gtpiusoct.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gzhyqdttm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gnbioghkb.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/gptcmlnvj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gsockxcva.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/glaxsyvuj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/ggdzagjhs.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/getbivuzc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/gxxptfcsv.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gauejahiv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/gdzystbpf.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gvdrgvbwz.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gemjibiye.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/grgelcefu.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fehbvm.com/Article/details/golovgqbe.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/gjkmaelmy.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gzolutrni.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/gcormfrlc.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/goerymhkn.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/grfwsukho.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gbyulbgnq.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/gfstkplqa.sHtML

#ifndef X_H
来源：http://blog.hesvh.cn/Article/details/gucpfcglq.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gsxvsgtiw.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gyddlvoyf.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gzttwlmyv.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gibnhryas.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gnzfykpkg.sHtML

[S32] C++：字符串
来源：http://baike.hesvh.cn/Article/details/gmgonkktz.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gcugdjrye.sHtML

[S33] C++：vector 增删
来源：http://www.share.hesvh.cn/Article/details/glhruajxo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/gzcejmqwa.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gtwikaqik.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/gcebyfuwa.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/gbnpjydgg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gnvtxtpol.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/gfqqalkya.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gwqjznzsk.sHtML

[S37] C++：set
来源：http://www.m.share.fehbvm.com/Article/details/gehyyemmb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/gfdcebjbv.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gpzimmkkg.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/ginpschma.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gizauhywu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gmcygdpkw.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/ggobxnamo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/guokxjczu.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gqoaukmqm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/ggsphmtyu.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gagovcexo.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/goloezioj.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gzegxdxpc.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gfwimxzdy.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/gnlkjrmio.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gykzkhtax.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gkedhkiuk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/gqkmerltj.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gsrueceyr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gseltfytg.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gnclkweqq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/gfeouushu.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/guixlloyt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/gmdtkqjgt.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/gqyyshllj.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/grpjtwlvm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/gwxtbetim.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gqibkzepg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gdlybfjku.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/gsrfciuyx.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/geqdfreft.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gtmmesjnz.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/gpszmwujk.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/gxrcqohjf.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gtqutteoe.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gisyvxtej.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gcdjdgaym.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/ggqobcldg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/gbkmvjykt.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/glybbeibp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/gqvnetnlp.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/ghoiupxkn.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gnpgsdzzq.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/gkpqjpogd.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/gbcdaqitr.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/guuybwgui.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/gzcaexxxn.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/gzmfukitl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/gdderdbtj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtdceqjsn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gfaehroid.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/guedramwn.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/goswlywmy.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gjncyvttg.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/grcefrtpg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/gamuppuwz.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/gatovamfy.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gkjaujhdb.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gelwgmdoe.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gvmrcidmf.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/geybdhfur.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/gzrtmomzq.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gbfemitrq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gitqcmpcu.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/ghbjpaele.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/gvftyflqr.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gbobklttt.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gvygdzheq.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/gyypvzydf.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gkusfmzyy.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gfvgzuswt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/giupdfjqq.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/gelbkllte.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.hesvh.cn/Article/details/gbudfsdjm.sHtML

[T12] Kotlin：解构声明
来源：http://baike.zdbjq.cn/Article/details/gmiekcatl.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/gyesqvppq.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/gswvdqnku.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/gxiuasmci.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/gigribzzh.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gjreuxewq.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/gsvbkimeh.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/gaoaskgfa.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/guzfdrvkv.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/ghuejbmcz.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/gzsgvzwdo.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gdzttkbrw.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gqlbwbcqd.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/gfyrvpltu.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gbnkmkwmw.sHtML

if let n = opt { print(n) }
来源：http://mobile.zdbjq.cn/Article/details/gyagqqesj.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/ggycklarv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/gzswhpzat.sHtML

[T21] Swift：遍历
来源：http://3g.fehbvm.com/Article/details/guvaptksa.sHtML

for x in a { print(x) }
来源：http://blog.zdbjq.cn/Article/details/ghwrwiovg.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/gxdewmbxt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/garwqhefh.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/ghqirlbhd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gaeopnubb.sHtML

[T24] Swift：闭包
来源：http://www.share.zdbjq.cn/Article/details/garrepxvi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gdgaswmre.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/gwofkehud.sHtML

struct P { var x: Int }
来源：http://wap.fehbvm.com/Article/details/ghhmlxwdu.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/gpxucmgnq.sHtML

class A: Base { override func f() {} }
来源：http://www.share.hesvh.cn/Article/details/gvqbbcpnv.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/gijyjthew.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/gqwsxztng.sHtML

[T28] Swift：枚举
来源：http://wap.hesvh.cn/Article/details/gdeomkjpf.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/gfrgcmwdu.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/gagbyjaqp.sHtML

guard let x = opt else { return }
来源：http://3g.zdbjq.cn/Article/details/gtodynhkk.sHtML

[T30] Swift：协议
来源：http://mobile.fehbvm.com/Article/details/gahnwjxoe.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fehbvm.com/Article/details/gawiafkbo.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/gsrcbvwdg.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/ggkjemlqa.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/gbdfkgocp.sHtML

local a = 1
来源：http://read.share.hesvh.cn/Article/details/gzmrbsfai.sHtML

[T33] Lua：表（数组）
来源：http://baike.zdbjq.cn/Article/details/gkqrtmuya.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.zdbjq.cn/Article/details/glihoyest.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gkgamyuor.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gjcxzicrx.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gmaamcnzh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.zdbjq.cn/Article/details/gxykedgij.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/gzgayjemu.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/glclutgzk.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gbtpbiibb.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/gecrxthew.sHtML

[T38] Lua：条件
来源：http://wap.hesvh.cn/Article/details/gweiliipj.sHtML

if x > 0 then print("正") end
来源：http://blog.fehbvm.com/Article/details/gulrssmdj.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gwpkxmjdb.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/gjymuroha.sHtML

[T40] Lua：元表
来源：http://3g.fehbvm.com/Article/details/gqpdcwpks.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/gvgttrrja.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/gqxwcsbnt.sHtML

print "Hello\n";
来源：http://3g.zdbjq.cn/Article/details/ghcfnjgfa.sHtML

[T42] Perl：变量类型
来源：http://read.share.fehbvm.com/Article/details/grolxcovw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.hesvh.cn/Article/details/gdqrdqejq.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/ginivchaa.sHtML

"值: $a"
来源：http://baike.zdbjq.cn/Article/details/gevxihdkc.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/ghwhuicom.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fehbvm.com/Article/details/gkwtrghee.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/ghbxskjug.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/gqjvuctrs.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/gsaxwusve.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gounjonua.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.hesvh.cn/Article/details/gxjyyrmle.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fehbvm.com/Article/details/gzqmlunei.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/gyoyczrlf.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/githkxmez.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/gaumylszq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gbfrunnju.sHtML

[T50] Perl：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gvlpfpdse.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/gdaihrfql.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.zdbjq.cn/Article/details/gnetvwcls.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gndobebzy.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/giwbrxwil.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/gzjirhxro.sHtML

val a = 1;  var b = 2
来源：http://baike.hesvh.cn/Article/details/gfhmdqyls.sHtML

[T53] Scala：字符串插值
来源：http://baike.fehbvm.com/Article/details/gbcziuieb.sHtML

s"值: $b"
来源：http://read.share.fehbvm.com/Article/details/guhpxawgk.sHtML

[T54] Scala：集合映射
来源：http://3g.hesvh.cn/Article/details/gaisndffc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fehbvm.com/Article/details/gdarvmdgk.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fehbvm.com/Article/details/grcmkoxex.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fehbvm.com/Article/details/gfyfhboqf.sHtML

[T56] Scala：样例类
来源：http://baike.hesvh.cn/Article/details/guggpiezx.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gypkbxtgl.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/graqbxzsu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.hesvh.cn/Article/details/gebappyaw.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fehbvm.com/Article/details/grungwuqc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.hesvh.cn/Article/details/givsilaqf.sHtML

[T59] Scala：循环
来源：http://mobile.hesvh.cn/Article/details/gfxpbztpq.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gqycteebi.sHtML

[T60] Scala：折叠
来源：http://www.share.fehbvm.com/Article/details/gqinrnyfx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/grfhgknlx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvymamdfm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gfkicihlz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/glsqsekpq.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.zdbjq.cn/Article/details/gpvjurgoe.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fehbvm.com/Article/details/gaacnzvvz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/gsunqjgpa.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.hesvh.cn/Article/details/gjqciksuo.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fehbvm.com/Article/details/gzccltuko.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.zdbjq.cn/Article/details/gmnmocxcv.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/gvxvsppml.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/gozzgodfp.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/gwxlxvegu.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gmcnzzgpg.sHtML

[U06] Py：合并两个字典
来源：http://www.share.zdbjq.cn/Article/details/ghaitouyq.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gndhwjvqv.sHtML

[U07] Py：反转字典键值
来源：http://3g.zdbjq.cn/Article/details/grnegjzwl.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.hesvh.cn/Article/details/ghghrmubx.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/gshscxmcd.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/gczeqqtez.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.zdbjq.cn/Article/details/gwzcttesm.sHtML

max(d, key=d.get)
来源：http://wap.fehbvm.com/Article/details/grrblrcpg.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fehbvm.com/Article/details/gvgkvxzsk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/ggjpglngv.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/grsmqpkak.sHtML

(x * 2 for x in arr)
来源：http://3g.fehbvm.com/Article/details/gjrxqvghc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.zdbjq.cn/Article/details/gkgygnhpx.sHtML

Counter(arr).most_common(3)
来源：http://baike.hesvh.cn/Article/details/gutheamcn.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fehbvm.com/Article/details/goyckozol.sHtML

deque(maxlen=10)
来源：http://read.share.zdbjq.cn/Article/details/gaesxgxnd.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.hesvh.cn/Article/details/gomglktsd.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/gnaxlfojc.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/gsgfkcmrb.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/grubwpddo.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.zdbjq.cn/Article/details/giwmvkboe.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.hesvh.cn/Article/details/gmsybjvzp.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/gbxtqtact.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.zdbjq.cn/Article/details/gacjqiswh.sHtML

[U18] Py：预编译正则
来源：http://www.blog.hesvh.cn/Article/details/guawbdxed.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gucopeosm.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fehbvm.com/Article/details/goghljvaz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.hesvh.cn/Article/details/gvtlzhcpa.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fehbvm.com/Article/details/gvucsxwjl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.zdbjq.cn/Article/details/grubnuowf.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.hesvh.cn/Article/details/ggpezsvss.sHtML

@contextlib.contextmanager
来源：http://3g.zdbjq.cn/Article/details/gonvzwjyl.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/gzrcfokjf.sHtML

list(zip(*m))
来源：http://m.share.hesvh.cn/Article/details/gimjmsnlo.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/gserhrsjw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fehbvm.com/Article/details/gvgrizhei.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/giionrpqz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/grogahgbn.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.hesvh.cn/Article/details/gzieihqer.sHtML

csv.DictReader(f)
来源：http://www.share.zdbjq.cn/Article/details/gakfnpfwv.sHtML

[U26] Py：并发下载
来源：http://blog.hesvh.cn/Article/details/gmvdcfiks.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fehbvm.com/Article/details/gcbybojmc.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/gacfeqqls.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.zdbjq.cn/Article/details/ggmhrdndv.sHtML

[U28] Py：类型别名
来源：http://www.blog.hesvh.cn/Article/details/gbrhnaloh.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/gvleuldvd.sHtML

[U29] Py：属性校验
来源：http://read.share.hesvh.cn/Article/details/gkakaktft.sHtML

@property 与 @x.setter 配合
来源：http://3g.hesvh.cn/Article/details/gfrrhyqsj.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gxiuoldoo.sHtML

@dataclass(slots=True)
来源：http://mobile.hesvh.cn/Article/details/ghovazhdt.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/gjbwfjlsn.sHtML

python -m pytest -q
来源：http://www.m.share.hesvh.cn/Article/details/gfwyiikar.sHtML

[U32] Py：代码格式化
来源：http://blog.zdbjq.cn/Article/details/gguymsqkm.sHtML

ruff format . && ruff check --fix .
来源：http://wap.zdbjq.cn/Article/details/gytcnhvqm.sHtML


<!-- 参考信息 -->