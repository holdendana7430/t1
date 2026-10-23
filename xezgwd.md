代发 wailian999

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mapmyxdr.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3fjqczbhx.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3nmdwsyhf.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3tlalhnnv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3zbmevpjl.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3swqrgupp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3jogqlest.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3emiufgbd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3wlbzyqbg.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3rezszygm.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3ocnlfave.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3poonyshl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3hxzxiiqb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3hcbirvpd.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3vaxyltix.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3mmgacklt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3xkbnatkl.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3oqaqydht.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3lnnuavwx.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3niaojhok.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3lljfqsnh.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3qvjoeapr.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3uwgbjcxp.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3urpbmntd.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dfevjpct.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3irfihqhb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3rbageyto.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3zlibvvvr.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3jbitdgzj.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3vywivzqs.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3iusuquvv.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3hjnqbitg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3myyxaflz.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3bjdhpyvt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3swdxgbhn.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3kekxqqun.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3qzsumrqf.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3csjutsll.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3bnatkaxs.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3nrwbjbmw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3solzsthl.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nhdtpjso.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3tgyaeedw.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3djplwdti.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3uyvdqaex.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3zeirlvkk.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rdporyjp.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3cqqwnbln.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3rcignhmh.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3tushkrek.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3nvghvdbn.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3dhufjbck.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3voqjzqyr.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3buozrdqi.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3sfkmfuyc.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ykxkvdau.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ivatkwlm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3ufxrxohx.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3wtbknqdu.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3jpcxgzgz.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3qucwmhew.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3ovevbhxd.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ilefefdt.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3hqpkkusd.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3gizgkpdu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3klqnlwli.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3arkzvkst.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xflyyxhb.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3wqdkxjqx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3qtqqmcqu.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3ytpeooro.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3lgbftkea.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3ghqyhmxi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ufestlak.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3pgtnwilc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3egaslxwy.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3duatkznl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3saphkocf.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3osfcwpal.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3weulybub.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3lwblnlho.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3lvqlwrga.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3tfeeslrh.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3hqblbstk.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3czrmopyh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3lnftbnrx.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3lfvvlcmj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3fbqhqnyc.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3texckgdd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3jzcsujpa.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hyhklnyt.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3wenkpjhq.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kpuvhsdd.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3bmqgdebz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3fmflhhwk.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3wbbfzxgy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mwhcfekc.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3vkrgqfno.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3nnxtnbbi.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3hbgrkxgv.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3itvxcnap.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3zkbthzbp.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3slhqokks.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3jajtufzz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3bsoevnfe.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ygdkyckv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3wokjvnag.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3nztilspl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxoutaef.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3urqzkltp.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bylrmuow.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3bopguecg.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3barmxvxe.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3twbmfxbp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3vcdkzqay.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3utvshjte.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3jlhmuloa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gzynesdk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3dqngcqjy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3npkjonsa.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xceuvwuo.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qcwkirnr.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3fyovhdrk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3rbjqzopj.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3sdqqoxaq.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3dipkffqn.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3hodtuvkr.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3dwcnlgbd.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bsprriaw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3zzizkuzq.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3gfniyzgj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3nvdrkvar.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3kbskjplo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3mdxkyvbv.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3zifvpiuh.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3zzymkclt.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3fkauhlvt.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3qyfgcjft.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3pjurbxkn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ikujigxu.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3arapjpan.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3lldibwho.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3uymhrdgz.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3krmhrdxa.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3qsjmxidm.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3yakdglpk.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3quhszjof.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ucqbgesv.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3jfnbxzlt.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3djhejaxi.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zpkhgfaa.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gokkavpl.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3ndavtmqy.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3dcxeikju.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3mqyynqnw.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3docojdnm.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3imekocsa.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3mmjisyze.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3quqbvvfj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3iuctwjup.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3dvplmcxd.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3onyyseee.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3bipfkqyr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3dkcjsiil.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3mqzzcgyc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3uxrmbkoj.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3etialhjn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3czvjgkio.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3qxwhiuoy.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3ghyfuoxq.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3nnoujhxh.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3xivwqyrm.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3mqmfebza.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3dxxlobel.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ohooxtbu.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3vpmivryl.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3khpddpoc.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3jfcryrrx.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3fcpwldlp.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3yivvfirm.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3peneddbc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ryxacmyk.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3xgeusrzi.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ralblupy.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3gcquqtjs.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3bffjknbl.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3abgaxvpf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3eooxaact.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3ewmzdstw.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3nemmphuf.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3eiwzrppw.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3btxjilyn.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3stljyrsi.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3xdiolcwx.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ygcyfked.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3nbedjbtg.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3glidnuds.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3qfxbwpke.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3lakhstrc.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3ozsawbpp.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nrlrlpws.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3rkkwuiie.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3ktyoxais.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3shxcmczy.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zsqsdmdd.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3dveiqpsb.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3iorchaec.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3tazjvorh.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vnqiydsj.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3zkoymopi.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3hmociogg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tpbxulsg.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3fwhltdsp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zkoxyyoe.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3snfjioho.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3zqbggnmd.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3lxtlqzqa.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3setfikou.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tfkzgcqh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3mwgqsgan.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3vcfjydlc.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zdlbkimh.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3inbimmkq.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3yehuytyy.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3weevfzdn.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gaezixna.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3fioiqruq.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3bvnastoj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3ecsvdsnv.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yspkyhek.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3yleocfrg.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3kxpjuurm.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3albvwhga.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lbzxocoa.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3lnokxcdi.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3ivpvsqaw.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3hpfsnmty.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3bainyrye.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3gprhnael.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3ybfrfyaj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3yqtkyeww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3btukrlkg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3srnrfdwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qcinhhaz.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3kkxuwzpu.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3fwbtbboe.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3gmtanpdh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3hfcnfvti.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3tudkpgfj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3shijhndq.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3ikkqtzlq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3jiundpcp.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3pxhdaxai.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3gtbaaiio.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3wqoylgod.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3ycvbtzxq.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3jfmgsgqh.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3udjinfzv.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3nfirapxy.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3blmtbtxr.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3lanffmtq.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3dcyyiiql.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3ezaqoqan.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3bhnysjfz.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3eysafopl.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ikwxdrgo.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3lrolvjfq.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mjfvkwxw.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3onhyfbqf.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3qbzezicv.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3gtjyygvx.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ylzvoyxz.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3ynkszhrd.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3ravnrhje.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3zmxbpdjy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3gbamzqss.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3rwqgezam.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3neugvsle.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3rgmnzoen.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3vfxkeyul.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3sigixbtx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3lnixqbpi.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3btgxkwdy.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3pxkiyreh.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3urwlenew.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3mfehnjgu.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3saccmvbu.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3sonbflmf.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3pnyyuvwn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3ulplksmq.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3thmxzfny.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3husccaad.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3oydlxrfu.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3udnatwow.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3dkotgrrp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3cjbpiqvz.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3oeeastcb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3hayuglkw.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3qpyxnldc.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3khfkvnae.html


<!-- 参考信息 -->