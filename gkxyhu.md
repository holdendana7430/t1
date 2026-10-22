代发 wailian999

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2leszfgzs.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2pnokglwm.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2tcsmstvv.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2intwxlzo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2htsvaujb.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2pqagiico.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2fzhxemqh.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2bhjbpvut.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2obrxhfkh.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2zsvsjnzm.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2wiagowuh.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rzgonihl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2pjjxjcuy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2xtrvadlx.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2fspnjvfh.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2vkecwaib.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2hwbvknoo.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2gpwzpsjy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2llafaoha.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2pqoijdth.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2mobilkjh.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2bkgjaydm.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2zbnvcypd.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2mxifmmsh.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lwyrkrpj.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qazncncf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ljszhiia.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ubjlojjs.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ujgmnbzx.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2lhhncihn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2juqkusvj.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2yjyjsuxq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2bwuijhdb.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2sjoudaxy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2xzysjsch.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2cygjtsdc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2fxqjjdqf.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2xfocitsu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2duaagbze.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2rhpuwdbx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2tsafurkd.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2ssdebcsw.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2oljhiqxp.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2kvrbritk.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2jzhdmxrp.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2bfrfdsyz.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jvqbdohz.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2pgshxapa.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2fzgsfmeo.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ypaarfvu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2uricjszd.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2owuhmtdc.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2jpjgjwwr.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2stdmvuzi.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2kucxguwj.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ihneipmv.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2pqnzcfzk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ifuxaanm.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ewxukguj.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2riqmtjeb.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2vtiecqwi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2fpiecxtn.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2dkbhdyzn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdvztvpa.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2hjwtkilk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2fazrqytt.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2uzsjjmbl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ptbpwrwx.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2qyhwyrrc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zmhhsllg.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2vszuxwoe.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2pwsejqhi.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2getjkets.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2wzwuudip.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2zgcsohut.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2vswnxuyv.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2xabyalum.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ybytzmfu.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2hgjkiuos.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2bkszlbbc.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2pjzdhomp.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2yjbtjiqa.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2enocosnn.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2uavmhgfi.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2zibchjgd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2mractdzc.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2uphxbdwq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulejodsw.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vstahxrp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2hypomytw.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2chuegath.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2xvnlcwiv.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2pooneohv.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2qeepekie.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2letlofxs.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2njfpudam.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qeogyvsq.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2kphsrmmq.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ymizvfkt.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2qcehktfi.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2rpixaxsd.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2lafpmjju.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2gxaobfdg.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2cfsmkmhj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ivcyfiuh.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2udjpenpq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pyoztltf.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2kgkfsqvz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2gqtxwrgi.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2lzcmweuq.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2wgvgdcbs.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2opebsraq.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nzfxswuy.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2yojyjjze.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2figjosff.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2nfrtxfvc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2cmpmxttl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wfapcdik.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2cmewhoph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oyzmhyvw.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dcvsygwf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vibzjlzt.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2lxxmxihx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2psaodqjb.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ytjlszpl.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2dzjvzkkv.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2keuoczpi.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2obpziqos.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2erstmubn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2zpdwyhof.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2rtxqbkvw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dxkkiobb.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2cqctwxdf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2znifnuqs.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2jiolvzov.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2brfqkmnn.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2nvuswhsc.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2igfcwzpt.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2mkfehiro.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2oyadvihu.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2cbtflvta.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2dozuecrz.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2btncrczm.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lwkpdclr.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2pnsehbhl.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2iqkqdcwp.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ddwvydrm.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vvgvnhae.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2sbyxeytb.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2jyesufxj.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jpyqxymb.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dazsowvz.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2xzqynkzp.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xunmmvph.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qdhjkdju.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ultityjw.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qnsngizw.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2qsrynsca.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2tednplfo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2oxhrkyoq.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sronxucw.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2pbafmwkh.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2bzwcekzq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ticiptwm.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2wtvhyese.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2bomunyds.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2wnwvqggn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2cjeaxmyt.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ptfiluic.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2bprklcxe.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ckaguwvc.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ctkzwxkr.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2klzyqgqp.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2fbaywbvf.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ukufalyg.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2rkzqlvug.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2yvdcpckx.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2enkewyyf.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2resfhlna.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2xhgkwtwn.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cdqswvjn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hhkqddvf.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2cbfgpzmu.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2cycbotbo.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2bmjqoljt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2tqhxzbua.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2jmkbcqkv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2gqvuyktu.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2jyudplnl.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ueiaechs.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2kzjdnokc.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2exxnlwyg.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2nvmzhvtb.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2nchkoose.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2hrhmdaiz.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2rvnxripx.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2pwfgzsxi.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2fzqcqfma.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2cvkomqhn.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2mwyidtrh.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fxnlcqni.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2vdayjpee.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2sknwjtue.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2dqnyvolh.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jbdrraak.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2lbdlldjf.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2qgsivfzn.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cpxqrqwe.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2hauykopf.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2nenwzhvv.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2mncdvfdx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjonglqp.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2bvhfkhvu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2prwizzfz.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2heghvlij.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2jgkdpcwi.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2npakeklt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xlopigqu.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2utqhgmeu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2qfnlyfbx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbhpejiu.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qpmkzfez.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2tdotjegw.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2dsnhtmjv.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2fswcrwyg.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mathqrbl.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2tialqiho.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2dsvlzhih.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2ytckbwew.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2bcomruke.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2zgfyfmhe.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2yiwjqlin.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2oywgruks.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dicyqxjg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2wursowlb.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2omfmxwss.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lafimssc.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2fycxvbix.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2pgpddwbg.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2jrubwdgu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2cgggcjxc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yljxjexo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2zdrdjjsq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oevzjexn.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2unalksyg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2xngvyhur.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2ahswydxk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qvcqexom.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2erliacbl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2kxwbervq.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2wjbwdwik.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2xzlhmhov.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2cdfaygyl.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2mlibeujh.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2woegsrdz.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2vqozbkvd.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2gyhqobqj.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2txnlvdgh.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2mseuhiaq.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ifurjrpw.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ywdlfety.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2gssraclt.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2cqxqxtns.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2twaiyhkj.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2veuhucud.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bpldovfh.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2jrqiaghn.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2uvarzpph.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2rzjmsfwn.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2vxiutwac.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2bcvzrsgp.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2dfhmmxda.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2tnwtfhjw.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2kfkgxcuf.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2hknxkeba.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2obsqovhj.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2yziifwda.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2kuzjxsfn.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2gaetfwpw.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2hboajdik.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2mfwcvuzr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2yfltiqez.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2jjogallf.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2skvskjfp.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2ufwhtbdn.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2nncfqrnv.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2hhawlafg.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2kexcqloy.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2hrwublkx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2sxipkmbo.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2xyuouhao.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ozrswpnh.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2cgqfamxp.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2viaodmos.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2yfqpbhsg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2vpiohygz.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2weurusgk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2jngppgfo.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2hsmeixkh.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2cfzzskjk.html


<!-- 参考信息 -->