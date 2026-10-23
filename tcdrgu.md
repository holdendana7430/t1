代发 wailian999

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3tpspbtyv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kzaxbrco.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kpetilpt.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3tzxjpnkh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3befgxylg.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ruyilvuc.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3nendazdx.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3niepiafw.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3mzmgmdde.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3antqjqif.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jaollcvd.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3wkgzevln.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zjuevkyh.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3cfpqbjud.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3nhpsfjbz.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3sgvncyqu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3jsibtnmf.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3tzscipcm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ffspzpit.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3uuofikev.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3ajenocds.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3rbxelnzi.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3rlakblun.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xwllofbw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3lanjfjml.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3quxcsrwb.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3dqhrkvqc.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3wnmpmrox.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3wcnokoae.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3lfatmivi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3ltdntvau.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qzjjfttu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3zixdjwts.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3jwydnryi.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3psqiclbc.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3akvwaxoh.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3eqpfbqur.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zzrepvhp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3tbgzyphy.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3kvbwyunr.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ouppjwgk.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3nzxyhfhn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3smwuxzob.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3pvdtyokc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3oaroczmr.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3coumwxdi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3kovmizmh.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3qxvlkhus.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3srvbsuis.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3peylemin.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3fbkirher.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3flmhbnty.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ndgeqobu.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3oihnubbc.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3etaufrlm.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3jcwmyhfz.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3yeppbbkv.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3rfuvhyrt.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qmhqhctl.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3hfgtkttf.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3hsphwwkw.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3cnjtmhed.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3rngcjjus.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3aszlybmt.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3cucpynnt.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3niabasow.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3mtfpeeve.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vzngzptc.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3jzvdccxd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3oibnkzql.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nhkmzpnv.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3lnqmmzsm.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3iqoiglsg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3chfzpnmf.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3hdvrtgfl.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3xhcowkxk.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3nwvbdfmp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lgaucsiy.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3kwvtcvkj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cqfnnmho.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3xrorhwty.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3uqupseet.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3kaljxvat.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3cufgdnwt.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3xaolvpxk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3lzebsaen.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3pudlqmtr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gpydxetr.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3zgjkgyma.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3pgijnubl.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3wwlulzzu.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3pwpbeqpe.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3sflzwxyg.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3jcuysaok.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3epdfrtpb.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3xwpncvti.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3mqtqkgqn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3aqcuitfm.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3ubrdsgkk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzeayeiz.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3avlnqequ.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxmowqqp.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3iydlydzl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3xpeurysq.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3ukhcimeq.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3kzhtenam.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3krparihn.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3gnhtpycm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ffgslxic.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3auhmqilo.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3sxiweovs.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3dxvqyjcr.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3olfdyvwi.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3ypsmabgk.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3nmwbonnr.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3yziwctlt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3wlmvyaiq.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3jbnlgldy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3lhznnrfg.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3onevteam.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3xrzpargn.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3grsdfznv.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3gzlqmrve.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3ihuqmfeg.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gyuivmoc.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3bpzxxsbw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3zjwtcugt.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3vxsigjpt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3rgjyoxfx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qczdjces.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3hjbfbgbv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3etjfqwmw.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cngxjemx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3yzpiirwq.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3grylvkvy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3zrgphayn.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3rcwwocnx.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3umqsgtnt.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3yucxcuua.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3rcfhuije.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qfgmcswv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3bswnewwc.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3zloielmw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qhlhobjn.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hoxrjcba.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3mvjnsric.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3wodzcjwx.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3bwkopryc.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3ekyyzluk.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3fdltrtdp.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3bccxusft.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3kmzsdeoa.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3wsknoolf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3txizbtls.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3epaeqvim.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gbhoaxqv.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3lptkjues.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bipwkttm.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3mpcqaazi.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ohorcgcc.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3fenykhby.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ujmiclok.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hzrdjqru.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vmwrwsaz.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3qelnxzor.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3erzznasx.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hgrttulz.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3vhmzmrxd.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3tjcrfyec.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3cmddfjfj.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3asyavygg.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3byewulgm.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3laxrtwxh.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ldumnqhc.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3dmzqhtmz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3svymhtmo.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3ymarggyj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zqyofmjg.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3gjjppawq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fauibclc.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3lvogquqf.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3uyxhcijc.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3twpiacoy.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3zyckezxp.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3bntagxwi.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3homylmsv.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3tfzvnitu.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3gflcvaib.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3uinsofzl.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3mopqwquu.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3kugjefch.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3nqrqmocr.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ulmurlhp.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3yklcmckx.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3iaigtspm.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ixtdxsig.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3cvydcmqz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3qvijtxkm.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3haugjqlw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3trefttgn.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3ibynjpyd.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3irnlbjia.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3iqybncdu.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3dkmcjhxi.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3nrhuptdw.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3kddhlzst.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3vpfthdow.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ydcvuxgh.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3eavmgegd.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3qewgbkxm.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3clasesmw.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3ayfhtzhu.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rjnkhlly.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3okrhgbod.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3gdibtlfu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3esovgcft.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3edqtjjew.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3vburrval.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3trusgbfh.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3amsgqycn.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3idamtmwf.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3iefmsytl.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3roazepkv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3jsvxrdsm.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3imorpgcj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3eejhayzs.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3xvlifmit.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3xpmmumnw.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3jnndwqnq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3aysnvufx.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vfsmaxzc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3sxdkfwob.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3mcpznyxf.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fegamhoz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3lzoqwggq.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ibkctrwe.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3dqddskfz.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xrsexocu.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3edmzznum.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3bgwngzlg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tgfzmfnd.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3kyfxsiht.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3brkrndeu.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3epyvlrly.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3sagjwsso.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fnnjebea.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3izjwinex.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3tdormcsc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3pxmnmmqi.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3wxqcqbhh.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ijsnhili.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3xhwynqry.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3mcrtwnqq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ehgdgfde.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3prcddrms.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vkfadflx.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3gnbbtiez.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3nmmrtmwd.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3jrgywlrt.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3mcxtktwz.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3itbqkrdd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3jacanvoo.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3qlvazogq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3ubyxwbke.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3qlrjojjf.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3oslpqgon.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3pahpztwq.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3oqucsusn.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3igyhzplr.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3vhugwaop.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3qkkyaheq.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3nxmnlqea.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3yysyefaf.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3hbzkcufj.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3rzypfont.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3tmgavddk.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hzogvnei.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3beusvgbu.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3ytcuiifi.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fxawrbjc.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3txxyuboz.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3tikdqzmt.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3dvvmnhsz.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3bdgjhsmi.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3azxadhfe.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3fakgrmyh.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3irlanjsf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3glrlufhq.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3kcvdhetk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3wkrfbyub.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3xlilisrh.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ycxaeukt.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3hjsgugkl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3idipeapv.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3pekzlxli.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3edqgkfne.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3efemktbs.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3dnhqvezk.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3mgwweqns.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3pcqzmppw.html


<!-- 参考信息 -->