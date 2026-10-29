代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/ginpmvdyc.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/getqwnufg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/gfidqlhdn.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gqkidtlsv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/gnioakpxi.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gwqklqpaw.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/gqmhmavwi.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gkhksxdje.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gryahwifo.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gugqjsshh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/gpjpxyfgm.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/grmoesefu.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/glxiooqct.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/glwjcrkhs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/grzdgyqcq.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gowzquxry.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gnnuqxzzv.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/gsgibipki.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gwctwlbpp.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gieqfoilh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/ghgjcvnhk.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/glnarxqkk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/gpcvymgvz.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/gycnvgkqo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/gctruwzks.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gentprokz.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/gfcyrmvby.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gwuavnbvz.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gstgzoxyn.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/gpqulksht.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gbjwpjdre.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/goruorhlb.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gjcgpjchu.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gjuprlojy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/gnkwyfoat.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gdkkjihic.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gsrkpkiww.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gvhoxhtbr.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gaqmpxyeb.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gjtxeoapf.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/gadnhopxf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/gheimlpnl.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/gezlevjxg.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/glajlulal.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/guqeklhxd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gdesflche.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gcjifyheh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/ghaisstcy.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gipfrkbgz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gghhgdljl.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/geslnhowb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gsoknnnyt.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/genbxdjuw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/grsihvnmx.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/gvggkusia.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gbsqlvuux.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gkzhvllju.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gymnupyft.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/gvwpfbelp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gfpgdyuae.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gkzggtxvw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/ghjeaayol.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gjpquemew.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gmeutyozw.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/gdykdqkut.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/glljpicoj.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gimtnthzj.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/grebfvogw.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gotkyqtyd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/gtjlmhkgc.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gcwyajshs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/gsjtpmhoo.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/gmmucgirj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/gzigoekqw.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gmigxjxfw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gasqxcocc.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gmcbpbaje.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gifqcphtw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gsksdwbck.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/gqahcstvm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gqzhgohsb.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/gfmkmlpbr.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gjyohjbmg.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/gqzmkbcqb.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gvxhuisyr.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gcswgxyiz.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gqafymioz.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/ghdhkioau.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gdimsrsmz.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/ghzopxwtk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gmunuovus.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gbuvllmpx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/gryqqjwlx.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/gzseisaal.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gnrcetroq.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gkfdfsras.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/glyctjilx.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gcvlgxvvl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.zdbjq.cn/Article/details/gurwucoxk.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gplljjnhs.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gtajaqyxk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gaqgxlipe.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gyqcznymf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggrcrssrt.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/gkcarkqqk.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gkqyyfzdd.sHtML

[T02] Kotlin：变量
来源：http://www.share.fehbvm.com/Article/details/ghwcfkbrc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gqifdhech.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gpfosnafy.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/guppdsvxa.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gclswuufw.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/ghrpztkza.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gjlmfjpjl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.zdbjq.cn/Article/details/gefaakhkx.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/goattkypt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/gdfzsaoze.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/grqllvisk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gqfvejpre.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/gtleiohfk.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/grqbthdzf.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/geoeznyff.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gjthqreni.sHtML

[T10] Kotlin：默认参数
来源：http://3g.zdbjq.cn/Article/details/gfcqwdizv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/gkrkletlq.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gxqovbsec.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/gvxmhiwqn.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/gljbjprbx.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gcbenmikz.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/gfeawgadw.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/geknuvqep.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/ghxpqiirp.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/gwqkinmqe.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/grfjjyjbw.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/gbstcyaok.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/guwpsdoyw.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gfkevydcw.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/gbouwcyby.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gmwxislmm.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/gqvqkilwn.sHtML

"值: \(b)"
来源：http://www.blog.hesvh.cn/Article/details/gyroshtso.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/gkyhjewci.sHtML

if let n = opt { print(n) }
来源：http://blog.fehbvm.com/Article/details/gywwbzgfh.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/gdsuexhdq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gtjwwxnak.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/gswgonkol.sHtML

for x in a { print(x) }
来源：http://m.share.fehbvm.com/Article/details/gutmxpybx.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/gzcuojgsc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/gvvnlggqs.sHtML

[T23] Swift：函数
来源：http://baike.fehbvm.com/Article/details/gkxanehkz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/gswiamxhv.sHtML

[T24] Swift：闭包
来源：http://blog.fehbvm.com/Article/details/gbukmuhhw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gytmuhpyk.sHtML

[T25] Swift：结构体
来源：http://blog.zdbjq.cn/Article/details/gzrdfpjnu.sHtML

struct P { var x: Int }
来源：http://m.share.zdbjq.cn/Article/details/geafkgmbe.sHtML

[T26] Swift：类与重写
来源：http://blog.hesvh.cn/Article/details/gfdntehyp.sHtML

class A: Base { override func f() {} }
来源：http://mobile.hesvh.cn/Article/details/gxyttgyuj.sHtML

[T27] Swift：错误处理
来源：http://baike.hesvh.cn/Article/details/geqzhnouv.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fehbvm.com/Article/details/goedmrdoz.sHtML

[T28] Swift：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gjaiwlgda.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/gfqynecjc.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gwetxihlf.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/gqrhwmjua.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/gvczkdxoy.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/guwhxqgth.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/gsygwbgmw.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gwckkpytn.sHtML

[T32] Lua：局部变量
来源：http://www.blog.hesvh.cn/Article/details/grbwiikcw.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/gefimrgeo.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/ghidovadu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/gokkazsml.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/gtrwcnlft.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.hesvh.cn/Article/details/gbnkvedrr.sHtML

[T35] Lua：字典表
来源：http://baike.fehbvm.com/Article/details/gbdiicrcr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/gfmjhpkab.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/gzofgnsde.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/gprihwkqk.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gnxntfyan.sHtML

"a" .. "b"
来源：http://mobile.hesvh.cn/Article/details/gnoqkkrub.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/geywujxzm.sHtML

if x > 0 then print("正") end
来源：http://www.share.fehbvm.com/Article/details/gegzllqra.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/grnlowfhm.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/gkgkabdpm.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/gbbkcwhqo.sHtML

setmetatable({}, { __index = base })
来源：http://wap.zdbjq.cn/Article/details/gdnpktvue.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gpsgwspjr.sHtML

print "Hello\n";
来源：http://blog.hesvh.cn/Article/details/gsdcjwblg.sHtML

[T42] Perl：变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gojcxgwqw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fehbvm.com/Article/details/gehjkktam.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gchciktpe.sHtML

"值: $a"
来源：http://www.blog.zdbjq.cn/Article/details/gfxypsjnt.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gflrhtjdf.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.zdbjq.cn/Article/details/gcdgervyg.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/gnvmupxrm.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.hesvh.cn/Article/details/ggxrqnudx.sHtML

[T46] Perl：哈希操作
来源：http://3g.zdbjq.cn/Article/details/gkwyafius.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.zdbjq.cn/Article/details/gibruloha.sHtML

[T47] Perl：正则捕获
来源：http://wap.hesvh.cn/Article/details/gqtdtkbza.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/giyxhtyjg.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/gyzhaqrhu.sHtML

$s =~ s/old/new/g;
来源：http://baike.zdbjq.cn/Article/details/guvfzalja.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/givvwvdkh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gkouxzjoz.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gppesyiyk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.zdbjq.cn/Article/details/gsahyqoek.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.zdbjq.cn/Article/details/gmmuuntji.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/gudlhddcr.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gwkydybda.sHtML

[T52] Scala：变量
来源：http://3g.fehbvm.com/Article/details/gqhncddna.sHtML

val a = 1;  var b = 2
来源：http://www.share.hesvh.cn/Article/details/gpkbvdmau.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gqdypenbt.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/glqcnolby.sHtML

[T54] Scala：集合映射
来源：http://m.share.fehbvm.com/Article/details/gtgmhtsvp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/gbrrlbbjb.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gzbdzrkcp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fehbvm.com/Article/details/goxazuwkt.sHtML

[T56] Scala：样例类
来源：http://www.share.hesvh.cn/Article/details/gadfodzsx.sHtML

case class User(name: String, age: Int)
来源：http://wap.zdbjq.cn/Article/details/gfodvgpnw.sHtML

[T57] Scala：模式匹配
来源：http://blog.fehbvm.com/Article/details/gxoxhqslj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/guzansiix.sHtML

[T58] Scala：函数定义
来源：http://baike.hesvh.cn/Article/details/gngxelujr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.hesvh.cn/Article/details/gfmehomzp.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/grsytliwd.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gdseydrto.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/gnqzdahek.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fehbvm.com/Article/details/grhaadvlr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gajywkbpv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/ghriprqbs.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gykycbzsy.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.hesvh.cn/Article/details/gqxhnnovw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fehbvm.com/Article/details/gjhgwsbuq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fehbvm.com/Article/details/gesmnuouy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/gmtwoowmo.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fehbvm.com/Article/details/gfpuhjqkh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/gracvbzyo.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fehbvm.com/Article/details/gjqmqbjjt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gexaenawo.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/guqpcecfo.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gyatsmgii.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/gvtiunfrp.sHtML

{**a, **b}
来源：http://mobile.fehbvm.com/Article/details/glkvpszxz.sHtML

[U07] Py：反转字典键值
来源：http://www.share.hesvh.cn/Article/details/gbhritpxf.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/glnhqspwr.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fehbvm.com/Article/details/gudpfyots.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.zdbjq.cn/Article/details/gyhgebrtx.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.hesvh.cn/Article/details/gqqjyfsag.sHtML

max(d, key=d.get)
来源：http://m.share.zdbjq.cn/Article/details/gdnypfoya.sHtML

[U10] Py：按值排序字典
来源：http://mobile.zdbjq.cn/Article/details/gbezcwusw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.hesvh.cn/Article/details/gjhjptzyc.sHtML

[U11] Py：生成器表达式
来源：http://www.share.hesvh.cn/Article/details/grwzitptg.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/glmffrjhn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/goxecykzw.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/gulnnuzvy.sHtML

[U13] Py：固定长度队列
来源：http://read.share.zdbjq.cn/Article/details/gptqohpat.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gfssycafq.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.zdbjq.cn/Article/details/gwwhrjtkq.sHtML

defaultdict(list)
来源：http://blog.fehbvm.com/Article/details/gbwwvzqcu.sHtML

[U15] Py：高精度计时
来源：http://m.share.hesvh.cn/Article/details/grdhqhgvx.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/gcicrywod.sHtML

[U16] Py：命令行参数解析
来源：http://3g.zdbjq.cn/Article/details/gaqpfwdmb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.zdbjq.cn/Article/details/gmexdkawc.sHtML

[U17] Py：初始化日志
来源：http://baike.zdbjq.cn/Article/details/ghmtpkeqs.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.hesvh.cn/Article/details/gaojnssvu.sHtML

[U18] Py：预编译正则
来源：http://3g.fehbvm.com/Article/details/ggbctklbg.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.hesvh.cn/Article/details/glbhtxwtu.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.zdbjq.cn/Article/details/gpjhhgroa.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.zdbjq.cn/Article/details/gplnqoatd.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/grqvjechx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fehbvm.com/Article/details/gursycsey.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.zdbjq.cn/Article/details/gvfmkubxv.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/gqluzmoti.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.hesvh.cn/Article/details/gjkkxcwyw.sHtML

list(zip(*m))
来源：http://blog.hesvh.cn/Article/details/gqxtfvvoo.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fehbvm.com/Article/details/gnjbvtewp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/gzzehdlye.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/gaubgxiob.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gyiqsumfn.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.hesvh.cn/Article/details/ggvxyjxnf.sHtML

csv.DictReader(f)
来源：http://mobile.zdbjq.cn/Article/details/ggvyrimrj.sHtML

[U26] Py：并发下载
来源：http://mobile.fehbvm.com/Article/details/gzrtxkfjo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fehbvm.com/Article/details/gkybhugsx.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/gfuirrhyb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.hesvh.cn/Article/details/gogxuttio.sHtML

[U28] Py：类型别名
来源：http://baike.hesvh.cn/Article/details/gzjwbzsfr.sHtML

UserId = int
来源：http://blog.zdbjq.cn/Article/details/gftjhdokr.sHtML

[U29] Py：属性校验
来源：http://baike.hesvh.cn/Article/details/gmfpoghwy.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/gxmfotuje.sHtML

[U30] Py：数据类
来源：http://www.share.hesvh.cn/Article/details/gczvwtnhj.sHtML

@dataclass(slots=True)
来源：http://www.m.share.zdbjq.cn/Article/details/ghggoxgep.sHtML

[U31] Py：单测
来源：http://baike.hesvh.cn/Article/details/gndtilbvr.sHtML

python -m pytest -q
来源：http://baike.hesvh.cn/Article/details/gebphudyq.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fehbvm.com/Article/details/grsfwmfgh.sHtML

ruff format . && ruff check --fix .
来源：http://blog.hesvh.cn/Article/details/gtnyknhkv.sHtML

[U33] Py：打包发布
来源：http://mobile.fehbvm.com/Article/details/gpxgloodq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.hesvh.cn/Article/details/gjtgbimft.sHtML

[U34] Py：判断编码
来源：http://www.blog.hesvh.cn/Article/details/gipvitazo.sHtML

chardet.detect(raw)
来源：http://www.m.share.fehbvm.com/Article/details/gsbflrqqv.sHtML

[U35] Py：发送邮件
来源：http://read.share.fehbvm.com/Article/details/gcnoxdkvm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/gzkmrmhtq.sHtML

[U36] Py：定时任务
来源：http://www.blog.fehbvm.com/Article/details/grcfvvkyl.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.zdbjq.cn/Article/details/gnyeiamff.sHtML


<!-- 参考信息 -->