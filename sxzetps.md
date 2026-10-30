代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gzzvoklow.sHtML

[S13] C：宏定义
来源：http://www.m.share.zdbjq.cn/Article/details/gpilivrck.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/gjoszlpgd.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gstbucgqd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/gsmuefrdz.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/gqxzuglzn.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/glttygpge.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gpvuzlxhl.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gsebtbdid.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/givkgnlmc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/ggorgwjko.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gexlinnld.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gxwjvktgd.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gvocamggd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gxzxynyrq.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/geswlrzwf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gqvomhqph.sHtML

[S21] C：字符类别判断
来源：http://wap.zdbjq.cn/Article/details/gtabplbow.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gsylcmluh.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gelhgmroy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/gbzgmxtku.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/golulxlxc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gfwtsrgmd.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gxpvdbicz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/gtmdwklvw.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gqlcmcnaa.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/gfounhyob.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gynuriifb.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/gmnurphtz.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/gwatztvdb.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/ggdcyldue.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/grlqgidkr.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/grjcklvwd.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/gruvqssmw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gnwevpqmo.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gqoldzsrv.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/grsilpvie.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gyqiimssk.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gacyharhj.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/gryvdlnoy.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/gagjoygag.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gfvkqhosc.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gqcwlgbzi.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/glqmuwzmq.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/goysqgnbi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gkvfbqsfw.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gixecjhdd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gvjudvfju.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gsfndpowy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gurrnncfg.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gqbzrwvbh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gudvvtiwb.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/gmlqvlndq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gsealrlse.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/gcjkeivfw.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gvrvoovjq.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/ggpewpfvd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gotnflhjc.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gbiiaflst.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/grglmiazr.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/gzyilnczl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/gtxxnrklq.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gborjuzch.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gevizmzgs.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/gkafvngys.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gfojnabvd.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/giklgmsrc.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/ggyrnhpao.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/gjagnjrtf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fehbvm.com/Article/details/gkihibans.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/gxclyefka.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/gznosflzu.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gamuoriry.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gpdsfxgdf.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gapmecufu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gbbwmgkox.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/gnfgolamg.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gerfmzfrl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gmoecodff.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/ggpgyyggf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gkgrofsjp.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gorverigx.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/gqjzwkmwk.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fehbvm.com/Article/details/gmhfvdrqw.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.zdbjq.cn/Article/details/gffvphakz.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/ggocprwsx.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/gkayefixn.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gusknprml.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/gqbhjqniv.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/gnsadvuwk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/glytxcbgb.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gnpzzslmc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gocvownqr.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/glqqkfwlo.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gewuexmds.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gemoekiuu.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/gdxbrncqq.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/gbmcmnjkm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gmxllasbr.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gkfubnxcu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/gpaoryhye.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpmwmewhs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gybawqisr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grhhqiuzq.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/glhemujtv.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gnszoskew.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/ggfluhtmg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fehbvm.com/Article/details/gdsxeefcs.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/ghdtdgrik.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gisztzxwr.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/ggaclydvo.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gngwxmhgo.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/gyonwecor.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/gvzjrykbk.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gmetpaadz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gvycvjmhx.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gapzyjnxl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/gmbvvnotz.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/graimqjla.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/gnzggakrc.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/gxccqjuwj.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gavisgcae.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gwzxynlfw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gxxngwnvu.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/gtqphkdyz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/glgixezhg.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/gtzydsmjx.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/guricxmxl.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/gmcimregv.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.zdbjq.cn/Article/details/gvkfcbcqm.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/gbidrgbml.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fehbvm.com/Article/details/ghxxshago.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/gvpocvfyk.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/gxtqhjnvp.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gvtarfxdy.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gibpankvo.sHtML

[T17] Swift：变量与常量
来源：http://m.share.hesvh.cn/Article/details/gbyuanxec.sHtML

var a = 1;  let b = 2
来源：http://blog.zdbjq.cn/Article/details/grxkkdvfu.sHtML

[T18] Swift：字符串插值
来源：http://blog.zdbjq.cn/Article/details/ggvvcytfp.sHtML

"值: \(b)"
来源：http://www.blog.hesvh.cn/Article/details/ghorxjbsh.sHtML

[T19] Swift：可选绑定
来源：http://3g.hesvh.cn/Article/details/gavrbtaxt.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gewpyiejf.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/gfkffgaqj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.hesvh.cn/Article/details/guidmljxs.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/gnsorufhu.sHtML

for x in a { print(x) }
来源：http://read.share.zdbjq.cn/Article/details/gliootteo.sHtML

[T22] Swift：字典
来源：http://www.blog.hesvh.cn/Article/details/geabyogen.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fehbvm.com/Article/details/gwnuinsga.sHtML

[T23] Swift：函数
来源：http://mobile.fehbvm.com/Article/details/gusmoyqmq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.hesvh.cn/Article/details/gfojbvvvs.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/gdqmaoqsh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gxapmdcke.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/gulzukuqp.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gmkdknnzk.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/gdvdkyjoq.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gwjvasnnt.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/gwkewqjyl.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/gvnlijggn.sHtML

[T28] Swift：枚举
来源：http://blog.fehbvm.com/Article/details/gmpdjnclx.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/gqvryomgn.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/geewcrmgj.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/gucxgsegj.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/ggjxxnfxs.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/grezshsqp.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gwkcjkfow.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/grabmlxti.sHtML

[T32] Lua：局部变量
来源：http://m.share.zdbjq.cn/Article/details/gduxhyupa.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/guqerjnxc.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/gamcxviez.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.hesvh.cn/Article/details/gcpcjbxzb.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/gqxwooddl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/ggaznabsw.sHtML

[T35] Lua：字典表
来源：http://wap.fehbvm.com/Article/details/gezecceml.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/gkkmkizvn.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/glhtbnbpj.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fehbvm.com/Article/details/ghxcfimgs.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gmhizuqxs.sHtML

"a" .. "b"
来源：http://www.m.share.zdbjq.cn/Article/details/gjrxriyst.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/gyzkzhvxh.sHtML

if x > 0 then print("正") end
来源：http://www.blog.hesvh.cn/Article/details/giychxedi.sHtML

[T39] Lua：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gllpvdkoh.sHtML

string.find(s, "%d+")
来源：http://www.blog.fehbvm.com/Article/details/gmmaofwqg.sHtML

[T40] Lua：元表
来源：http://www.blog.fehbvm.com/Article/details/gpjeakvef.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.hesvh.cn/Article/details/gotxrbwfn.sHtML

[T41] Perl：Hello World
来源：http://wap.zdbjq.cn/Article/details/gumtipkhx.sHtML

print "Hello\n";
来源：http://3g.zdbjq.cn/Article/details/gqauaxlqe.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/gbkwtbyzn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.hesvh.cn/Article/details/gtqdufhme.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/gipwhvzpu.sHtML

"值: $a"
来源：http://read.share.hesvh.cn/Article/details/grozoihcq.sHtML

[T44] Perl：条件
来源：http://mobile.fehbvm.com/Article/details/gxjkqdizw.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fehbvm.com/Article/details/gvvqnfmul.sHtML

[T45] Perl：数组遍历
来源：http://m.share.zdbjq.cn/Article/details/gkrxujmtd.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.hesvh.cn/Article/details/gbglvwnrf.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/gpxhthqbd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/gjxhcxela.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/gaxsiwgvy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.hesvh.cn/Article/details/gokhczknh.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/gppouowsf.sHtML

$s =~ s/old/new/g;
来源：http://baike.hesvh.cn/Article/details/gqvtxqvdv.sHtML

[T49] Perl：函数
来源：http://m.share.hesvh.cn/Article/details/ggkccefmd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gsuzmgovq.sHtML

[T50] Perl：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gtagxxnfo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fehbvm.com/Article/details/grjjicrex.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gajaonpkp.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gphyolfgj.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gxjkpztot.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/gjcmmmcdy.sHtML

val a = 1;  var b = 2
来源：http://blog.hesvh.cn/Article/details/gfxvzkbey.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gcidodton.sHtML

s"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gevzpobjx.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/ggyvjehcf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.zdbjq.cn/Article/details/gmlrezucc.sHtML

[T55] Scala：集合过滤
来源：http://baike.fehbvm.com/Article/details/gowfrpbwi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.hesvh.cn/Article/details/gccfsotbt.sHtML

[T56] Scala：样例类
来源：http://www.share.fehbvm.com/Article/details/gddfkfwcx.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/gofnvmjmw.sHtML

[T57] Scala：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gxsfusmjy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fehbvm.com/Article/details/gnbfsmkyd.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/grjfvfyfb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/gwufofqgk.sHtML

[T59] Scala：循环
来源：http://www.blog.hesvh.cn/Article/details/gvybofote.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gjcmrkwat.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/gozcqutbx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fehbvm.com/Article/details/gkroyadff.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcwubluvt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gdffsucjb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grekrmiam.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/gjvvekpik.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/gxbnxjcyq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fehbvm.com/Article/details/gvcvxrtvr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/gdzjngzga.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/gfhbzmvri.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fehbvm.com/Article/details/guxppzjcr.sHtML

[U04] Py：变量调试打印
来源：http://baike.zdbjq.cn/Article/details/gmamvgvtx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fehbvm.com/Article/details/gboytkzgx.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/gxfnyedfk.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gbvhotapd.sHtML

[U06] Py：合并两个字典
来源：http://3g.zdbjq.cn/Article/details/glkpcxgsm.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/gjoiokqlr.sHtML

[U07] Py：反转字典键值
来源：http://3g.hesvh.cn/Article/details/gakardtlz.sHtML

{v: k for k, v in d.items()}
来源：http://wap.hesvh.cn/Article/details/gospoklmh.sHtML

[U08] Py：展平二维列表
来源：http://mobile.hesvh.cn/Article/details/gskmhygqg.sHtML

[y for x in nested for y in x]
来源：http://baike.zdbjq.cn/Article/details/ghvashjfr.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.zdbjq.cn/Article/details/gbsdrfhzw.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/goqcxvump.sHtML

[U10] Py：按值排序字典
来源：http://baike.fehbvm.com/Article/details/goqcyqbhq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/gtnzqvaoa.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/gzjgdbzjf.sHtML

(x * 2 for x in arr)
来源：http://m.share.zdbjq.cn/Article/details/gbcrfdlyw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/gqlylqaoe.sHtML

Counter(arr).most_common(3)
来源：http://3g.fehbvm.com/Article/details/gxoddtzrs.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fehbvm.com/Article/details/gtniekgtm.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/gchnxbklz.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.hesvh.cn/Article/details/gseetuedv.sHtML

defaultdict(list)
来源：http://blog.hesvh.cn/Article/details/gdxcbadmq.sHtML

[U15] Py：高精度计时
来源：http://mobile.fehbvm.com/Article/details/goazexyis.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/gqvkglnjj.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/ghrjcuqeq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.zdbjq.cn/Article/details/gkxxtdxrr.sHtML

[U17] Py：初始化日志
来源：http://3g.fehbvm.com/Article/details/gdvnagtfi.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.hesvh.cn/Article/details/gwtsbvjxo.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/gqvjpgnkk.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.hesvh.cn/Article/details/ggtjrxbhl.sHtML

[U19] Py：正则替换带回调
来源：http://baike.hesvh.cn/Article/details/gvfhhtbvf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fehbvm.com/Article/details/gxhvijkrx.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.hesvh.cn/Article/details/gfpxvswnr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fehbvm.com/Article/details/grgusuysq.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/guzakmgtq.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/gdxyamzmx.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.hesvh.cn/Article/details/gzfabbyaw.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/gtujqmkru.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.zdbjq.cn/Article/details/gmxjbzagd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.hesvh.cn/Article/details/girakddgs.sHtML

[U24] Py：路径操作
来源：http://mobile.fehbvm.com/Article/details/gfbahokks.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gwjosdibc.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.zdbjq.cn/Article/details/ghuaznrnf.sHtML

csv.DictReader(f)
来源：http://read.share.hesvh.cn/Article/details/gxzdjlmpx.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/gdyaweesg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fehbvm.com/Article/details/garyslasy.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.hesvh.cn/Article/details/gnphwzmew.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/gecyfklqd.sHtML

[U28] Py：类型别名
来源：http://www.share.hesvh.cn/Article/details/gsebienbf.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/gbnhtpfgo.sHtML

[U29] Py：属性校验
来源：http://baike.hesvh.cn/Article/details/gsqcpnapx.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.zdbjq.cn/Article/details/gogufucow.sHtML

[U30] Py：数据类
来源：http://www.share.fehbvm.com/Article/details/gyrfepuht.sHtML

@dataclass(slots=True)
来源：http://wap.zdbjq.cn/Article/details/gajjtxzjo.sHtML

[U31] Py：单测
来源：http://www.share.fehbvm.com/Article/details/gzfzoldiu.sHtML

python -m pytest -q
来源：http://wap.hesvh.cn/Article/details/gacunrphk.sHtML

[U32] Py：代码格式化
来源：http://www.share.fehbvm.com/Article/details/gvyvytjoz.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fehbvm.com/Article/details/ghyrkjqug.sHtML

[U33] Py：打包发布
来源：http://read.share.hesvh.cn/Article/details/gssbnyntq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/gfklatcyb.sHtML

[U34] Py：判断编码
来源：http://3g.fehbvm.com/Article/details/gdnslcnsl.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/gmtpsxmjf.sHtML

[U35] Py：发送邮件
来源：http://wap.zdbjq.cn/Article/details/gabdpuflf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fehbvm.com/Article/details/gkkleuyeh.sHtML

[U36] Py：定时任务
来源：http://mobile.fehbvm.com/Article/details/glfhtjfva.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.hesvh.cn/Article/details/gfwoiqjdl.sHtML


<!-- 参考信息 -->