代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gezyhbjmg.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gnlaelilr.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcfelfrn.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgjazguc.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gtgihraxw.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gjmoakexo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfinhnnmg.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gbahkisle.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmigxabhl.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gzouzvbav.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gtzlmcryp.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gxwdqsgus.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gnuwvbpeu.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdgrklzy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrnqonka.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnqqpzlc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/glbpfjfmb.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gqvegmqhs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goucxigax.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gabsotnia.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbumjuxdr.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdfoxhss.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gqnbgzryo.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gokwhkfbs.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/giopquchw.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/glbtrjsrj.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqhetkbd.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gyguqowkd.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gvpwqcaks.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/grekzalin.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gweklaeyl.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gdewlnppv.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvelybdi.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzhxwqvf.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdctzpts.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gvomiyevb.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/ggjhmixps.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqbvewmw.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhicemly.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/grwitcrvr.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gobhmtcoe.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gntfptvkp.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gbvswgbxw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsctclvgr.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzeqyvbt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/ghgksbapo.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gchmmhhaf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gcobkvawr.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gkabwxmch.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gixvlnpqe.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlqwavvv.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzwgqnpg.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxyqatbq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/guxktmubd.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gvdyowuda.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzivcqde.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnlmuvli.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/geejxnyyc.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnmgsyep.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gjldtmpvc.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gcbbrnwek.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjfdsqyj.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gufacftit.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmaljlwss.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gdeheoabk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gckiaeone.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gprfshwnx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gapvjpmja.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/ghkqbqifm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/grpyzxizd.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqcdvtiw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gunzsyqwv.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdktmfqfj.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvfeequa.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gennfzrwn.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxkwwpcz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbxjazhf.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghiysttoc.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfwzbald.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gmllmpmtj.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhtnppel.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gegfunkog.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyjfhter.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnfdlmhp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gvcgfkuva.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvyhcmvg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gshdrexio.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gqjpoaerb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghevuhxnu.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/gealzyhig.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gxbxxucaw.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcmpisud.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/ggkuzseoo.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdukhppk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxbkecsn.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfixqpcd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gekxmpwto.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gzqvmzlfn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/giacjqmxx.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwrppjqj.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntliirec.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gxpbmveyu.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchxdedmx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthfbmtpv.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjxbvwnv.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdsqpbxk.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/gybtkyqaq.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbwjtkqg.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gypdvrbuq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/ghlmspffe.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgrlgkln.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gjlkxgpnl.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfwdoqan.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/grayiedhu.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjccbhtf.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gquqsyuub.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gyigyilnl.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjjxzwnm.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrdqnfhy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/gnwellqdn.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/goxenqkuq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbbesixx.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxidwcxu.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkqlchqn.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gljiloemn.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gbkutbjfl.sHtML

[T14] Kotlin：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gojovfuqa.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnuldksqi.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofwhewqb.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnbgvims.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqobpqzi.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gqbypaapb.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/gytmehrxt.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxhqjwjs.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gniikhqax.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gajuepsqz.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/getyyuyfr.sHtML

if let n = opt { print(n) }
来源：http://3g.fanxiaobao.xyz/Article/details/glbxhbiyu.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gprpgnqxd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gytfiunri.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gekalgiey.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/glnvynfuu.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/gybyvgsbc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gefukqbst.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gujsbaate.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/grmjmojij.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjtnoqrw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqaktkjbz.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/gopkvorlz.sHtML

struct P { var x: Int }
来源：http://3g.fanxiaobao.xyz/Article/details/ggyzdgsrj.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gimznrwwd.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/grsvxdgly.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbzbmzfw.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbarofgmo.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gxycbwnvv.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/gvcllvdlz.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/gbkkbuiou.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlsjmbpb.sHtML

[T30] Swift：协议
来源：http://wap.fanxiaobao.xyz/Article/details/gtefifwte.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnswxyrdm.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gqjmvzlco.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzqhkqqv.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gqieysvgi.sHtML

local a = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjatwjxq.sHtML

[T33] Lua：表（数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gcjockfgt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fanxiaobao.xyz/Article/details/gorsqxxpc.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwfavmid.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fanxiaobao.xyz/Article/details/gaskcsewy.sHtML

[T35] Lua：字典表
来源：http://read.share.fanxiaobao.xyz/Article/details/gnalotsig.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfycslje.sHtML

[T36] Lua：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmfuunbd.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbyuxkgh.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtuovubt.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/gymfpwjkl.sHtML

[T38] Lua：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gnzwiancf.sHtML

if x > 0 then print("正") end
来源：http://wap.fanxiaobao.xyz/Article/details/gcsuathog.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gswizjsff.sHtML

string.find(s, "%d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gcphdbzas.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnrgcdhv.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsxdbkmx.sHtML

[T41] Perl：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/ggrqbklyi.sHtML

print "Hello\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gehgrdgkd.sHtML

[T42] Perl：变量类型
来源：http://wap.fanxiaobao.xyz/Article/details/gdhipopje.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gznvszqbe.sHtML

[T43] Perl：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gdhrnvbqd.sHtML

"值: $a"
来源：http://wap.fanxiaobao.xyz/Article/details/gzhmbfvil.sHtML

[T44] Perl：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gszuvuxkt.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gagirawwt.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gobbujurx.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwjkhvogr.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gakjlazuo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gunfzdsgc.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/geicmzhjr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagdjvtvb.sHtML

[T48] Perl：正则替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqdxnbdl.sHtML

$s =~ s/old/new/g;
来源：http://blog.fanxiaobao.xyz/Article/details/gjtsrazqe.sHtML

[T49] Perl：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gvyzearij.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvvaqxqdt.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/geqrlvxes.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fanxiaobao.xyz/Article/details/gynnfsmrd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmerbvppn.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzyochkq.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgtptecx.sHtML

[T52] Scala：变量
来源：http://baike.fanxiaobao.xyz/Article/details/ggqhadeif.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvfemicg.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsjmvhvx.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/guejejdjl.sHtML

[T54] Scala：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gukdlsrez.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaomivacx.sHtML

[T55] Scala：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gzleyetbd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfhpqxuh.sHtML

[T56] Scala：样例类
来源：http://wap.fanxiaobao.xyz/Article/details/guphsodvd.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvfgugps.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gpirzzasl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/ghxbwispf.sHtML

[T58] Scala：函数定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhjtqevk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fanxiaobao.xyz/Article/details/gslduircn.sHtML

[T59] Scala：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gkbzdtsxt.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnnlamou.sHtML

[T60] Scala：折叠
来源：http://m.share.fanxiaobao.xyz/Article/details/gozytbjoq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbqyqibp.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzgkltyz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gfthpxcgz.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxscaouw.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fanxiaobao.xyz/Article/details/gkjxffnsz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fanxiaobao.xyz/Article/details/goszepyfv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlklkpmh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapzekfii.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/gbihcpryb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqjfmtzh.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gteaznhgs.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fanxiaobao.xyz/Article/details/gmyctqpge.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fanxiaobao.xyz/Article/details/gpdrnvxfa.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gqjhkvgki.sHtML

[U06] Py：合并两个字典
来源：http://3g.fanxiaobao.xyz/Article/details/gerybszwq.sHtML

{**a, **b}
来源：http://wap.fanxiaobao.xyz/Article/details/gkgtklbzn.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fanxiaobao.xyz/Article/details/glhjfklqc.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/gzoxedtph.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gispxiavm.sHtML

[y for x in nested for y in x]
来源：http://3g.fanxiaobao.xyz/Article/details/ghcgnwbwn.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyjajjuu.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvptorsjp.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbtcyxdg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgktbigg.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gzruernrp.sHtML

(x * 2 for x in arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gshzaywwa.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/gjsucstza.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvulwwfc.sHtML

[U13] Py：固定长度队列
来源：http://blog.fanxiaobao.xyz/Article/details/gjevbbpad.sHtML

deque(maxlen=10)
来源：http://3g.fanxiaobao.xyz/Article/details/gzzanreqo.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gdroetlav.sHtML

defaultdict(list)
来源：http://3g.fanxiaobao.xyz/Article/details/gupyxvlvu.sHtML

[U15] Py：高精度计时
来源：http://3g.fanxiaobao.xyz/Article/details/gflfpybvh.sHtML

t = time.perf_counter()
来源：http://3g.fanxiaobao.xyz/Article/details/gnnvfculg.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fanxiaobao.xyz/Article/details/gkzqqeati.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvoqfrmhz.sHtML

[U17] Py：初始化日志
来源：http://3g.fanxiaobao.xyz/Article/details/gulrsltzc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fanxiaobao.xyz/Article/details/gqszodpvy.sHtML

[U18] Py：预编译正则
来源：http://3g.fanxiaobao.xyz/Article/details/gipexjtgm.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gmxnzveur.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fanxiaobao.xyz/Article/details/gllwwxjax.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fanxiaobao.xyz/Article/details/ghpvagscm.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fanxiaobao.xyz/Article/details/gfgrmgspt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtozlmap.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbyfxmed.sHtML

@contextlib.contextmanager
来源：http://wap.fanxiaobao.xyz/Article/details/gfugyssvi.sHtML

[U22] Py：矩阵转置
来源：http://blog.fanxiaobao.xyz/Article/details/govrgmdwj.sHtML

list(zip(*m))
来源：http://3g.fanxiaobao.xyz/Article/details/gnjevgjen.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxrzehmr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicbaytkf.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gunfziamp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamutmuyp.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fanxiaobao.xyz/Article/details/gmupsuwai.sHtML

csv.DictReader(f)
来源：http://3g.fanxiaobao.xyz/Article/details/guyexxfyy.sHtML

[U26] Py：并发下载
来源：http://3g.fanxiaobao.xyz/Article/details/gfvbwnldl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqyctflk.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrktzkxc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fanxiaobao.xyz/Article/details/glljgkoaj.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/gswzhxcvk.sHtML

UserId = int
来源：http://www.share.fanxiaobao.xyz/Article/details/goxnfntcb.sHtML

[U29] Py：属性校验
来源：http://blog.fanxiaobao.xyz/Article/details/gtjyweblh.sHtML

@property 与 @x.setter 配合
来源：http://blog.fanxiaobao.xyz/Article/details/gosrylkmv.sHtML

[U30] Py：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gkanoeikr.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsubamft.sHtML

[U31] Py：单测
来源：http://wap.fanxiaobao.xyz/Article/details/gsvfwrnuq.sHtML

python -m pytest -q
来源：http://wap.fanxiaobao.xyz/Article/details/grejgngbt.sHtML

[U32] Py：代码格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/glwqtdxez.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fanxiaobao.xyz/Article/details/gxduytaup.sHtML

[U33] Py：打包发布
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrfoggqw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fanxiaobao.xyz/Article/details/gcizzibai.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqemzlmt.sHtML

chardet.detect(raw)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvciyikmm.sHtML

[U35] Py：发送邮件
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkchvffn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fanxiaobao.xyz/Article/details/gyrjfoczy.sHtML

[U36] Py：定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gysalfchr.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyxlirle.sHtML

[U37] Py：读写 Excel
来源：http://3g.fanxiaobao.xyz/Article/details/grzfxozvo.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrgegsaa.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fanxiaobao.xyz/Article/details/ghprouidk.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvfeuxsz.sHtML


<!-- 参考信息 -->