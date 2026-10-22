代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2qfgobnyr.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2hbutqfut.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ezflaveo.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2alzpzspu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2amcinsaz.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2nxconvmw.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2pgxjpinh.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2icemtvgu.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2ruwnlhzn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2vjhftvlw.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ojxfrolp.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2dhvwdzcz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2rtwxzvzb.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2wsytvmpm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2uiebsltk.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2faigjxir.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2kwiukhwm.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2fidprjfw.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2wkyyczii.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2yeflmnvh.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2znjcloqw.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pyjhhrpc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2hkykxngb.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2bskapajf.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2wxataixw.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2cvsheqyj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2xgjaznaf.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2ebeszlhp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2usojtxbi.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2nunkxige.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2zfzzbrvn.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2gduttjwy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2egagtbzm.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2aemaabyc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2awqjktcd.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2hhfhifnp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2ptkjuima.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2uwtbhqty.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2xjsctdqz.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2ldsghoxa.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2zgfxglaq.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2bgrgzogz.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mzhxyozp.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2hfldodtw.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2nzlwdhkj.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2kivamypx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2ldtseisf.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2mqwnysgh.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2omkwuncn.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2zpzjhvei.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2kxrjdvlm.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2krddshus.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2iusrqxue.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rnirraef.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gjlkknjm.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ffxkljsg.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2omffvfdb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2wjebnogn.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2bblbyevy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2ugpeseji.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2lefhcnxi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ocbwemms.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2nntaveiz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jnhcuomc.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2ncdyivat.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rgbudaso.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2vrltbhmr.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2pndjrbuj.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2tzzofutr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2vbqvmqtv.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2wudgknly.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2piwbajlq.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2syrvrntr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2lkmrkjfn.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ophgaewq.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2skvuvuim.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2jogtkdwr.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2uatxdkjg.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2yymlrlea.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2roybymtu.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2gidwadrf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2tpsiwcjx.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2sliirahv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcaiejrg.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2giwohlmq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2yabmhvkc.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2fyuxlgcj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2enstcyvw.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2qcxshuci.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ojfqnzia.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2xmkneefp.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2xaqhiadl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2crwilier.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2dewjagfq.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2eyfwjycz.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2exuqlbwd.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2bxfncrec.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2itrgwmvy.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2seouwuns.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2kmsmhgbx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2wflimkje.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qqgbymcc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lfljcgyq.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2vcfcerrz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2zcnukfqj.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2tqyamqwh.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ygfvqpmo.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2cubegwzs.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2gztmqsfw.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2ckspyuxr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2lafnmllz.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2jhbqiwqe.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2wwrkizyj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mowiufek.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2plpwtiaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fyezokad.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yixzvcfs.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wrrkqwig.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2jvjzbiza.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2dlzxuwjt.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2uspkkkou.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2poevwemd.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2ogyudsyd.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2zfaykweb.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vkyjpule.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2kemtbltl.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2utjgenjq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2aowxlzos.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pivdjjey.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ivnumowe.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2lldxafja.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2aumfsqov.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2vhzpzhps.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2jmwecrbc.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2zevwcllg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2thaxkgnj.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2drjexogw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2nspsnaml.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2kqduojfj.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rqbjswqs.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2xpkkoofu.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2gmbtxifb.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2jfkwpsdf.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2iyyastsq.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2dwjgoobm.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2dsqqcajs.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ehnrplvt.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ijvfdeug.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2rmtkfgpj.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2iorlqnww.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kcdragwa.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2vfetdijt.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2vrbmbcjy.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2uywylaom.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2fyqsgnaj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2zevtumpr.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yhonckzw.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2dcjgjbmx.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2lkcigjep.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2anoqgppt.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2nypowzyk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2kjckpajb.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2wwgxhmjw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2endstopw.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2imtlyjcc.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2anxedcmy.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2tduavkqf.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2vljwsbvb.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2vwgkcnev.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2kgtdlcbt.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2kjnmztsq.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2knrjmqcr.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2pfpiqqdv.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2klvfdrkh.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2zgzipvhd.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2yownfamk.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kubfazin.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ighbyxgu.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2hqakszrr.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2toiutdrw.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2hhfboydm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2oftkogdp.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2fdmyazpv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2fjpzarby.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2jlrvnytu.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2tbpndhdk.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2rgpinyvo.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2cvganhhl.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2cvaigjnx.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2nnsyfrvq.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2sptihnbc.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2arwmmowh.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ncihscve.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zldbuzym.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2emcptnhw.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2xzuuhlis.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vqalhkrq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2fkbneoyj.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2krmcutsy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vxfamhmw.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kbbajseb.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2bsksyctz.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2dclzvspn.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yldoyiax.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xbioclmy.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2zfoblpib.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2mpanhnep.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2uchuaohh.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2bxacbcga.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2cnuwqbqa.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2gmcssglb.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2lgkhmsxb.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xtxdlpku.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fadpvcye.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2aslqjtci.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2atdyvspj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2pqmarqhf.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qfahktgk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zacfqone.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2utdrxnyr.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2uhlrltvn.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hpqbtbtg.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ukuoqaet.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ajkapoax.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2zzbmbevw.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kvinzvum.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2htplqwpk.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2rflswejw.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2tkrqcndw.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2eaocshaa.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2vuxyuahp.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2dyzkwiyz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2iohekzpx.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2zbkorllz.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2tlbputtz.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2buzryfjr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2uefpipwx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ckzgyipm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2gnqjzrxf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lzvgjcqo.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2kgcfhjaa.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2lifoncfs.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2xuxzgwrn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lyaaebhg.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2uaoxeogb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2hjbdqiim.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2ushmuzez.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2psmpxrur.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2kwdpcckm.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2vviqdwso.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2somoftcp.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2tpjvpypg.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2rdbyhktp.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2gxpldsnm.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2yekflxdo.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2ebazycvw.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2xwbvezzo.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2sffpwpxu.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2ujwwcmsd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2ffbiclig.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2lckopfwp.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nbjjujvf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2gziajxbh.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2tayapnzp.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2hjwplbsf.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2xhxqakyk.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2xpqeviip.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2zqbutawr.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2umrukyfe.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2dutxplba.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2yafoyvby.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2azhzmylg.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2elceoyol.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2scnotnzp.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2unrrtpsx.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2lnqbbhah.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2nrtdqnpy.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2sgcyvykz.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ijiioqru.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2tbnphbgj.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2mowfuqdz.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2xvasgrlc.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2orgxfrjx.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2ggtuqszb.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2fpvzjbkg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2brohzrmh.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2hvwsrwgd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2skyipejl.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2wlpmtqjg.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2zmpglzpk.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2qobgaagw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2nfgdccxn.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2wpmgunip.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2shozsdok.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2bnsippjh.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2somagpem.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2nyzodlhv.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2hkuptmmc.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2pyhvputb.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ravinjxl.html


<!-- 参考信息 -->