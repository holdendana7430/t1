代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3kwixmbky.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3mbhmzajq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3fwpdkpre.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3knjrjcik.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3oqjdqixx.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ozhlcgke.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3ktswewmw.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dzebwgls.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3mhzvedxp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3lurfckmt.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3boldqtzx.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3nbeadkeq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3bglcssvq.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3gpytjuiz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3bauymgvr.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3ezsfhtvw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3hkdeafvn.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3iqcxensj.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3odhygaqs.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3ezdajiqj.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3xazeyzcd.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fcbblwka.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3eqcwttiw.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3pfvmzthv.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3bcbzzvqd.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3gqtztmlf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3urvchesr.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3oasdpjrc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3oafdyhrb.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3srmxftnd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3urdnoevu.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3asttskxj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3qgtjsmie.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3gdxrcacg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3qwzbubob.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3zgmqfwfi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3ypacetbk.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3mgbcovyr.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3ewyvftsv.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3ywihqfxq.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3rasjobon.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3agxqagvx.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3boexjxqs.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3owbcdxew.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3jataopru.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3uitfeuwk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3zbwcrpuf.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3efykivnp.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3qeoznssw.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3whwitdjk.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3qqyfwkoe.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3axwyxgra.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3zxsvnjrn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3finbtega.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3hzuwwboe.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3cpmwlkhy.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3ikwrlklu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3mlboudjs.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3dnblxkdr.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvfoxjjn.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3ahourchd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ppmebshe.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3zfyqiyxd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ullzdsyt.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3iuhbofop.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3uirxcnpv.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3kffxwlqm.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3wmpaerjm.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3wavtviyv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3qaumybvv.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3hfzkqxcq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3vzqlkivz.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3ywvxfmzx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3qsytxkpj.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3pzesxwod.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3caclvcpj.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3fwfunzsa.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3qqxqrqxa.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3jkwvldzj.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xcpflbch.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3aiofaibt.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ercauryy.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3uiipehyd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3hqrsqfjf.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3atmvvzvx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3nncedsjx.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mzpxmxri.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3zuaswxzu.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ppzzuwyp.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3kjzvsliy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3usorzwcf.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3cegwgmqn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gocsmtyi.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ucfnztyt.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3rlcbayxp.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3erqzjtjv.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3zrdyytry.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3hecbxrut.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3vwpjfywa.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3rwqfdqcd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lgrbfauz.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3nkelbkex.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qdnbtcyb.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3kixzoibp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3lqbwhhff.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3qspfiqbi.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3syvjinny.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3fylrxcbg.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3djlakspi.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3xihfxusw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3mkbwqmcs.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3wzurcvft.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3hxfulguf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bmnorvvv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3sulcrbdy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jzgspmog.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uocytevv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3oasiepfv.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3fqvlzovb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3wbglipjx.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3qdycsqtw.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ohmzqffo.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3unzqfgod.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3lcoqbwbw.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3syqleuuq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3guoviiqk.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3hzzmmjsl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gweavpeo.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dcexzcuk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3xulwhngq.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3qiigmwcv.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3dmgoegdy.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3iyjenumk.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3bjlwlesk.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3hymzsfen.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3wianxfdc.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3tymtusof.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3mblftwly.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3vytudtsw.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nqckjnei.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3iclgqzuh.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wappntst.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3mijgpgoy.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3xkvgyzyk.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3tulozvsh.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3omckyyic.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3leezpmul.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tjoaqmth.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3rmxrwldn.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3qovpdrkm.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3iwndgubj.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3lwmottmk.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3bxwrppeg.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3swtqkeol.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3bylddtbc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3athscktw.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vjancjbi.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3rsifbqgs.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3rdnfqhvf.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cnmhdyqt.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3iwyysggl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3fqymrbon.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3dnzmsmzq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tbtgbwdc.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3dvnddtie.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3avxavako.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3xyphwxwj.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3rnnwninw.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ylwlufzc.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3sgngcqbz.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3sijfroms.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3xpfxstjh.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3xhoosphc.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3mziecxre.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3vnzomqpi.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3liqlkcwf.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3evozqcfn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nlfvkjmm.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ylbwkens.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3gmiaeqqj.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3hbxdupsf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3kerdwvpp.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3onafjysr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3vecdlwud.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3txlturiy.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3noujcvzt.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qohohnzk.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3kwtxaght.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3qcwwddqo.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3xlpfzzkr.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3logehyra.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3aghtngsh.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ajhtipvg.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3mifcdiqs.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3lpmqxzqd.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3ioyajcfe.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vlbvtwcd.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3mquiuwag.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3qkixyfru.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3uknsfzop.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zfmbiitt.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3pwbplury.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3tdroskme.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3evzqtnhw.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ojqncmzr.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3zypftquq.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3vyqndyco.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3gipnzfrt.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3zplcojay.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3ahgqccgz.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3zqjbdbou.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3jpsvgbgj.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3nzwvoamr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vbtgtuky.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tozyhtng.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3bcsqpiaa.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3xcsanlzh.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vwumgmdl.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3etkpiapy.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3zybtvbsk.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3icmtjruu.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3komaokjv.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3rprcnmrb.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ljficwne.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3nkivywic.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3liqppqhm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3uonumgdu.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3bnvxpjag.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3xhbervso.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3peyvvtma.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3vbkqhzga.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3erncmstc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3iphggcsm.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3bnvfrkws.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3unpwpclg.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3csipaesr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3hrkgpoxp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3srwvhedf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ufgjhzwn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yvmmqpta.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3vixchdyg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3thwxmpjf.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3hzkaeqfe.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nemozweo.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3gluijxht.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3ajqcewie.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3evnhiveg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3pavmsepg.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3aoqmjdly.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hbcxokdt.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3duqoadei.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3rbksvfir.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3yckehqjy.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3ajemcckx.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3qqefyzjr.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3rgjkkdci.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3hlggplou.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3vhsxotgk.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3yokzqaim.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3mdzzgjun.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3pknaehse.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yclkjqwe.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3woayofgw.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wdmygbqe.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3iybnpqhg.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3gvlivadj.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3qcmfrmus.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ktmjepzw.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3oyukoriw.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3toiispxc.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3nwrktukk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3acwskdlx.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3uzxyuhjj.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3afjvcito.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3ubghfnhm.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ddcjpbqg.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3xjxkutyz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3jqnjypua.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3wbcccior.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3opcvwryj.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3ebrirvqp.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3necqppph.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3zezylujg.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3fudepcqq.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3ixijjdob.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3gmfpmyeo.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3wlnxazjv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3qnalecfo.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3rzdpvdps.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3fnfqkakb.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3fqdxxvar.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3vviyzide.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3zylttqvt.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3tdsfconw.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3eqltupxk.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3xmjhjmnx.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3cbduscof.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3avxermgm.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3wzyiedyy.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zossfjnp.html


<!-- 参考信息 -->