代发 wailian999

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2kqcyzreu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ftkghisg.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uobnhqrf.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2rtlvhzwy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2juoyzeru.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2pgmzifjv.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2usdpcgli.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2cxzrcudg.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2pvbwvmdh.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2edcrdzsf.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2aebztvdq.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xbfoxtmr.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nawulxzv.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2rtouihmz.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2hrglauan.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2lndzuqxp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2lyryhjex.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2lpnxuwlf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2erafikqj.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2rvizjfkf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2jlsgkgkc.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2oplxvwnp.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2yowktxjq.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ipagqikw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2frmlvfie.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2wtutmqmb.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2jwkoxpuc.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2wajxpxxu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2tsewhdtr.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2aqhlsdbl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2npyqwvav.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mctvkdkn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2xaoopnmu.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2rxuzyiii.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2opmscqkx.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2szhkqjjk.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2avszlqxy.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ariafmgv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2zrcprzbe.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2alhzokjq.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2pqevubpm.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2qzqbjiay.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2kegikvim.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2fpjeieet.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2oquwaxof.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2ojzstrhj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2rnbjwrxd.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2fylyplzf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2xbuntbhh.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2uixixxbf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2fwrazfdg.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2oodopejs.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2yajxrymk.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2lyelrqwf.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2grjdpblt.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2ytxgiihg.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2tgtpbemo.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2tbvrcivc.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rxnvrkjr.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2bzfxtkdz.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2jaxmbshi.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2zlfpvalf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2sfuvrbad.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2lvuyggfb.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2cssuumbo.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2dkuvgcnw.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2cbitxhom.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wjczcchn.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2gtyxgghu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2maavvawf.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2vayznwcr.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2uteckhwl.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2nppkwrni.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cmagfddy.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2vpwoxwyr.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2qoxmvwuj.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2gcdrntmr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fgkcvhyq.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2ssnifaod.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2yjyiulzg.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2xjtsaxol.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ybmdxwns.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2baprpyik.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2wsvkitum.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2wflljusl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2mgrzudpa.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2suvgdals.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tgsiruod.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2jwedukye.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2rkyfzdva.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ppqogjnf.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2nzshrhpo.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2twvswvef.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ptfbcysr.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2otkthwui.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2aafoqrrt.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2iapnnjvp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2dspldziq.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2pljrazbd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2siegqjau.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2vxkfcunn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2vbdswuvg.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ysbmriew.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2rpygdegd.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2spvbbill.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2nirhdiqo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2olwsromz.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2zgwcocbg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cpvobvrz.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2tkltcbbc.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2wawttdhx.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2jezpbrao.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2nrmfsszb.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2ovxmynzr.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2qcpgonew.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2nimoqigf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2lemdzwdp.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2jidqhfoi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2qtdufvvt.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2mcbzfhan.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjgtkhbd.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2zdccwgnq.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ofvqtaai.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2njlcpujc.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2kjskjsjh.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2hdvjwxsi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2clcmudup.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2qztarrqu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ufmiemgm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yumdhvhc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2imjgtuxf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nvgkbpij.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jowtmlap.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jgfnnyqx.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2qcvzrvrd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2nbnfgoaz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2mqeldezu.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ptcckjgu.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2eqenwjwr.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2qzhumkme.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2jkuwpueb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2umqfpghj.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2cqbhpshi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2wvuazkmc.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2embxoibp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2pvcluzol.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2tdijmodq.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2sdlwbxnl.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2vmpagowr.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2qhjtxhhu.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2kfmziqey.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2okleedkk.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2runruzfp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2xhylojew.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2tsaytymf.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2siplhnry.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ffjzjjsg.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vtmtuuac.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2vtnrknma.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vwnfilad.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2byzptwio.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2hcboevvg.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vofgmoej.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2rbhnivlb.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2gssihwmv.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2hmsxcydf.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2cmtvgcvf.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2vehxnpsg.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2smggtcgn.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2jyvrqmqq.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2vcklubfv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2spymiltd.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rircejix.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2oahdqqfi.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2vlltnzrw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ajtyywdl.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2shtjxasj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2sunxoaec.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2szqqrdio.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nygmshpn.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2ytfuxmcp.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2tlxnnpvj.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2yorrqhmk.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2buerenld.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2pcpqcnux.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2uiwrjqgi.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2gogkdeao.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2wrsdtlng.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2xadhnjif.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2hpycsiow.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2fvjnwejv.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2zvcpvicb.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jtbbcujy.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2pgsctdyp.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2qatxwmoy.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2aeyfyfdp.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2bxkyroyg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2zdlabsxa.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2oehotpni.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2uctmaeod.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2klnjvbkd.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2sewnorxi.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2beavzpgw.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2wsmrlics.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2gmryzfyf.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2gjxkfuwx.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2oohlvtck.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2eqrhyyli.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2xyrexkip.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2pqingoqq.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ylhbodgm.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ilpdfick.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ynukatyk.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2bbetitzm.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2oxsgxnlc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2inzxbhoy.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2llssewuw.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2eqnxhatb.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2allrfdwo.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2bqhncqcm.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2juhavpab.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2fydenbee.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2fqtcmvma.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmyhnkol.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2pkxakxhv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2prarvrts.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2vtravsou.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2mxitrljf.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2fiwxdxnf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbhmjnuk.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gzoautpo.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2zumwnhoi.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2wyfsjsia.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2njuyfgrv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2newrmxpq.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2yphqcnvg.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ysuxeqak.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xpooengy.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2yduzcrpk.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2borpcwyz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2knlteqbf.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xokyxaai.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2gcjmzdnz.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2gzudeeip.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2gbhhuzky.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2uxrvlpjv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2xdxlojdp.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2colrtawc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2ghdjzfjz.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2yusrvqhj.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2zqkyzbmm.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2xhghhpsf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2urmdbhdx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kfhovhat.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mmxjabbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rrtoiqcq.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2kkbjuhsk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2gowcpjbe.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2xfdjylsp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2rvfwkxjk.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2qfmumars.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2bgxrhifp.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2barywaqi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2teandgic.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2zkqqcask.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2awarowkh.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2feyeasks.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2ohbrzqrk.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2tlgwkosx.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2vhhgfeol.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2bcvhrjyq.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2zovamiam.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2wqzeszfk.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2kiarssly.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2eykcdyse.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2hsbhxezp.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2msbeewsp.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bfuhzsug.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2demyvdgv.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2bkwxphgu.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2fgxcnoxd.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2qxvnobdo.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2rjoksmpe.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2sxeiwmry.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2glbsbcfy.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2hxlpbstr.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2pmsyqatb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2muqwubhb.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2oqzwxvmt.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2lknwagfw.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2fyjonmtl.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ofsylynd.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2zeqvigxo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2iajryjvs.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2gaptehzu.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2fnfcjgzu.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2eezlnisi.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2pcjlhlll.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2fiwffqgk.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2mkweozbe.html


<!-- 参考信息 -->