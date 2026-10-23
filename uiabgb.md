代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3vwyejmdn.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3ghrqqfjg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3bqxsiiei.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3faaznltx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3pkwtvtxl.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3bcemvzgt.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3yzacbjrp.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3czvibbiv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3lwhcjzzr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3aonwfhtb.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3tnazgczm.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3lozukygx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3jhbniewi.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3mcesbtyb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3jxocqied.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3cgwvgqya.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3ychiqlce.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3frldcpax.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3shjtxlnp.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3bhcnjbyt.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cgrpeoye.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3yedbkfns.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3fgluoovh.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3vvwknmll.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3littsmqa.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3ypcaiopq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3vylsofkq.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3iehotnhe.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3fzlzqtdw.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3sliynhmj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3lyqvvquz.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3wkzxehnz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3fhvrywsf.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3nkrppmjr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ngzqumqf.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3htkkzopt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3jcqwhsyd.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3utvknrdm.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3xsavcbpo.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3fzefqftq.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3egrmihyy.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3gsxxyeog.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wgmcsblt.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3ldtuovfp.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3btkjibkr.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3jmmqgnom.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ehnccsit.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3btojcexu.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3xgnhhaeb.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3fqzygtin.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3xyhedxef.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uqgdwmmn.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ujehtgap.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybgewmgv.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ipzamywn.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3fhoawobt.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3gmoatjia.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3llxbczzg.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3vntptnhz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgyhpyad.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3magcrwka.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3stnehhds.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ydbdpinz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3izgmsfiy.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3wjaepjep.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3yugvrglm.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3ggbtbiak.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3pvffkiwc.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3emxrgftw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3xuohhbkd.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3zwezhkwh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bwnnnvrj.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3bpqkudil.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3oavmwgmy.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3mqqxbcsx.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3ndyxjrrl.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3serimhot.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3frirhoig.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3rjiypeet.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvsibehu.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3izufdiqv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3tmowuial.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3yafeefwr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3txpiifkf.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3atdxdddp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrlioouf.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mnqzvljg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3wvwdtrbb.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3hkaxtswh.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3oyrsxtbw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3mizvjefu.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3olesejhl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tqhhcbse.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3pwnibavz.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3nteajfcf.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3zohtdmey.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3gcqjkglw.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3lywgivpi.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3udzknjsg.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3imagjttn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3zsvmtlli.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ytcofgvw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3ghvfxaov.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3noouofxf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3vpessjvo.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3bfcmlmer.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3oioqljjz.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3ilvhhpfh.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lezrmtkf.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3askvscio.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3sogaiunp.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3cjvweugc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3qjpqtbjv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cskxswie.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3lguarmlw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3racqmcsa.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lsraexvd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mgsehxzq.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3zppwzylg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3ikahtfhu.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3dqrkgozf.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3djokybut.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ezdlydxr.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3biebofle.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3sembkdpl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3kzveqtvz.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3mfnhwtym.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3unpcoduo.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3atjkrdvq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3kupyigkm.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3covvfrdu.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3tknyjvxm.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3edyedtib.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3lomwuckw.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3gypnmwnd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3yqqzrrvk.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3tbuxdexg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3vmximtyo.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3tvhnmtrb.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3efxrldgk.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3swzkkwdh.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ojpyjzqy.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3qutuwlwn.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3aqzswken.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3zexndajn.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3jsgoacro.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mvsevdkc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ktqemull.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3edvptcaw.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3qblpfkoo.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bbxqjkuw.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3yfgzpzrc.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3qsmzihac.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3pjhancxt.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3oigghqdb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ynymeqja.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3lgimxiaw.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3fptbprte.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3geozypkt.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3uylrnhyy.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3hquwsliu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3ithctnao.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3eolsmcsj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dkamprpt.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3gcniyrnk.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3lmrhscfm.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3tisralvk.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3mnulvwxt.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3vgjklrfe.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3ommwwmbv.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3xvzavdmg.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3ftlvqrdd.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3opkeaewe.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3glamrclf.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3zfrpuafx.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3vcglgdlg.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yschnncn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xmzzkgdo.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3naymuhxt.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3viijxdik.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3jyocuwtw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3sizrvfbh.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3ixjbekgq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3kujehgmr.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3uvkihfiv.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3twawifyy.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3rjahzkef.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3uzaogguq.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3pzlxlzmw.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3dplktovm.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3onixwzwd.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3svsqfgaf.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3uhsppezj.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3zhnkflrk.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3vtgvrepa.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3jkknsukq.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lykqdvsf.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3qrfrgvnt.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3dosvvcqo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3raqmmyoe.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3uqbcaxvw.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3wmpoxmgj.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3kudcnbks.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dnufuzhm.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3ujrwfefs.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ttwyxeqj.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3nxhiisiq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eitvjcsz.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3jgtukgci.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxtgksvo.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3yzuycwab.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3qysqopvf.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ynzfzkcp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3luulzddq.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tiairzfp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3tdrlwetz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3zuzdhwnm.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hqabcqlz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xjqdgofd.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3embpexwv.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3cvqlgsww.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3mmlmxzoz.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ffnkrnxn.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3lozgkcbv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kzceiwnk.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3akorjtsx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hoqcfgpn.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3hlshfrgc.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3rcajaryz.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3civrddyj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3atovfehg.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3aavuamro.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hkjkllaa.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3mewpawyf.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ixyfgmcp.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3wpaezorx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3mrnkjccs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ccyupejh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lulextpw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bxrkljsb.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3sfwyivne.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3lswgczfq.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ppifqvoo.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ytsvwqon.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3zihbqyzq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3irlqphih.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3ipttqagx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3prgqbftk.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3whshqdgo.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3uvqdfonp.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3iwcuajyu.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3gunihxac.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3jimbgjxf.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3rgjswipf.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3yvnoffwg.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ixbcgczj.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3yxarinux.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3kwqrzkse.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3ovjjkaeg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3tachvroj.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3voadkdws.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gtzroczg.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3oxlqafvr.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3aejnsvdx.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3dlspvstn.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3hocrjmkz.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3opnbykdi.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3czersifv.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3rdpyznss.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3daqxnyvw.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3gujwcrux.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3gtooejuf.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3ymfjdwfv.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3cmxtllkb.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3gkbnhtmc.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3kzphskhu.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3idtdsfqj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3znftohpz.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3faggbcpi.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3aaydupih.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3hnbmttvh.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3rriutnpp.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3itsyqzps.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3buefmvag.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3hlcqsrhh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3cpgtlvpj.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3enzjwqbj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qzoriqsw.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3dbuegryr.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3pbuyelxo.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3ecubojnd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3ofmvocip.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3riyhhpkq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3xcvabofc.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3wobewifq.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3pktlmavv.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3fqgqyvbo.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3zojdojgw.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3poevfgqs.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cjwprpdn.html


<!-- 参考信息 -->