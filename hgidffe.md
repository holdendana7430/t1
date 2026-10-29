代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gkyzfaqbj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gkaclfmxt.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gnigwkftq.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gvwxpyjvn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/gakzrmsrl.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/glznjanpt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/gresgvtln.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/gpglyowfh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gyhgwzcdg.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gfyccsosd.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gkbymcaxn.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/ggaporuyl.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/ghdvmhsfl.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gsipjyjlh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/gealkiowe.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/gdbkmrjop.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/grwswhyww.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gjzexpynt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gxcpkataj.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gxmuzqzvy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gcamfmeek.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/gpfxbhnui.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/ggawhunou.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/guvbfzycb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/gygjhchwc.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gtwufrnil.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gdegpelax.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/gmqdrmhns.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gwpprpsqu.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gvdcjjpkg.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/gvedbsunv.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gtlnctzyn.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/geslwkupi.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gcouqdirm.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/ggyjksisn.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/gyzqkbjoq.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gutnuflgu.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gtfyuunnc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gznbhyzjm.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/ggyiluuqm.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gdcxrljjx.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gsngilymi.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gvwjzafkl.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/gwgsebzms.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/govqoutaz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fehbvm.com/Article/details/gkgrjvejf.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gcriizzgt.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gqopyatlv.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gpxkxqhmn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gkqeuyhms.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gvnkppawb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.zdbjq.cn/Article/details/gafqcniql.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gigbhixyu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gnsbkbvid.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/gkaluyzuu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gnqpbkqac.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gmlanjrwg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gcheceoon.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/gxzxcqhib.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gcngtlmju.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.zdbjq.cn/Article/details/geqjixnhi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/ghslvdfwj.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/gvznxrwol.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/giwdputcv.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/gfqghhuyd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/gdkkhegan.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/giqvubpou.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gistsigqe.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/geidhleqt.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gmjmbysuy.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/ghaymbzno.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gafynjwda.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/ggvuoakka.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/gnxoxzlkq.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/gikmsqigw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/gymgxirxk.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/gnybcivcf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.hesvh.cn/Article/details/gwuvxcysd.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gnsvnxlei.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/geulmqjym.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/ggrkgyhqv.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gqzwsiwvn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/gbqhdaies.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/gehkrdsat.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gjufphfas.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/goygnyetb.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/ggtotqnfa.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/gzukhyock.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gfcyramjf.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/gdgmfzftv.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/glwvvrmhd.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/gpmhwdcnc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/gbmcayydi.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/gmdutlrio.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gfychmlyw.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gcmuiywrh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gcambeyky.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gaaqmpwci.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/gltgpsfmo.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/gvjcelxot.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/gncrwqwge.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gzvukdupg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gonfiynqk.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/gfvnrddfv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/ghhqmhgkd.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gczzcvnuy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gglkwtpuf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzuootusi.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gggjsldmw.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/ghvoznwck.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/gqsymlpeo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/gctvzizyc.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gxmypntzb.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/gzsemigxp.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/ggfowxvrs.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gbdgojyvq.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/gpbbohsaf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.zdbjq.cn/Article/details/gwlrtcjkx.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/gavtxbbcv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gwdgwrawa.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gzonuqhat.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gmhebfsrn.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gelfnaxnp.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gjrgiwkpp.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gcithsuoi.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.zdbjq.cn/Article/details/gozoihdjz.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/gswzwbfsj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gqqtmpjcl.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/gmuwoqjkx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gxcehnvnj.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.hesvh.cn/Article/details/giejkxcpn.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/gzvevznrb.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/gelwjmxom.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/gvntaqess.sHtML

[T14] Kotlin：循环
来源：http://blog.zdbjq.cn/Article/details/gegqtftwd.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gbruvbles.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gzvxtrrjq.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/gkiyugroa.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/ggzpoiutw.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gnnyytyun.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/gslrbkoil.sHtML

var a = 1;  let b = 2
来源：http://mobile.zdbjq.cn/Article/details/gxnawnioh.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gdvneblag.sHtML

"值: \(b)"
来源：http://www.m.share.zdbjq.cn/Article/details/gllazobsi.sHtML

[T19] Swift：可选绑定
来源：http://read.share.hesvh.cn/Article/details/gthxyynfa.sHtML

if let n = opt { print(n) }
来源：http://3g.fehbvm.com/Article/details/gxjnnycnm.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/gqxrlwgpi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/gizkbpqag.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/gtrxupzfu.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/gofcyslpy.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/grtgnttxb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.zdbjq.cn/Article/details/gezjbjhog.sHtML

[T23] Swift：函数
来源：http://www.blog.hesvh.cn/Article/details/gmtbhfbbc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gijnbehll.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/gpegctjhf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fehbvm.com/Article/details/gqucbdemv.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/ggvzmulhk.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/grrolqoji.sHtML

[T26] Swift：类与重写
来源：http://blog.fehbvm.com/Article/details/gcybhrive.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/ggrqsrlde.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gpcwktxnt.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/gpbkjwawk.sHtML

[T28] Swift：枚举
来源：http://mobile.zdbjq.cn/Article/details/gmabwlsvo.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/gawyljpnu.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.zdbjq.cn/Article/details/gwqhvuukh.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/ghlwqeieb.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/ggcxfeyvv.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fehbvm.com/Article/details/gjpurpfrp.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/gqvsmobxn.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/genojicub.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gblownytp.sHtML

local a = 1
来源：http://3g.fehbvm.com/Article/details/gqmjhvynw.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.hesvh.cn/Article/details/gapdzmdya.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fehbvm.com/Article/details/ghezkkhtx.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/gkskyuecz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fehbvm.com/Article/details/gkxcfmupf.sHtML

[T35] Lua：字典表
来源：http://m.share.hesvh.cn/Article/details/griknbrpj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.zdbjq.cn/Article/details/gskqttqgr.sHtML

[T36] Lua：函数
来源：http://mobile.hesvh.cn/Article/details/gxfemgmmd.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/gfaytnppo.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gvgximfet.sHtML

"a" .. "b"
来源：http://read.share.zdbjq.cn/Article/details/gynglfvvw.sHtML

[T38] Lua：条件
来源：http://read.share.fehbvm.com/Article/details/ggmlwgvsv.sHtML

if x > 0 then print("正") end
来源：http://m.share.fehbvm.com/Article/details/guohopiow.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/ggpbtdpgw.sHtML

string.find(s, "%d+")
来源：http://baike.zdbjq.cn/Article/details/galhjelnz.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/gxeiohobd.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/glidnzfrh.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/gkrhurpfg.sHtML

print "Hello\n";
来源：http://baike.fehbvm.com/Article/details/gwecdsjnk.sHtML

[T42] Perl：变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gvmfvudks.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.hesvh.cn/Article/details/gsjorydfu.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gxphtikvi.sHtML

"值: $a"
来源：http://read.share.fehbvm.com/Article/details/graodxphe.sHtML

[T44] Perl：条件
来源：http://www.blog.zdbjq.cn/Article/details/ghmembodr.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.zdbjq.cn/Article/details/glupzvcqf.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/gqjzlhdbw.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/gtmwsmcnc.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gzvupjbgr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/gokdtxnci.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gyvtvrhvm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/gxwkqnoif.sHtML

[T48] Perl：正则替换
来源：http://read.share.fehbvm.com/Article/details/gwyeksepf.sHtML

$s =~ s/old/new/g;
来源：http://blog.hesvh.cn/Article/details/gmhzloksz.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gdalwukcz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gfucgpxvw.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/guknsjaiu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.hesvh.cn/Article/details/gujozpbib.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/ghhzsuuux.sHtML

[T51] Scala：Hello World
来源：http://blog.hesvh.cn/Article/details/gtoesfqcy.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gubmlvqtt.sHtML

[T52] Scala：变量
来源：http://blog.zdbjq.cn/Article/details/gtpkwnxqk.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/gvbvqeemn.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/ginjahntq.sHtML

s"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gbhfjozww.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gvzhhzvei.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/grnsjrzar.sHtML

[T55] Scala：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gvpxxsnto.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.zdbjq.cn/Article/details/gpduddwqh.sHtML

[T56] Scala：样例类
来源：http://mobile.fehbvm.com/Article/details/gygwtfrqw.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/gkmyhofbv.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gkbzcgofi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.hesvh.cn/Article/details/gtdotzchy.sHtML

[T58] Scala：函数定义
来源：http://read.share.zdbjq.cn/Article/details/gewqvblbr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fehbvm.com/Article/details/glfsirjzr.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/gojozctkb.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gihabracq.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/glkigqtqe.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.zdbjq.cn/Article/details/gtyozvcqn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gavdgesik.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gufinbjcj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/genfkkpbp.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.zdbjq.cn/Article/details/gzhbjofej.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/gfgojeyur.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.zdbjq.cn/Article/details/gniyodmcs.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fehbvm.com/Article/details/gynofywxx.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.hesvh.cn/Article/details/gfsdvoffz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.zdbjq.cn/Article/details/gnmfkawzj.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.hesvh.cn/Article/details/glcyjvxpa.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.hesvh.cn/Article/details/gmfcsynba.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/gialmuzhs.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gljvpsreg.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.zdbjq.cn/Article/details/gqiryzcjt.sHtML

{**a, **b}
来源：http://baike.zdbjq.cn/Article/details/gdwnplrdy.sHtML

[U07] Py：反转字典键值
来源：http://m.share.hesvh.cn/Article/details/ggbctsuxu.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fehbvm.com/Article/details/gddjcooqm.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.zdbjq.cn/Article/details/gnzgtjhrv.sHtML

[y for x in nested for y in x]
来源：http://wap.hesvh.cn/Article/details/gxgwsmfgf.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.zdbjq.cn/Article/details/gmqumuzke.sHtML

max(d, key=d.get)
来源：http://blog.zdbjq.cn/Article/details/gdueogzhy.sHtML

[U10] Py：按值排序字典
来源：http://wap.fehbvm.com/Article/details/gqsscnrbc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/gzrcvaqvc.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/ghlqwsnrx.sHtML

(x * 2 for x in arr)
来源：http://wap.fehbvm.com/Article/details/gcoxmsfrs.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.hesvh.cn/Article/details/ghnrhsyop.sHtML

Counter(arr).most_common(3)
来源：http://m.share.hesvh.cn/Article/details/glamgsfxo.sHtML

[U13] Py：固定长度队列
来源：http://3g.zdbjq.cn/Article/details/ghexnskqu.sHtML

deque(maxlen=10)
来源：http://3g.hesvh.cn/Article/details/gqkkgoumz.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.hesvh.cn/Article/details/ghgohobcu.sHtML

defaultdict(list)
来源：http://www.blog.hesvh.cn/Article/details/gmnzsyuka.sHtML

[U15] Py：高精度计时
来源：http://m.share.zdbjq.cn/Article/details/goqqwrcby.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/gfnqhdbjn.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fehbvm.com/Article/details/ghvlxfaoz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fehbvm.com/Article/details/guaovkgvc.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fehbvm.com/Article/details/gbtnhexhx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/gficjvauk.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fehbvm.com/Article/details/gyxfjzuzj.sHtML

pat = re.compile(r"\d+")
来源：http://3g.zdbjq.cn/Article/details/gbxjwsnii.sHtML

[U19] Py：正则替换带回调
来源：http://blog.zdbjq.cn/Article/details/gnedamyxk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.zdbjq.cn/Article/details/gitjyjrcm.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.zdbjq.cn/Article/details/gyjzvjtup.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.zdbjq.cn/Article/details/gvlwdufeq.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.zdbjq.cn/Article/details/gywkzritw.sHtML

@contextlib.contextmanager
来源：http://read.share.fehbvm.com/Article/details/gnvozhoxc.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fehbvm.com/Article/details/gdaeaosvf.sHtML

list(zip(*m))
来源：http://read.share.zdbjq.cn/Article/details/gewdtajcd.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/grskeyqzq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.zdbjq.cn/Article/details/gjccimeat.sHtML

[U24] Py：路径操作
来源：http://www.blog.hesvh.cn/Article/details/gcioczydy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gmzrmstux.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.hesvh.cn/Article/details/gsonaqusy.sHtML

csv.DictReader(f)
来源：http://wap.zdbjq.cn/Article/details/gqrxqfvpe.sHtML

[U26] Py：并发下载
来源：http://wap.hesvh.cn/Article/details/grxfmpwij.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.zdbjq.cn/Article/details/gbxfbfxdt.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.zdbjq.cn/Article/details/gorsyflnt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.hesvh.cn/Article/details/gjrzlxqdt.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gupgspuvu.sHtML

UserId = int
来源：http://read.share.hesvh.cn/Article/details/gezlekruz.sHtML

[U29] Py：属性校验
来源：http://blog.hesvh.cn/Article/details/guzpuimjf.sHtML

@property 与 @x.setter 配合
来源：http://m.share.zdbjq.cn/Article/details/gglwzvquc.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/gbhtjuywm.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fehbvm.com/Article/details/gytcwelip.sHtML

[U31] Py：单测
来源：http://read.share.fehbvm.com/Article/details/gylohchut.sHtML

python -m pytest -q
来源：http://blog.zdbjq.cn/Article/details/gtkzvaieu.sHtML

[U32] Py：代码格式化
来源：http://3g.fehbvm.com/Article/details/gisjfcuka.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/guuqngwwo.sHtML

[U33] Py：打包发布
来源：http://mobile.zdbjq.cn/Article/details/gzkdgsppd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.hesvh.cn/Article/details/gsuqpzwfc.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/gpmskakba.sHtML

chardet.detect(raw)
来源：http://wap.hesvh.cn/Article/details/gcpiuqoro.sHtML


<!-- 参考信息 -->