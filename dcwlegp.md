代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/grtlvroyr.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/gbmxvxycg.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gwusbhdyk.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gkpqiyfny.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gumrzellx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gvoeddmax.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gyatwugua.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gpzaphind.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gpbkckweo.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gnqyjseju.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/gafluwtlb.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gmwwzxbic.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/gyayyocff.sHtML

[S15] C：类型转换
来源：http://wap.zdbjq.cn/Article/details/grvukmkpf.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/ggcbviten.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gwrhpkfum.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/gsqoxpkrm.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gbszelysl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/gkigseatg.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gnbezhktp.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gmgqdwimp.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/gweemspus.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gubbuujpq.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gwfuhktpb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/grshyvwsf.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gposrhqmv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gxdgluqvm.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gnrbmudqh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gwjugbclc.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/glzwyvndo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gascfprdo.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gozueqiqh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gugptphom.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/gbnprfkdn.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/gghnwylzk.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/gtbilqwll.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gqeykeljz.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/gsgajdoet.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gpvebpdyz.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/gwhsyeubl.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gvbqfswiv.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/gzqwdjinu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/gbuacprtj.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/gqbnynlir.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/grmuiqcnw.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gmvrnjuvh.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/gqkaeinog.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/gcocjdnsg.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/guubsgyiu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gysszhaqr.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/ghlpgmziw.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gxlkniaza.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gvovyeggs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/grihxftho.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gxjgrorzx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/gvxktcdzy.sHtML

[S35] C++：map
来源：http://read.share.hesvh.cn/Article/details/gcdrhtdrj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/guohzbkhu.sHtML

[S36] C++：unordered_map
来源：http://wap.fehbvm.com/Article/details/gsbbtsrhy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/guhtikkxr.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gcifriwzo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gmwwodwfd.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gczkwndee.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/gjddjdauw.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gowcfudjg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/gkqeosdzv.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/ghmbykkjy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/gewyigpoh.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/gzsmsfytq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/grqsaynib.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gingqydzz.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fehbvm.com/Article/details/gzcwxjehf.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/geukivlbb.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gzoeczbci.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/grfmesbpb.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/gtzgzhanf.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/gepgplgez.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gxnrstngt.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/gagzomnwq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gosimalhy.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gvrpjkjxy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/gtirgzxnd.sHtML

[S48] C++：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gbeboratc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/gtrpzvjwu.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/giunzjlpx.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/geajnilkw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.hesvh.cn/Article/details/gothqpmmg.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gbebcimke.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/ghjycefyu.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/gwjuxnhmt.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gxugrptql.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/giubaacwi.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gihaxhbqx.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/gnjsgtqct.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gprewuysg.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gdsifxdif.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/gfmydogrz.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/gngkgolhj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gbnonfwxv.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gwurzwhks.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gwszfutxx.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/glgpqzjjx.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gqvnbngcb.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/glgkyytdr.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/gvgttkssw.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/gqshderrw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/gdsobznml.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/ggeugmfiw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gleixlavx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/guzupgrlk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gxyilwajw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghyobiwvm.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gydrohknu.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gvbgyggxh.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/grepxtcku.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gymafvvyi.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/gfsxuswxr.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gkklqoshu.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/gqwdzubwb.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/genpkwlzq.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/ggptvdeqp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gebujnijd.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/gsynbldzd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/gfeehyeuh.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gamurqhau.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gjmhzuvna.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/gkexkxxka.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gvgajzvje.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gboeioggk.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/gnxotvniz.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gkgteopht.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fehbvm.com/Article/details/goirkvamq.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/glfdyxakd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/ganhapvru.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gezpangyu.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gpkofqyuf.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fehbvm.com/Article/details/gvnlodteg.sHtML

val m = mapOf("a" to 1)
来源：http://3g.zdbjq.cn/Article/details/gvevmqvle.sHtML

[T14] Kotlin：循环
来源：http://3g.hesvh.cn/Article/details/glabxlnqm.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gcpyhlrbp.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gkyiftvku.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/gfahwjmfd.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/goutvvbai.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gvberkiot.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/gkdhbteju.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/gzyowwxve.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gnlzqzhwd.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/gtwrlmawu.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gcssnhiwu.sHtML

if let n = opt { print(n) }
来源：http://baike.zdbjq.cn/Article/details/gqlreqjkx.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/ggapyccka.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/gmtiesnpa.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/gprwwdeda.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/gfxshrfkc.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/giufskzzg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gegixwifx.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/ghljnungl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.zdbjq.cn/Article/details/gyubbvvps.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/gsqkgbibw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gjwfsowzf.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/ggareyfvg.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/gpkzlucav.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/gsudkoskl.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gytmtntja.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/gejoweukc.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/gnbqrpqpf.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gtzdbvpda.sHtML

enum Color { case red, green }
来源：http://www.m.share.hesvh.cn/Article/details/gzdsunmqj.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/gtzekpfub.sHtML

guard let x = opt else { return }
来源：http://m.share.zdbjq.cn/Article/details/gecrtarjh.sHtML

[T30] Swift：协议
来源：http://3g.fehbvm.com/Article/details/gmnufwicb.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/gzgoxyxuc.sHtML

[T31] Lua：Hello World
来源：http://www.share.hesvh.cn/Article/details/gazgtenlr.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/godawlurs.sHtML

[T32] Lua：局部变量
来源：http://wap.zdbjq.cn/Article/details/gtgrayfyn.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/gxewswoql.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/gibbcjkpi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/gvpdtxztv.sHtML

[T34] Lua：遍历表
来源：http://www.blog.zdbjq.cn/Article/details/gwlxawwlx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.hesvh.cn/Article/details/gflldmzaz.sHtML

[T35] Lua：字典表
来源：http://wap.hesvh.cn/Article/details/grcargmvq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/giluoxjmi.sHtML

[T36] Lua：函数
来源：http://3g.fehbvm.com/Article/details/gecvhnufd.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/gwjfefrev.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gjltihseq.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/gyivqtoco.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gtwdjjsgb.sHtML

if x > 0 then print("正") end
来源：http://mobile.zdbjq.cn/Article/details/gnvtgsswu.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gccrysqwr.sHtML

string.find(s, "%d+")
来源：http://3g.zdbjq.cn/Article/details/gexcawhio.sHtML

[T40] Lua：元表
来源：http://3g.hesvh.cn/Article/details/gohsybcen.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fehbvm.com/Article/details/grfeaxmjq.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gqjdmkxpt.sHtML

print "Hello\n";
来源：http://mobile.fehbvm.com/Article/details/gfjfokvcf.sHtML

[T42] Perl：变量类型
来源：http://mobile.zdbjq.cn/Article/details/gqfnrsitg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/grgbjjkfr.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gtgtkjomd.sHtML

"值: $a"
来源：http://www.blog.fehbvm.com/Article/details/gzsfiiqud.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/gmkacxhfj.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/gznievram.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/gyrhlmuop.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fehbvm.com/Article/details/ggnqzkjei.sHtML

[T46] Perl：哈希操作
来源：http://blog.hesvh.cn/Article/details/gqckvitqv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fehbvm.com/Article/details/glxuzgwab.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/gvnozjyhl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/gmvbbldad.sHtML

[T48] Perl：正则替换
来源：http://www.share.zdbjq.cn/Article/details/gvvdxvwpj.sHtML

$s =~ s/old/new/g;
来源：http://3g.hesvh.cn/Article/details/gvstfrgxk.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/gphqwrvzs.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gdlekrlmz.sHtML

[T50] Perl：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/glkeqtvdc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.hesvh.cn/Article/details/gqghgctew.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/glfjjyynk.sHtML

[T51] Scala：Hello World
来源：http://blog.hesvh.cn/Article/details/ggabkoarf.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gphfcmtaz.sHtML

[T52] Scala：变量
来源：http://www.blog.fehbvm.com/Article/details/gqusuzfoj.sHtML

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/grfnsthnf.sHtML

[T53] Scala：字符串插值
来源：http://3g.zdbjq.cn/Article/details/ggcogslkv.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gtafutpct.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gxgbmxzoo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/giidbekau.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gmzcxjxbz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fehbvm.com/Article/details/gucybdbem.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gmynscowl.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gumzuussb.sHtML

[T57] Scala：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gtdrdjfaf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.hesvh.cn/Article/details/gucroedje.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/gcprmqeau.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.hesvh.cn/Article/details/glyiiomuq.sHtML

[T59] Scala：循环
来源：http://mobile.hesvh.cn/Article/details/gwxmoeggd.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gzqjvjnlf.sHtML

[T60] Scala：折叠
来源：http://m.share.hesvh.cn/Article/details/goygzzpqu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/gubfejzer.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gumaauvjt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gnfprqvsu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmtdtyemq.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/gzqtaltxr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.zdbjq.cn/Article/details/ghhmvyldt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fehbvm.com/Article/details/givjfawku.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.hesvh.cn/Article/details/gjathfqpg.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/gwhwcnzbl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.hesvh.cn/Article/details/ggdwwexfj.sHtML

[U04] Py：变量调试打印
来源：http://mobile.zdbjq.cn/Article/details/ghgcwihda.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fehbvm.com/Article/details/gicphuemi.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/gysugxdvf.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gltkqxhsu.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/glrijuefa.sHtML

{**a, **b}
来源：http://3g.fehbvm.com/Article/details/gnfkygnpg.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/grgtkedfh.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/ganuqgori.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/gozumtxqi.sHtML

[y for x in nested for y in x]
来源：http://www.share.fehbvm.com/Article/details/gzdmgokji.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.zdbjq.cn/Article/details/gbdgpxwmr.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/gxunkgvhp.sHtML

[U10] Py：按值排序字典
来源：http://baike.zdbjq.cn/Article/details/goqfpubbe.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/gbbnoypbb.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/giukgenkt.sHtML

(x * 2 for x in arr)
来源：http://baike.zdbjq.cn/Article/details/gfzsnnttc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/gniaflgus.sHtML

Counter(arr).most_common(3)
来源：http://m.share.zdbjq.cn/Article/details/gtbpygfls.sHtML

[U13] Py：固定长度队列
来源：http://blog.fehbvm.com/Article/details/glpjbzsax.sHtML

deque(maxlen=10)
来源：http://read.share.fehbvm.com/Article/details/gsprdtanq.sHtML

[U14] Py：分组收集到列表
来源：http://3g.hesvh.cn/Article/details/gmzelwjzb.sHtML

defaultdict(list)
来源：http://www.share.fehbvm.com/Article/details/gkvucxxvb.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/giirsxmvb.sHtML

t = time.perf_counter()
来源：http://mobile.zdbjq.cn/Article/details/gohksgqhh.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.zdbjq.cn/Article/details/geskkkgoq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.zdbjq.cn/Article/details/gammqxzlz.sHtML

[U17] Py：初始化日志
来源：http://www.share.zdbjq.cn/Article/details/gwhwjjaoz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fehbvm.com/Article/details/guktavsak.sHtML

[U18] Py：预编译正则
来源：http://read.share.hesvh.cn/Article/details/griwihiop.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fehbvm.com/Article/details/grqtvkxfj.sHtML

[U19] Py：正则替换带回调
来源：http://baike.zdbjq.cn/Article/details/gtbvllokf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.hesvh.cn/Article/details/gcdabnkfo.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/gcwaqxvni.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fehbvm.com/Article/details/gfknmxldn.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/gxudmbecs.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/grnxkvaeo.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fehbvm.com/Article/details/gmggvslze.sHtML

list(zip(*m))
来源：http://www.share.zdbjq.cn/Article/details/gtizmidek.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.zdbjq.cn/Article/details/gydyahrao.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.zdbjq.cn/Article/details/grjywbahg.sHtML

[U24] Py：路径操作
来源：http://www.blog.zdbjq.cn/Article/details/goopakfqq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gkyiomfxu.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/gnczvgnle.sHtML

csv.DictReader(f)
来源：http://www.blog.zdbjq.cn/Article/details/gmdnqghhd.sHtML

[U26] Py：并发下载
来源：http://www.share.zdbjq.cn/Article/details/gbojrtzyz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/gwfdrdnsn.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fehbvm.com/Article/details/gahnlnrhb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fehbvm.com/Article/details/gnfpjufar.sHtML

[U28] Py：类型别名
来源：http://read.share.zdbjq.cn/Article/details/gszttbcaw.sHtML

UserId = int
来源：http://wap.fehbvm.com/Article/details/gymqubrfe.sHtML

[U29] Py：属性校验
来源：http://baike.zdbjq.cn/Article/details/gaoccvmde.sHtML

@property 与 @x.setter 配合
来源：http://read.share.zdbjq.cn/Article/details/gbyipnlvl.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/grjwbjqyf.sHtML

@dataclass(slots=True)
来源：http://read.share.hesvh.cn/Article/details/gkmlnfmls.sHtML

[U31] Py：单测
来源：http://m.share.hesvh.cn/Article/details/ghkaopdil.sHtML

python -m pytest -q
来源：http://baike.fehbvm.com/Article/details/gxubymezm.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/gzoxuiccr.sHtML

ruff format . && ruff check --fix .
来源：http://3g.hesvh.cn/Article/details/geuzrmtmw.sHtML


<!-- 参考信息 -->