代发 wailian999

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3gyiizdny.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3udzypcje.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xllfvdux.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3jfvcjsuk.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3yfhgbudr.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3aznqqggw.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3jpahjtkz.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3csdfbfxj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ywbilwam.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3ncrpzajh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3nzdpoisv.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3smdfhgzv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3fafzbkur.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3wqjydftg.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3nqqamhih.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nkyvsvse.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3xxmjqhqe.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3lqarfikm.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3enuyehro.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3hoyywzhq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3yshmgbuk.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3wqjomtta.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3btjdyudb.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ckgufzgw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3xkcdnjnn.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3qqqdseff.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3wnkmgdfx.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3tpbtxxts.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3uebysvrf.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3igkwabax.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3lpxjmicm.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3efwoelha.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3uxaknxoz.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3olbncfwg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3bplpfbou.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3lzhwwfhy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3wtghqwhe.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3wbsqkskr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3pdgzzipb.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3viqofkti.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3tnpbuswn.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3bedplfpa.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3mcdyuewb.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3xdcwunxh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3mtzbfmwb.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3xxmaolcj.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3vklvckwd.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3ohteyvnk.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3mkbfjzpt.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3yucfngma.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jtxraaft.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3otzmzbjb.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3zhepqohr.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3rzjicmye.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3yrvfpdab.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3rfywumwx.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3oudskeez.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3lcojpzvh.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3kwjcmswe.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cloxxvfb.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3llmqaffj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtavalah.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sqwscedz.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3hkteyjng.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3kumwouwu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3hvmtikbq.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3ibbfugod.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3zxbjxdvs.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3mssqrzwx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jjunleyi.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3dunsxyhq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yutrvvio.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3rzaybuob.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xkfkhbpk.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3nwtnmrgq.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3lfhjwatf.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3gsrqvfyb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3dcnnjkhl.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3wfjobmdu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ovcvatqr.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3gtojoxrn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3dqofdurg.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3sapeeqtp.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3bbpcxhnw.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3vtwrggvr.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3xdqlzuam.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3vipaftfp.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3fdjrupjw.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3fuakhiir.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3zzmkeaue.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3bfeiikuc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3qdunsiiq.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3indhlcmb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3zdendlvw.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3edngnays.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3mbmvgzxk.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ljrtvnhk.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3mubyrfpc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3jllcdofr.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3agyormry.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vvfnokro.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3tflppwxb.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3qitqyloy.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3iydauqra.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3aewnercc.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3uhqppryc.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3wceqbwsf.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3pkdfuehh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ywunrgfd.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3gtdmvtys.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3usmquiqz.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3isexjgko.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3govjwrrs.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3erlyraye.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3tbxydvzx.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3bwiuetkb.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ihuetxwx.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3ftzevpsc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3yibvhafo.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3hwvnzqcl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3gbuppbzz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ukpphsuh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3yinyrzwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rgltcohv.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tgpbvrmt.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mbfwkpdl.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3iezhbtsm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3cbjjasiu.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3kriylwdy.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3gofwpcux.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3lpfzjcwc.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3mjxalafg.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3riezbfnv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3ziuwrgod.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3sgkiyrbw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3wosszsbg.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3sykffriu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3pkbxigoz.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3qtytttag.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3trklnlxr.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3uvflatyu.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3stinxbsg.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3fnabwnul.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3sgxthrwh.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3grhaoqcy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3wclrorjg.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3elgdhhvk.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bagzucko.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3gproqtyl.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3cfntvcdu.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3ceeirsyo.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3eteabeys.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3dcuqzhbh.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3utkvpqwr.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3deuschfm.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3riouyeok.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3chxqxtxp.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3itjelvch.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3cqnnneom.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3toskbmew.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3fjwchamq.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3fuiozdmn.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3dzjupfby.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3errggygw.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3lgsiqtjo.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3vrvyhjyf.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3xgcvwiad.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kmogxqvj.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3gwzpluda.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3sahomymh.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3voqfabai.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3slfvkezl.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3nkrsxvrn.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3hkchtmfo.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3ljaphqvc.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3exjzfvcv.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3qipdmtnd.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3nvrgionn.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3auzjelur.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3tlnflfvv.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3gsfotjye.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ruahnnmx.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3xjotapwy.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3yeocdgtu.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dfystkmr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tbqfjkrf.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ohtjmgbh.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3edwxaqoi.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3hinoxrup.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3iqciyivh.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3gqfgywrh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3dvinkkcc.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3llghtppf.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3uktxtzqp.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3uswcxyyd.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3avkthcyh.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3tnnunrmg.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3cvquyifj.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ocjwtmzd.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ojfbcfnf.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kllviqnq.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3jiscdvfn.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3buphjlvd.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3yavobtdb.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qgtatphx.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3tgyzymgy.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3psuduhwh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3mzoiueuq.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3eafhaart.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3phfrcori.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3hmvlvtqv.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3qctpjulc.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3ppoeccae.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3qqwwqaja.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3jmzusopt.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3luabfdmi.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3tkguzowe.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3twjgybpr.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3vcvenvov.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3prknrwdb.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zmkfyuit.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3codvlgdu.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nowoopev.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3ysdbcaui.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlhuuhvy.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ksaprjqs.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mcyalmis.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3nbkwgzgk.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jbqjiflq.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rlxveedl.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3vwyctrfg.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3jdixowjp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kzsfjkdz.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nnbvwgam.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3agwulivm.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3szblftnz.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3hjktfscb.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3novfwflh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3uqlxtdjs.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3ufmukcep.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3bggeuszw.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3hsoqpwaa.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3vcjwjcue.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3cohvnkke.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3idrhhodf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yioqylno.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3lnbetxza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qmqyghxm.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3ueghabrp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3zsufktqg.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3ndgfolsv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fxcymknk.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3fovkmnlm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3hthxyswl.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3hcahvuwj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3oqmtxzii.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3dcwvjeof.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3xwbjtngw.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3hyqvluzd.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3vepctlzs.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ivazzivq.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3thajrjch.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ildzwkhe.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3cktohsny.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3yklfarjo.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3xpewvuag.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3yvfvcxqd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3aenwliaq.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ykqmhdnf.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ubkpzhtw.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3kjnguczx.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qaooxmlu.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3qlhpvoof.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3kzlxdjwg.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3dxwuhsyy.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3lagyyjue.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3qmkhdjhn.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3hgejugze.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3wurpchlt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3hhridwdp.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3fubqidrz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3juwmvows.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3blqkegjo.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3wmlcvqbd.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3rwczlpyn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3apezkavl.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3tgrnuiyt.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3tyrbaegq.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3zvzrhqmp.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3xnrjvmme.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3ztdcttow.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3tqegwtoq.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3hnbjqgdh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3gpizlpci.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3ilhxnwdj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3mtxqeckq.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3nrcpsrtt.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3mkswlcyc.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3enjkmenl.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3fjdpyrrc.html


<!-- 参考信息 -->