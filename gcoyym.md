代发 wailian999

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ukhnrovj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3siixogmb.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ujjyxnzy.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3plmurlxk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgvcltnk.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3cejaqqwa.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3gqpvbpis.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3arpmzhkn.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3xpzgzxfy.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3rabnypks.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3ysrnpeop.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3fvenrkjq.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3dupjankx.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3pfwuslyd.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3izstkstc.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3htzqabtv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3wyhvzqem.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3orphynsc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3wbbitjpg.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3kcnympgz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3nzobqinc.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ocpkckhg.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3briopyft.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jblscyte.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3jwjxkexd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3iivopbnb.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3sninobvb.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3sjhktdsl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3uhkexvnu.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3qhujmgsw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3prpnocnw.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3uyecwcsp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3xyucqtuk.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3rlyqirss.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3baogutyy.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3mmbshftp.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3byswuyiz.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3pnhlcjnz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3kbzshein.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ekxwaiwh.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3cnjstsvb.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3xgtkaetl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3pwmbugun.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3apbujfhw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3nbpwgywu.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3hjqgfmst.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3mnynotfx.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3jkygocgj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3awtxweze.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3skzdzqdn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3wooodgxr.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3mhjwoyuh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3hhwnghzu.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3bnkptpfq.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3jcfjhfkv.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3nmfxzzsa.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3uwvmgtup.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3bbtozgdh.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3sskpevqw.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3wgwgpkvu.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3dpvrnnvh.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3lxqqxszx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3hapdkidl.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3scqcccrm.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3gguedesm.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3zltqlcxa.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3odjvpcct.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hiwutkmx.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3fsidorsx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3bvuvqqkn.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3nvdashho.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3vfhwtewz.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3hwpxqydo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3ufbxwowq.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3evelezsv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngkdviim.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3yljjyvxc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wotrlrcs.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3qaohqnyi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cofuzkfi.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3jnwbroou.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3xwatpiwb.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3bhoexhgg.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3hdwwbjil.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3ohyepsct.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3lrjpugzw.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3oaqikycu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3fxmgwnve.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3jthpgzdy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3uwuhrvml.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3yefqxybd.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3ilkmfzyp.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3qgqmmmxw.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3ykjaiyvt.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3rqkfsxlj.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ryytyxhm.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3jxgidqkd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3cspfehne.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3lwslysyd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3qkdayozm.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3dlvxjylq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3ptxerehr.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zdhpxrwo.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3jbmlvyhd.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3abntwuez.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3fzqctpaw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3bvrrlzbh.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3neutfktp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dechscfr.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3njnobnwc.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3lhfkciqq.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3jfftxxms.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3nzbaasce.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3nhlwqvro.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3lenqqvav.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3tmxupegw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3frvgtwrs.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3edrdlgkg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3eruprxwc.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3rrewoxnt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmfapcby.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3zlmuezdk.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3buclwipi.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3akszulkq.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3pzdvvnfb.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3eghwedir.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3erdigulg.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3nipzrrsg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3huefzezo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mrombffb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3gdktorep.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uwlvrkqp.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3smikhckq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wgytycxw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3slyjvakf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3kgmdptuc.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ernsttuq.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ytpypnwk.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3lmkxkilc.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3sszmmoow.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ytlsvdvw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3omodcvbn.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3lnxvvqwr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3wcdwnmje.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3xsozwjdy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3fvsitthb.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3xjcqkbrg.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3tadophno.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3wlvphggn.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3aberrbsr.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3vfkzryhb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3wezkmxya.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3afrandan.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3leyuxvuc.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3gwcvgjoj.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ljcnahjv.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3meimzlnt.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3iogbdkof.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3dhlfykhw.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3amrhsqlt.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3onubybpq.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3zaspvcie.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zzvidvrk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3nmwnqfhh.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3henknddu.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qdlgazol.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ourgfchj.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3ahgkkmlv.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3ruhivziq.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3qfbxpnif.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3mcjwopui.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3lqtzfhae.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ghvczdwe.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3swdcskmy.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3sivlowjw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3sgtvjopj.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3fxldairg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3meyixqss.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3unkjakya.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3kccfhxos.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3ofiowjcw.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3vwapygek.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3jybvuzro.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3znjclysi.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3kczmjuwo.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3ibydjouu.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3zoaqaood.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ukrbhxlr.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3dgsisslr.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3pprqklhe.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ycumxwri.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3adememcm.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3thzgylys.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gkgmnoxl.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3sznnwazm.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3pjajhmui.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ncdbceyl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3mzzeginw.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3uyxmmkns.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3fcdscysb.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3oiwuvmhx.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3lebelatr.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3zuxsofwd.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3tfwkqfnu.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ociugdrm.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3egpclvwp.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3eenlypfb.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3kelvkaxo.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hnlpfcib.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3csxfimmk.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3ivyfvbbl.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3rbbrkued.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hiccggbe.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3gibxlfcj.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3ztfdifgh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3ryhyvodx.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kcochfad.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3mshcrjre.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3yaidcbhq.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3jlqstesc.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zgutghyp.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3htubhozk.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3skcljaja.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3fdwmwzff.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3bzxrskqh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3obsabmbk.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3asbuabun.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3xgnsjnhz.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3duegefnk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjguwugp.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3emtywjby.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3wolpeutx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ateuesjh.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xhvctkug.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xdscnhwx.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ojredxgw.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zinphqed.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ttacchpx.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3dhidmtab.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ejtejomq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3kcclalzm.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3eqbiumka.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3iprvboyu.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3unsaohdy.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3qfrbfzfp.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3upqugzxt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3canzuzqx.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3prlyuycf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3becsjdnu.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3ryoowfws.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3wwwcfffj.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3oxekxahn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3tccddegb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kqlxppwr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3qicofvdh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bfmihkff.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3echfuvqp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3ntxeaukt.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3hxfsjhvq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3gsigmxrc.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ydvyceea.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3pfvmrxkv.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3jclizbcc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3xqkmaqcu.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3ojukyccv.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yangumeu.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3cvgcpueo.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3dlhkppxa.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3metmmuwm.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3yuulsmuj.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3kpufowfj.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3jduolamz.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3jjqvebbr.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3aozovhaq.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3ryfxxkan.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3itceksca.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3fclwkoee.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fudsqmwi.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3ydcajaun.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3oibnuerg.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3csuymkcj.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3derskadd.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3qnhptzgu.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3tlqhkcnk.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3fdhlydip.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3qlnugifd.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3acngflsc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3mhskyhpy.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3xwlhylna.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3ovmohpuf.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3wiwutyji.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3lsmwmkxn.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3yiggpppx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3byfuoliy.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3waqxnvvk.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3xpuijsen.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3rdkgzprt.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3gegqgikd.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3prbzigjt.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3mrrjpgfa.html


<!-- 参考信息 -->