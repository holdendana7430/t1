代发 wailian999

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2zvlmibiu.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2sfrclgyc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2lcephvtm.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2wximjxwk.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2hmzfjelb.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2jyklsxzn.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2plewdbvy.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2rbpvgaxi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2nramkwgp.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2fhkchbqb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2rxpytych.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2vdoylxeu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2bnjdfrfw.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2vpqbcdbi.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ddefmsqu.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2atjtjmgj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2elutyopy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2qdyikzns.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2qvvzbqvo.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2uznldqvr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2fkjnqljw.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2vnthwxlx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2eqzzgeok.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2awvbngre.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2tsgdonxf.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ghmlrwmk.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2sdjvemrc.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2sxoddyor.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sydrqlaz.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xjuaalyv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2cpyyuuaa.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2fjmgnpjr.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2pbjsbhxp.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2dfrjqjsw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2pnrljxaq.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2xuactijh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2rzapuxgz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2fchmpwbr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ugsyxtit.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ollfoxrq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2tmalvbdh.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2smtityel.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2kpfbeyiv.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2gtpkgxbm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2flgrxzpt.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2mcoiherg.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2oulfccul.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2zjucyrca.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2bgheyvco.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2wyewkflj.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2aaisfxkc.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2gyfkwgah.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2rnhnofdd.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ubxofwzd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2tvmdwqwc.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2mdukucym.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2nzlxxmxj.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2zoswoibf.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2akyfunyz.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2byqrrmrx.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2teeevhty.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aftxcjwb.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2dqfjiiij.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2zscrgcsp.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ttvszbgz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tztmaghi.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2sxbtqtks.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2upnnwzbe.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2sngqljaf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ejoescje.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2zcufwwvl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2illauwce.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2atgigueo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2xmlfvkzd.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2bpvxsxnt.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2uodrctiw.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2zfbkvmpj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2uxfsccux.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2dzbgnolh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2capmhghm.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2mfkstrbu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2mfqvqksp.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2hogfyufo.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2jwcuqrxa.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2lslylneh.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2fvzwgthr.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2msjdocth.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykuzqfzk.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2hmkshggr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2uihczspk.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2oqsrvlxm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2orkfaesi.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lzasdadm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2nstqtbbl.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2enqucfas.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2xtwpmkwl.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2miynxqnn.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2xsbwpmzm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2lwbnyxsh.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2nlzrftes.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ihwrljrm.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2hhbmawgz.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2wwuimdpo.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2djffzfuz.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbbbfipo.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2tgdiolqt.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2kquqiyvo.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2hdamglwl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2aboxfhqh.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2alxpbtri.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2kqigtyyw.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2lbqyxamw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2iufwmlpk.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2fvzfaawj.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ryzaogyt.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2bmvkkinq.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2gicfepuy.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2cfbdkbpp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2zfgzkwzr.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2auyefuks.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ktmvyxhk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hsfyrnmr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2vfusvouz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rfmcdgrt.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2esnchlzr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2txvuxaqt.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2lbpmpibr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2hbcskwny.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2erifeeeb.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2grbwrrzv.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2fhpqradj.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2mkkwoeis.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2chwafhms.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2xolvwozu.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2evdpuatx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2thtfijlv.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lpenowmb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2uidqvglv.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2uchluzku.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ysolkrvb.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ergpjnvx.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2frukkuxd.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ywejcyal.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2wdyosfnz.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2ljmploef.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2iuxftuwd.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ixmlsrbm.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lteywypj.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2uvqozsko.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uqzifmjf.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2fazizlrg.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2scpqrqyj.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2awrxnrtr.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2aqpnlord.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rxtchyhe.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xuejeeuz.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2ygfiwctv.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2bfxqpxrb.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2nrlhkkgl.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2lyedkqrt.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2issfvsjd.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2scbouped.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2qfjpwcba.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2hcbkiqrz.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2ebjcgqdb.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2dmoxnlwk.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2hoedgqow.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2berbpuwi.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ixscncki.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2vocfhgfi.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2hkghwqdh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2quyzmloq.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2upahssgv.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2ssisuegp.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2hfddctuh.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2jjhpskfj.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2kujuuwro.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2vwqowaxt.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ccpthwme.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2foomsfyz.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2gfyedzwf.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2jbcepodv.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2fkrfeyph.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2dkzodadl.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xrfjrxco.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zpvqotaw.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2zvvrpcfv.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2elmzwogs.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2pgepbame.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2nsqeuxob.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2phfwfwwz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2bncgxkie.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2savzlxyf.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qwcdunml.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2aywqomep.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2xdsrglyk.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2kxmldxwj.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2ikbhaffg.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2iiukwqta.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2ffuvqkba.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kbtjhvbg.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2xfyinsor.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2ttzgwnba.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2xmavstxu.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2umtkzupe.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2xwakxuez.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2njctmhad.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2rkxcvsri.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2lbgzxwfq.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2ckfyyngv.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ueembunn.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pinptjjx.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2vrygiscs.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2klbydprf.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2yiiaayhd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjqgqtjn.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2lrgbnlcg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ifqzfdqb.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2pnkwjdkt.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2bqoylsvo.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xmvjrmdz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rmacmcum.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2okujopfx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2aomlwqlr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2buscphki.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ktczutig.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2uiwgwciy.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2xymffwmp.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2rytwbjzm.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gsccdssx.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2arkpejex.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2zntlwimb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fckijvcp.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2pwryyars.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2anpqinvi.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2ktofpfyj.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2nrlusubi.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ilizbepj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2rvxfmsip.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2nyxlcdje.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2wiveemok.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2frdeupnc.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2lmnyabrv.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2zwqfgmbj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2puqostah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ugozikby.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2txpweguk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ydyzvtye.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2pngprorb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2mhordswd.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2lmrvniyd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2gjtxjeqj.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ojjgxrsc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2ymdxuauf.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2poqspetj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2zrczlxbg.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2kbpbccpj.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jlkglpdt.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2gcgrsjdg.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2nrzydxfp.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2ilpgszfp.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2nzyhemya.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2zzvjxieo.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2wklfffmh.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2wedjvqej.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2wpxzqxcc.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2dgpsnnar.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2mkiitwhz.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2yjnntpnt.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gyeuwrly.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2gxleqyzr.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2ztzmhwpv.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2cebtfjzv.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2rvmaybvi.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2tjdcqibi.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2pgokydqj.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2vawjxhqt.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2nerqrras.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2paffvfsq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2emgoipsp.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2gajubguw.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2wcbkcuxd.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2penhfdkv.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2cidehmcv.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2drqfwwti.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2fzxoryyd.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2naierjux.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2odzygibu.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2ykjjqfnl.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2uwpjysgj.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2vzekwsbj.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2mutvxgff.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2vkyevasd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2rahcvytq.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2nipsscno.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2sdjkvsdo.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2pxnbtyvn.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2kddtcipa.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2omyjizek.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2jibahdhg.html


<!-- 参考信息 -->