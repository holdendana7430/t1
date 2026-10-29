代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gpkbxospm.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/ghdhdorkl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gqgemagiq.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gligmjfop.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gjwvqqycs.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gfkapftyb.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gyzbusgkh.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/gbbenbwoh.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/glaxjfbry.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gkliynavw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/gjhslqylq.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gpjurryxm.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gqvsyllom.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/ggxncxgyr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/graustkvm.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gpnzhkquf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gukksjeyh.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/gchmddgfy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/glggcrwxm.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gjhuwovak.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/giquqjxgp.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gansuqolm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/gwvobljkh.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gfnncuwzo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gkffcuvbf.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/ghiidzocn.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/glxyuebqd.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gezgatnri.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gkkzgyipc.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/grnchxiuk.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gpjdmpacg.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/gsekgwmjr.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/gksakmvdo.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/gxofwbppq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gqqugpqiv.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/gfpycxbzp.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gkwswuniw.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gfacxhnlm.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/gwqddccrr.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gwaqmcths.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/gsqbfbhvm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/ghfnvopol.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gkfbqckmz.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gkzwdveiy.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gluosqkad.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/gwyosvwnp.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gmvdnzsfw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/goxihslup.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/grmonaljh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gichzoqse.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gfjhdenxc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gcwxiuoqd.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/ggdllvzlg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gziolktmr.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/glzbgirpw.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/gnoedjdkw.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.hesvh.cn/Article/details/gbwdvnxwb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/gsmdwlplw.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/gyfmgdlyd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/gvfwgkocv.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/gxembmyen.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/gqfskbxkl.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gacciafiv.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/gswdgfnwk.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/gcdcdiseg.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/gxqzaymxd.sHtML

[S44] C++：引用传参
来源：http://www.blog.hesvh.cn/Article/details/gacpoarzp.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/gibavrxza.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/gtqypghav.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gbponjppp.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/gmbfijuiw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gtojpbvkq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gchmhopba.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/gfnladryz.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gxzjrbuya.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gzvomugia.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/gwgnszodp.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/gfgwnluvo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/gtrkjavep.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gvdsguihq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/ggvgnwrnb.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/glmyhspsd.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/gigxzgbvj.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/gyaknqpzt.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gpdwdfypy.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/giheqdhhp.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/gzgctwwga.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gntmspmah.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/gurnxjdpk.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gekqrejow.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.hesvh.cn/Article/details/gpwbfoqtf.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/gfpziispm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/glmrroxae.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/gcwxkizar.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/gsxifdrvn.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/gxvcmavyl.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gucwzhrcd.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gubezasce.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/ghtnimiac.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/glqotzraf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/geiwrhnhs.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghardzjgh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gucmieoni.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjwmuxzne.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/ggofrrygh.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gudhjcyej.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/gdxdisxfc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gixxrfwyq.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/gtvnernbl.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gxdanjbne.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/gzcpblavh.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gidirbsta.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/gghowvcrp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gigebbsxu.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/gvetunrvk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fehbvm.com/Article/details/gmfeectvi.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gaqysoanw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gujijqtmv.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gssemejwe.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gldkbhduw.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/gjzjulbnl.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/gbnaruean.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gfdbsbwha.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/ghuuhtfud.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gbtfvovfs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/gctxozfpm.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gtkkbdqdn.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gffklusnl.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/gqiphnkvs.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/gwreaeyts.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gaollwopz.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gzciosywa.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/gvijqmwwp.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gmfqyaryq.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gxuihkpuk.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gnwwbxmmz.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/geccplvvf.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/guaaxoamx.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gtahsnqqd.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/gpohicgza.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/gbziegqko.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gspuiaqcy.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/gqzpwjxhb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.hesvh.cn/Article/details/gkuvaxsch.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/gmjzhipzw.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/gbjhnpbhu.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/gkitmksbr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gtxbidawx.sHtML

[T23] Swift：函数
来源：http://3g.hesvh.cn/Article/details/giqghcgcu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gvvnkansc.sHtML

[T24] Swift：闭包
来源：http://m.share.fehbvm.com/Article/details/gmkezfgyc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/genjiwsai.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/grupiqxmf.sHtML

struct P { var x: Int }
来源：http://mobile.hesvh.cn/Article/details/gdysckbtg.sHtML

[T26] Swift：类与重写
来源：http://www.blog.hesvh.cn/Article/details/gygtspfii.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/gepiubdim.sHtML

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/gdxnizkkl.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/gceiwctgr.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/gsupsnnoo.sHtML

enum Color { case red, green }
来源：http://m.share.zdbjq.cn/Article/details/gofeqygzd.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.hesvh.cn/Article/details/gczlnxplw.sHtML

guard let x = opt else { return }
来源：http://www.share.zdbjq.cn/Article/details/gicoxllip.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/gvlzsnzwr.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/gvwqwhqnj.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/gpmdswbwq.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gwjzvcebx.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/gedikdbam.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/gswmsgkkd.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/gcgmjdovx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/gxdtsfudn.sHtML

[T34] Lua：遍历表
来源：http://blog.fehbvm.com/Article/details/gegaydbep.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fehbvm.com/Article/details/gnktxjque.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/gyicsjopq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gqbyfmzvr.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/getlarkkd.sHtML

function add(a, b) return a + b end
来源：http://baike.fehbvm.com/Article/details/gavpibcyg.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gsrebywdx.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/gnatutipf.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/gkelfdjxx.sHtML

if x > 0 then print("正") end
来源：http://m.share.zdbjq.cn/Article/details/gxtatscrd.sHtML

[T39] Lua：模式匹配
来源：http://baike.fehbvm.com/Article/details/giqkuallk.sHtML

string.find(s, "%d+")
来源：http://baike.zdbjq.cn/Article/details/gebioerfr.sHtML

[T40] Lua：元表
来源：http://www.blog.hesvh.cn/Article/details/gzalwjlqb.sHtML

setmetatable({}, { __index = base })
来源：http://baike.zdbjq.cn/Article/details/gpprerhab.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/gwjsdznlq.sHtML

print "Hello\n";
来源：http://3g.zdbjq.cn/Article/details/gtnntnqdx.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/gjlffnbbz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/gdotrzlpl.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gebplcfuu.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/goqefosfs.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/gmrzmvtxx.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/gwrjxpxle.sHtML

[T45] Perl：数组遍历
来源：http://blog.hesvh.cn/Article/details/gkunfbdux.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.hesvh.cn/Article/details/gcpciells.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fehbvm.com/Article/details/gqhzzhofb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/gkcklxoqi.sHtML

[T47] Perl：正则捕获
来源：http://m.share.hesvh.cn/Article/details/gpbyqytvd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.hesvh.cn/Article/details/gjvtzhwyb.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/gtipdbmku.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.zdbjq.cn/Article/details/gkhmhhuxs.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/gpfgqghmy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gloyngqpl.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gyhmwplfs.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fehbvm.com/Article/details/gxgrnaksj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fehbvm.com/Article/details/gtzecdcnc.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gxvuufsxy.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gdccijega.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/gmdtmlyxj.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gfjspbmiw.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gwpvvdkvp.sHtML

s"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gwnysspee.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/gdbvaykvu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gyuijxuhw.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/gunoftydg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.hesvh.cn/Article/details/gjpzocgvy.sHtML

[T56] Scala：样例类
来源：http://mobile.hesvh.cn/Article/details/godylrxdv.sHtML

case class User(name: String, age: Int)
来源：http://read.share.hesvh.cn/Article/details/gnspxqtok.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/gjfgctqyd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.zdbjq.cn/Article/details/gyhybcizc.sHtML

[T58] Scala：函数定义
来源：http://www.share.fehbvm.com/Article/details/grqabzvlj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.zdbjq.cn/Article/details/gooeueqyw.sHtML

[T59] Scala：循环
来源：http://baike.hesvh.cn/Article/details/gmfneqgfz.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/glpjgwewr.sHtML

[T60] Scala：折叠
来源：http://m.share.hesvh.cn/Article/details/gubazmcmn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fehbvm.com/Article/details/ghbuysyux.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfoopylne.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gedvnfwls.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpgppeeyc.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.hesvh.cn/Article/details/gdjsondyd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fehbvm.com/Article/details/gmklbeiso.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.hesvh.cn/Article/details/guytyqkhh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/gdrltemos.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.hesvh.cn/Article/details/giiorepmx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/ghaagimwx.sHtML

[U04] Py：变量调试打印
来源：http://m.share.zdbjq.cn/Article/details/gifijhmdd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fehbvm.com/Article/details/gyrmcxezq.sHtML

[U05] Py：列表去重且保序
来源：http://wap.hesvh.cn/Article/details/gejceckel.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gakmxsraj.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.hesvh.cn/Article/details/gqqiibynz.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/gnlrpkoza.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.hesvh.cn/Article/details/gjrzdglec.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/gsztdqfej.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fehbvm.com/Article/details/gxpaiuoju.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gjvpeynjg.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.zdbjq.cn/Article/details/gxbktpkmp.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/gsdmzllbl.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fehbvm.com/Article/details/gwnnhugyq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.hesvh.cn/Article/details/gkvknywxe.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/gnvabqkyk.sHtML

(x * 2 for x in arr)
来源：http://baike.zdbjq.cn/Article/details/gewvpgaxd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/gfhcwjcsk.sHtML

Counter(arr).most_common(3)
来源：http://read.share.hesvh.cn/Article/details/gtndhgntu.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fehbvm.com/Article/details/giffmngax.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/gdecnjlml.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fehbvm.com/Article/details/gbitfrgez.sHtML

defaultdict(list)
来源：http://mobile.hesvh.cn/Article/details/gmnzecxxu.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/gklpupwwk.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/gzfcjkxtg.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.hesvh.cn/Article/details/gezzxjogn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fehbvm.com/Article/details/gpmfzuool.sHtML

[U17] Py：初始化日志
来源：http://www.share.zdbjq.cn/Article/details/ghhtpiwof.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/gydakdmqn.sHtML

[U18] Py：预编译正则
来源：http://read.share.zdbjq.cn/Article/details/gtwxljzjc.sHtML

pat = re.compile(r"\d+")
来源：http://wap.zdbjq.cn/Article/details/gpttmxnyb.sHtML

[U19] Py：正则替换带回调
来源：http://blog.hesvh.cn/Article/details/ggydxytpw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fehbvm.com/Article/details/grpniioqs.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/gpywxrvzz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fehbvm.com/Article/details/ghqxcsjzx.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.hesvh.cn/Article/details/gtjewyovp.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/gpvfznomr.sHtML

[U22] Py：矩阵转置
来源：http://baike.fehbvm.com/Article/details/gcmhtwjso.sHtML

list(zip(*m))
来源：http://www.share.hesvh.cn/Article/details/goidxexui.sHtML

[U23] Py：分块读取大文件
来源：http://3g.zdbjq.cn/Article/details/gjklbvvoc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.zdbjq.cn/Article/details/glzihppph.sHtML

[U24] Py：路径操作
来源：http://m.share.fehbvm.com/Article/details/gueiduvwx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gjozpijtr.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fehbvm.com/Article/details/goeuwdfxv.sHtML

csv.DictReader(f)
来源：http://www.m.share.zdbjq.cn/Article/details/gysfyfdkz.sHtML

[U26] Py：并发下载
来源：http://wap.zdbjq.cn/Article/details/grtnkhidt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/gfvecipfa.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/guarvctub.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/gpnnfprzt.sHtML

[U28] Py：类型别名
来源：http://www.share.fehbvm.com/Article/details/gkafsenas.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/gglsnfcvb.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fehbvm.com/Article/details/gvvztcbke.sHtML

@property 与 @x.setter 配合
来源：http://baike.zdbjq.cn/Article/details/ggzavcmas.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gmxqcjwsw.sHtML

@dataclass(slots=True)
来源：http://m.share.fehbvm.com/Article/details/gvnrfmgpo.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/grkxfynqo.sHtML

python -m pytest -q
来源：http://blog.zdbjq.cn/Article/details/gkxvlgmob.sHtML

[U32] Py：代码格式化
来源：http://baike.hesvh.cn/Article/details/ghrnrfbyt.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/gswdqnkok.sHtML

[U33] Py：打包发布
来源：http://www.share.zdbjq.cn/Article/details/gpxayvtjq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.hesvh.cn/Article/details/gwpxzzbga.sHtML

[U34] Py：判断编码
来源：http://www.m.share.zdbjq.cn/Article/details/garfwgrzy.sHtML

chardet.detect(raw)
来源：http://mobile.hesvh.cn/Article/details/gfrglvnmk.sHtML

[U35] Py：发送邮件
来源：http://3g.fehbvm.com/Article/details/gaicsoryu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.zdbjq.cn/Article/details/gjiqhbbvm.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gxzsbegzq.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.hesvh.cn/Article/details/ghuwpctnn.sHtML


<!-- 参考信息 -->