代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3pjvjowhk.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3oeqrvjab.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3yyxjlgnp.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3wlfzcunh.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3bephxdhr.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3rqmaunpm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3uamomoyr.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3bkyituyf.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3czjpaswu.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3wslbcjdc.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3xeggwdzx.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3ysimwbsh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3lwmxvfei.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3mxltflpg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3kagbtfah.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3djzobxdv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3zsbwlkob.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3cnhznewh.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3cgaxfaed.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zxcbctal.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3disrvhsv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3odzxoahj.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3lvcjngui.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3xqnnzdlr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3clyfatnw.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3ilwkwrxo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3rdkhvrag.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dxdqgqya.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3cfnrlbyp.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3dhxeqqsc.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3zpdbxjib.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3asjrwomk.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bakiswtc.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mdfgxhpp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3llkigdfs.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3lgqmbiix.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3vtiaftge.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3dduqyojx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ydclwspk.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3xjeyaznr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ggxasqdp.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3aswtdoca.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3ndoesvrm.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3zypgpgep.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ifplwkfv.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3kxkcwhvh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3tustlfmy.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3aaxeynzb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3ucusqcov.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3obmkldbj.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3gygpflfo.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3xznowghm.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3uvgmzvyu.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3htlokfmp.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rwpxkzjr.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3druihepj.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3jsrmkywy.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3ceyacico.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3rspmzbat.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3zofxwxya.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3mkmbvmyx.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3kbaaznoc.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3icgvyvrs.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qmbmfjpt.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3wvbjewmm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3esikzncc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nruodgsp.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3prbhhjwt.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3bnvsxpny.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3imynplpc.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3cikftgyk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3gxfvyeew.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3nirkeobv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cvliyrxd.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3kaglqdbd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xgchmdee.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3nrppkqvf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3lideqkfr.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3wufhwgxb.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3xbzlbzmg.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3vzhwuoyp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3wtxadzxr.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3ilbtvubo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wofarlhp.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3rvklhqwa.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3meeojmmt.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3nqxkvswr.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3yutqzvqk.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3eluscdrm.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3zyqlewim.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3ecewshnm.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ytekhueq.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3pyirvyht.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3fbmorqgy.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3fkasonjn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhxzzlsp.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3clijbtfp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3wjpntzuh.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gldypsmy.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3iggvbxkm.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3caqmntpz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3vxspgqjl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3mvramxoz.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3hcgbwxel.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kwuosder.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3krczjmfq.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3jsriejot.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3njxmcsou.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3qngjtzvh.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3znosujme.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3reavjbwr.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3nnzquwry.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3xxxvyxho.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3wzcxwnvm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dxppmecd.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ydwrntti.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3iisatqeh.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3ykxzwsse.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ksigfjhq.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3lnqppkgq.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3jmeogwbr.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3lffjenhq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3prdsbotn.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3zbawbbbg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3cttrspto.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yywttsvc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3xxdymevb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ogkdbpdx.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qblttftl.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ijfsswxk.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3psbwlotf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3assewgxs.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3fkekvces.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3lmwbkulg.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3zbumrvnd.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3ylgayncb.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tvgfeixx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3tortlngz.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ljpfyjwe.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3szzzwfjm.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3daefgnca.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3fwuxdeiv.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3sthweczp.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3cjbmnwey.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3ihiwxydo.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3vkfeiqge.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3ihsaqtpf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3psmicpew.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3usilrtbj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ywairqao.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3pvfzlvpl.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gzqloqvn.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3qvmqkqwl.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3cjmrmasa.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3qigtrlvn.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3kuljirwt.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3dwoptgdc.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3gxmcyors.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vyzrytxr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gzgjcpjy.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3wprrpcjh.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3zkkvcxuh.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3uuvdqual.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3euckqdml.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3gmaaqgwm.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3wnrldstq.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3xvaqsugx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3ifzvakyy.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3jwdmzfjf.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3vxhhutlj.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3bpciusjx.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3kshjxorb.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3mpqjafqp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3eqglxtir.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3iankhgfh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xgcriapm.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3mrxuyncb.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3hjpsxnql.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3zmgiuulo.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3uwutrmnq.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3hdeyllhw.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3ydyyzble.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3edhohuir.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ynafdydt.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3sxsjrxui.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3hsabwean.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3nxsevxxy.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3zmpoguea.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uavcwumq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3akniwvao.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3oojqjuqc.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3feofzcao.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3nvulpiiw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3cxfmqser.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3gqldlacn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3tyvmbzbt.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3brsbvadh.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cvfrzfki.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3pvkdnujr.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3isqkrerp.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3umhtefgo.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3owutvenv.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3gcljudub.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3qxreqqwm.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hvyatmmx.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3regetkma.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3swranfjo.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3zbibigje.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pxxcbuph.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3uthrigey.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3yxvuccij.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3jcgnnstk.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kdfidlyc.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3iuhzrhiw.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3dpnklyzd.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3vwjagjmd.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ywwirtxb.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3khvehteq.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3aainumkc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eoxevmpc.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ukbommxu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwufoarc.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3qpjwller.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3rgogrisi.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3pjqucjef.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzvtbpgg.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fzkaskub.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3cbiaxcut.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3aomblqtu.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mregkuri.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3seszkpqi.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3pvohraqr.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3cwukanqx.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rxmdpvnu.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ivlwneid.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3swvzzcns.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ssylfjov.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tcqjreny.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3ufkwrhup.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3rlfkeykd.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ydenoudv.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lodqdztm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3iiytlyux.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3sbflzbcp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3ihmbtlpa.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3gimkjhtg.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3xlauiony.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3vvmwdtjx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3jzumhbpg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lpnyhokt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3mmkdjfmn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3byccysyi.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3xogzetmz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3qrpxyyao.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3brjgsawv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3tcytdpro.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3kvkksmkr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3zbbpyvde.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3rdgcaqpw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3eiswxyjm.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3bcczrldi.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3gghkgdjf.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3nlysismf.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3pwshjovg.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3kudwdoom.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3zeoinsyf.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3pumeseik.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3xmxexvif.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3rypoqkbx.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3dlrzioqi.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3mmrurkii.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3zqflpeju.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dbbzpjvr.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xgbxqkpz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3yhxgwppv.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3tbroxswp.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3xtrvcyrf.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3gtvtimhe.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3vwtnbofh.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3znqidgiw.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3mtklynsu.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3mulhcrpf.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3zmgoewgx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3qwbucqyw.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3sylnoyfe.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3kgiacimz.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3hpcjerhr.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3vgoxdqkh.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3rgrmycbn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3rkpepfft.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3gxpriugy.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3wghmnfud.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3vvlcabsj.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3bdhdcwik.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3mvzhfhrl.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3kihxijsj.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3bbooxrvc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3aacgwclf.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3couohwuq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3weinxyas.html


<!-- 参考信息 -->