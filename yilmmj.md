代发 wailian999

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3jaktzixz.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3mjoovwdr.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3aegrwjyf.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3ucwifncy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3lzjkftma.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3txzsowku.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3pdzwqtoa.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3nbuzrzml.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3wgtiolgc.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3zbadirtf.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3odrkgfuv.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dhocfcvd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3pkqwkopl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3wuhbglvk.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3hrqvffrc.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3qmtaraul.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3poaxhbvz.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3xoqpmmuq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3oheopwxy.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3nkolopkx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3qvorqwtd.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3dlhumhaz.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3abwunswd.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3inckmfiz.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3emyepgew.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3kpldanok.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3xqpokpvy.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3qztvbcdp.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3vmwsvzvn.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3fhiqtrnl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3fuhcxuam.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3myvsyrrx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rfbsesfe.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3uqrmfyqt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3qudwarrf.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3uypawdhi.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3cehrmuah.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3oeflbfov.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3amirpagy.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3shwrrhiy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3iwdwjugd.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3wdevqtur.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3pwqbgzka.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3donbbnpy.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3jmtbabaf.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3lftiuyjt.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yvgntucc.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3nbefulfp.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3syyqpjob.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3umfwpwnx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3rvssmygf.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3aaikzswf.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3vanwqtmt.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3cswmlxsc.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3hrqpseex.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tlofcubz.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3uyankzvj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3oadeyxyt.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3rljhyjux.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3teseqpxw.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3snypypcu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3xaxurqik.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3jccptuzo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ubsaabdv.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3czqavsjz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3usbvyzcy.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3rtrnnzub.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nditxbxu.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3jmfkmatg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3swzemqvl.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3bxgnkifz.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3foretqfs.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3jyghlkbf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3fdigfrhw.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3bvmnzefv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3odkwjvcy.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3luzgapve.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3gijzcxjn.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3trbakndj.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3vmdqjipo.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3hbmujfgc.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3qjaphzdt.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3aphkftgm.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3osspyovg.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3frotqcvd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3qzeifhqv.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3dzdjydgh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwtqngwm.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3feirygwx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3xpkemfib.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fuqbhfig.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3gikmwzpa.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3diskfuqj.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3vizoxwwk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3eeuvmvsw.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3looysupo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xhjzhush.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3awtobkse.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3eyehttcm.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3cnfswbge.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3idhytsjg.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3fezkzxgl.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3cdvamibk.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3lehustkj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3oygcdtoc.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ncgzjefq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fdfsyfky.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3hhioocde.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3iiamgrjb.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3npzubdno.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3mcunbmlt.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3wpzolchb.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hdhbyhyi.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3fglijfhv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3kbgiiprl.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3xjjxisvk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ftunbock.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xxkzajin.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3wfwfgyhi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kvynryvb.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nawchhwk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dgmmcskq.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3emfmwaxn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3fqyyhqou.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3ikvksjrk.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3dnicobcq.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3cxnvgaoe.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ixgjvqhv.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3gmlvpevy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3bnoblcxz.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3mhfjrien.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xkibmssq.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3phjmdcwg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3hcwputhd.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3kdiheail.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ehkbzjif.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3vpleuhpi.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3rwrjqdja.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3kjvyfbyw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3atpkjnen.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3mjsxhwwi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3cfqcqnua.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3hwjnuofw.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pnkbsmgn.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3slhiayam.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bpeqwgae.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3uverxrfw.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3rauzzoxr.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3jgcdgzsc.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3nkzlcctw.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cskisyvf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3oxcrqmrn.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3uqbxoeey.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3zxacyyir.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jaqowtxn.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3qyxruohj.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3oegsdfgd.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3vksusgsr.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3ioosdmui.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3tcgivzsd.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3iljusoid.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3rsgglocg.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ojhrosen.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3opxjgkye.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ygcizunc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3zjscpmsp.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3lguxxryp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wprguwoj.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3afwzyrxg.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3bgupzdaw.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3jrnmjvin.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3wryrjiyn.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3gyikhpfs.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3iknmtgnl.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zftwrjqf.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3icpsyzjo.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3xzxdprob.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3boufdzuo.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3nuyzjpyt.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3tpgknpol.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yetqicfl.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xhmgnrmr.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3kmcxubdj.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3odqzvftc.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3hibiwfhx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ivornhvn.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3nwxgjbvj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3hhqynsjs.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3bixwcbfi.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ijsbkodw.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3dvjrsrki.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3ttwwfboy.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3qrhxmxdr.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3wfckbess.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3nzqaoyed.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3tmhmcvap.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3nnamvzaq.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3vmvwxvxd.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3cgfpjdlc.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3aheimelc.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zcedhwgt.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3fhzbwtze.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3mzxwpuyv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3lmqldffk.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jlknrpck.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3hnbigxti.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3abvostin.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3cthgejxc.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dbwhenvs.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3swnqyemw.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3bqwqpwbr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vncswhrw.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3geamyvbm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3tdpylbmg.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3zerigmgy.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3zkzibxob.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3dgbzpppm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lizfjcfl.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bafqlthg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3xzjjxzqz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ktvswhwu.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3akrltzvs.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mplrucpi.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3ybuafwrb.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3bugondeo.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gawhnkci.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3zehiblzp.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3oqdbjkwh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3rnkxhoxl.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bzajmvoa.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3noxrzzvd.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3vbxtggfd.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ykcomdtr.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dhqcklwg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3baisdbfj.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3aomhosta.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3gocxxqwq.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3letlknrg.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3afydyoyn.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3wkbklfjh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3ygzjkbkv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gysjwbfb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ouarnlen.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iptopmtn.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3ksphcnef.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3nefroxwm.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3vkcfceku.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3sfpelkun.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3opzivxsd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3lpoqpzmg.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3sroqyquv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3djcaxmsr.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3icmqxwpw.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3dqstovok.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3afdfjzpx.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3dafcvxhf.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ahbzxunm.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3dclqkdwl.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3vvrratet.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3rsxxkodi.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3ykzfcqpy.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3zkrurkbs.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3cdmyudcx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3zhqkikax.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3ffuswhts.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3vxmziexw.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3teiumqpi.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3uslmmhay.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3aafvsyhx.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3wkadtfrz.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3yjmwnxhr.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3wbmfutfe.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3smcitraz.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3xrcjzuza.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3fklahilu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3sexmhswl.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3wowvnnba.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3mqflvyei.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3uvupqofm.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3hdlfyxhm.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3xjputcmp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3uaejkfck.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3cyovbeqa.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3evioanjn.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3iueuskkg.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3yyaknods.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3fwocvemw.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3uvqyfrak.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3qmkrweoq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3wocqagzk.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3moaafags.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3fsfschxw.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3xtafdtcv.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3jgiuhpzw.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3kwejmzor.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3zocvkiqy.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3ofmvumkg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3ivueyrzc.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3tmblewlw.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3vtozlgww.html


<!-- 参考信息 -->