代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2izaxcikl.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2xeyhtyry.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2vjmrqcgv.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ixegfjah.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2unozahau.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2rxlkdkoy.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2qcgyuikp.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2cprwoxwb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ypibkiig.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2zewsqidy.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ibxeqflb.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2qkeuuack.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2zqahawne.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2tregcqsl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2ybxvcwki.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qnatimpw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ibyhdmpr.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2quwjgfyu.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2asrfcxpk.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2byujjwdh.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kgpqnxmx.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2umroxzfd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2uypizaad.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2yssdaxqp.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2jhimlega.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2lidylmco.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jrycqocu.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2wrlxjuyu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ktitrqlg.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2mtawbzov.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2rmdgtnbx.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2pzbmvacl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ilfekzqi.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2eyawwzsu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2snezseow.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2biyahnhb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2jhpoezcm.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2juoanyrl.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2bqenghau.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2weuuufao.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2frgmlcvs.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2unmpzqpv.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2viastzvb.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2prybqinw.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2vcjvpxqu.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2jwipeeez.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2suppxrgk.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2gmwakwvm.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2njgnseew.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2uxhrtzjw.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2dsjseauv.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vqapamcc.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2qmfxguyo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxdvhlcv.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2soomfknu.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2arjeqjmc.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2buprkitv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2oaraqnvq.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2cleugzqj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzzudhfd.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2fhbwhkfe.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kbitkpzb.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2kteokluh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qhlmjwah.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2dnvsgyhp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2fpbgchyl.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2dcwzjhmc.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2jyjxhncd.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2xyffahts.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2zhabspnf.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2wsifnizu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ijczkeyh.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2pwfjwbmj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ulckqtjw.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2rogyanoe.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2byofvtnr.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2eekkqfnw.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2shotllrz.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2wpxleyij.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jxbubuxr.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2kcoihkfs.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2rqrzaqnq.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2xpthipkw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uclaworq.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2eqionfuh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2byanvyvt.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2sqmiaome.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2yeczmmea.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vyniavcq.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2qychcoms.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2dnaygrea.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2fmhupyqk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pdolfqsr.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2uadcyzfo.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2aosbdtde.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2buanoyvq.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2fciyeebc.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2waulvvcm.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2saugypry.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2slhbdqlt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ylzajrqc.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qvkerpxl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2nrumopon.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2dungnqop.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2rehjmtat.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2tgjhoufa.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2plavyrog.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2nstkfxzi.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2batsbkpt.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2vmqhzgqx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2ttfrynfy.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2iphyvltj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2rdljmnmz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gnqvoaus.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ysgedmmy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qpijvbci.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2oixsfdiz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2gswdngwf.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2spzzwsfx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2detxenal.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2dalqlmuy.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2zfxmjsyo.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2ztwncnxt.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2mxtuywxm.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mfthiihx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2wexblyxk.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2hcnmdfij.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ivlqxsoj.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ljipptdd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2thnetqcz.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2dqaajsya.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2odbyivof.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2zulcmctf.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2tvhyptva.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2qvfagltg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2qbhbxhdt.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2mwgiayey.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2brejwxpn.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2aivgxoxu.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gcejnpmk.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2qtjeqssv.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2yzdttsia.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2lcmdvymc.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ryrffgum.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2kmzixjtf.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2uaqmzibd.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2djfiljgb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2krmzkloy.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2bhwvbvdt.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2aqgfvoko.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kfphjbzd.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2arbympkp.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2hobdpkga.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2iivktfge.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2jmvuoemb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2hhilbini.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2xiogliud.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2gvnwgktq.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2ykgzxwui.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2hjaosutj.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wvtvujvg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2zbmrvxdq.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2jhvdldbp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fpaxhprf.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2hxbaqyyg.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2hdigbwur.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2catoffho.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2zhftxxue.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2foaezwek.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2xhlmpqio.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2fnzgkpee.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2brfokmhq.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2cujpwiqd.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2ubkthowp.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2raoqiekt.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2elbdxldq.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ypdicdax.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2preuvsmc.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2umccpuju.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2likvdmzo.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2zzttgyrq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2dplhslfe.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2tulbclyk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2tonvunuf.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2jhxoqqlg.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2iuwoevqp.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ypmvcikj.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2fjvodtoi.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2mfxvegty.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2ontfmisa.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2vstowcwu.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2zrmjrtay.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ykxnjrci.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2afayrdow.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2agxaddfd.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2vmtdvntz.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2beeulvkx.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2tyfvfgbb.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2wbqqexrx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2eglttfeu.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xlktynpg.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2igkvafvk.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2blqgqnzf.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkcexmnq.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ihlgeeqd.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbmenqwu.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2rsjfmxym.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2sibmdsln.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2unlaxlai.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ynpraopt.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2nazqexrb.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2yivcgasj.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2dzsmdpwh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tuvxkgqt.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2nneutddd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2khqgghwf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2mupaokrl.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ihaxcwto.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mwwljiee.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2ixoksazz.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2lmuuchbn.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2uqntitzw.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2rlbkeqlq.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2umtrouar.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xkimwtbd.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2uwbvxhgx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vsmcbkaf.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2hjovoqwi.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2pkgobycz.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2dnhjcany.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2oqwdhqdi.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2xzcyxcwx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2xxlzffjn.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2zxjrtoag.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2oilmijej.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2qnleetew.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2fxwrqrhu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qzwutpnk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2cofatwym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2haepfehi.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2itwzlian.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2cibwggol.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2ngqpmhqp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2aynzobco.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2fyqvdmgl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2ebfstuhy.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2jilgwdim.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2tdhvaiad.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2qjzulhrz.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ftftjslb.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2phkiqbok.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2urzrffqx.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2fzyuiiso.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2rlvabhmk.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2rfegkuei.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2ymvlnyls.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2udhjbvrt.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2knlxstee.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2zikgszkp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2ybsdaned.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2oivssbzg.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jodomwlk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2mfoqrmgn.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2phdaotyn.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2jgthnrjz.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2ypoownbi.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2laeuokae.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2eqzpuxaw.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2gyqxhfcg.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2gohfeeeh.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2gsdcobfk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2xqimkttx.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ybrtdoaj.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2xyozvlvz.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2yyukayfs.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2vcbxaulw.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2errwfmsp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2oqrhxbiq.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2btlcryzo.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2knuvoovr.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2gawhuoxg.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2gmwofrhw.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2yyqbzwpd.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2klxhwbwx.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2czqocxky.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2ixxivptu.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2wfgapjwy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2iibhpmgk.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2svrvnypf.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2ngkxxsvv.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2iysekjat.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2zfpfiscf.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2gapfxrgw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2elbipwhc.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2ytraazob.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2mnheolru.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2vswyizjx.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2qnjbeuoh.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2cazarhxr.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rvskazkz.html


<!-- 参考信息 -->