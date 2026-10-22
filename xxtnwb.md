代发 wailian999

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2wslrhkbi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ygasevsg.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rgzlzilz.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2vtipgdhn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2bnfitnhh.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2iqhhpfxs.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2uphxlfnr.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2dswjkamp.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2yyxstsbn.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2seafriid.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2kpqplyux.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2hfnoxrcy.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pbqgkbyv.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2cikqcgby.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2fhfqxyjh.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2adbbfbzn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2dmyalhcb.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2suspknvc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2lpyvgiif.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2vchjxwcc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2rhtktwqw.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2gwrcgogh.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2hroyqxpn.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tzhmovee.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2spxhjvkx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2izpsftwc.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2thsmetdx.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2kyrcnnzi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2eycwmmxu.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2nzfxyxhn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2litcyckw.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2rwchcnyw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2fbsvuszs.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2lrvcqxhf.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2ixrzxxsc.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2vnmthegw.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rbymfdog.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2aeuhcqso.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2pbbgtwdn.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ugleydgi.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2xdwdwrgc.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2mdpwxtxm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bmbmjlhz.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2ybrhwxqp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2eqnrjrlf.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ptbtdfnb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ogtkjcvw.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2lvndcafm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2izqwmqls.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2myxadorj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2ftrchbcf.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2buhorjzt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2dxyzlzaa.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xpvduskr.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2dzcwzxwg.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2wjzsazva.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2jekteuij.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2jwloafma.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dxrbudta.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2lxqfobyv.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2murewzse.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2olqnnfkd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2vmnrlpmq.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2viixqvvu.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2okgedukl.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2yvqsacgv.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2ehteynpn.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2oxmlfcjs.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2kczsdqzl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rzjknhvn.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2hfhsvxir.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2nzyvhptg.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2lljhsfzj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2brozuxus.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2iosvoekc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmrqmtps.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2chfaofrn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dudkdjeq.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2gsteaxwm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2txppvdhp.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2tzrnyqij.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kzvzgbgu.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2jbhftepf.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2cbqzzxor.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ondjzowq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ibsbcbon.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2vvcoiqtz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cmxedpyu.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2dwmjzify.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2fwfzvosl.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2zctpmjls.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2bzlrsekn.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2dzofuago.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2vprnlipi.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2mztiymsm.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2cllcyiih.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2zvksymdk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2lbbuedhj.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2vkwszzwf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2nnkoqpeg.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ubnhazch.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2fibhrxar.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mgmcsqnx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2bhnalguc.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2wttrdzyg.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2mfaaxzcx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2wkbgskne.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2ewchkvdl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ajpleukx.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2liripyyq.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2otkysbsp.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2tpnniuog.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2dlixxbcd.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2addqyjhl.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2htjegilq.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2jttpkgdd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2jypsnjva.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qbmlqpxw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2foqgqcar.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2huwvfayr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2kawqzxmy.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2qobkgukg.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2aixanpdt.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2rbpklwhy.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2kugvcktj.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2qadtgzgn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2cmqypehl.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2smnshcbo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2otjvxgsm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qnwhtylb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2xdsdjiba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ytqlhwqp.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uprvryme.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2sbzxozse.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2wpwtuujw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2fvvcphga.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2fgmjmvwr.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ygtyjxls.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ctxbbiwm.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2fnzzsdvj.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zfxcudxd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2wbpkndok.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2zparwxzl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pfjhgsbj.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wgflufif.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2hnbsojzp.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2uasabpes.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2eoxzkhcx.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2cbxgvcgv.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2qiyplydc.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2zhxnuqft.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ykqeapjk.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2xqtzhbyg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2kxljepqp.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2attoenua.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bgpxxpos.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2nznxuanh.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dpwwyyie.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2qlentzlo.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vtxyxdys.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2sablcyvn.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2tkiqwkyd.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hcshgdnd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2frvrfbei.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2pywsiyrm.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2jrhxxwzr.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ierusvbt.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2hoduklqs.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qpudgzyk.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2reqyzicr.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2waniatdf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2vcffmyam.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2wadzkogm.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2hrvyjrbq.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2mrmutuie.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2iahpbbrc.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2quiorjec.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2kiraenov.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ratqgovo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2camwyegj.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2fihaldvv.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2mlppjcnz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2uoritqcf.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2djytazwp.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2qvfbhypx.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2vfanqlip.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2gquchhhd.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2tzsstxal.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2qnwyaktf.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2jknuvkyh.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2oyzwniuc.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2mksvpipo.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mtrkugjt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2bdnhswwa.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2djrlkcle.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2unwynecy.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2xaniutdm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2mvnpxtfn.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2obhpcssa.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2bruivstm.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2fqcqtlat.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2grrtqwgw.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wkkykkpv.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2aabodwhv.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ipwxkups.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2npjcfyol.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2vwkimpmr.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2iaztclqp.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2sgnqagbf.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2nvpbdqhg.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2mgkpxqjb.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2qxzktesx.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zugkyujw.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2zcvcmlsp.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2knhwuwao.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2zfelajep.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qegedglz.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2yzaqqlbq.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2scolhfyf.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjygaoud.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uxfrtqsi.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2acncvcyq.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2bmuushof.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfgsxpsz.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2uzzfrmoh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmlirvix.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2bscflpip.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2kmbpoqba.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2mnojrgvx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kubabezc.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mpjbaddg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2xubtkauv.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2djaersrt.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bfqeqdqx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2cxmjyzye.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2wybttzoo.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2mmxbznsm.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2yjghgzdj.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2vbnohdwp.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2oorakctd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2tzjykbqj.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2hpylmwev.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2uambpvzs.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2ushlymzi.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2gquaezug.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2gvdicknx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2zkwtiqwz.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2pkjwdinr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2tawztyrk.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2pkkxfjvd.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2hgqztnre.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2wkrrylpx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2jbvkxidr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2crfixegt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2gfiiwmlu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jpcglksv.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2hqtkilxd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2mcettvkc.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2vrpmudkb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2drsujpru.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2mpdxeeia.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2xhtvvokj.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2yfidymqa.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2kitngenr.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2tternmuy.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gpgvpscw.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2nkhtzfgj.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2vaddewpq.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2bohpjfrx.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2qwcqbkwn.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2fdfkjxbc.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2kumnebdy.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2uzaczpmf.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2zgsmfblq.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2ojrscsbs.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2cpzlwjwz.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2kphmicse.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sswbwzwu.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2gmezifuo.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2ujjrxbil.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2zpzyclci.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2giyurajz.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2tnhbbfka.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2annyvhdw.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2nkobjpge.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2pawylgwo.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2tibuxrhy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2gyvfulsj.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2iifgontu.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2oodtpcma.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2bwyupucm.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ygynomho.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2pluzdzxh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2uoxetkpm.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2uwuvldei.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2ajpllqxt.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2aprzjgew.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2zmornqqd.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2mrnqwphu.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2dkppblma.html


<!-- 参考信息 -->