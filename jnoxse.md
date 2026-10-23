代发 wailian999

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3slfgmwwz.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3tugfumtq.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3nalecxke.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ibysluep.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3kwrcjutn.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3dzagvvdi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3befdnhhh.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3wqiwusom.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3byxosblf.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3oxdcdtfw.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3klagfquy.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3aqabrubp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3ereqfrki.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3ijurcvhk.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3qwicdnsx.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3rjldclgq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3nubioxmf.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3mvhxqhgo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3cfmshbfl.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ssohexfe.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3yujvympn.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3jdgljchz.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3wsmrwmhh.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3qcwbnykc.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vecokkfb.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uemrjnwi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3dqwafrla.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3eksqkesz.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3xldkqdlu.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3bxgrccll.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3xjpjuotf.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3wpdshdvu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3mxpksgwq.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3qiorrtds.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3bwuxbadw.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ovnxtjcr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3pgmqwzau.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3wfjxnfiw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3kzabdlrx.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3yvdoaqbb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3symtfnnf.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3hjmwynzg.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3rvziqggk.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3wgvlrvxq.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3zcpjxpiv.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3wtuicahv.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3olwbldom.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3btczmiuc.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3pwkkgjvd.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3djxyiyij.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3mhtdqtxf.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3qaytupun.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3fnqeoglv.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ngiumbxc.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3hdtjwgfr.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ybqyrrck.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3uydifuwp.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3pptbyzkh.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nkjgupqj.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3wivkvgyq.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3dzuvvzxr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3zzwxlwor.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3kuhrsklg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxxpcqbx.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ylpvpesg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3flmtatuk.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3mbmqzpxf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wamsczuy.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3hsnkzuoh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3yvvwfnzu.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3gthvbkqj.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3hvccqmwf.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3dievoset.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3xbgkarbk.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3nrzswqik.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tidhrzfr.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3gpisjiqg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3pekcrepa.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ayitsmtc.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3xducfcyc.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3zeyzoqje.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3gxxpbbwj.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3sivsuzwy.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkqesqxr.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3fdwonkfi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3nodppxcj.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3rjnjiyzi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3rcurlhos.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3qrrsfwpf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3fkjawgjz.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3aygopoap.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3kgaoggxp.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3thwupxoe.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3dtkoedet.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3gqtajgey.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3izfsjudi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gktoswfr.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3sfdcuayc.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3osngyifn.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3fubsmubf.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3rxdfltot.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3aqptiurj.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3getxjaou.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3hlottklv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3yfnasqbj.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3lawkrlaf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3gfuzbtuk.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3bzzkclrk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3dspzvtvm.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3kezokjbi.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3vowgvtdw.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ncnfkkfi.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kmjspmuz.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3smadheia.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3xjljjzoo.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3dpsgcwsl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3xygilomr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3epbrrjrn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3twplzzau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cegphlzs.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3banptuki.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vjxhiseh.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ilmbpevx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3yhuupetk.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3bfleahtr.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ibyaemfq.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3akoidcju.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3goocxtth.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3shqgiysj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3vxicaije.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ptdtzjey.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pbwvewms.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3xvxrzxlv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3qvcokkxm.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3zspyyzde.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3yfvquuol.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3fwaejnxw.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3zjiyjfel.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3eueumnnw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3ijugouji.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3yaqksjun.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3adfkhpsi.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3lomkdbgx.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3evqtjcgq.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3qfgbrjex.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3mbegbiea.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3rpxtcsgi.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3kflmplgv.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3hxvjxjde.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3krnwjgey.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3skhyduvh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pzlwyunh.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ixkhmovy.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dwzkviwe.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fwwqwxic.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3funlsiya.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3mvgrmwtz.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3stekwzxw.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3ertixlbs.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3hksvyawv.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cggfupxl.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3bzgpmpfa.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3wcbgaugt.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3ryalmqik.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zhiuirin.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3pitarewd.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3afagjxlv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ypdcxdtx.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3ksbebsym.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3vvplcklf.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3yrtjnfbv.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3vdwtbmvc.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3iuyzszhk.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3uqgbarer.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3mubjxytp.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3bpsqlknt.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ynvkahbx.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3xspnehuy.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3vstqdiel.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3ghxyjkpu.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3enmdqrit.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dnzbrirz.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3yugsbzyr.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3vjkrjlmo.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3udtegyac.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3laiwqdnz.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3qwvqwpnw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ddixagiw.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3eeqxhhqn.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3vsfbmawp.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ghknhqfh.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3unxjgllb.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3didhlnja.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3borkhmed.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3wsirmxnl.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ffpqktfi.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3flrbrskn.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3avvjtlar.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3gpighwil.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3krxatxcr.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3msfgzcwh.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3sanyvorc.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3otakoyrh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3cidspvst.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xvnxxzvm.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3dsxsonlg.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3inkdorsw.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxiqosjj.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3xlzrhvrb.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ferzxfzf.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3epuknrgw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yssbhkwp.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3tnxifgon.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahcycmdm.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ikheigdu.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3qnokiawr.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3vbvsqguk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hazieinf.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hjlgtnml.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3xfvtiojn.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3jkifvrsw.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kmynhfje.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pwhmtbgx.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ixgmosop.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tjwawujr.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xgguglpn.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3tnjzvrzg.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3sbsmgzij.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3xbvrbeni.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3wlmuoyay.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3soqmilzv.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3bhudbfaa.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3llilrwpq.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3pztkzxcz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3wpupywcr.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3daadzpyh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3jzvxjift.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3mvpztcdg.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ktaalzqi.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3nbhiswcz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3plbvkpdn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jhtamtjz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3psjbuagh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wkqijdhy.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3fmrprimb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3wbjhqxcu.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ssjdioxy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eijekxgu.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3hrlhmlzk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3wqvvkwpf.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3pyqnfkaf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3rvuyoopi.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3nloioxbv.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jmsmvxam.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3sqiwrelm.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3aotakkog.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3orjhtqjz.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3bvhvtkmy.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3itflullv.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3tycyskvs.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3pvufcjsj.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3otjjcwoe.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3pavpemfy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3qhxggtai.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ekobfnef.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3byllkcjf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3lvbssbfr.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3emsxdhpz.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3eovnjbar.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3dytjmjwo.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3gncnybyd.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3bmubcfwf.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3juooarsh.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3ewwyjdqv.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3wcoiuvcm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3iiyheybw.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3sphyrptd.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3kfeupgld.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3cispryhd.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3dcaomfpk.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3xfxjsslw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3bztwqgam.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3nntnqjkf.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3gxpsjadc.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3aniajwex.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3scyyrlpc.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3sdmoctfk.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3eszlmwaz.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3cotnbbcj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3utdbcnra.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3gnxsgqit.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3libescet.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3gyrqavgw.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3tmzqnfhy.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3bhljoofo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3mqagsdtg.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3onnbqnvl.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3einfopkm.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3levolymn.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3eugxwyil.html


<!-- 参考信息 -->