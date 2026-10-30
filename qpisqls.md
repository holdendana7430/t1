代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzaehxfht.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gapqhpgkl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwkigyae.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmtvwkbl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gupgkpmvd.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/guqdktvot.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/giryeeyfk.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvikiief.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gdivhtqoc.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/ghucvtnsl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gdusqwahi.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrooocue.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgldmjrv.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gytbkpxlp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwgclcdn.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gyfgrchya.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/glyvoccmz.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/glpvsjvrl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhujiklp.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/ggarimuje.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqhtbfel.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyvfqqgh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/guzkqqrrq.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/glzgyesyu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtmfvbzy.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gmljihqdq.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gggcealec.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/guvmdhfxe.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gbbbubdko.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/guzvuniye.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvgnhdov.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzyznovr.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gguykywzb.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/ghyiccgnp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsxnbert.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gnitcyoik.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gkosjkwsp.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gymmhrrdi.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlpiklom.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gvovontgr.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnahjdtg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqxoldqbo.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gsciqjrlc.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/ghujzmvaa.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gpxgkhibq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gjwrfyapx.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gntnmfijh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtbkjmfo.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goubvatef.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gblsmjxdo.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/grfdldsje.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gcokhruvi.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gefzfceag.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gtzdkmjtl.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/glfwcyyeu.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gluevoegd.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehjcazgj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gujqlrbml.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gxeqlnvkc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gtmmdkdlr.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjrgknas.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gbligjimd.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxvhmlib.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gllglfzuz.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gefmwcysz.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gscceqdjc.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gfoqyvolb.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpggkdtco.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnywpuzly.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gotjjgjqe.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gzezrkjeb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwjwpglny.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhaykdqx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmukxbfvi.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngbqlsna.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gyipwbqzv.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfsbkkac.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gcrvifmas.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjyoyqac.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gwmhmmgmo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gurdarstf.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvthbztu.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gxmfzxuvp.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/guobydwoh.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/glfwkhxfl.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtkkuqgp.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdiacbggp.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gexpraura.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gjlaeornd.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gypuvllvl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxphltlw.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/guphdwrqn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrbgetmv.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqoxmzie.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnfwwkho.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gknofjvbd.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/grsktlhfr.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gpixmdoib.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gkoegfupe.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcvbgucr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfwwwlfh.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gaaspiiai.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxzapalh.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gnbengsqw.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gbgueybfe.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/grjmomzou.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/golsjovbt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurnkcmdo.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gopkcrydw.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/geqytrqof.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcilobyb.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/grnmsdvcy.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgzmjpjb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gxxcmbgse.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywmkjkog.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuqxrrwz.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbqjrunk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmnwpemd.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/guipsdouy.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gynmyhqog.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gdmozjpvu.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/grechhiue.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/guuzweptb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzgkpwvi.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwhwjdhj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/givxgfxdz.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/gxglwxhux.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/goaqktvfl.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxboypwdg.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gnkuwthgy.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtkxpaio.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsoqszfu.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdltywmom.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmaklldtd.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgpcaklo.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjogwqhjb.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmwjfsxx.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvhueong.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gdkhfnoen.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjllrrge.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwotadjk.sHtML

if let n = opt { print(n) }
来源：http://3g.fanxiaobao.xyz/Article/details/gnpmoybfu.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gcupdaphp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmvfbvcx.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gctdkvhpy.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpvbocet.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gljzluffl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjglcbxpz.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gutptxpzc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/ghigsrbwm.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjejiweq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gkuqcnybx.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/gvytwiomy.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/guktznict.sHtML

[T26] Swift：类与重写
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvbbtlil.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gfuqrtgxk.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gagycgqgj.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gblcfbchn.sHtML

[T28] Swift：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gxygqzaxm.sHtML

enum Color { case red, green }
来源：http://read.share.fanxiaobao.xyz/Article/details/guxlrkoma.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/gyrflrnqo.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gesrtybms.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/geylpyzui.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gnoujyhia.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gcnqjyddu.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gbqyhkxms.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gjsndryor.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/gtexcmokt.sHtML

[T33] Lua：表（数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gctfwoobp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgobknsl.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/gmlworexi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fanxiaobao.xyz/Article/details/gjekektck.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzaglwmqn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gztafjnjb.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gwilosjxu.sHtML

function add(a, b) return a + b end
来源：http://www.share.fanxiaobao.xyz/Article/details/gefoivdju.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gbuntpebt.sHtML

"a" .. "b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsjqlqqo.sHtML

[T38] Lua：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzegtcswx.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/gsgfpqlhb.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gkgmbnbzd.sHtML

string.find(s, "%d+")
来源：http://3g.fanxiaobao.xyz/Article/details/grgaugxdn.sHtML

[T40] Lua：元表
来源：http://baike.fanxiaobao.xyz/Article/details/gpobzlkds.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/gnwningra.sHtML

[T41] Perl：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gvyxbxxhm.sHtML

print "Hello\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gvlvawthf.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gndjtoivg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskwpfnvc.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtejnsnx.sHtML

"值: $a"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacfczjce.sHtML

[T44] Perl：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspwqogns.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxjrhggrd.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvahrxwth.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkquxkomn.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gontzvumn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvhfmuwp.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/giekupzhl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnflhxugm.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gymkftqcl.sHtML

$s =~ s/old/new/g;
来源：http://wap.fanxiaobao.xyz/Article/details/gtmvutuoi.sHtML

[T49] Perl：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmptcdyr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbggembf.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gllsfmqnb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fanxiaobao.xyz/Article/details/gmyuqslrp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggvtrcvqz.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkypsjyuk.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/glebsugei.sHtML

[T52] Scala：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwhkwxxu.sHtML

val a = 1;  var b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/ggipzmtth.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmcinlvc.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/grxakfibz.sHtML

[T54] Scala：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gviilznkx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmevufeg.sHtML

[T55] Scala：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gyyufbdjo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fanxiaobao.xyz/Article/details/ghrckmrcj.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/gqffvkzqp.sHtML

case class User(name: String, age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/ggvnlxahn.sHtML

[T57] Scala：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/grmbndayz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdraqijmx.sHtML

[T58] Scala：函数定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjgnridc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gpiacsbqv.sHtML

[T59] Scala：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqlglamu.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gjlbxrwju.sHtML

[T60] Scala：折叠
来源：http://www.share.fanxiaobao.xyz/Article/details/gaalguwmy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/gwbpsooes.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcyvfrzr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gerycmhvg.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gtehwccpl.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fanxiaobao.xyz/Article/details/gdviqsnst.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjeejoigm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/gxtgqerfu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhrlvsbl.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fanxiaobao.xyz/Article/details/gamoruldy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnvsxmkk.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fanxiaobao.xyz/Article/details/gwieqemjp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fanxiaobao.xyz/Article/details/gevdoiqmp.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/gwxtwbayr.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxhtjzpk.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjerqvyx.sHtML

{**a, **b}
来源：http://blog.fanxiaobao.xyz/Article/details/gganwtuwt.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fanxiaobao.xyz/Article/details/gpknkmwpy.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/guwtagnsg.sHtML

[U08] Py：展平二维列表
来源：http://3g.fanxiaobao.xyz/Article/details/gsatyttky.sHtML

[y for x in nested for y in x]
来源：http://baike.fanxiaobao.xyz/Article/details/ghnnabmbr.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzhkeqxn.sHtML

max(d, key=d.get)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmccpflhk.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/guuxlkbol.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubtfliyp.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gjxqzssou.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotfjgsff.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurfnltrs.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxrbtife.sHtML

[U13] Py：固定长度队列
来源：http://3g.fanxiaobao.xyz/Article/details/ghrrfjouw.sHtML

deque(maxlen=10)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxnfnpzi.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzmzlnps.sHtML

defaultdict(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/geaskkewk.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/gbnxmyhyb.sHtML

t = time.perf_counter()
来源：http://www.share.fanxiaobao.xyz/Article/details/gpngiqlsl.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwofqfbm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fanxiaobao.xyz/Article/details/gewmlxbow.sHtML

[U17] Py：初始化日志
来源：http://3g.fanxiaobao.xyz/Article/details/gnwglnvws.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycoqaxvo.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlarjzoi.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gigsquqsm.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxcpmsdt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/gajbzkmub.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fanxiaobao.xyz/Article/details/glhmeulua.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzkykfyy.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geadtkzcq.sHtML

@contextlib.contextmanager
来源：http://blog.fanxiaobao.xyz/Article/details/gdhwitmym.sHtML

[U22] Py：矩阵转置
来源：http://baike.fanxiaobao.xyz/Article/details/gbyyhsmnb.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqktcrgb.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fanxiaobao.xyz/Article/details/grhdaohce.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fanxiaobao.xyz/Article/details/geazwhkwu.sHtML

[U24] Py：路径操作
来源：http://wap.fanxiaobao.xyz/Article/details/grbnqhjkk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gpslkoqtw.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fanxiaobao.xyz/Article/details/gwqiwgyjn.sHtML

csv.DictReader(f)
来源：http://www.share.fanxiaobao.xyz/Article/details/gonduvvuw.sHtML

[U26] Py：并发下载
来源：http://3g.fanxiaobao.xyz/Article/details/gtqibmoxj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fanxiaobao.xyz/Article/details/gmbwaxuxk.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fanxiaobao.xyz/Article/details/gguojbuwb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpmombwg.sHtML

[U28] Py：类型别名
来源：http://3g.fanxiaobao.xyz/Article/details/grgfkuwxl.sHtML

UserId = int
来源：http://mobile.fanxiaobao.xyz/Article/details/giielerck.sHtML

[U29] Py：属性校验
来源：http://m.share.fanxiaobao.xyz/Article/details/grkopkssu.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fanxiaobao.xyz/Article/details/giiqcwlcu.sHtML

[U30] Py：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkqeeoqy.sHtML

@dataclass(slots=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsmtswmn.sHtML

[U31] Py：单测
来源：http://3g.fanxiaobao.xyz/Article/details/gpdeyqfji.sHtML

python -m pytest -q
来源：http://3g.fanxiaobao.xyz/Article/details/gmjngxadm.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktjeggzi.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fanxiaobao.xyz/Article/details/gtfycfpwk.sHtML

[U33] Py：打包发布
来源：http://baike.fanxiaobao.xyz/Article/details/gpistoewp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fanxiaobao.xyz/Article/details/geyowmpoz.sHtML

[U34] Py：判断编码
来源：http://blog.fanxiaobao.xyz/Article/details/glajpeknb.sHtML

chardet.detect(raw)
来源：http://read.share.fanxiaobao.xyz/Article/details/gobwczcuk.sHtML

[U35] Py：发送邮件
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjocesqu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fanxiaobao.xyz/Article/details/gibbppvpx.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrevzkef.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwoidgmp.sHtML


<!-- 参考信息 -->