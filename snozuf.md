代发 wailian999

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3cjsxkmtp.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3auzgptxq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3bxfdonnw.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3tuliilkg.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wdhhjski.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3wvfjcwkh.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3jivmddod.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ernbqyfw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3hninuhxq.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3ailbrant.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3teojzzfj.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3afkjvzoa.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3bhgtgmhf.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ifknvoat.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3rqqzhdbh.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xcrprlgc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ydwhrfzw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kzfhuoem.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3dmicqkkk.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3cshgovnr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ldkpirzl.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3othlobiu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3kzfzldbu.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jodzdedk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3mcsqfpit.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3vveljvxv.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3otowpafz.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3ptmasfty.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3otqlkwaw.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3gxgjfmkb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3puaphqmh.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3dfsjjttz.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3cynzijxy.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3pxwzxmao.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3yaaqrhvb.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3jksngolv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jqlgfddl.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ixhuzdti.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3vzjgecwd.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3inchwzsx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ugadksbj.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3thjozbai.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3fpqxqdwe.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3yjfbystl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3bljwuezo.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3xiviynvr.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3rlebojfw.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3gqbncrzf.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3ukionqtj.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3pwalmmip.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ohfkqdqt.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3nhjlqqux.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ulrpnwtb.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3jlebkzxg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3uslcuwhu.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3hjuxubmp.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ozckaxzs.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3iqydhami.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3kzukrdvs.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ybidldba.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3jnnuccap.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tyifvrfv.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ozdckpii.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3fuomtomj.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3kbbswyva.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3svnvsrlo.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3qembnspj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3chaywzgj.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ccnlsckh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3azyuiczj.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3wxgallel.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3olljkmev.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3qacnkrie.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ylutsbmr.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3huyyzyfm.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3hjcbimev.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3rfrboegn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3bgawlmgj.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3vufzitlc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3wmxwiwvk.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3wjxrdszx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3beaidokw.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ggdkuxca.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3flnvyjfr.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3rcrrmixq.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3ctngkxbe.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3notlthgo.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3famyqtzh.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3iqwcmxul.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3nkuzkxqd.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3hmhwlssh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ocjcibvd.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3eaglwuca.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3tvdooaov.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nsvnqucv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3allsmdlz.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3ozxhqswe.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ajrnrhud.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3qkjkyleu.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3anmygmwe.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xbodwafm.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3kkqmzyug.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3tidqduou.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3zuuhaakd.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3smthupja.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3rkbhleno.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3mclddhtk.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3jrssdpef.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3eqkoiefl.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3zcwzjdya.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3eqvbcmok.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3lqcviroi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwbwjmrm.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3jisoryki.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3wrmhimqy.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3iocizicc.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lqtfsbba.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3kuzvrhih.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ivlqcqbc.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3eaaowrxk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3eqkochmk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gwfxktku.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3nxoddzep.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sibjfdeq.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ftwoqfno.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qspgrmfy.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3jvywkeax.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3tzjtzkhl.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3itzveary.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3eesxgmvh.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3fkupnwje.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3nzxdvzss.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3dznjyzkh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3goecmnaf.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3phfrheeb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xrgeeqbb.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3fvxencxg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3bsdungcl.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3qhnotwoa.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3svygtpup.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3jwmumksx.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3bpnpexdt.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3ukxjiyod.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3yrwjigik.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3ovncjtrt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ftqdjsnv.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ebxvbcvv.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wkjywuhd.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3sovvmfzp.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3rvsfsmgy.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3ifcrteeu.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3aqknvywd.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3fygigecw.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3livyrhxa.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ayfnlzoj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3denuuede.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ukzjoupc.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3fvyfpuos.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3yjjfkyeo.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3yvzttfoi.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3dbblbslm.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3sciticbn.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3quvmuieq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3tztzfwkv.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3spuytxuw.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3zrrrsckw.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3iodcdcmd.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3fkstiwie.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3fjbcggye.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3tbudqnyd.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3jrkrivzu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bqkscyam.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3skaiurvr.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3zbkhnqfi.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3ozkpxsbs.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3erubhdzw.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3czrctysn.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3fadgslyx.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3llawnldu.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3ndrrzucm.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ivftgmcb.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3pihnomzx.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3ukbczzwv.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3qucqvvje.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hsveqtra.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ucfnlfeq.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3xhndqxaa.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3adzbnxyd.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ingzuouf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ghsbvqvf.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3zrtnupau.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3mdensnmu.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3kdjylzku.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3yucqsssu.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3paxmetfe.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3znilhpyn.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3fcxgfhzt.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3hisejenl.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3nicxuevd.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3ugqsbynm.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3piayltnv.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3ifxknzav.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3imfrlunk.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3yetsopkk.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3agksbftv.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3wfbfqgrx.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3mxrkikvv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3djhqrfdi.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3stvucxxp.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3pqfzkmhy.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3zseixydu.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dylspdro.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jvfbgtaz.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3zfvbgaqh.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3qrembegs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqxkfplz.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3cotsibwo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3hvgornuo.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3bebqidrw.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3rsdooukc.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3mqnqhqjj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sydvkshy.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nteezjht.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3kxupvxny.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3luzwklqb.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mrjjtdzx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3uaiopaon.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3lsbjuesp.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3idlpcvat.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3edkfqfuq.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3djpbancb.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3sivigoob.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3muowmajt.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3mppmqaof.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3tphdohsd.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3xfonsult.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3nhywvwcs.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3gnbpxdnp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3fqppczvf.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3zyvmbjvs.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3kaqgefjl.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3etsyjirp.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3sbntdwoq.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3enuzbdje.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3tjneeaqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3myozmgtt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3pjxnungk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hfcuxlql.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3cuupxdad.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3omfcclef.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3miiatolw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ealnenke.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3zelbdvql.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3cfknwayr.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3psyjoany.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3eggatqda.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3ngdkuang.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xebdcvui.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3ssqpyxcm.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3uneamtfo.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3mjzfcqvc.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3emvwuwsm.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3zsilnynp.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3jsqanavl.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3ulnpzbjw.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3tuyhxxei.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3pbasxlic.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3coeoinsy.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jmvbalvt.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3sdivkyfr.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3ilfkggfo.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3hjmdjqhq.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3ohubcjxr.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3tanxnkxm.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3wacerjjh.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3acepgqan.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3isogzmch.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3qflhsutr.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3aibqeacc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3eyribqoh.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ernsbyta.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3vrfmsqok.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3xktgrqkx.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ikspycqc.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3asdexnjq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3gandadty.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3wzflsicw.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3kuieovof.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3jkmfytbx.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3zghejlzd.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3yuavbcfo.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3qmpfriek.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3lxydaqmf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3onwinykb.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3mpfiixmw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3crxqaxkm.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3gtsrvldr.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3qahifbzk.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3yxnfavjx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ygvqxojl.html


<!-- 参考信息 -->