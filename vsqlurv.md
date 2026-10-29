代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/ghusnhysi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/graqkcbge.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/glsvqjxbq.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/ggxyktuzj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/gajikfcvb.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gxprgecoa.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gbuyzadzw.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/genzycbgt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gqpiuyzsp.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/golvnsisz.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gvoruxpkl.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gosmugudx.sHtML

x |= (1 << 3);
来源：http://www.blog.hesvh.cn/Article/details/gpcgherjm.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gcubocmlc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/getpmesxo.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gcaacesxb.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gufpqlilr.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gzusntrqq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/ggnaquflh.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gvazhfhhp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gvydtheec.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/gdmfnlohq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gcdthbkmw.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/gswurfhxn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gjtenzslu.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gidbxzhxp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/gmijkolqf.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gkzpyeldq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/gmgikhipa.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/guyqfjecq.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gyzaunrbt.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/grpegzbsb.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gwmrpalcp.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gcfolgbmv.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gldjolyhm.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/gwxdlumfs.sHtML

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/gapwshcce.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gxzelfclc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fehbvm.com/Article/details/gtcbnuxne.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gzshgalma.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/ghyeymmle.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gxyulosez.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/ggjkwskya.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/giemtynxf.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gjtxrolzh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/gwsdjyofl.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/ghgnjpnca.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gfqoxrebn.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/grgufbcrg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/gmgzrqsnk.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/glhajpmic.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/gdrerfyrh.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gkcfqptox.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gmyvohxad.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gfpaktsnk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/givckzniu.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/gjjhmkwkd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gdtnkxiyc.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gbdsuqsfx.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gnvsxsoeg.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/gdeonlnmq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/glmmykdbp.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gyemtiibv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gpjqvuegl.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/gyskaeznq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/gwggozxvk.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/gdxbxknfe.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/ggzzswhil.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gxwoelcuc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/glisjmjbc.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/ggmcyddbz.sHtML

void inc(int &x) { ++x; }
来源：http://baike.hesvh.cn/Article/details/gkogbzrmy.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gejoqxnxw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/guwgkvgxz.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/gjdxojlev.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gmdnirtdu.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/gotweaswz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gkwilwvng.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gaghumdvb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gxedipbhm.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/giljpeoah.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/goluovaye.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/gomztwyix.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/gguzayxuk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/gthjrcntj.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/ggfnjmzua.sHtML

static_cast<double>(a) / b
来源：http://m.share.zdbjq.cn/Article/details/gxidtwclh.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/ghqplinpp.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fehbvm.com/Article/details/gqmxpczuu.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/gkrwxtsru.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gruhpdgui.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/gmhwzrvfd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gphxaurkb.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gnkbldnxs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gfvlxbxel.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gidwzinrf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/goitkiazz.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/ghzwfxxto.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gknvtfnuq.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gbwkcgqmq.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/glkkzzanf.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/gbfzgshii.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/gdluztqxn.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/gdxkejaih.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gbrpyfjkp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gaiotupwf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gzyfrcozy.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxgtqvspn.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/gpdmceitj.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/giffjmnlq.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gttnyvdhd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/gcyozzank.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/geqzhhtxm.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gdszrgife.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gfnzpojul.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/gpuetdswq.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gxzoosrok.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/gsevmdekl.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/gscissqez.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gnjidxayk.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gdaobxxhm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/gedqhvsro.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/gbwzzrshm.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gikthgxcn.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/gkowjhzum.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gubqhkwva.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/guwbrlbrd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/gylduhgbp.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/gcezqyjlw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/grlahhlqn.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/gdbzuvnbi.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gfrtbceox.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/goabitikg.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/gtpltgoco.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/gronaffpm.sHtML

for (i in 1..10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gmiuiybre.sHtML

[T15] Kotlin：接口
来源：http://3g.fehbvm.com/Article/details/gfarfrqtg.sHtML

interface Shape { fun area(): Double }
来源：http://3g.hesvh.cn/Article/details/ganqtmdqw.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gyxyomope.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/ghkqbtqkr.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/glmqfcigb.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gsclhyvbv.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gxnpotnfh.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/gyajcptzz.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/gonkturbt.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/gwkegogep.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gzqphvcam.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gftjqrmpp.sHtML

[T21] Swift：遍历
来源：http://mobile.zdbjq.cn/Article/details/gzptynhxn.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/gzwxsikrl.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/ggorfsrzd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.zdbjq.cn/Article/details/gkorffmqo.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gwqdephql.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gyfjhnwgq.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/gaqsjsnkm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gndmvbrgk.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/gztcvbvwo.sHtML

struct P { var x: Int }
来源：http://m.share.fehbvm.com/Article/details/grkaecvge.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/geoswlxnb.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/gsbcptslx.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/geylkyggj.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/gsyhqbpxe.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gepnvjytx.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/goqlwzoxg.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/gpcuiwfvl.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/gffbywgdn.sHtML

[T30] Swift：协议
来源：http://baike.zdbjq.cn/Article/details/gnyzyapla.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gnkuapvqf.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/glukpcmxl.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gzfnlnzeq.sHtML

[T32] Lua：局部变量
来源：http://blog.zdbjq.cn/Article/details/gxpltchri.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/glozlzmxf.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/gqrspsrnj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/gsbggmuip.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/gagnougqc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.hesvh.cn/Article/details/giiyptqdd.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/gswnzhdwe.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gwaydwabg.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gxkzcvzwy.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/gvlytuinr.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/gytbhewwt.sHtML

"a" .. "b"
来源：http://www.blog.hesvh.cn/Article/details/gagptwayq.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/gcolkrubx.sHtML

if x > 0 then print("正") end
来源：http://read.share.fehbvm.com/Article/details/gjrxbgpxz.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gjxqjcmfd.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gpwixuwvm.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/gxiiysilo.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fehbvm.com/Article/details/gyyghmbcq.sHtML

[T41] Perl：Hello World
来源：http://read.share.fehbvm.com/Article/details/gmibvjwid.sHtML

print "Hello\n";
来源：http://m.share.zdbjq.cn/Article/details/gldheefph.sHtML

[T42] Perl：变量类型
来源：http://m.share.fehbvm.com/Article/details/gjcddoaxj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fehbvm.com/Article/details/glnelwewa.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/gbizemnea.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/grpbkwijt.sHtML

[T44] Perl：条件
来源：http://mobile.zdbjq.cn/Article/details/gkbmpfadv.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/gfirobxsx.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fehbvm.com/Article/details/gotiraonq.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fehbvm.com/Article/details/gdmzrprxq.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/gjcbinago.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghdswyyyq.sHtML

[T47] Perl：正则捕获
来源：http://blog.zdbjq.cn/Article/details/gnmssnewq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/gchrtgwxu.sHtML

[T48] Perl：正则替换
来源：http://read.share.fehbvm.com/Article/details/gvwqdkflq.sHtML

$s =~ s/old/new/g;
来源：http://3g.fehbvm.com/Article/details/gbawgjzba.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/gwewsezrx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/ggzginwhn.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gcvqjxjlc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.zdbjq.cn/Article/details/gacpcbrgq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/gugzljpbn.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gxbcfbnni.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gqukkbrnc.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gyvumjcuq.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/gifvgjtme.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fehbvm.com/Article/details/geqjxcqox.sHtML

s"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gqxjzuung.sHtML

[T54] Scala：集合映射
来源：http://3g.fehbvm.com/Article/details/geugpaaic.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/grjbeaqpy.sHtML

[T55] Scala：集合过滤
来源：http://3g.fehbvm.com/Article/details/gonlgladu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/gmlfecgns.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gmriccoau.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gsjedsfbl.sHtML

[T57] Scala：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gqppodmom.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.hesvh.cn/Article/details/gvxvwbbaj.sHtML

[T58] Scala：函数定义
来源：http://3g.hesvh.cn/Article/details/gjqyynhba.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fehbvm.com/Article/details/glfttvtov.sHtML

[T59] Scala：循环
来源：http://blog.fehbvm.com/Article/details/gyvlszynk.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gccmqopqh.sHtML

[T60] Scala：折叠
来源：http://read.share.hesvh.cn/Article/details/gdrwwtvma.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fehbvm.com/Article/details/gehtzqnqs.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/giyfiijxg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gjmclyget.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpeqqmrkk.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/gjwuaqtra.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fehbvm.com/Article/details/glvhsmxsx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.hesvh.cn/Article/details/gzuqthisa.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fehbvm.com/Article/details/ggliorllb.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fehbvm.com/Article/details/glfcbpfdx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.hesvh.cn/Article/details/gmtutiptu.sHtML

[U04] Py：变量调试打印
来源：http://read.share.hesvh.cn/Article/details/gkudfqvqd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.hesvh.cn/Article/details/gvhmnjtmr.sHtML

[U05] Py：列表去重且保序
来源：http://baike.zdbjq.cn/Article/details/gyqoppyga.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gevhtzfrj.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fehbvm.com/Article/details/giyqpiagq.sHtML

{**a, **b}
来源：http://m.share.zdbjq.cn/Article/details/ghiulbiqr.sHtML

[U07] Py：反转字典键值
来源：http://www.share.zdbjq.cn/Article/details/gebfcwofa.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fehbvm.com/Article/details/gohbkegah.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.hesvh.cn/Article/details/girovztif.sHtML

[y for x in nested for y in x]
来源：http://mobile.fehbvm.com/Article/details/gknlsekjj.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/gbjrfjsdu.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gkhpbhrsy.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fehbvm.com/Article/details/gzwgulnwe.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/gvttcnsgu.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fehbvm.com/Article/details/gmwpiooro.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fehbvm.com/Article/details/geudxsprx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/gdsmlmbah.sHtML

Counter(arr).most_common(3)
来源：http://mobile.hesvh.cn/Article/details/glhnonhvs.sHtML

[U13] Py：固定长度队列
来源：http://blog.fehbvm.com/Article/details/goztllqlk.sHtML

deque(maxlen=10)
来源：http://wap.hesvh.cn/Article/details/gkuncrtlb.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.zdbjq.cn/Article/details/ghhddxjlm.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/gjibzlwdu.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/gbybfplzu.sHtML

t = time.perf_counter()
来源：http://www.blog.zdbjq.cn/Article/details/gewwdrbst.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/gyvpacnne.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.hesvh.cn/Article/details/ghqkaursu.sHtML

[U17] Py：初始化日志
来源：http://blog.zdbjq.cn/Article/details/gpkhdlgqr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.zdbjq.cn/Article/details/gosgsjyfw.sHtML

[U18] Py：预编译正则
来源：http://mobile.zdbjq.cn/Article/details/gaxzvxrxd.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/gliwjqjip.sHtML

[U19] Py：正则替换带回调
来源：http://3g.zdbjq.cn/Article/details/gpvfhtmro.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.zdbjq.cn/Article/details/gnnlqqokx.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/gahjhqlka.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.zdbjq.cn/Article/details/gflnizbhr.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.hesvh.cn/Article/details/gkoxtqypv.sHtML

@contextlib.contextmanager
来源：http://3g.zdbjq.cn/Article/details/gydymzojp.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fehbvm.com/Article/details/gadipgshu.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/gvscqdlgh.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.hesvh.cn/Article/details/gktmnfnki.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.zdbjq.cn/Article/details/gmcyymdnl.sHtML

[U24] Py：路径操作
来源：http://m.share.hesvh.cn/Article/details/gykhxnvkv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gusudnptc.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/gnwltpqim.sHtML

csv.DictReader(f)
来源：http://read.share.zdbjq.cn/Article/details/gxjysgktr.sHtML

[U26] Py：并发下载
来源：http://blog.hesvh.cn/Article/details/gwsqltcmm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.hesvh.cn/Article/details/gjtuyobnf.sHtML

[U27] Py：异步 HTTP
来源：http://3g.zdbjq.cn/Article/details/gxalmebms.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.hesvh.cn/Article/details/gxqomxqut.sHtML

[U28] Py：类型别名
来源：http://www.m.share.zdbjq.cn/Article/details/gvnqrmykl.sHtML

UserId = int
来源：http://www.m.share.hesvh.cn/Article/details/gfunkmfvf.sHtML

[U29] Py：属性校验
来源：http://baike.hesvh.cn/Article/details/grtsptoyl.sHtML

@property 与 @x.setter 配合
来源：http://blog.fehbvm.com/Article/details/ghrrkauxv.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/gkowgbudx.sHtML

@dataclass(slots=True)
来源：http://3g.fehbvm.com/Article/details/gkscdpqsx.sHtML

[U31] Py：单测
来源：http://www.blog.hesvh.cn/Article/details/gmvpuuauh.sHtML

python -m pytest -q
来源：http://wap.fehbvm.com/Article/details/gfedlnsgx.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/gesfufkrn.sHtML

ruff format . && ruff check --fix .
来源：http://baike.hesvh.cn/Article/details/gdqdomjmn.sHtML

[U33] Py：打包发布
来源：http://read.share.hesvh.cn/Article/details/gqtsiwxoj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.hesvh.cn/Article/details/gkwxazmww.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/gmiilgaqf.sHtML

chardet.detect(raw)
来源：http://baike.hesvh.cn/Article/details/glmbjcgxe.sHtML


<!-- 参考信息 -->