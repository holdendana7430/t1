代发 wailian999

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2jsumawkh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dsqjlnmx.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kpaynnez.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2uftaxomc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfkfvaoc.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2slntozix.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2hzeaximl.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2mqjigeai.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2wjukdcjp.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2xomfjjjd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2szlddjty.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2enpffdfu.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bclcwwdh.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2fwrwegpz.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2xhpgdedf.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2hrljosci.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2wjjfnyux.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2xokughkd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2wmqsgmjh.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2lcjvbowd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2bnqhecru.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2twkryalv.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2zmxcvxzh.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dwhgoxai.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2glcnouff.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2uualpgsm.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2gfnqczmz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2drgjdsxo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2dlggsadk.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2xmksspsu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2osrtbrih.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xyxspzou.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2txunpcxf.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2tpplilky.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2gezbvkgs.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2cctcovsi.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gazpweai.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xeczajgf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2rfjhpltv.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2rqdghfgn.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2aspmoyzm.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2nktsusbb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2arlpyumb.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2tzbmlqqw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2rlzfbxdb.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2ydhzseol.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2aqaterek.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2tdckirxw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2dwdogcyx.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2tslerxod.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2skealxtf.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2mzjznbrw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2tbjysjzu.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xuctvnjt.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2vqkcpwof.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2yadhsoxc.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2idhxxmiy.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2braftlop.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qtruzfap.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2uxzkgnvj.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2rspjygys.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2nyquxtug.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2owpcwvye.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2cgnttlat.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ymajdyjp.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2kwmsetfm.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2apiqntwr.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mosnoomd.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2fyqejsex.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ggpzfgnx.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2ilcyvznt.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ogycgjpm.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2syacyfmu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qfqqxpft.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2rqbkjtus.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2hzujogvr.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2litixhhg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2yhdsmkoh.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2cjtesejn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hcflltbb.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2euqxafhy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2lljdvost.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2itnungrk.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2eoflpkcy.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2lqlvpvts.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2deusajwe.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2dlmnnusr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2frrgwafp.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2qoneituk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2gdaoksnr.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2awzewnrc.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2sfrdnkzx.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2garkkoni.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2tevvmgpr.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2sammzgtw.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2qswoslrh.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2xjbedzyj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2bnjrzusb.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2osjgcetm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqyoqigd.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2imruxjpc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2rlqvjfhj.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2bbqpbexs.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2vxixyhfc.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2hkmlzzky.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2uqcnlrkb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2nbpelmey.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2heelqvaq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2iyekokmy.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2grsakjxm.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2jcjopqtm.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2fpkztrvf.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddeeijxg.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2ndeqlxvy.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2uotmkaii.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2mrcahzrn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xmsmduzl.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2wlvxyucz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2ttfuwmqb.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2mlvdsofy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2ixzsmtnn.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2xtwjbfxz.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2stzmjkhn.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2xpvadtcq.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2phksoauv.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2hryximfv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2bubnuzzv.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2pcumurnp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2pugdzfjl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rayupdnh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2tknqeyaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2htqkucjq.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vthnkleq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ijbdtshx.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2qoamldux.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2vuscvqsi.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2wdiigesk.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2vxawoerh.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2tavpcska.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2wlncexkf.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2nyjtahub.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2vhlaooai.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2otumxmkm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mvxlnfhg.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2jihilssh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2bjdgztnx.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2intoourj.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2geiuvqkq.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2snxlowrj.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2pvapqger.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2lgenoqwr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2tacaikny.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2qfbascfj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2jpmcwtgy.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2cgaarxqs.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fgyivitf.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2tzgdiala.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jmwcdjyb.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ctozuxux.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2srpyradg.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2rjfwnapr.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2gkoonmhm.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ghqmhpim.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vbcjdsyr.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2woozhmdp.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2mfxmprxt.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gwupicgv.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2evrcntly.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2lpiimjwv.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2gaaqpdbj.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2qxwvprfn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2oxjufdrw.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2fcyekasn.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2bqrqwxle.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2ovlaofaw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2mogorscv.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2oidiumdp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2kwcfgbpk.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2xwjjgiuj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2wtmnkahs.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2igzezxub.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2zgqsanik.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2bswvsvbn.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2owkqyufr.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2xzvwhtcy.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ffqgmuqd.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2fjfjmdwb.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2vlhcratu.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2xvombteq.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2aaxruwge.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2nozhhzex.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2ygloskjw.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2etdfxujb.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2rwcgufuw.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2xkoaztzc.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2ngovwquh.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ovkwjcmz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2uxdxkvgv.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2pibsvujk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2axmngsnh.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2bffhmmjj.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2kznfjrca.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2skvgeggs.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2crpqimgu.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2mntqhgqk.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2pjihhpyj.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2zpejtatz.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2apcxshoc.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fbpggdlm.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2grffhxoc.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2qfpxianx.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2britwxcu.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2njiomkvg.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2guasmalv.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2fnjoflps.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2eqxfsxrp.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mxzlyyci.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2eqmdjanl.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2vbnkiekn.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gszrialm.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2kydvdnno.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofggepxe.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2wgtqdmfg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2llbpufzx.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2bezmyzbm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2hnloqgac.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2vfotcqul.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2nsrplpnh.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2iozhtrkh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljmomwwf.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2oznaasyy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2mqhltdys.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2uhnnfyde.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tscqxhxo.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hbvlazqq.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2bitsjidn.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2sygjvggr.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2auzwvhly.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2dbnaixcj.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2livbjrhi.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zzetqphq.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bsbmfrhg.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2klwjfgtu.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2mpjstmop.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2qfoygajl.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2mykfgnri.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2lugmrqew.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2xjueesds.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2gfhnlgdu.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2grazqlev.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2daopyzad.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2wlorzxiu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2afnagayf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dfpzsqnh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ruqxrgth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xkzygmox.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2ioanpcvc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2wmdvfkib.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2fvyriykv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kcafoylc.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ivpswqgp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2euzcuioj.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2gxjyaetz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2cwrpzpty.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2cswglhoz.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2vilygppu.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2imoqpnju.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2vdbtjdvp.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2ndllgukm.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2gaaojysq.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2nzggxyzc.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2pydgiphe.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2gutjigjj.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2qjmzhsgp.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2eslabcne.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2fasdoxmf.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2yibpymnz.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hmrmmvvi.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2tvgsffqs.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2flkhvxuu.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2yfngrqcv.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2czxrkiux.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2bugsrzkc.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2wjkrkwgf.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2ggeeefuo.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2gmyfliji.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2zozeniqw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2ackjyftr.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2vsuzdicf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2gibgcjfq.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2scefbmii.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2nfsythsc.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2rzbmkjip.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2bxomuden.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2axaebzkw.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2tnhpatnx.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2ncdazmek.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2eqijfkky.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2taqgduko.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2odgahvzj.html


<!-- 参考信息 -->