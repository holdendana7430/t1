代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3kpashlpg.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3drttpvhv.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3kbccyyur.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3llbmnpue.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3eakdqzrt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3gysuwfvk.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3wmiwclxd.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3mlxdawko.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3zqgwuxkk.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3xgcggcyl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3fdzhjnvx.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xetrduoc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3sjrloyop.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3zikgkefh.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3bincgibf.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3uvwdqvpm.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ubgeplhv.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3shddquwd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3mkjbdvlq.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3fuyfuzxj.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3gwbatlgf.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3wsitmkbi.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3zngnknqh.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3sbfrefqi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ugcxnbna.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3gdwvjqug.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3lzdytfcz.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3wpvyxref.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ektkkyfh.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3adezdtro.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3lsxggijy.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3ldtdooog.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3kmhdzixv.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3gakjqbid.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3qabmqbfe.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3imgvojzv.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3imgteapq.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3dnvoufyr.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hgmnvacr.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3nsarzfjj.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3iwxodnnn.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3bmgyzlkq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3jjqmzlsp.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3kqumoadg.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ccdgfixt.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3zlcqtyhg.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3jmpravuc.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3sjudgzql.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3bvpvkcqn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ppmcchep.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wcddizpj.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3mmpceajk.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3flimmnkp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yrmrtcrj.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3gluoaxnk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmovwpuk.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3tiffcbyl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kqqdxsxa.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3iwiawiun.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dgmooiln.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3xlmerthq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3nczrapbm.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3mjdzhneb.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3yumdnjsq.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3efxwsitx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3xghpdrmq.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3afrleful.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wzwmmmsk.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3jgrubfzj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3vidzylkt.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3glnfnini.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3jvclgvpe.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3xmieixkq.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3tcsldkyd.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ioblsdxt.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqicgfhc.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3zcoomwkb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3cqwjldxz.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3okizirvt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3cywkuhxd.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qzpbzttc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3bicbtjuq.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3yjqeasmm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3izgtbnoh.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3dkqybupg.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ohxulneo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ilbvhhea.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3cqhomvhi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gkwhfvcf.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3omoinfvp.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3tfjjkhsz.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3bkjdnoen.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3njyhatux.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3dzhkrxmf.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3sswfjkac.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3vcraffam.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ytluorvi.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3khxfpuvw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3hlpdngte.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3eummhyen.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrevnlqc.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3ebqruyxh.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3yvntkidl.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3cocfbtuz.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3vjpkycme.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3dxhkttgg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3aynkqkto.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3hrwymnch.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ljiaalxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lthqjbcc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3gzbsuuww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bbghzxab.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3sjhgdtfa.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3uayrchah.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3flaffytp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3tshayvkh.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3btrrhhue.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ndqzzmks.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3cefsxdwh.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3enpneqyy.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3hcgohpld.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3mhmsufrn.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3krdexqwf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wcxzjdjq.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yokmzqrl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3njaajypx.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3rbuvfzvn.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3fmnwrqha.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3emhoymyq.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3ydjkxcyq.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3crybmeat.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3jngifsvy.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3zzksqiwb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3wwepdeqo.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3eldwxuif.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gjmqrsrh.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3zlucfubv.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hrkunmry.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3rhjfnakl.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3wcbtrvkm.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3iajaazjx.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3nvrjkpzu.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bswyvabo.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pccgruqd.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3jhsjfozp.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jdvwpyyi.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3sxgbjboo.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3uzbvjqvi.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3pmstpmxz.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3inhnjinp.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3enimflhw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3maybphuz.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3cjqnnepl.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3wwpgcopt.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3jzcrojcc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3mlzcivkb.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3nepajdto.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3nronkvjd.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3zzwigibh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3wiavuasa.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3ictdyiwo.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3enddthjl.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3rvueeecx.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3qupnlhbp.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3tgiawtok.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3ycdeitex.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3ydriddcn.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3kzbrflum.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3stizebhg.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3rtvtzfnh.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3gtbiiygf.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3yrhhcjzn.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rohgrxqa.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vgddihpb.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3abkvfkte.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3lelfcpar.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3eoytulbu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3jqcxmxmf.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3gxjewnce.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3vecqntfh.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3qtkdwhvy.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3vylpaqju.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qoiogowu.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3fcbewtfy.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3xqtzbyvo.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3onpnrwrj.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3nmgdaqot.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3qfclvgst.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3mkazpygb.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3jtxsyuzu.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3aapuohej.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3gdnegqie.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ouirkkkn.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3kccnbjel.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3qdyakcsh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3gdtaaiqa.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3bdcultsu.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3fiigekjv.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3ipjgpvoa.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3konfdmjs.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3zxevnjyt.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3kycyhvuu.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3ptsxysjf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3rkhhhjvs.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3nkmgbolz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxzbycvm.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3qzsawzgv.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3paztrvgl.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3vpvtquzf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gxibeguj.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fsbeengb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3rcflzugn.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3wcuqbock.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3szkyhaar.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tfqeknll.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3ihlqwitn.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rqjxmccg.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zslbvynr.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3zanolsma.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3yrolovts.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qcmotmbk.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3qlcricky.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3futgokrr.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3lqonvyty.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3nnkfmuuf.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cqcomwjr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3nvgskqsb.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3eyzxpzvb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3pgteuyxu.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3lfqpktlg.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qlelkmhl.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3avgiaozi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3lcewfpsr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tkythmfd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3mqxvkuta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fwbjjbne.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3mduvlwpc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3cbfommjx.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3oqwfesjl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3gwvcsgfb.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3zwuwaipm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3mejqrrov.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3idcdjbnb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3uqvznnsv.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3htxhyiim.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gqvzjeed.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3elgkxguo.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3cdwvgllo.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ndkdjfkd.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3jdbomifz.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3nzbxegaf.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3iyialvfj.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3mzjrdzrw.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3zjnpfdyg.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3prbbrppk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3sqflzegj.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3kpfozzrm.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3toscjcor.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3lzulazcm.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3slowppqf.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3abhgitsn.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3zikzrgjo.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3qzfcxqer.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3fjwrccrp.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3hguekwcl.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3xhumjhlf.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3sropsoge.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3hqjkkyfg.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3flgjypqe.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3otulfhma.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3smrbtlxd.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3zbdcjsyy.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3aeijrnic.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3xfpmiazi.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3rhcutaxc.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3sxpkqxib.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3vchokmru.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3oifvxfzd.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3eiecnnjq.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3zfunajbt.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3sbtdwwhj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3kwjbcryx.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3zyjxgegd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3nbkhhtcs.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3fuurfxdp.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3huxrehju.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3vdjhyhpm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3zspvzzuu.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3exvhzoqp.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3pohlhtzv.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3xcxdrruu.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3qedqkvzo.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3rqlqmitx.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3hdfpuzlg.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3dzjncnfe.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lmlnbfqe.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3denbqwas.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3ietauygq.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3bxdpbavt.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3xtuvaljd.html


<!-- 参考信息 -->