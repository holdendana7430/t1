代发 wailian999

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2ehnafofg.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2cjpxmjbh.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2imbordnk.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2ksjgodaw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ecpcclmj.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2sivdsejq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2eqtvmkcc.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ssrthxdl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2rjbudyir.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2ioploeyw.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2qmuefgby.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2yuyhxvte.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2mxdupjxx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vcflyixg.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2jlluqyhq.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2uxktyusn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2aneamjdd.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2sjkxlxbn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2yijqphau.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2akjsrmsm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2rfhrflrk.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2bmuofckn.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2tycdqxvp.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2yopkwbdl.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2rwqfmwjy.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2qwobfcbf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2qxklgsla.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2foixrxla.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ioehbzwc.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2jjttrxub.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2yphoeoii.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2ovmdhuht.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2smwmyfzp.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2bwykktpj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ngkregex.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2yjjrzqrz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2aahjuezs.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2bdsxteqk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2pmidzqvi.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2edqochpz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2wopawarc.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2fucsfebv.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2eazctgdo.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2bttcncas.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2lijjemkt.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2isnbizdk.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2idshugwo.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2ouwiaqmh.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2mgrjjjbd.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2axtzimrh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2offwmyrl.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2ynbjyuze.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ccrvfwpk.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ismnhxwx.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2bjarbjid.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ywxofztk.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2vqzmjcnr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2oecxqffl.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oiwmgpdw.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2afejltqo.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2jfpqqpqw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2kmzaogba.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2rpfujdui.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ysykwzmu.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2cvuasrzn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jfwimkks.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2mylvnbpv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ljfdifub.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2iozdyujb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tucrytkt.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2wqgwjqsh.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2exaiibnp.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ocfkhfwv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2naynubii.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2jlmlcyys.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2fttwncjr.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wdjjatoj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2noovaiet.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2blgsbvfd.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2gsavzhcq.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2krzfmkbb.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2uqveyhhi.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2jcshtzix.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2mxrvqtjb.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ovcaipoq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2efmotluj.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2riatwusx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lezoeolm.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2jofonjqh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2zaokipvj.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zpfsqvpe.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2twjgapgr.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2epgyeszt.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2wpuwbzig.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2aatifbax.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2frxycycg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2awbkfqio.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2aqtoxvsp.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2khfjwqlt.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2dnckpcod.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrdxwghy.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2eaxpetqr.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2awfxvcao.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2qogmfshe.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2wvvwbwob.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2idxfjxxm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vpmhgzdb.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2humsrxau.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2lqqyvtjm.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2iihjfbyc.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2gcsoxzsj.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2tkhflhuu.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2pymqfppu.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2kxkenmzf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2piezhtwg.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2kannkaoc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2yrfiwpoz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wqapykkr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2thfhyqqa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zfdiqkje.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2eflorclg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ikqetszk.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2tuckemvb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2fmzmbizj.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2axbddjxo.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2pudyqqfx.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2drnlwzgl.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2morklayf.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2nrcewnng.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ttrphvuv.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2tyjghgqg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gjklhtkm.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2uuvijnrw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2fluzsxuj.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2aubqmfnf.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2yjtkyrni.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2zvpmyezp.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2blrwlfjx.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2squoyohf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2jxlwawqy.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2yfntxjlc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2tgcxutmq.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ylivgojw.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xgjcdcak.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2gzllqmoa.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sgphluap.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2synxazjl.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2svbtpmsh.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ryxfezej.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2umjyfbwq.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cajwthiq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kparctzv.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2rbhfeprc.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2bsxpuoog.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wvvfkssl.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ffhbbnnn.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2jzooohip.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2mkaqwbwb.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2cjykvfzn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2oekzpufi.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2pgjyornm.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2cembllia.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2cdctoitm.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wdeudtpo.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2zlyxrngg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2rhbybxhu.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2bcjnxqvp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ffooclay.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2pjkmfrmq.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2dpmvnbrr.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2cdbwwmov.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2yefwzrfo.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2ihnulccx.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2aocghoxe.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mhnpfoqm.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2cerjlncq.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2vwxqfwnz.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2etuuvgsr.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2gnwrrbii.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2oivmdfnp.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xgfihkxr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2bzwwswoy.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2qsiurjom.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2asnojorr.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2svthhkcz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2ptlxqzai.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2msmvelau.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2uopvtkie.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2lpbgznyy.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pocaxdnc.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2mwqxcdya.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2xcbwueek.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2qahmqkjd.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2eeotxqxu.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2noeoehbg.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2fnxluzvo.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ekdtskrh.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2kuqcmcwg.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2cnrneaji.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2pvexqpgw.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2aghyngia.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2rcfkhioj.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2pggosjzp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2lmajwpjq.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kvrbundk.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2vhhkbsvd.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2iobfboyw.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2dfcyrbko.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2qfvqhuaq.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2dsaoplkz.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2pgjspwvk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2vbntcuhq.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2axcqwqkj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2taekjwbk.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ihzgdbgi.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2hvbdfixe.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2noeekpgl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdktwiaz.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2higwhyda.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2bndmcfdq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2yjobwhaq.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2oadrgxra.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ujnnszdu.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2tzurikfd.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gosslbgy.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ecfsjxok.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2fdaebxes.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2oifkullt.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2duwajuqu.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qjupabvo.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pdsprbtv.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2xrlfwzca.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2tetnksxf.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2znwsmnqe.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2iocraoit.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2dwtllrep.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2uwchzlmc.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2dhfjywey.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ukyicblg.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2oqzmhqlx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2odmrkcxy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pwcwuvvz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jzisxejy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jcboubng.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2diqkvppv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2pyeuovkx.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2qyggyzdh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pqitibeo.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2gytvogdt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2eamdlsxk.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2owsrfctb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2ubhgknbx.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2puxijyhk.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2gthqpckj.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2yndxbutp.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2fjkxjmrk.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2dslizspi.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2kybbnwrc.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2hoyspsgk.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2lshwjfil.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2wyipjzce.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2zethccov.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2nlraktsm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2iavfhqxf.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jwscgmor.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gcidefbl.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2yfldyuex.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2npsstbai.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2wifpqogx.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2rmkyhsra.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2ltyetmkc.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2xxwhtazk.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2tyfwuwlf.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2oudzmebm.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2sbdrghfy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2fvtgljrm.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2xpelfwtp.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2vhgzzrdd.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2bnfmckcz.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2gdvmbmkh.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2iviahbcr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2xjevdaes.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2nsnsyahe.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2vvluqxxh.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2tuvqmros.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2qwbnnrwb.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2gqjvnkac.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2qyfoxxzp.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2fkpdaxls.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2awrjklle.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2ocakjcag.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xiifxhez.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2eqmnphrg.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2uxcmmtjn.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2ylfpjoxs.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2zaoyvkrh.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2euuyllrv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2mtckvzgy.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2ooaxoqpc.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2lndnmwgm.html


<!-- 参考信息 -->