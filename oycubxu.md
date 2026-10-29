代发 wailian999

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/gqzidlcvh.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/gpsnzldzt.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/grevscqmr.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/gyeckorom.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/gfypqvzjl.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/gvcddyetw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/gumprrnti.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.zdbjq.cn/Article/details/gipqtxkkl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/glevucfud.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/gxtrsjbid.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/gvcbygwcb.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gjcbidwvx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/gfqwvnufm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/guesjmdxz.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/giclgqayh.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gfeysbklz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gmzalhrqp.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gpswvytpi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gkyvtxbbg.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/ggxoomjpl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gncjgjlyc.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/gygovekes.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/giiqseedo.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/ggkzagcsm.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/gucemiqaw.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gjlinvvmb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gddkfzoao.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gzqjhrzeh.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/ghflajulg.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/gmdyatypn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gjmamdnov.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/gvwmlqqqk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gdzketcxe.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/ghiehevdh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/gduyrpahe.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gnbspbatz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gzprayzkp.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/gjbztdeze.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/gdfwwwixo.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gdtzrdpjy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gecobztcs.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/gabkjnwdb.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/gayhgnfqd.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/gqdcyiqpp.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/gpyqdcjzm.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gvvnfsqqm.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gasearbhl.sHtML

[S28] C：静态变量
来源：http://m.share.hesvh.cn/Article/details/gwwkyjncn.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/gtmooyuzy.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/geimvuvwo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/gnrwuiccg.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/gpjvgpncx.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gkqviifzs.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gabazrjhg.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/gxttiokkt.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gzmjactgu.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/gpfcyjimo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gwbqeqlxu.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gnrdanknl.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gmchqdqnn.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gxapnsaom.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/gxjzjhqfv.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gvzllvmcp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.zdbjq.cn/Article/details/gtybhtudk.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gvhwmuitw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gqbaxyyic.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gymhfjmvn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gujgzwsvx.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/ggpfwpqpc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/gpuqgmnjb.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/ghjripljc.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/ghudoxbou.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gywmwhmnt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gfvjxtqlb.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/gqqulybon.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/gltykhtkf.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/geijgywki.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/gxayesyxk.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/gfcoualwj.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/guioltvvg.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/glswnmvth.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/glaarhbhs.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/gobyncjca.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/gqvbfrxqq.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gtkxlersy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/guxdcgtbo.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/gacjctxnz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/gtokzcxjp.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gjbpirsbd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/goeiatlbt.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gzscnarvm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/gawabsqug.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/gxoobgccn.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/gpxzvrxuo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gdwabgnks.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/gueezscbh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gokwgmwky.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gwnajdhzv.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gdjjrjbip.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/golgdlpcc.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/geowbwzsv.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/gfggzwhex.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gwhgwdwzc.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/girjyikpo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gshkqatoc.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/gbpmsizjd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/gzaxtweik.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gxtfwqrkq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/glmfcifzs.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/gkatbppjl.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/ghypemcnp.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/glcrdmueg.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fehbvm.com/Article/details/gwecnyhfa.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/gjvioqvnl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/gwoojezzp.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/gebekqzga.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/gijkfzxiw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gostnhnka.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gwhftbawr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdyjmfxkh.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gsgyuocmj.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gzzhfzkql.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gsahtjdch.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.zdbjq.cn/Article/details/grgqivvyx.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/guxkqhqvp.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/grasckqzq.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/getfsubfi.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/gpfvbolbb.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/gwfiotgpf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/gltnaytib.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gwwivwwvx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/ggeyzmcyq.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gfbaihxca.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/goctimorg.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/gjykereom.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gesoecoel.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/ghynawzae.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gcwhqsslb.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/gjhowemzi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.zdbjq.cn/Article/details/gyxxfsjdu.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/gwcookzfn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fehbvm.com/Article/details/gpdqbxrdn.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/gerigxdhi.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gvpihyoqa.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/gtzehjnva.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gnpqnfuop.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/giqyyvvuu.sHtML

for (i in 1..10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gwhvgyibd.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/gauwuqvkd.sHtML

interface Shape { fun area(): Double }
来源：http://blog.zdbjq.cn/Article/details/goyxjzbde.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/gzuaaaekt.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gaamqkehn.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gkaznxqeb.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/glzlomcaz.sHtML

[T18] Swift：字符串插值
来源：http://blog.fehbvm.com/Article/details/grkrcovhg.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gsozgffdw.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fehbvm.com/Article/details/gautdbzdf.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gadqfwlke.sHtML

[T20] Swift：数组操作
来源：http://blog.zdbjq.cn/Article/details/gnhwpcbkd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/glwsnixrc.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/grcwhutgq.sHtML

for x in a { print(x) }
来源：http://www.m.share.fehbvm.com/Article/details/gcbhlxrmo.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/gsneofvmd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/glxlxqrlc.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/ggqciuexb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.hesvh.cn/Article/details/ggyuwefqf.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/gozpblyls.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/gkvxamthp.sHtML

[T25] Swift：结构体
来源：http://3g.zdbjq.cn/Article/details/gymdlrqtc.sHtML

struct P { var x: Int }
来源：http://wap.fehbvm.com/Article/details/gbvmauuut.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/ghjwpymfb.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/glvhcrahu.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/gkaocnddi.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/gaejewejh.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gvmrvecio.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/gdparjfnd.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gbjebnzvu.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/gmprdveir.sHtML

[T30] Swift：协议
来源：http://3g.hesvh.cn/Article/details/gakxgkslv.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/gfrdfzsno.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/gzqzevdfq.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gjvbhnqhw.sHtML

[T32] Lua：局部变量
来源：http://www.blog.hesvh.cn/Article/details/gvpvxinbw.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gtjqruvfv.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/gzanwnlxn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.hesvh.cn/Article/details/gncnnhuou.sHtML

[T34] Lua：遍历表
来源：http://blog.hesvh.cn/Article/details/ghxdurxaa.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/gjdqseiqs.sHtML

[T35] Lua：字典表
来源：http://read.share.fehbvm.com/Article/details/grelnedxn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/gjpswpsua.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/gvnxvechh.sHtML

function add(a, b) return a + b end
来源：http://mobile.hesvh.cn/Article/details/gwognqllh.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/grjtupyew.sHtML

"a" .. "b"
来源：http://read.share.zdbjq.cn/Article/details/gkexwqemo.sHtML

[T38] Lua：条件
来源：http://mobile.zdbjq.cn/Article/details/gmvwglgif.sHtML

if x > 0 then print("正") end
来源：http://www.share.zdbjq.cn/Article/details/ggwkipvaa.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fehbvm.com/Article/details/glciwfmcp.sHtML

string.find(s, "%d+")
来源：http://mobile.fehbvm.com/Article/details/gfmwonltl.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/gkcfkxkma.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fehbvm.com/Article/details/gbbzlgfsf.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gwelpdoye.sHtML

print "Hello\n";
来源：http://read.share.hesvh.cn/Article/details/glspmppdu.sHtML

[T42] Perl：变量类型
来源：http://www.share.zdbjq.cn/Article/details/ghigejozt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.hesvh.cn/Article/details/gsopshalv.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gcokyntpv.sHtML

"值: $a"
来源：http://www.blog.zdbjq.cn/Article/details/gwmcibytd.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/gfprsfpws.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.hesvh.cn/Article/details/gjjhxxjxg.sHtML

[T45] Perl：数组遍历
来源：http://blog.zdbjq.cn/Article/details/gaqrjivbt.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.hesvh.cn/Article/details/gjzqnyjuc.sHtML

[T46] Perl：哈希操作
来源：http://mobile.hesvh.cn/Article/details/gddpnwcrh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.hesvh.cn/Article/details/gpfgdltbe.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/gtlmcuxff.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/givagwwex.sHtML

[T48] Perl：正则替换
来源：http://www.blog.hesvh.cn/Article/details/gyyfrnlme.sHtML

$s =~ s/old/new/g;
来源：http://wap.hesvh.cn/Article/details/gzathpcyl.sHtML

[T49] Perl：函数
来源：http://wap.hesvh.cn/Article/details/gtoqumeqp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/ghyjdjuod.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gzxvrhwyq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.zdbjq.cn/Article/details/grcdqxpwh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/gitrfawhj.sHtML

[T51] Scala：Hello World
来源：http://3g.hesvh.cn/Article/details/gigcdgjib.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/grgugpsvp.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/gpxodiyye.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/gygrcmxnc.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/gngpydzuv.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gwtjnddit.sHtML

[T54] Scala：集合映射
来源：http://baike.zdbjq.cn/Article/details/gtvqqqomy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.zdbjq.cn/Article/details/gmexlisdp.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gjpcgqtjw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fehbvm.com/Article/details/gowzfsmgz.sHtML

[T56] Scala：样例类
来源：http://baike.zdbjq.cn/Article/details/gmgxvsaaw.sHtML

case class User(name: String, age: Int)
来源：http://wap.fehbvm.com/Article/details/gysjsknka.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gdowwrymm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.hesvh.cn/Article/details/gjreliznn.sHtML

[T58] Scala：函数定义
来源：http://3g.hesvh.cn/Article/details/gcmkluhsd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gwglkjvhi.sHtML

[T59] Scala：循环
来源：http://www.m.share.hesvh.cn/Article/details/gyemumyet.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/guahqucze.sHtML

[T60] Scala：折叠
来源：http://m.share.zdbjq.cn/Article/details/gzvbeexmw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fehbvm.com/Article/details/gccedjbuf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsdcjflbi.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gvaiuywcs.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnlevebfa.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.zdbjq.cn/Article/details/gkhzorvom.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fehbvm.com/Article/details/gbbkywsfu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/gjhysxqnx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.zdbjq.cn/Article/details/ggkuwvoth.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fehbvm.com/Article/details/gfzroxpwx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.hesvh.cn/Article/details/gqjoocnuw.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.hesvh.cn/Article/details/grafpmjju.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fehbvm.com/Article/details/gehpxuvnq.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fehbvm.com/Article/details/ggssprksu.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gdxclbvfl.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/gltxfwuuy.sHtML

{**a, **b}
来源：http://baike.zdbjq.cn/Article/details/gardbsetr.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/ggedqbojo.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.zdbjq.cn/Article/details/gjsnmvbcb.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/grfblziyc.sHtML

[y for x in nested for y in x]
来源：http://m.share.hesvh.cn/Article/details/gxlfwfktz.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fehbvm.com/Article/details/gkrwiloch.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gbertlyhj.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gnogfexuh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/gvdazjysu.sHtML

[U11] Py：生成器表达式
来源：http://baike.zdbjq.cn/Article/details/gooyqajaq.sHtML

(x * 2 for x in arr)
来源：http://m.share.hesvh.cn/Article/details/gtcyjwmyj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.zdbjq.cn/Article/details/gttczxtfc.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/gzpljxoow.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.zdbjq.cn/Article/details/gkjhzzala.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/gvnsbfzav.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fehbvm.com/Article/details/gxcsfrpxf.sHtML

defaultdict(list)
来源：http://3g.fehbvm.com/Article/details/gvcjfirgt.sHtML

[U15] Py：高精度计时
来源：http://m.share.hesvh.cn/Article/details/gsoblfrrb.sHtML

t = time.perf_counter()
来源：http://read.share.hesvh.cn/Article/details/goxyjhhmj.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.zdbjq.cn/Article/details/gfnbvkceb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/gthyrixhv.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/gtfgdulzv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.zdbjq.cn/Article/details/gdbjuytue.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/gxgtpuyry.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gkquxlmot.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.zdbjq.cn/Article/details/gxfvygpwj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fehbvm.com/Article/details/ggxielexr.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.hesvh.cn/Article/details/giunkaobm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.hesvh.cn/Article/details/gukegrigi.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/gfvwjyagg.sHtML

@contextlib.contextmanager
来源：http://3g.fehbvm.com/Article/details/gvvgvvfxi.sHtML

[U22] Py：矩阵转置
来源：http://www.share.zdbjq.cn/Article/details/gijyaxbwx.sHtML

list(zip(*m))
来源：http://wap.zdbjq.cn/Article/details/gkdakuryw.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.hesvh.cn/Article/details/gdmwjjusu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.hesvh.cn/Article/details/gvoiarobm.sHtML

[U24] Py：路径操作
来源：http://www.share.fehbvm.com/Article/details/gouzrqozw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gxtqwnxkm.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/gygrrochx.sHtML

csv.DictReader(f)
来源：http://m.share.zdbjq.cn/Article/details/gjbhafvia.sHtML

[U26] Py：并发下载
来源：http://mobile.fehbvm.com/Article/details/gjjxrczrm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fehbvm.com/Article/details/gksdacbbf.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fehbvm.com/Article/details/gfzysagtx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fehbvm.com/Article/details/gdedtlnmi.sHtML

[U28] Py：类型别名
来源：http://read.share.zdbjq.cn/Article/details/gekqnynbv.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/gdcdayuqz.sHtML


<!-- 参考信息 -->