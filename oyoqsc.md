代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjqobhnt.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2aosefawr.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2sjggedue.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2btptrftd.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2zqpihwxm.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2jbdvihsa.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2okaqpywe.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2yxeatfbu.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mnylmphn.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2zrxrjpja.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2pvlhtjmi.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2odjblrzr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2extjczzh.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2acqwvhdl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2lsiekygg.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2zotaokvd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2zvefxwtv.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2vefhlrgc.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2hsmlexoj.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mipcordv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2xhdfqcoe.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2gmoqkezl.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2tttfxxeo.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2gnkcwmuc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2heicwgvj.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2eqedsani.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2nwdmdpek.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cqcfgdoe.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2agvvmztn.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2bzwyzcbf.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2lnqedgme.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2dtunrpoe.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2mxmenhgq.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2tphojoip.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2gnwerzvo.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2hrskbfbd.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2qafnswxl.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2scxeezee.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2lvulfnko.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2hboygfxs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2tldsypix.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ivjtdfgx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2mtvjnnfs.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2sujlekoh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2instqvew.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2gqwrchel.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2nkhkadqw.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2bcapxhki.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2ppgdvmrg.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2vjqjmgbp.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2gjmvpdqm.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2zbtsgfoj.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2zrlrtbeq.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2tqplmbym.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gabjocqj.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2mymrhvql.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2vupwcqnv.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ebykwpni.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2mhmrkokj.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2coroceok.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2immqvvwd.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2yzhktray.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ociqrmjk.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pnstdibs.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2dnhzbkvc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewyrtuub.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2mfmvorpa.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2nopkkohs.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2tnjsmmex.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dllaxddv.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2hsxyqvzc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2eobvgquo.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2bnnjtbnr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ktamaehu.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2nkdysqal.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yohvqmjw.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2zuhfkgco.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2biccadfd.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2cpxrlnhk.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2qeedwrol.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2hduvxfct.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2mubhxcmp.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2aruharza.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2iuuivkoc.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ihibvdqp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ovjngwls.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2ertoqcdk.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2vjadporb.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2hsumevae.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2enkniikg.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2dogtwteq.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ninrssia.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2wnrcuigx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2dpcevwdn.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2ahpyiaos.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrlhazwl.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2tumymftb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2xfzzrvzs.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2azoipkyp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2uwjaswzd.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2tcrbeivd.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2uemgxwep.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2idfzhocq.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2bbtxvquo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mulamsid.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2dmnrcfil.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2sjdnwvkv.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2ztlruzij.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2srschrfg.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2ahqtnmsj.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2hhgfprso.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2geztebgr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2hdddncbz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2gstlylij.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2cxrxonbq.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2gpqmlxrr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2aellruhv.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2hulysmcf.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2dekdtfci.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2hrjykwbs.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2hhtgrfjj.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2dqlcimts.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2mvvmpjyk.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2kwrmtxxq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2aeyvddjd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rgxoqota.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2updmqwue.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jzjvpjnp.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ihhvhdsd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2pagmqewx.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2vuznrpae.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2hkqjztow.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2tmouxarx.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2fejhdkgm.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ujtpopib.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2oujnonea.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ecffgxkh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2rwobwhot.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2mfboljkp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ooafnxhh.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qfbeamud.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2kzutrmlz.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2lkxkmrfp.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2hvyijemq.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ykfjieyz.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2gqxulqed.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ouanohvg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2rcncdceh.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2aqgyrtiw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2uptrhmxb.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2nwsxghbs.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dncfvtha.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2jejjshlc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2orhpcrbv.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ljwukchr.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2zqkuchvo.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2xurgjiey.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2terimdfx.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yfbrnlbn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xbennnpo.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2ytwobdsk.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2lnnctdzt.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2obwbagyx.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2mfyyezpl.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2gfplnutf.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2bcxcvdxe.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2nbekudya.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2vxgdscmx.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2umzucyuk.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2rtqhgrbv.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2zsadpwjw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vkaybwvj.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2sbnfwaua.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2epbglfql.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2rnsohghv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vnkamdsx.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2glssysob.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2gcvnjyek.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2qtlkquaq.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2kpexxdxf.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2fgudguio.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2kfbkbtiw.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2ymttgjwv.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2gzezvalj.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2dpcxjnkt.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2djoadlyp.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2uizfhhfi.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2djfoyull.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dnomtrpr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ehgaheku.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2lzphhfpf.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2qdcabsww.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2puwnpujr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2eiwoaqmg.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2cmhcunbz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2ikosqafm.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2jmbapgzn.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2axgbmhov.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2orondhrb.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2yjrnpfkr.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2cyxokmly.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2jmkjxgjy.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2dgeugcps.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2rmzapfrp.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2jxrikwvi.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2dytgnvxs.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2upiqekxq.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2iiapfhac.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ywcrboou.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2epeauqes.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2toaowwtu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2tsoxawgr.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kaxwxjpu.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2tfguvblx.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2cjcidmbm.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fttxrptm.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2owmebdrv.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2sdxdjnoo.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2bjrklvzh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2gcyoxovf.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2lvsxppqe.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2aylvnkpc.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2kydsqzfm.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2ykrawjtg.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2kdvzlpmb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpuuamrk.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2pfepjesl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2zoulxhbp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddsqjxgc.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tzdfmavv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wryjnisp.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2dhqsompf.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2dmiatejc.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2pzgvthha.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2fhcuesgn.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ifepaxcb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gmgxsxjy.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2dplxokoe.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rtdhqisv.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2uhmmgogj.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2wrpkebmh.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qwrqzijx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2efzzpeyo.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2pbhdqquc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2lbyqjkpg.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2inrfytxj.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ikqgvgbv.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2roeiifqx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2tgyeowam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jlnnpudr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2gtidfpzl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ezsthmki.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2nqjhhyuy.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2wozvqtof.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2ykfhowyv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2mmwlucum.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2trdfmxex.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2xcqmksgv.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2lnmjusgc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2wiusrexm.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2vdpdqdya.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2vilwvnoy.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2synmjcns.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2fweyebpx.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2lzyaapym.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2iaetbdmk.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2ubzuinkh.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2sgqgsvws.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2kmpuiuns.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2jvjvwbeu.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2fncsxqmr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2baapdmre.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2cjxgunqt.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2kdasoqpp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2ecimijqi.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xdhvjrln.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2kefojzpx.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2evzshach.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2bvtgtztc.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2uemrlifl.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2zzawexhf.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2woulcmon.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2yqfdkjfe.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2ghrnzobd.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2dpdbtjpp.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2pphnppav.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2efivpgss.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2slxvejsp.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2voffvqfb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2astqxjtt.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2aktwznbm.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2gxgnicrg.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2vowwaral.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2cassivfg.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2otrkzipi.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2flmyystn.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2lsmvurgz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2msmgpudu.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2jkcmthfp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ezgftrpa.html


<!-- 参考信息 -->