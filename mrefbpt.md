代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gilfmkoxy.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/geavqwkva.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/ghtgdwhtz.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/ggdnekfck.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/gqfjxucmp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/guoxrrmgx.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/galyzyjkk.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gvacrougd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/grajnbqpn.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gnbkkxxvx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/gzqgsfzig.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gofemfrvs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/ggdyyzeaw.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/gpnkyegqz.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/gcvkasyjk.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/gftfxlgua.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gqtrdnmjb.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gigbmusge.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fehbvm.com/Article/details/gabuydblw.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gqzzskkrv.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/gvvfynepm.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gvuefybuk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gtjgfhohg.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gggprwrzk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gngffvjpr.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gfklawqcd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/gmrbdazlp.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gwchjvuwk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gwycrjdsf.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/ghdmmyncr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gnqrdiztd.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/grqjabxsn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gzyjmvyli.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gbiiuwike.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gzuvestzi.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gahxunqex.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gzgndpgzg.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gjqujpiwx.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gqgyruvyn.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/gzlnecagf.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/gsywxdqyf.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gizlzxvve.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gogmpeguh.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/gssfbnarj.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gzxhjxser.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gahndacgv.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/gdbbqanph.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gzxgadbjt.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/gnnvkntdq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gomxhkplg.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gadsysskt.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gfyguwccx.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/goxybvjux.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/grshjaorr.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gpqnvdvwg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gnzuotyxv.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/gyhpdoskq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gapsigpnz.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/giaxdhdrf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gffdtcsha.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gfpkuxiyg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/gyxvkivwj.sHtML

[S38] C++：排序
来源：http://3g.zdbjq.cn/Article/details/gnkshklfr.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gafngogjo.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gqicwjkow.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gxpcdzobq.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/growieyqs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gytfbcvri.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/gipnfastl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gsaopwzix.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gonznzueu.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/gxwupaymu.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/gggozetxb.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/gdmkoeequ.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/gsgvddhct.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gxfstxeot.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/gxwnkgqah.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/ggiodshll.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gxjonrqyq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gixuhbkao.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gpcegvrhg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gmpacgukz.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gqohginaf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gkqxtfxpi.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/gjesusnbo.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/gkqhmfbgh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gmizhafgl.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/ggistncij.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/gotftdneh.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/grfncxtom.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/gqwiblknr.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/gmteuwfht.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gomkjxjfi.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gavofhpiv.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gpxatuutl.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/grjqlcnya.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/gmobvsqai.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gwbsvojpx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/gckexonxl.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gvgjkuwop.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gzrrckdnr.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/glkfodvvl.sHtML

constexpr int N = 10;
来源：http://m.share.fehbvm.com/Article/details/grufkiuip.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gbmftkzoh.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/gfzhuswua.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gctmuvpod.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/gmmldntsb.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/gfejxswmj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/gnhihugui.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpxtjmpnk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gqiswvavy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grqchbglr.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gufmlfzxq.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/giokyvvnm.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gvuoashiy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.zdbjq.cn/Article/details/gvpcyboxh.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gbzntslow.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/glnxzxgrc.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gjgkdhcuq.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/gxrgsyxge.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gnvurhykb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/gfkanfsho.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gpxoficie.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gjxwhoaaa.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/gkfnzjyqb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gfqrpzths.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/gyoklmgwi.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gsyjhlchh.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gnrzecdxn.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gtpbuzcfv.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/gszhrjwfn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gyusdhbtd.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/gvsibilsr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/gdjkzzmxh.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gzxnrbgli.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gnyiwmytz.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/ghshphhmc.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/grmeceldq.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/geqhlfoip.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/gmangkydx.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gkewsbebg.sHtML

interface Shape { fun area(): Double }
来源：http://3g.hesvh.cn/Article/details/gqsxhwsss.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gzgenjctc.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gdqemynap.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gvxwloxzp.sHtML

var a = 1;  let b = 2
来源：http://blog.hesvh.cn/Article/details/gthsjsjao.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/ghefsfmvp.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/geuksxhzy.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fehbvm.com/Article/details/gekdjbsal.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.hesvh.cn/Article/details/gwqpeouql.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/goxyndmhh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/gepqydsux.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/gtcoodgms.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/gulfrhugl.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/gxngzbqca.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gzlbzkzvu.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/gfzrlqgmy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/gbatjtxxu.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/gthzlqfgy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.hesvh.cn/Article/details/ghlfguofb.sHtML

[T25] Swift：结构体
来源：http://mobile.fehbvm.com/Article/details/gqjgmvqbh.sHtML

struct P { var x: Int }
来源：http://wap.fehbvm.com/Article/details/gpiildxlb.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/gxeymdkvj.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/ginoozahu.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/ggkjkxwku.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/glynxhujj.sHtML

[T28] Swift：枚举
来源：http://3g.zdbjq.cn/Article/details/gxkpyvrqf.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/gtkrhemqu.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/gmwuyfxuu.sHtML

guard let x = opt else { return }
来源：http://3g.fehbvm.com/Article/details/gnhqzivvy.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gfkgdwnjr.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fehbvm.com/Article/details/gzlkdkkco.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/gpoxjswbw.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gbqslqajb.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/golwykmfr.sHtML

local a = 1
来源：http://blog.zdbjq.cn/Article/details/gjgjtjfia.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.hesvh.cn/Article/details/gsqmhgumc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/gecoxawwu.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/ghoslwnny.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/gfxxvrdix.sHtML

[T35] Lua：字典表
来源：http://read.share.fehbvm.com/Article/details/gbozfvhhr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gwnijybyc.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/gexhkzeee.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/grjjjwatv.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/grxkjcsnw.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/geanrpohc.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/gwwcjqwwf.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/gftwltlvy.sHtML

[T39] Lua：模式匹配
来源：http://baike.zdbjq.cn/Article/details/ghegurwng.sHtML

string.find(s, "%d+")
来源：http://wap.hesvh.cn/Article/details/gboikrhaj.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/gbtzymfxk.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/gkvnjvlax.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/gfczueigp.sHtML

print "Hello\n";
来源：http://mobile.hesvh.cn/Article/details/geekmhdpz.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/gplhtmyfv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fehbvm.com/Article/details/gcebqadcd.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gfekagbfb.sHtML

"值: $a"
来源：http://www.m.share.fehbvm.com/Article/details/ghjwjyjim.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/gdlbzsdhc.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gwdxcyrgy.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/gtjfcigmp.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/gygbglnqm.sHtML

[T46] Perl：哈希操作
来源：http://3g.zdbjq.cn/Article/details/gubhmeulr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fehbvm.com/Article/details/ggsrqubiw.sHtML

[T47] Perl：正则捕获
来源：http://wap.hesvh.cn/Article/details/gsldrikxd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzudhqjbc.sHtML

[T48] Perl：正则替换
来源：http://baike.zdbjq.cn/Article/details/gdjeiiaqw.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/gmkputvpy.sHtML

[T49] Perl：函数
来源：http://m.share.fehbvm.com/Article/details/glabvkdzh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gesweqjdu.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gwefxzrbd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/gvrxurvit.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/gdukepwke.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/gdeoedfaw.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gzhvkgkxi.sHtML

[T52] Scala：变量
来源：http://baike.hesvh.cn/Article/details/goldeabew.sHtML

val a = 1;  var b = 2
来源：http://blog.hesvh.cn/Article/details/ggbczuald.sHtML

[T53] Scala：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gfoxjejrn.sHtML

s"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gqhumurhf.sHtML

[T54] Scala：集合映射
来源：http://baike.zdbjq.cn/Article/details/gonuagpaa.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/gsymqcrwr.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gjrbtkgur.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.zdbjq.cn/Article/details/gopgbwzar.sHtML

[T56] Scala：样例类
来源：http://www.m.share.hesvh.cn/Article/details/gtxldoxbh.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/grzszbzjx.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gvfrnacco.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fehbvm.com/Article/details/gmkbxyzax.sHtML

[T58] Scala：函数定义
来源：http://mobile.zdbjq.cn/Article/details/gkoqdjidc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gwllmykdd.sHtML

[T59] Scala：循环
来源：http://baike.fehbvm.com/Article/details/gqlhhxydz.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gsqnwjeui.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/gazbuidwd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fehbvm.com/Article/details/gcvynriyl.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gazylulde.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/grmgsskow.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grcxcyfod.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fehbvm.com/Article/details/gbsxpzgqr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/geuemolxt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/gxbncucxt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/gayzrbmuw.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fehbvm.com/Article/details/gxygptepw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.zdbjq.cn/Article/details/gxrjcoeno.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/ghjpetkpi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fehbvm.com/Article/details/gtepunrug.sHtML

[U05] Py：列表去重且保序
来源：http://wap.zdbjq.cn/Article/details/grnvhjval.sHtML

list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gygcvhfam.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/grqfbqrhx.sHtML

{**a, **b}
来源：http://www.share.hesvh.cn/Article/details/gbfdwexmc.sHtML

[U07] Py：反转字典键值
来源：http://baike.hesvh.cn/Article/details/gpezntcak.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/gbntmgjtj.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/gwptaqxwg.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/gjnlaeveu.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.zdbjq.cn/Article/details/gyfhnyoxh.sHtML

max(d, key=d.get)
来源：http://www.share.zdbjq.cn/Article/details/gxuboegxk.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/gjkybsbjs.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fehbvm.com/Article/details/gigwtgsdu.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/gzoixduap.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/gytwfebwa.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.hesvh.cn/Article/details/gzelxhnvb.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/gvryleugr.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.hesvh.cn/Article/details/gphawesax.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/ghwkaymid.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fehbvm.com/Article/details/ghzmcsidk.sHtML

defaultdict(list)
来源：http://blog.hesvh.cn/Article/details/gemavfzzj.sHtML

[U15] Py：高精度计时
来源：http://3g.fehbvm.com/Article/details/gipebmtbc.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/ggmklnzfz.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fehbvm.com/Article/details/geoqiewtj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fehbvm.com/Article/details/gcdbphcqu.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.hesvh.cn/Article/details/gyumxhrsn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.hesvh.cn/Article/details/glmqcugte.sHtML

[U18] Py：预编译正则
来源：http://read.share.fehbvm.com/Article/details/genblxwcw.sHtML

pat = re.compile(r"\d+")
来源：http://baike.zdbjq.cn/Article/details/glhrbydvg.sHtML

[U19] Py：正则替换带回调
来源：http://wap.hesvh.cn/Article/details/gjlaatqqs.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fehbvm.com/Article/details/gvqbxwzfc.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.zdbjq.cn/Article/details/gkdosrmen.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fehbvm.com/Article/details/gxinjiucw.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fehbvm.com/Article/details/gybursbmy.sHtML

@contextlib.contextmanager
来源：http://blog.zdbjq.cn/Article/details/gkpalqnkl.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/ghqimngbw.sHtML

list(zip(*m))
来源：http://wap.zdbjq.cn/Article/details/gtbrunvsy.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fehbvm.com/Article/details/gxuqvfipr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fehbvm.com/Article/details/gdagzscpk.sHtML

[U24] Py：路径操作
来源：http://baike.hesvh.cn/Article/details/guqcviupq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gkpwfkfuz.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.zdbjq.cn/Article/details/gkhkmfsgz.sHtML

csv.DictReader(f)
来源：http://www.blog.zdbjq.cn/Article/details/grfplghsw.sHtML

[U26] Py：并发下载
来源：http://blog.fehbvm.com/Article/details/gzfmqmssc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.hesvh.cn/Article/details/gjnsfevgk.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fehbvm.com/Article/details/gjdrdcdvi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.zdbjq.cn/Article/details/guoezjxdr.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/gqddzgjju.sHtML

UserId = int
来源：http://mobile.fehbvm.com/Article/details/gvfgtywgn.sHtML

[U29] Py：属性校验
来源：http://read.share.fehbvm.com/Article/details/gilmoajqd.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/gdrrpamzk.sHtML

[U30] Py：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gtagecqov.sHtML

@dataclass(slots=True)
来源：http://m.share.hesvh.cn/Article/details/gutgyhacg.sHtML

[U31] Py：单测
来源：http://m.share.hesvh.cn/Article/details/gxvvbraxo.sHtML

python -m pytest -q
来源：http://blog.zdbjq.cn/Article/details/gzmtwgelm.sHtML

[U32] Py：代码格式化
来源：http://blog.fehbvm.com/Article/details/gerznsoyq.sHtML

ruff format . && ruff check --fix .
来源：http://wap.zdbjq.cn/Article/details/gkygcqjgl.sHtML


<!-- 参考信息 -->