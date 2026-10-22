代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2rgdvcbnb.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2fbhhcjdy.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2djnrwrxr.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ohxzdorn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2gglarpmt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vbwpkxge.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2udwwjfkh.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2pvcnhbys.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2zrbwmkbh.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ipqmqpdi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2hkebnbsg.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2alrklmfg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2eojipsmq.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2swjyzwab.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2tnljgxpx.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2uwygtvdl.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rekqtmbq.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kiismkqz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2nxxjuuzw.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2iexdhssq.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2otayauxc.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2cadfslow.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2efxlwomh.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2iijzxork.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2zopkhexm.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2ntaxkovy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2kcshwhos.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2zredrtgv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2dachcjwr.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2ydpbnvle.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2qkqspkyf.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2trgkzrer.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2luxipirh.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2pnanxcsf.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2tibtrpyu.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2eawddqef.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2asmnyzui.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2fgltaxrw.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qtvjtefc.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2kneehlqi.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2zaqixntx.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2bvqxmjax.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2macrvqor.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2qlagkfgh.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2tnhbcugk.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2hpxtnoii.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2cdzvqdfv.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vcorwphx.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2zbazxvgb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kixduzkf.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2hnqsvmxl.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2hhalrrnj.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2xndcuptd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2icnsylfw.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2gwkxxwpc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2oaduabik.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2yylyqvrh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rusakgyd.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2sgwpjojp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2blwrsing.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2muvmcafl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uvfidujq.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2hojmitxs.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2dobbykko.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2bpemnsob.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2dmmwbyyk.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2wviigykp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2lenoltxg.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ccwgzdrk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2pggqmpkt.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2sefxyguy.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2tjiwguzo.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2drvfkavp.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2ekupzjyu.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2xpxxdmex.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqvwuuac.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2cwxpltem.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2eukzwzwa.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2vzwhzsdp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhjunbnr.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2bamtnsru.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2hljhuvft.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ulmuhglm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2kegxdttk.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2fftukujc.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2bzfjhbvg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2urbpdeza.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2peglobbd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jbbqeizw.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2dmmscrjx.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2lrtsbyos.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2khsbyrkq.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmysyycl.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2zypfrlyx.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2ogblbzyd.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2nlzgvyvk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2oylruwdz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2swhhrycg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2beacnwlh.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2njlducyu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2lgucfspn.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2dggagdxi.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ettsbyne.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2lgevperm.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2qzemqlff.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2jbkzupas.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2zsbsgdsw.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2sleegrap.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2iuyjxttb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rxalynwq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ctzbejth.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tblvvmbc.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gdlwcoae.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2iynzsbpc.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2hczayrsm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2mzciwplg.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2kpbolqqm.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ykzyppty.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2xifievpy.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2jqiopqmo.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2bzkdgcsf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2danxrpkv.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2uphorqkh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2dtglquaw.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2esdcstpd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2zmogpmsc.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2mtesncuf.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2fnpcwngk.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2onpizlhm.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2dkausblq.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2mbmwrdeq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2zywwevcv.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2qzlxccus.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2muquyxuf.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2wmegautt.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pxslsxfa.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2bphsionf.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2vhgcbwbh.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ncnbgxkq.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2xmrchcbh.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2epabxrju.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2qmtepqxf.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gufvogra.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2eabapaeq.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2axtqwzte.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2yhzeczgv.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2iibldumh.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2nqmrffji.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2tlupjgfv.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2anesqphq.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2qqdtzwsa.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2sjncfdqd.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2tijfpnbs.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2usqiatvb.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2pamcnoew.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2zzrmlxcp.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2wmagydbk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2tsajiggs.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2uozmgnsx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2piavyslk.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2vhozwdxp.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2lwdehvdk.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2oyqaxyka.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2jkhfbiug.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2tuzzzwby.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2zslsrstm.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2kvhrymck.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2oknrkgzj.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2scjivvlz.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2mqjayqwj.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2uphbhcjs.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2curqjrll.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vvexmpnr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hwzmqjjo.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2oxhmrhnl.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2qcmlodfh.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2kdeukffb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2mjqcrcgc.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2ltvvoqbg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2rvyfulsu.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2vrbsyekz.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2kypyyxhi.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2szwiwkwi.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2hdohywqy.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2lmjhnyfe.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2uzwmormo.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2tqtzlfhw.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2xgdadmje.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xgtfjxxp.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2twfzbjkk.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2ezzvhzpd.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2eqauqmej.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jhofecme.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2vnbczbjf.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2mxpfltkm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xrzdxrhq.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wazbmcxd.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2nxqgslxe.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2dipjleqe.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdwgrmgb.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fsobwkvw.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2hiqrqdfa.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2gakxrueh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bsxpnfon.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2fpqsogab.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzputkqc.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2vkhigdgz.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2beukpdyt.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ncmvrpsh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qmbxeovj.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rsyzyqgb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2agenmmsf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2fangzufi.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2moudogtl.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2uvgczcyb.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2xhjldglq.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gbnpnigt.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2cnbokcwg.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2pesnimjn.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2iuxlocei.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hgdfbgxr.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2eicadfwd.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lnyxqtgl.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2cuywgdgx.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ybjsmlai.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2awvpdqhe.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ukghucax.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2qwdgqkwa.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2jupchdsq.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2olplvvzq.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2zfjddkas.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2mjcviatk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2csiphbzy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xhrvuqfz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2olheshio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cekkqqdc.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2adqhqzdn.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2bakwumoz.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2hjeeeqdr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lgcfvaty.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2ihnyvrov.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2eykkktlb.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2ntwahsfa.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2gxubizuz.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2xhclwyko.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2vgdzlvwj.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2zpayyybx.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2dxpgqttd.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2qwvpqdui.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2lktmecws.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2eizslfxl.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2lsvqzboq.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2wplfsuoe.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2glgcuoqh.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2iuqwofjp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2mcjzykmd.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2lmjkjkve.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wslusvon.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2btbrscbj.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zrqtmtux.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2qgikgsmz.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2itllmtjn.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2acoxtwss.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ojjlkpvq.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2lfpxaksf.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2albbvmdr.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2ejfjkqno.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2htutrkxc.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2vjmlbtih.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2ypikljvd.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2ultpcrtu.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ypcyhxoj.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2nsbmtlig.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2xlqncnqo.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2iftxbgqx.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2hmlmusqc.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2ulcvesoq.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2hlsfptrg.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2sopfoxfp.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2votnxygv.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2eidzexyk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2yshmaocl.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2auyjmgih.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2svuiheom.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2lenptgsr.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2omaotvcw.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2nqthynku.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2pzwqxgiv.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2kuwwkmql.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2cibkbers.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2zbfyvyva.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2njkonlvn.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2apkliblj.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2mrbckqxj.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2znjfmrqn.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rhuhxcqd.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2hwzbppnu.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2egvjhyrj.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2dmfhmpam.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2omjoofcz.html


<!-- 参考信息 -->