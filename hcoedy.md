代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2yziyamdh.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2wuxkbyoq.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ydfajxgm.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ujvzyxkh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ltwjshda.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2tidxdgyl.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2rekifswm.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2fblhmlud.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2gwjxunih.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2pwqyefgd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2lshvomjq.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2yfaflhcv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2pyqlrocn.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2lrcwutvj.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2fsfqxuja.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2qwtlkjov.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2lyhwgdpf.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vqfhddjk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2edzfcuev.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2esgpilkp.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2atglpjnn.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2drvwlxmh.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2fxjwgvrl.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2wibanzpy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2zsmulbtn.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2xrlxrmtk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2vckjrbcw.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2dxttisza.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2wnogeldw.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2dspyaxhj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2mqumwgfd.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2emuoubdg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2yqbysobl.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2umgjfxih.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2nywamjuh.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2bmkhqmhr.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2cyjnyptd.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2mgzeizpg.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2agwrepdv.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2cbgjjxgw.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2pntprlbx.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ltvgabty.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2imdhfryc.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2luwrksij.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2bramhatv.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2btzvfgel.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2sgiylozj.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ablbjjwa.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2pxurvajl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lnimcjic.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2ebimokmw.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2xinejcde.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2szfdybto.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2xyadqlla.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2zkorbddx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvxyljxt.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2lgdezhxe.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hjukjjfx.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2yarbnfid.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2iwwmgvor.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2pnltwzka.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2jnnpukxa.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2buzavbvc.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2tqrudjmg.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2cryegjow.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2nzvxqobf.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2iyhiymaa.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2vdsmscvg.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2apuhnvha.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2zgwuyynu.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2iuzwjzfj.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2inlpykzr.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2xhbiypkh.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2glwyvovv.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2crparxhg.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2scemndef.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2iosodudg.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2feyaohjr.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2syvowrup.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2jsexjzal.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2gwqgispz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2tsvpuvhs.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2laheiaxh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2seunpvnj.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2qpsvizhg.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2vfnqlbnj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2peruzsja.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2frshjalo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qqfdcvnn.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2lwbkyuti.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2vnyejqcp.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2okpeeebp.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2fstudwkr.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2bqedviax.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2fvqqlpec.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2glehqpwj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2oigmiixl.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2btvscqsb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gyqwzzlb.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2darfixtg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2akeowiey.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2uqvccbwq.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tujagaof.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2galxegtf.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2rygxuikr.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2nxwjqruz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2dgyqprvt.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2mocmazmy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2dlfzalcn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ebcjmixr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2rkdhtauo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wktchsif.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ddpcplpf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lxllrfdj.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2mclinjsx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2rxpbdkxk.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ogdnxzsh.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2abozjwhd.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2yzyqxcah.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2slcfgsxu.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2mrbkmxpl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ndzfqjuu.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2gxulkyry.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2zuurkfsj.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ucpcsuoi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2dhyyycoh.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2lckwvjmb.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2tzzcbmlp.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2akhqdqit.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ukzendrd.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2scgwrygq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2ukjymrzt.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2qbpdfclx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2napyvyxa.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2pytklees.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dlbtrbms.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2wvjepfeg.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2gmlguawp.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2zldkupzh.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2cgmpgpxu.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2soywdmwb.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2zodmcoiu.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2irkuynns.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2sajeqhzi.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2vhzkdgcw.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2dnhdqgkl.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ugpsnnil.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2hwxyxsrp.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2kdszobmb.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2hcfckqej.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2smqgizks.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2hhngfwgq.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mcrhnviv.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2unzgcpee.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2nwxbwtir.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wrnlpkts.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2cfpbrbey.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2tpnvbkuc.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2qcamgvrw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dujeuzyb.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2xvrpszsh.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2nkhgfylw.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2vkwjfkyh.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2mxutzkri.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2voswjxir.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2mfldhjwr.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2nugcgrbz.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2xwyqvmkr.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2wzbdreil.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2cjeyglng.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2ebqsvspv.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2ianjjjir.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fpipchqi.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qzjyclie.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2grnlgwre.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2rujenwav.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2grnfhjlk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2mpxixnwl.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2jiwnkrmo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2gdxfvbgn.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2umuumigi.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2abvycxhc.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2iwbzszzb.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2tvtavqhs.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2jckjskjp.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2jvitnpyx.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2lecbebql.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2bdogupmp.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rbfzeylp.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2iibrvryk.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2rubtcaeh.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2jzhryois.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2izqeqvqu.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2ssgifmtg.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2hktiedtk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2oiyctzou.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2cvmxmcry.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2vbfiidgg.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2xdlowrdr.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2zkobczfd.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2djsvtfhu.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2lrsdnjkt.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2irhvwrlk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdwebhtd.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2cenaidap.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2daknzkyj.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2mueovdlt.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2udvqsyoo.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2fiksehim.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2yziutruv.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xuqvgirq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2kdkveort.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2yszrtqtg.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2khrkaiiy.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2npfjtvpw.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2bqctvpva.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2hahreuvq.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2eqidawqo.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2rlpgwqlh.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2esjmqygp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rqvhofce.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wirvvgxt.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2srgbkgiz.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2eifurqls.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2rhmxrxbg.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ympesfml.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2vgrfbzjj.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2vwrhwvsc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2emngddjy.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2tarifrcy.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2rvtlcjql.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2hfjvxylj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2iafdiany.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fqkfiypy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2jmpiockw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2onslnfvb.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2msdvkgbb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ytjojsze.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2mrgxaezz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lbjyhjbl.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2syxzbopt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2ffjxnpnb.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2rbzrpgeq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2qnirjpkj.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2zombxkxg.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ssxfjdcq.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2iiklutzl.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2dlzeaabn.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2yjbcdlds.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2unbmljyh.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2borzcrub.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2yhskhmso.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2qnwybule.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2srfpqoqt.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2kkycwlke.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2avvdguje.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2cidtqwvb.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2meiwwxnt.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2jefmwazy.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2giavaypg.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2wysyshvo.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2epyepvvy.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2hltdpazw.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2wrtcnstk.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2vuxtosbi.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2udrejhya.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2ixlndzkx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2upmqlwhj.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2kyxfwveb.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2wflpaszi.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2idvonpqe.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2yhazdpzm.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2cpdiqmzf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2rsaizhfd.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ufklrifo.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2splngrdr.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2ykjsyniw.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2spiytxhc.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2mxttvdsl.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2pfqcedcy.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2rpyeodun.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2gpijdjnf.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2lmyiumkl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2xymeyjdo.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2flgdmdrz.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2odkeqkzx.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2qlpnwskl.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2xqzjplqh.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2xliboehy.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2pvegkcko.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2wnyjdrpj.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2bcbbquzn.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2ogldhlty.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2pzerhopm.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2twrftrku.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2cvtrnbqy.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2cncewocm.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2hdmykvgz.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ppipzunc.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2pdjtmpbe.html


<!-- 参考信息 -->