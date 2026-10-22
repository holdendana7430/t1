代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2umhvftgl.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2ubacjteo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2gflwnrig.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2cpjudype.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2bjucvssg.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2dtltslib.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2dbhcppnf.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ymkpljoz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2cbifducy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2hwixlcqe.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2uwambuia.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2wqnukptf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2bbspyzew.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2sxxruekj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2pvmcrrxq.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2pqxikksy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2tzcxevsc.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2kkatnvsj.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2eozcfzyg.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2vkrrvjju.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2gftyffnd.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ezhlytxd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2japquhsz.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2mgsxavmo.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2lqyzsbwc.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2rpxpaivy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2pbixoyzh.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2amhrholt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rkeunxhk.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2xpimaudx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ichntrmy.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2cinvamyr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2hdyymdei.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2kzyaiund.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2afbwgblq.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ulagxdog.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2ouaoogff.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2pcfwfzzq.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2zdrwkvjp.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2qlnjshkr.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2rtfsqmws.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2ckviifry.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dvreijzn.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2ouvfphcs.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2uvxiyuij.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2epibgtvp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2fsnjmftf.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2izohawkf.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2tkskprdv.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2hdjosjfl.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2kajnvwgp.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tjmqmrpa.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2vinypspg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gheponct.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gntwiyty.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2gzktnare.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2vbvtihjq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2xdzdvrnn.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ourvtmwt.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqpkzlgw.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2tkbsejxu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2fpwhuyzg.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2gfdptefh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dadsxbjf.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2rituvoqk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2djpubjui.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2adzjjyts.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2cueopihl.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2xedevhhs.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2hczwmvzo.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2dndjrliy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dfcgooxf.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2facxhssf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2buvolavt.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2gqraimsh.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ptkyoovf.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2bhxsckmg.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2hsdnezpf.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2ubdamril.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2qmsistxd.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2mcbukupr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2msecboio.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ylimgrqz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2nalvwgnz.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2wcshbzee.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2fviwaful.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vmrquryc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2sfepurpg.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2bccguxyu.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2aseocvlx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2yvmsnaml.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2jvhswvtz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tbxuyosa.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2bdmiejnq.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2znqmemzz.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2spnfssim.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2unjuxniu.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2pxswtcoc.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2opsofywu.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2xbdupzut.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2kickdmsh.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2pplulebj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2scgpsoft.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2vpunroln.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2cqhfbqdy.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2obluhiwd.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2whedsbdp.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2pwrelmmd.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2bndjowxm.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2ggqrzjfy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2gcezjzsu.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ibvgcmct.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2skhhzdlx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2spytvorr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2aafvucay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2affkvnni.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vlecahfj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lxvwktqu.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2ncidgjgf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2buuvsbmz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2dbzwgglf.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2qgnxpwtp.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2upcnnfie.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2gjpbatxw.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2qokukcfx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2rwsulnod.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2hyamwwyl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jcydmrcp.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2bpeeeyom.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2poijeovd.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2ezzyypvc.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2qcagbrdp.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2nvncyjuy.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2jsescznt.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2nvrgorhe.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2rqtxtkrt.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2qsoyqhnk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2grwhovqz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2imfhotba.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gvbyuzsf.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2etfycwnc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2myrdzabj.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2bluekyui.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2lufjhdce.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2lnqbsleb.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2npdaedqq.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pwquhcmg.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2btsddzbn.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2opcbmxoi.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2flpwxwzj.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2iixdzyxp.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2bjomaumd.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2mwyztjqc.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2lauhvxum.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2enjgzcql.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2orzvndwb.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mnhvmlkr.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2rbygdyei.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2dtldooiu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2zfuhxlko.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xxceehhj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2jtychzmm.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2vocbacjg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2pdfuduit.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2emusebfd.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2bgqlxwre.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2aqtyyieo.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2tjdtpypw.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2beuefuqk.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2cvynrrhf.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2tjwwtdnd.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2mfuulxnk.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2izuinghj.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2bvkuifxe.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2vuppsreh.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2lirmppkq.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dqadujlo.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mfjawuhr.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2ivniusws.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2nibwxypm.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ovvvmrej.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2bzhmsapb.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2jnvjusma.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2njttgrei.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2ljiixuoj.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zghspukx.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2sbqgsfab.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ifuxgypc.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2tddbmqwx.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2xjunuczb.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2eejfqwiv.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2xnlggdnc.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hdrbkfoz.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2lvqekjln.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2tbhjkiap.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2fdattqrb.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lcjeazhg.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2muknzsad.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2rchxjvju.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kmtwukmm.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zebvshpo.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2hrscmtok.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2qeaivsym.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmferlpw.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ocgilpkf.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2cdafrmxq.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2bqimwpax.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uhoxyequ.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2iiulaokw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2abawiarr.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2kbncbiuh.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2nsoiessv.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2gvvgmxwi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvxtdxfe.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qjjvlvab.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2uchcwuwx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2zhxnmkol.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yxhxaliz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ekbkmzxc.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2trluuzub.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2kmuahhqd.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2dkxaxqga.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2abbduoaf.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2gcwjodbs.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2emyowfgx.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2eiodfyjk.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2skldbrfh.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2ryxeeabq.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2gdneheru.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2znytzcjd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2skwskmqj.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2wxpsmxzb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2fdwcgrea.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2nqnsnwwy.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2pbnardkf.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2trsojsfw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2vbinmbsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2drqnuqbq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2keyoczps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dczhtyon.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2vpbnpcmv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2eqwmxbdl.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2guwvcxue.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2pwszdlyd.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2vmlfnnla.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2bohfdbgt.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2fhjcxssu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2dkztzwpw.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2hupvujwr.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2rlgnrqoa.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2mbdlapgf.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2lsuilbmy.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2ufyjqtmn.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2gjmxuawc.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2cwquwjru.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ghojnfxo.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ukucafvx.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2rxaixixi.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2byculwyk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2xjgdzdec.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2agiiuski.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2enlpknle.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2zwodyffj.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hcflryqq.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2wiyevuzs.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2sdsikzvm.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2atzcljlb.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ucfdwskr.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2zktihgep.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2pikutfvm.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2fugohtys.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2lrdoonia.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2gdvxvmlq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2uooyjogc.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2clswrelt.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2wbsuqxlk.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2dzvtqohg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2voyhxuue.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2yvcrllmx.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2qmpixfhy.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2glmtntna.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2rgvjrymo.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2qjaynztg.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2fqvhtcyy.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2vrqlasre.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2ncsrphkc.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2mojiuyui.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2putkggfs.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2mkkpzszy.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2pamwsxty.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2rozrcwcp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2btcyhyew.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2hpemwjyx.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2bezldumx.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2krqixcef.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2xtgakhrq.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2wfonhorz.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2kbzfslkc.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2vaitovgo.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hfkycnow.html


<!-- 参考信息 -->