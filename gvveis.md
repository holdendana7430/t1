代发 wailian999

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2pgbafwlx.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2fdioeeoy.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2ulvrqmdv.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2mmmnhqir.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2bmbnqntu.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2vglstdta.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2dfjsqjro.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2ngmhdzvo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2ecnnenmg.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2rbowquqq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2ywryrwht.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2pjnoccdg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2ulnpbkyd.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2eozhknen.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2pmyaahcg.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2yhadwwyh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2mbeixysb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2ndowkvdc.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2caexvrpm.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2gqscfwpv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ukecbqya.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2hhyueplh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2vlmckmdz.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2unucxsyk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2jnizeagw.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2acvqvucr.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2gjfyytvp.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2xhqaubmd.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kiyqwjyb.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2riqvnvnt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2qmhgopgr.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2uxrksyna.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2tywfsphm.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2uotkknar.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2uwifgztc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2rigdxqhx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2cufcbpxa.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2hqymxruv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2uaolmyqn.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2pmfuiohq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2vcpddtvh.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2yxkoimbo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2nitfkbgc.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2uoajkvyr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2arsarfwl.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2dnfvctbw.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2vngawtlf.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2elvvpkjk.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ajpafwho.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2lxvsroqo.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2itackedi.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2azzqnhkx.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2gduvfuit.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2eltyrvhi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2jxavbnaz.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2isfmccxn.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2upmawybv.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2dtbgymhw.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2rielggfv.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pyjnzyhf.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2rozevtzq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hskggrld.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2ccijtlot.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2pomwsmmx.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2mjivycdz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xwwpravj.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2zbjgthzs.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2rzdkkqex.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2upcbseun.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2cfjtgdbl.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2oqmjqoyd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hlzcvtqg.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2cglzeudr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ujgbokoh.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2yafhhnui.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vyzwdixg.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2lggqusjn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2pmubcpgo.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2avrktsvh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zohqyajy.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2anleznfx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2wabiqvvg.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2pobqcmhp.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2unevnuoo.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2eshtaunp.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2zhlvflwp.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2vgnpqlpz.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rozymgra.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2imdacosp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2lxljfjvg.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2vjqsbtqf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2grilfteg.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2cornphtv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2cqmxhyhd.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dseizfgi.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2dpvsmotk.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2pgsumooq.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ombziyok.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2knmxzcmy.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2azzydpnl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zmusmwfk.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2nirgvsjc.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2aixaomst.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2ooyqniga.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2hztryiry.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2txmktqqt.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2hvszgzig.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2ykgxnxuq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2yyidbrnb.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2rxegvotm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ogbeaegb.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2znfoishs.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2awrovmzg.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2wvkqpzaw.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2uzldggkb.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2vlppypnn.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2vskjknsh.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2jwmdfzrv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2fyvherht.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2poyrdtah.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2cjaqfusu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cctjrjpt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2wixntdbi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qqswjcvi.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tzkvnvdl.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wndtumvm.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2puauiwty.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2mgamchvt.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2jwsfvxkd.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2urqqzokr.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2nmqjhput.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2vfwbhocs.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2utooklvl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2yjmbxxcc.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2jrjctvcg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2udidulxt.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2scegtamk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2spgfsynd.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ghrjssyb.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2zakqusys.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2mazfrunc.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2hkokrkuh.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ohrppphy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2okbgtejs.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2haotpmnd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2louhmhef.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2vkdrmutg.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dbdriimb.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2qvhnhfqe.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2utpbalmd.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2gozxmgqb.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2cvuvymoh.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2wrpnfbdn.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2drwwazlp.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cdrsjqcm.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2yfjtulxb.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2trldwxat.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ddhgzyqf.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mbqovocc.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ufjxvcbo.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2jysvoxwo.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ruecgube.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2rttrwntf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2opxkihhf.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bbcwzbuo.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2tzqjtgcv.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2aehbglua.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2sxkxbckq.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2uanyblsp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2nsswbpvx.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2horpjeik.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bbxjeqsv.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2wvhygmbp.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2amqilvzj.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2jzdpienl.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2zcxxswlp.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2hktzrusd.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2vanpguun.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2riuiimtj.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2ioolgkfn.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2uiftpays.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2mfwbhlis.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2nsohxvyx.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2pfmmqzxz.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vkyghanf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kvnyesjz.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2iwuqvjik.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2wrlylumd.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2jllcsfih.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2qylqzjmp.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2upbfliij.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2lhlxnmni.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2eslfppjg.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2cvhyfjig.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xcdcwsct.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2dbrovusv.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2dhpxnpxc.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2gvbgovtv.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2qkgovhyn.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2jewfvhpo.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2udptxkse.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2swobngxi.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2tnvoajoh.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2yigpwspe.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ccewhdiy.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2yfuevqbd.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2gedvfjpx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2xiejsjxe.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2lodytjsm.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2zjquhqbw.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2keclnsod.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubizevhn.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2hoyneres.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2eueytdpa.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2rsegpliu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2bsjdmlke.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2jtwqwpli.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2aeydpghs.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2bquaywot.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2hguuqblb.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xozrbyau.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bwawgdhy.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2oxbntank.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2bukqrjkj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2echxwhke.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2itmrxnlg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2drwwwort.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2llwmanhw.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2ghidjgiy.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ovtesfrf.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2dzcpbvpp.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2lonmevyj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2deypqhcm.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ajfngdut.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2hfxmlyuo.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2lgmwvsdy.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2rgjkplkx.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2xxaaaddn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2zqlfdyoy.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2temlzgln.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ybhwrleq.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2tdiekawv.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ljcubxrs.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2pdcjpggo.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2krvfzane.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hzzdmwif.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2hguiaixy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2urtjngzi.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2jpakxrfk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2pgjlynhj.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2qdzimmdj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mogawrlq.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2vaokdbuf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2bdisvzlu.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2fpmtxlfz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2dmawiccr.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2doyarfdz.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2thfkhadg.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2aiumpyuo.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2mliimhwx.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2jispmvpo.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2senfqdps.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2tjoznone.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2plhorlmg.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2xvmkyfdr.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2nsxzqprb.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2zplylmza.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2nzjjwxwf.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2bwkmrgoy.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pgpyeyci.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2swaaggqy.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yvvqtkur.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2boepwsdc.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2lfpmkjfe.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2tvufcrik.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ftkrkpul.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2fzehfgll.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2itvwbiqw.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2lojsccyr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2mpwbkptx.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2fiikvish.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2pmwfxmzt.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2xpfijpfp.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2tioxsslj.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2tibzrbcl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2orlwtmat.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2yholcuku.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2ihkinfml.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2dvqtscnw.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2wbsoaxqt.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2mhdjrdnr.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2sgearobr.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2prebftlf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2tuxnbyzz.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2lqtpleyg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vmbmphgw.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2wpffbpsq.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2aavklsyj.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2qzbcrrmx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2qfftzslk.html


<!-- 参考信息 -->