代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2xtmcndxt.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2bgjppjdt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2dlgfbhig.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2yjqkrtzv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2aatkkhqa.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2pecoxeka.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2kkxdvjzv.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gcmxufqi.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2dhefokzq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2kptqavlt.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2fwmgmfvk.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ffwueyus.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2loyqadyf.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2acferxtv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2zbkghjdg.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2lzasrczd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2fmqwhtmh.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2aozkfurd.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2exfvpflk.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2dzripmmo.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ogrllepk.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vxwpxect.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2pyyipwws.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2fszpueny.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2dsevuxes.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2dgjctllr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ybbwxxbm.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ndkyavpm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2wonrgacd.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2hkkkmpoh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2zkfrktxi.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2yuqbbnhb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2ahmkpwuy.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2xaconmiq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2thhoggag.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2lgmrvcwd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2rqajuznz.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2uyezijwr.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2xvlkfouc.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2darjvzbd.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2hqhdxzou.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2cbdjwbyc.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fbbmquem.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ccutbgfx.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2kugetbex.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2iaakatgi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2bvvzmave.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2rplhsxsk.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2cbkiyekc.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2utzznxve.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2nuikgvdv.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nlcvmjgk.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2ouwijxho.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mexvplse.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2fkkekgrj.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ykcbobjk.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2lnhvzcrk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2drcmaeoc.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2jxwwewlm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2bfgiqzzk.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ooazphoz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wtoywqvj.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2lypceknt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2acfohphm.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2theoclou.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2qrkydexn.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2xwqfqxzl.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2rinanyxo.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2zwcatqlk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2sdxnwnlo.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2colkrpxh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2upqbhcem.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ijfahdyf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2gbifcnvk.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2bpzntywg.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2ummfyoui.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2opzgyhvc.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2bwhnqunu.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2oymfxqom.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2pvdpaxtd.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2zosqdvdn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2gacvydio.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2bmwlsxvj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xygvefqx.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2gtvhmqat.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2bbtydvda.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gfeyqagb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2odezlewc.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2wwnaikgj.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2yvhhengj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2nemrwooo.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2buxahsng.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zpifabsk.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2usqipsdf.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ajugpoki.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2shhkrtpz.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2mmcfvxif.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2uulqfiqz.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2urjwktdn.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2enrhmvdb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2fhzyvhkw.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2udqipodp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2elibssgl.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2fngcphhj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2lahabwdo.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2wlgwuctj.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2akrmtatn.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ldinoutu.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dwhwpsye.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2upkzzmpu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2pjhqanbo.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2pqhzogyh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2pwnnoila.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ziuogzgd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2aakcqhjf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kxdojoou.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wixrjffo.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2asulbwdq.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2hvoomknl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2kdbbbtfs.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2kkrkjbcw.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2whvjdoso.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2dgaignka.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2drcwiuzj.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wfxdmhxz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2lboiijqp.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2wbqzgvbn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2uccxxzop.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2yvevoqjx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2wunprihv.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2hlqynfny.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2dxctrzrt.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2xrgjwmpv.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2uhvpvyov.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2gyxkhoas.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2pabsawxv.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2mmcjhqfj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2nkeevtdi.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2lbdevceu.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ortwpryp.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2obkboozi.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2yzwwimme.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2kxyehwai.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2diqauyrc.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ururdalj.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2uukroeot.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wmdyjhrc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mydyuvjf.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2pupqnihs.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ybpbiabm.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wxezufxi.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2czgikwgj.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2vjmdhvme.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2rulaifdm.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2qfkyrlky.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2jktonxah.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2igfjhmao.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2sbqsktht.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2ksucbzxg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ddqumrgh.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2uqlntdgc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2qokafwcb.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2umxdibtp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2qqtivjwp.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2usufrjrf.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2iwcsgrhq.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2pspgcjnh.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2lzhywfvf.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2stukhvxx.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2mtduuvxm.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2aargjuqz.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2pbmqtztk.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2lylwugxw.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2tzeewrpn.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2oynuzles.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2oaztjwmn.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xmcnzsxb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vchyjqrc.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2wyuvxtgy.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2ocsaeffc.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2nueqjdjp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2uxnvefeb.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2msadxgqt.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2votsgxpy.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2hvfjsmfq.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2cyhubjru.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2tndqwsjj.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2tdatdfiq.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2obzofepj.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2reayyivv.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2xlahqklu.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2ghlquusn.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2doicpnkl.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ntkctsqj.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2mwikpjzv.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2aurbzyks.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jycrfduu.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2gjgwbzkx.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2uiyjqlkn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2rdfefmro.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2knxozppg.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ucdohctx.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2hmftfgah.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2blcqycbk.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tdphgjlz.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2pjwfywan.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2iikfjqgh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2pmqdbgfo.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2yyuahlnq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2fpmebukf.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2stwosqzc.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2wepjeirm.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2spzlhkvt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfgrmddh.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wloqpakl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2ubtrrfyi.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2bcilstyq.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ntsfuawi.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2sepjclbk.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2eyjwazat.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2rrrhvaib.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gyfvajuq.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ovmkkeqn.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2dwwqlols.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2deomjfaw.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2epqmzvrr.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nwztjqjo.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2sckogazz.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2qpmdtzbi.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2yarprpgm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2imusyfdf.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2vcgmzxqf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2rprtcxft.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2zweulkys.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2zjwyuqwz.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2zsjseshb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2tvuhlkky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iulwmvdx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cpcmhqgd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rbtyyyyi.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2nsrptkbi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2bstbfmow.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2sqqirogp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sqrnpgnp.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2qrapwpji.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2gaxefhnd.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2oaultepq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2yepoewby.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2xicnjqat.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ncljvddd.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2foekvbal.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2pdftvpuz.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2fjycxrhj.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2frgqrceq.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2xbqxoyau.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2whzbojkz.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2ubpdlvxl.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2wsnyqprv.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2xxwxrjrq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2idqujnwz.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2vpileabb.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2yzyzzkjs.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2azjkhnil.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2igaydiwk.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2kirrubul.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2tvqlshuo.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2hfpvlzfs.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2qvlimjeh.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2uegoiefj.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2yogznhgi.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2hiuvyarg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2hjwelnqd.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2yfyhtgtj.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2clkczqvb.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2zqwfeqoq.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2rloowlnn.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2aztnyujc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2puhcjyne.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2oqodfwoi.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2iijxjbrd.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2hkjorwlo.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2mxjdjsct.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2dbjgxvdk.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2ptuthfdb.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2oamgxgsd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2wyemzqry.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2nvisvvsy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ooqdwnkr.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2stmdqnfg.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2esdizjsa.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2vkxupwfn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2rmhpnnlw.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2eqzixrgm.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2qfvhngie.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2ljwbwszz.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2tjgamtrt.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2jhiwkxlj.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2gltymuzb.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2meqocrip.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2dtnnmogi.html


<!-- 参考信息 -->