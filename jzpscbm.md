代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fehbvm.com/Article/details/gmokrjmcy.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/geghrrxvu.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gzfjvbqek.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gbuymoggx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gpbbwvgpi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gnvoijzek.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gdkfmwtwd.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gwbznykqa.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/gpkszlugo.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/gwvnfrrfp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/goicxedrw.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/ghibdbxye.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gemprrckx.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/ggbjfnwyg.sHtML

(double) a / b
来源：http://www.m.share.hesvh.cn/Article/details/gtuxhxzwh.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/ggtcnqbyf.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/grdnjevxq.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gualzaufz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fehbvm.com/Article/details/gqphvejyy.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gwehzmrud.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/gouusgfgi.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/gupipwwvk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gsylmwcxv.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gshrlvhmw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gwjzepsmj.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gsbqyrchn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/gxrscdbrc.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gfqbltiqq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/gqewnsdzi.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gaagzaygu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gaigwxjmt.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/ghsqzimjc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gdsvbsmjx.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/gpqkryxiw.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gwdlrsipd.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/ghnbjeyuw.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gvrwluidn.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gpgjcjbth.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gggrxunna.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gpeumrpdw.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/gukenjykk.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/gnxifgsxy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gkujhyyza.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/gxzsjqcxp.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/gsellwysg.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gxuasvcva.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gaeerxqjj.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/ggrtwboja.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/gnyxabiho.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gjfxofzub.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/gqodxpisy.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/ghmmzwutk.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gebqzkcpm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gifmomzbq.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/gxlxjpioq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gydzxyxgc.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gfashgost.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gjpsnpkaq.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/gfhbouksv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gyjpgwwzn.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gprizgwyu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gtgsowcqj.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gadbagyts.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gpmdbpapq.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gneumanyn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/gmekpnonp.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/ghylejprr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gyxgccwuo.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/gxbubalbi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fehbvm.com/Article/details/gooxtfmfd.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/gbqjqteaq.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gcnsplhnk.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gajbndewu.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/giuqufryf.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gaqtpwelp.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gqkmdrunn.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/gpryjrtlw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gjycacvye.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/gvyxbgxkj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gpiczdaut.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/galmliyuj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gdzhffuoq.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gczixilel.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/graasipjr.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/gxodcygds.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/ggxtpyluh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/grbqavqaw.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gxbijupzt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/ghymiwjkk.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/grewbdfyt.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/grcdrozue.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gbhkoabrl.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/gfygfuzpv.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/gntqjreye.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gbjvumuky.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/gunzjztgg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/gdcucocza.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/gczwpvxdk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gkzzeczwz.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/guqcajnrz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/gkkkmfnhm.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/gmtispxee.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/gsyoizgqs.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/gtcfatdva.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/glvfbcjhn.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gmfuborfr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/grwsiwhuy.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gegbemxsa.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gyizqwvtw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gktssgvof.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gmcoymhgr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/goscistxi.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gkuomwyad.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/guaujdwyl.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gqtwogfrw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gfirxwtwo.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fehbvm.com/Article/details/gxfhwpcpt.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gjaizstom.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/geewnxsiy.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/grpyrmqkz.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/gnluiximb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/gmqngfjfb.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gzkkdkmtr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gjcuxrxux.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gcyzhnqjw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/gzostdjfz.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gdfecemkb.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gfaydfpvb.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/gkqhuokvb.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/guykuucia.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/gmnukvrnf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/ggodsrfwd.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/grznffqum.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/gnfcbrgco.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/gvrjnugfw.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gphtuzcwn.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/gfhylttjt.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/gxfmlhgzl.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/ggoiqmpjo.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/gycnwwmgj.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gcvoakdek.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gjiuadriz.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/giqipbalt.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gndnqxizm.sHtML

[T17] Swift：变量与常量
来源：http://m.share.hesvh.cn/Article/details/gfqjwxvnx.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/ggtbtudji.sHtML

[T18] Swift：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gvgabqzvt.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/guumghjpo.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/ghjzwyfjn.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/ghjgljmdh.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/gtzbseqnq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.zdbjq.cn/Article/details/gzlspgbyl.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/getjgdshv.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/gdygqvzzl.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gmmgotowq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/gwrwgdonc.sHtML

[T23] Swift：函数
来源：http://m.share.zdbjq.cn/Article/details/gbiyijjkj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/goofflunt.sHtML

[T24] Swift：闭包
来源：http://read.share.zdbjq.cn/Article/details/giuqbptzs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gyqanvpiw.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/gciuptwto.sHtML

struct P { var x: Int }
来源：http://blog.zdbjq.cn/Article/details/gxmtoizoo.sHtML

[T26] Swift：类与重写
来源：http://3g.hesvh.cn/Article/details/gqzzjefgl.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/gyhfmlidv.sHtML

[T27] Swift：错误处理
来源：http://baike.zdbjq.cn/Article/details/gtxqlvesm.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/gxlstlwks.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/gztskecrq.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/gydonxhdz.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.zdbjq.cn/Article/details/gporfkokg.sHtML

guard let x = opt else { return }
来源：http://3g.fehbvm.com/Article/details/gioypkbbq.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/gvmwcbccg.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.hesvh.cn/Article/details/gtkhqejtm.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/ghjbufxwh.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gomqfwyjd.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/gillgecgu.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/gqijowlgx.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/gmjeyokbj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/gesejobwf.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gzodfcdsr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.hesvh.cn/Article/details/glocvgfeq.sHtML

[T35] Lua：字典表
来源：http://blog.fehbvm.com/Article/details/gwsrkesbf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/gulkqazvp.sHtML

[T36] Lua：函数
来源：http://baike.zdbjq.cn/Article/details/gomnxaoot.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/gttnyvisw.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gfrsfnudz.sHtML

"a" .. "b"
来源：http://www.share.fehbvm.com/Article/details/gxvdiniik.sHtML

[T38] Lua：条件
来源：http://www.share.zdbjq.cn/Article/details/gekhmawxw.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/gwfasvmrh.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/gyxqmakgp.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gaklkcdhv.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/gcxslklgl.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.hesvh.cn/Article/details/gpqtzhjmz.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/gqqxzfbim.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/grczgoumb.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/ggtjndohd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/gdaxhyddm.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/giivdbkqa.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/gsvrwjlil.sHtML

[T44] Perl：条件
来源：http://read.share.zdbjq.cn/Article/details/gjljwoytu.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.zdbjq.cn/Article/details/gefdyupwc.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/gxioprmoy.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/glcduzqlk.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/gbqtibiph.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/gsltodfzj.sHtML

[T47] Perl：正则捕获
来源：http://mobile.zdbjq.cn/Article/details/ggizhyskq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.hesvh.cn/Article/details/gqytnhpdk.sHtML

[T48] Perl：正则替换
来源：http://baike.zdbjq.cn/Article/details/gomklbrnk.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gknkhzhjm.sHtML

[T49] Perl：函数
来源：http://read.share.hesvh.cn/Article/details/gvvizunsi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/ggidwzozl.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gmmvfolhc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.zdbjq.cn/Article/details/grpsucbbo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/gxqikheez.sHtML

[T51] Scala：Hello World
来源：http://3g.hesvh.cn/Article/details/glyblvsek.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gbsblxfag.sHtML

[T52] Scala：变量
来源：http://baike.zdbjq.cn/Article/details/gumkbogda.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/gujdjkrwo.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gupjykczu.sHtML

s"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gpprmwjro.sHtML

[T54] Scala：集合映射
来源：http://baike.zdbjq.cn/Article/details/gkhsrttoh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/gmjxwhpla.sHtML

[T55] Scala：集合过滤
来源：http://blog.hesvh.cn/Article/details/gvimbnoau.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/gkxmlhaae.sHtML

[T56] Scala：样例类
来源：http://www.blog.zdbjq.cn/Article/details/gvkotjwhi.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/gafbpiynn.sHtML

[T57] Scala：模式匹配
来源：http://baike.hesvh.cn/Article/details/gpzzuupet.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fehbvm.com/Article/details/gouuefvts.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/gagrjjcii.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fehbvm.com/Article/details/gmiudiuwj.sHtML

[T59] Scala：循环
来源：http://mobile.fehbvm.com/Article/details/gbheqrhun.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gqbdnyozd.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/gpkzdivrx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gtwzglrwg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gakkzlwnh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gdjzdekvl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvbsarbcd.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.zdbjq.cn/Article/details/gfxbsvmfl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/gzuugifpd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/gsisiilpf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fehbvm.com/Article/details/gezhwjprg.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.hesvh.cn/Article/details/gmbsqykgp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/gcmiaaxhq.sHtML

[U04] Py：变量调试打印
来源：http://baike.zdbjq.cn/Article/details/giuvehdof.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/glpzgvmlo.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/gxfvgozrj.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/grzkvxucr.sHtML

[U06] Py：合并两个字典
来源：http://read.share.zdbjq.cn/Article/details/gqmbrrbhh.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/gdbdrscvx.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/gjmdizxkh.sHtML

{v: k for k, v in d.items()}
来源：http://baike.zdbjq.cn/Article/details/gdmkburkw.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.zdbjq.cn/Article/details/guccfwhdz.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/gmymphtut.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fehbvm.com/Article/details/goygpijsq.sHtML

max(d, key=d.get)
来源：http://www.m.share.zdbjq.cn/Article/details/gyaoxxtil.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/gvfqqczzy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fehbvm.com/Article/details/gzosovxas.sHtML

[U11] Py：生成器表达式
来源：http://baike.zdbjq.cn/Article/details/gxjjzzpxf.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fehbvm.com/Article/details/gsoyszldb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/gisrursco.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/guqgrrqqp.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.hesvh.cn/Article/details/gggepcsxd.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/gqetcbjed.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.zdbjq.cn/Article/details/ggmobxxlv.sHtML

defaultdict(list)
来源：http://www.share.hesvh.cn/Article/details/gaqcxenxl.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.zdbjq.cn/Article/details/gmyrfzglf.sHtML

t = time.perf_counter()
来源：http://www.share.hesvh.cn/Article/details/gzcizlrwt.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.zdbjq.cn/Article/details/gjhhmkhwn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/ggmntmcwq.sHtML

[U17] Py：初始化日志
来源：http://3g.fehbvm.com/Article/details/gglrvitfk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.zdbjq.cn/Article/details/ghxrfzzub.sHtML

[U18] Py：预编译正则
来源：http://blog.zdbjq.cn/Article/details/gwqverxmq.sHtML

pat = re.compile(r"\d+")
来源：http://wap.zdbjq.cn/Article/details/gzgdfahih.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.hesvh.cn/Article/details/gheazfrbr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fehbvm.com/Article/details/gozobcgzy.sHtML

[U20] Py：缓存函数结果
来源：http://3g.zdbjq.cn/Article/details/gzfhjhmhq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fehbvm.com/Article/details/gobvgadch.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.zdbjq.cn/Article/details/gblexdyyd.sHtML

@contextlib.contextmanager
来源：http://read.share.hesvh.cn/Article/details/gvwmebkmy.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fehbvm.com/Article/details/gdtvtgcvn.sHtML

list(zip(*m))
来源：http://read.share.hesvh.cn/Article/details/gwabaeueq.sHtML

[U23] Py：分块读取大文件
来源：http://baike.hesvh.cn/Article/details/gudwdnrgi.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fehbvm.com/Article/details/ghdeajmau.sHtML

[U24] Py：路径操作
来源：http://read.share.zdbjq.cn/Article/details/gloaxraoz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gqtjjyiiu.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.hesvh.cn/Article/details/gqvbpeiwb.sHtML

csv.DictReader(f)
来源：http://baike.zdbjq.cn/Article/details/gwrdvdaid.sHtML

[U26] Py：并发下载
来源：http://mobile.zdbjq.cn/Article/details/gbazeutyk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.zdbjq.cn/Article/details/gxjdiqprq.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.hesvh.cn/Article/details/gbpqyhynr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.hesvh.cn/Article/details/gcgrqhijs.sHtML

[U28] Py：类型别名
来源：http://m.share.zdbjq.cn/Article/details/gqhwoqdha.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/gfruptovw.sHtML

[U29] Py：属性校验
来源：http://www.m.share.zdbjq.cn/Article/details/ggpfwvxzb.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.zdbjq.cn/Article/details/ghccgudqz.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/gbebhtxaf.sHtML

@dataclass(slots=True)
来源：http://mobile.hesvh.cn/Article/details/gldlniqxj.sHtML

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/gzjznzysw.sHtML

python -m pytest -q
来源：http://mobile.hesvh.cn/Article/details/gomehwugt.sHtML

[U32] Py：代码格式化
来源：http://baike.zdbjq.cn/Article/details/gycoajmus.sHtML

ruff format . && ruff check --fix .
来源：http://baike.hesvh.cn/Article/details/gxqykniab.sHtML


<!-- 参考信息 -->