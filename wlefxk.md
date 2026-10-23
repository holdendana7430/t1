代发 wailian999

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nxqmkibs.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3mthcgpyl.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3wxcxewbk.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ivayfszx.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3yxctaxej.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3rijjptmr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3fhtkmwew.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3ekhnmptw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3roekzzdw.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3bzojjliu.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3nprjyiqx.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3avumxfmk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3fvjcwxjy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3jdbgafrt.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3haopveyl.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3xnaqogta.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3mozyvczh.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3iqhvbvtd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3mauguhag.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3pbihjknd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3goxtoalw.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3agevuudn.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3abvehddj.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3dyzlotce.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3dkhglrbl.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ncazzzmz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3izynhjtr.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3klpqntgx.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3kqxshjzk.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3xibmpjdd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3aqjdqdyy.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3aniunflx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3uclpitam.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3vbocorzx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3wuviiaya.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3arjesavt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3tyuitper.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3kubjfxqa.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ihacvglj.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3xqwvjhww.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3eslrvefd.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3zppdasbi.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3kglxhmks.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3ywbagxfu.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3rnmsncou.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3ilxellqa.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3emjlpfwm.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3tlysowue.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3rgleyidm.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3rayhvxvr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3xhvzorzh.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3fajekies.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3gltdtbos.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3bvljmkhd.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3gxzxbgtw.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jrydwlmn.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3oqpadsxf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3jvjavowp.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pmobjiki.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3gafehedc.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3fycblued.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3avnergab.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3pdkcavfr.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3mebmjyyw.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3vvicegst.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xamuaftv.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3tgaixknk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qcdawdne.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3xtfihtnq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3nbjvajej.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3jcjemrxb.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3hyocnmtb.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3lphhcawa.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3upsosgjc.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3xuwlrryv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3kbnhsghm.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3hhwebehn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3hhxmkrvj.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3qpsfpmqs.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3rbisbveo.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3llkfcffk.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3hhohccee.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3njiauvmz.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3lrlsxrdo.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3vcfhrqgd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3oyfgeazm.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3cthryklu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3xebzwere.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3esxjmpzt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3beelbgsm.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3sirxlfue.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3nvxlrceg.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3tmztkuya.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3fepyuhrz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3vslxvvtl.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3xrewqyiv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3indxfelv.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3sonkhuky.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3rixntkxi.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3iwmdhswa.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3zchghdbe.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3fpuxwajc.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3rmxwzkdz.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3fojwkgir.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3avdxeuwb.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ozgwcasj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yphtmbnz.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3jlwrdzim.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3whdqzhin.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3ssccrece.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3phzobzim.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3vcvufdnk.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3zakxukfu.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ixthfhgq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3vxkubuuo.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3ggdiikft.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3fpwleefl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3anuoyank.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3pmgpajxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vdidqxsm.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nvptyqct.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3peqmkxhd.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3iuvhequa.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3mrdkzuvo.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3xvmyqkot.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3xuvxrhde.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3lvnqryjm.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3hhlrghju.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3ychqilet.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3lgssbdhs.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3jtjmujrz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3mjpjqqdv.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3lqbdfomq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3aungpheq.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3majmicbp.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3gxbqrgak.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ymxiyawa.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3amqfmxxq.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3wgvawwqq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3jtiopxok.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3lokjvozw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3qrkqanio.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3uomzizdp.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3uproihea.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3ortivlsj.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3opfromth.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3khoudayj.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3xnusffgg.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3pkbwqmqx.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3hlpzmpux.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vsulhkrx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pqvuimzc.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3elmikhny.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3uyrefgij.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3tcvlcdxy.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3zbqwlwct.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3pnqrqedk.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3ssobbzta.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3nfvxvykk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3khgwnjga.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3nretcbsq.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3izzyzege.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3pojeloqi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3jbauvefg.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ljqtpnlt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3pyghxjhs.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3esuoufcx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3yvajzkpe.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3hhqirhkl.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3yhofbnwo.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3hrklozaz.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3maeopujn.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3aplcjjwm.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3ytvorfzc.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3aotfwfoq.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3dgyykiai.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3qootpmxe.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3bjoqbcbz.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ksnkmkmy.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3bkcwqqeg.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rnbgvymb.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ptpaxlvq.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3evzmfgcz.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3kjjkaxzq.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3wkygzphk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3upjysrlv.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3tspseegn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3miynuhgw.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3cxlxmspn.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3ckgatczu.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3aguxuwoa.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3ewbggqox.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3axukyaqq.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3mnykzrcm.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3yjmocvkr.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3ttnmkjan.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3avksbgxq.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3liurdzdq.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ephdgxim.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3icylvxvq.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3funyfdzs.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3saiufhih.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3adgiwwek.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3kwbdblhc.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3dhuovcis.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3zrazcmyy.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3nsdejarh.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekowkwqz.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3cqcvxafg.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3pnzibhhx.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3yhnsjbef.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3ciinxbwh.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3scgpnbsw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ererkeec.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ycujmusd.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3jqthtbpy.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3ebqukdip.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzfsatqu.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zoerioku.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3rpfbfpft.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfuzubqx.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kohylwgm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fvfaeaet.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3krlqpely.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gvawkxju.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kmnlgtrc.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ujeyualu.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3pxixfnpz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gtzcbalr.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ixxyvgqp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vdvtjznw.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3ajrckzzo.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ptezfqtb.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fzzotheu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ogjgxupu.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3ybwmmxpk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hwxgatyj.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3vckkwinf.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3enlyrzdy.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3aizplpou.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3pptipebu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rwobdcpw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3joexdmsc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iwcejshk.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3syqvifhr.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3zrejwkwp.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3wavkmknn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3mnzzjruo.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3xqunnvba.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3hsuowkfz.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3raaddjol.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3upbavngh.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3olkgtjud.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3mjeeyyhe.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3iwvofpio.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3vrgwgfzt.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3jplbqlab.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3bumogaxz.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3abqdaxjv.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3zrjuhkdd.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3edwizyso.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3bwrlgvzw.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3wajqsxsl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3qdyosoqo.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3qhtrecwq.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3cifjrzkd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3bdskgswd.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qwggiohl.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3hzxyuzia.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3tsbhgpsi.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3kerxgqom.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ohxxzsbx.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3xsspijve.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3qeuppclh.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3qyphsvwa.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3nqljdtfe.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3gzuqpxsh.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3qdaazubc.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3dwkotrfk.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3oubatyxk.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3qprtseou.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3jcbclfhp.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3tkxkayml.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3ufuorcdn.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3begrfidy.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3hujdclcy.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3loiktyck.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3ootyqvjm.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3nowkauwg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3xaoyfqea.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3xypqphji.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3umaswdeb.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3jgqmvsrs.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3fidxunwk.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3effmclxb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3vzewaqdd.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3skufosqg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3onyfhhql.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3jvywuctz.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3xqvhxflz.html


<!-- 参考信息 -->