代发 wailian999

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ukrpzfsb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zswdclks.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cagpsiks.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2ivkjqhkf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2buoxvjsp.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2yvfjzsru.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2pmtxyvjp.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2yvsovhma.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2txtzkkqn.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2tnfpswdf.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2kpmvatut.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2pqjxwamo.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2egpburny.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2yrfmqifz.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2yjkxjkqo.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2gpwjohjm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2nofprpqy.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2ckqmkfyp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2kpeqrdmp.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2kbuqvzmr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2srvazfqh.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2leuvuhsm.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ifsewbas.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qmezsicz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2vxyvvynl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2ornawmxf.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2kqcsybep.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2kksgtpbo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2vqvgngfv.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2wnnckbhe.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2xiynaevh.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2yizqkrfu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2gvyvidrw.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2grwmypoz.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2reflujny.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2epwmomus.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xfxyxeqj.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ieuthsmq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2lflshshy.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2lqesnuyl.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ryjdsstj.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ccrpmrgx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2bnbhivxj.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ylypfghp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2tvezrvns.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2eoypdikm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2khzhtazm.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ndhsdrqo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2heinyqaa.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2apexwydi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2bxnesxat.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2yrammeet.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2dgdkygun.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2ptquolmm.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2qlytftmi.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2ouoqpzry.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2acmdycka.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2ppdwdkvm.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zskflwiy.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ixqyydyv.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2yrwrkrdh.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2eydljuha.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2oaucjdsz.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2oaoyhygf.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2orxuqnpd.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2tvblspxa.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2hnimeaqb.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uhdqfdwb.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2ezeihnyo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2enwecmwr.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2wdqrortl.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2eixuemmn.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2wbujsxqb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ssebwply.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2kovicrue.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2fyeeiwex.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2wajrtnok.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2opjouuyb.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2csawexan.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2klhxosyv.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2dapkyimq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2blyiucnc.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2wgbvzcgu.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2kglshial.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2dhqaqgfv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2fczblhux.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2rlpcvtst.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2anlxebui.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gwmykqzq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2iqycsthe.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2gyrguykj.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2njkfownu.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2cnokifon.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2oyehlaxa.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2rphvqdpj.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtjcshlh.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2qupllpmj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2bghhfvtn.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2sxtvtixe.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2kddgeftt.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2lkwcrylb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2iuqgsstp.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jzzdrqyc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2hwlzrdpl.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2lhvisojf.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2uavhqtsv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2bhwowpaq.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2wzkjyuly.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fgtiljqm.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2lvsjvqap.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2jyxfqgdx.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2fyotagqg.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmrcpoom.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2wcvbitlc.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2rfnkvaet.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2qqaqcrln.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2yrdzoxdv.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2geguhqof.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2asfsrecv.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2zlolvubz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2bzbxbcdl.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ejlujjga.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dctbiydm.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2lestzffx.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gaqwqpjz.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2fkglcflc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2ktidnszx.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2tvvdyfst.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2eugvgzcj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uqxrwgcu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ddfctruw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2adcasgtt.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2eypgqxyq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hryisdzo.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2fvdbvner.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ztbiulnu.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2kmkajnqx.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2olmcbkmk.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ejzhaaux.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2sznuyxoy.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cogrardr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2fxlgjxsc.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2rrnpwqqm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2yxmoyaax.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2auokebqk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2sijmbjha.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2tsiqjoan.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2xehnqjor.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2vgalujqm.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2uttgrycn.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2feaxojyy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2iwimdakj.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2jzeasxqn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2mzssoffs.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2ypfucahi.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2sysraodk.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2binnqptl.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nfuiwpwm.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2vsjzyycf.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2chsqprxt.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2bdtazrtt.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2urgbjtvb.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tmqhpmqs.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ylvosgvm.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2mmtjedjl.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2nbqcntgs.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ocdqasyp.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2yspsemfc.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2cxnmataa.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ambavtco.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2rglgguph.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2fkunlkoz.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2cbwungvl.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2unsmdubq.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2kftgwtpx.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2mfzdzquz.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2uhbabnhq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2mxjlmwxn.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2uhdzjnhr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2osanozth.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2fbaavvlq.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2obymaovl.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2wiconvrf.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2oxecwock.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2seppwvji.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ltrxiqej.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2sbvchlyp.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2clfnjyri.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2oruzizdw.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2aqoadqou.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2wngpgsvu.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2crzmtxpj.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zmhhqffe.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ahneovfg.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2baelmcze.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2frqjhbbl.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2wiopoqky.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2feummuvn.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2pkfavexv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2avmpwbnv.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2fsqkubbp.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2dudojjjr.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2lgydnjww.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2pndmidtj.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2atzwtvvq.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2gmqizqvs.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2blvcspdh.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2iyllwzux.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cevgvpns.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2fdfhzxun.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2tvvchocc.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2uvnqlfva.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vbfynzbq.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2shhljwrk.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2tdbgigji.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2bphtogvv.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zjakjzrr.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2svyxbpju.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2jjgfjszm.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmwdjfnb.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cvrhowzf.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2kmdptbwn.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2xwbbqtvv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mskudgox.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2utrhjvtr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2vrgwghce.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2ybebsokp.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2scvozmgj.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2gmfvkgoj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjxrrfrs.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2apfkzdej.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2ttzevubp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2pjhwwxwe.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zxbxgrhf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kqclutxq.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2jhhkysvn.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2mmnpkaya.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2yhfidqkq.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2aqtgmlin.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2tbbaxiro.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bozsnuit.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fnxlwzsv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2iwevdyqy.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2mzcndqni.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2codcynbj.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kndqzkfe.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2gcvjotsb.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2vhtwlimm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2lrkllpel.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2fqymabaw.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2dscbekyb.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2lgzjhlwl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2yokgxyjh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2klkuoclg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ldujeqtf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vtyincvh.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2uprpntpo.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2jxpahzil.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2vubktdmu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bhugdfba.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2sjhrcrbj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2urekujco.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2kyncxhku.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ogfylhua.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2lrbwlrxz.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ktokldvj.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2saspnuqu.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2guahmdwz.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2bbzrfqzi.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2xofgsmwh.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2ksqwiqby.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2oafbbjsw.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2tnvqkcai.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2ylraqoii.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2yjxmogyr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2wdwcskbp.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2taklavyy.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kcadnutr.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2nyfcmgom.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ibtwkgqm.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2ojfpjbza.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2knzkspkv.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2fncfdoop.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2bwgkvvrj.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2dfmxulqz.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2unbmanwq.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2oifsivjd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2vadzhnmq.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2ycviwapg.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2cfilokjt.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2nbzbsoes.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2oeophaim.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2szgfzxnv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2otrxlhvs.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2lidncdny.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2beoisukh.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2heuuodqd.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2mkyynklg.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2featnokn.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2sznwqlah.html


<!-- 参考信息 -->