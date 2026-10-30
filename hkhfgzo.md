代发 wailian999

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/gsyrppomw.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gucouvzds.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/ggerkkidh.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/govonbfoq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gdsiumrud.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/gedzzvmkb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.zdbjq.cn/Article/details/gjdyxmtpn.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/gyialwtxy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/gzdoxwabm.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gdfdfrneh.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gbpomzxdw.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gjtihzyvb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.zdbjq.cn/Article/details/ghptnceyv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gknlfovyg.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/grkxtdgib.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gkeaniywz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gvijqosrn.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gdwdfaakl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gdadbwxep.sHtML

[S14] C：枚举
来源：http://3g.fehbvm.com/Article/details/gnirgzseu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gcmdupmmm.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gkyfadzic.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gdhqhcjwp.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/gzevechhk.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gfmwtmirr.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gamiwcybz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gwnwtzgrr.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gpgbvwnft.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/grmmsqvbp.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gagrntuuo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/grcvqvqbv.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/guaxhyreg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gnqhvfbfa.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/gqkslectf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/gxepjxrei.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gfzxssekj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/ghnvarpni.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gjrwpxetz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gdfvbmrey.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/giphywxcu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/grnmqrjzs.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gmoifqwdm.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/gsdlmdukr.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gebngbcsl.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/givymozfw.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gnwzawbwn.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gwrpsrtpl.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/gahjrkesu.sHtML

static int counter = 0;
来源：http://www.share.hesvh.cn/Article/details/gocnudilg.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/gxcrocjkl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gfihamack.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gmcmdimua.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/giqqrcrod.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gxwnkocgq.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/gissgelsi.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gdxyxriyl.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/gylvopcnu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gansszsab.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gchkyqwsr.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/ghvqftkwk.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gbzhkzdgu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gjidiciom.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/ggyqbslzj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gxvtrpbod.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gbmpvyfcd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/grsitaxae.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/gunlyviya.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gxpcdjrav.sHtML

[S37] C++：set
来源：http://blog.hesvh.cn/Article/details/gatlulfra.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/gpnwnhlzr.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/ghkkddtvv.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/gvtqqjqrq.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/ghugzgnkm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.zdbjq.cn/Article/details/graslcghx.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/gelmctztp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/garlaltng.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/gcfkbkrue.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/gdhmtafyb.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gpwrtjgjs.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gnksksohp.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gguuhjgaj.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/gkwwvqurx.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gbxtcjdqo.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/ggtzokbbf.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gdetigkuj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/gbxzyuldz.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/gnfrfvkrn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gyyozcoar.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gmpkbgfuf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/gzjuicppe.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gjzjjktyt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/guyfdvhlx.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gwvdjirma.sHtML

[S49] C++：写文件
来源：http://m.share.fehbvm.com/Article/details/gdwahwdeg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/gfvbaxnuc.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/gxjwmybwh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gildpclhr.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/grkddgqjx.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/gyiajthgz.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gzuvkemvw.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gusxlxpec.sHtML

[S53] C++：移动语义
来源：http://baike.hesvh.cn/Article/details/gkuqvmmrm.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gidolctcy.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gixbtgatj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/grirmyech.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/giqdfmasw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.zdbjq.cn/Article/details/gvfctxanu.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gsroznijc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gpctiqbcl.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/ggqtzowiw.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/gbbmtqaog.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/grxuzvbvl.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/gqhqdhlgq.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gbtbnolro.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gtlxaxqnt.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/gclrvsqrr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.hesvh.cn/Article/details/gbtzisewb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grbpuyfhj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gxikfawjk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcykrekwr.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/gglqbeisl.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gtjnvdler.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gxspfzrdb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/gqfygiumf.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/gubpmuivs.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gaeyoknnf.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/gspshemar.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gygkgcvzm.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/gmeyhhltp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/gzvkioitu.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gnldgscqb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/ggwnjvgrx.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gxrhhsebf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gexbfbynr.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/giyvylicr.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/gtbwyaspt.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/gpidxptzn.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gqtdzunqd.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gztsgwvxw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/guxygotqs.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gvpvzntwr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.hesvh.cn/Article/details/gjpyrmenq.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/gaorwtlbz.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gkflqrffa.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/gnrpqdxnt.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/gqsogpwdb.sHtML

[T14] Kotlin：循环
来源：http://blog.zdbjq.cn/Article/details/groayfayu.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/grvwsiifz.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/gyzklqlgr.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/ghxrlbpiy.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/glwxriknj.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gqyvtqpso.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/glysssaoo.sHtML

var a = 1;  let b = 2
来源：http://blog.zdbjq.cn/Article/details/ghgxflckt.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gxlymmmnt.sHtML

"值: \(b)"
来源：http://www.m.share.zdbjq.cn/Article/details/gzzldqiqz.sHtML

[T19] Swift：可选绑定
来源：http://m.share.zdbjq.cn/Article/details/gugzodfuh.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/gaxrswsju.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/gflaasihl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/gkegyhrcs.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/gjwgermok.sHtML

for x in a { print(x) }
来源：http://m.share.zdbjq.cn/Article/details/gwvrjccwx.sHtML

[T22] Swift：字典
来源：http://wap.zdbjq.cn/Article/details/gvtmdzpem.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.hesvh.cn/Article/details/gkhatizvy.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gvczjhtjl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gfefkgubs.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/goxfkyoko.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/gnbpwvwlv.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/gqrhstsqn.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gtdsuyryq.sHtML

[T26] Swift：类与重写
来源：http://3g.hesvh.cn/Article/details/gaermzucy.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/gpnelyqfs.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gwgsvqeyj.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fehbvm.com/Article/details/gryatalte.sHtML

[T28] Swift：枚举
来源：http://www.blog.fehbvm.com/Article/details/gfnsqspzc.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/gafgexeiw.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.hesvh.cn/Article/details/gmnjzflrj.sHtML

guard let x = opt else { return }
来源：http://mobile.hesvh.cn/Article/details/gteuedtoa.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/gqveaalpe.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gvwldpeam.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/gsndcmktz.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gguydeicb.sHtML

[T32] Lua：局部变量
来源：http://blog.hesvh.cn/Article/details/gttdbpoxw.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/gabuctnoq.sHtML

[T33] Lua：表（数组）
来源：http://blog.hesvh.cn/Article/details/geibhuijf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/gcdgktydn.sHtML

[T34] Lua：遍历表
来源：http://baike.hesvh.cn/Article/details/gjystuiyy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fehbvm.com/Article/details/gbcrwpyrw.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gkphirxjf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gkjskpvzy.sHtML

[T36] Lua：函数
来源：http://www.blog.zdbjq.cn/Article/details/gntpydsxi.sHtML

function add(a, b) return a + b end
来源：http://wap.hesvh.cn/Article/details/gbpalyltq.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gixbpftrr.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/gjpgbvwpm.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/gldgzfdoo.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/ghjnrhjpb.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gzzqzovtp.sHtML

string.find(s, "%d+")
来源：http://m.share.hesvh.cn/Article/details/gnuvgxhxg.sHtML

[T40] Lua：元表
来源：http://blog.fehbvm.com/Article/details/gvxbqzvdf.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/gtcgkutqt.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gsafafzhv.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/gclxwcrwt.sHtML

[T42] Perl：变量类型
来源：http://wap.fehbvm.com/Article/details/guraodzgs.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fehbvm.com/Article/details/gqwqafxuq.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gxcqueamf.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/gtceswzpo.sHtML

[T44] Perl：条件
来源：http://3g.fehbvm.com/Article/details/gkiwstvgz.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fehbvm.com/Article/details/gphnwzpej.sHtML

[T45] Perl：数组遍历
来源：http://blog.fehbvm.com/Article/details/gvaryvtby.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/gmtnbvcmy.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fehbvm.com/Article/details/gqyngzssp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.zdbjq.cn/Article/details/gdgbeqvfy.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gtuvoxuic.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/ggzpuzpay.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/glivegktw.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fehbvm.com/Article/details/gewqsukxa.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gxrhpbrnv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/ghlfedxgv.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/glbabzmir.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.hesvh.cn/Article/details/gowzqqevf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/gfrnscmmi.sHtML

[T51] Scala：Hello World
来源：http://baike.fehbvm.com/Article/details/gommwpirr.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gzwtwyxqb.sHtML

[T52] Scala：变量
来源：http://wap.fehbvm.com/Article/details/gcjftpcau.sHtML

val a = 1;  var b = 2
来源：http://www.share.zdbjq.cn/Article/details/gmdahkotv.sHtML

[T53] Scala：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gacmcsfye.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/ggtwrkeaw.sHtML

[T54] Scala：集合映射
来源：http://3g.zdbjq.cn/Article/details/gasacqrde.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/gmtzszdry.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gwdrtowsf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.hesvh.cn/Article/details/gcfhhqvvn.sHtML

[T56] Scala：样例类
来源：http://3g.hesvh.cn/Article/details/gdxbjxfgf.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/gkwzgsaaz.sHtML

[T57] Scala：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gycpvyhrr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fehbvm.com/Article/details/gzqvrxfed.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/gagmitjgk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gigldkmhl.sHtML

[T59] Scala：循环
来源：http://www.blog.hesvh.cn/Article/details/gwnpazhfg.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gjmsmufsa.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/guhqfkieg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.hesvh.cn/Article/details/guvxqimpl.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwzgicfib.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gtwjsngru.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtcoyqrjl.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/gnykuatvq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fehbvm.com/Article/details/gvbbxzlmu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fehbvm.com/Article/details/gxvivlbzu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gtahfmspy.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/gluupywdl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.hesvh.cn/Article/details/gjjezikqt.sHtML

[U04] Py：变量调试打印
来源：http://m.share.hesvh.cn/Article/details/gnpzrdbtc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.hesvh.cn/Article/details/gejdqrmfe.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fehbvm.com/Article/details/gbpqeaujb.sHtML

list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gdargbvpr.sHtML

[U06] Py：合并两个字典
来源：http://baike.zdbjq.cn/Article/details/gqfztkyma.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/gpbayzxxv.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/gmbvdklji.sHtML

{v: k for k, v in d.items()}
来源：http://baike.zdbjq.cn/Article/details/glwmlnmwo.sHtML

[U08] Py：展平二维列表
来源：http://3g.zdbjq.cn/Article/details/glbjucuhv.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gaotngogj.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.zdbjq.cn/Article/details/gdtwqtkry.sHtML

max(d, key=d.get)
来源：http://3g.zdbjq.cn/Article/details/guqhpviae.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/gpsgcyltr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fehbvm.com/Article/details/gnyuekets.sHtML

[U11] Py：生成器表达式
来源：http://www.share.hesvh.cn/Article/details/gikxmcoor.sHtML

(x * 2 for x in arr)
来源：http://3g.zdbjq.cn/Article/details/gsyxkiduj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.zdbjq.cn/Article/details/gsowheojl.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.zdbjq.cn/Article/details/goqytikhm.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fehbvm.com/Article/details/ghgjlqwsw.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/glhmigezm.sHtML

[U14] Py：分组收集到列表
来源：http://blog.zdbjq.cn/Article/details/gmadoyujk.sHtML

defaultdict(list)
来源：http://www.m.share.fehbvm.com/Article/details/gkeggwefd.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.hesvh.cn/Article/details/gbhkemfmi.sHtML

t = time.perf_counter()
来源：http://3g.zdbjq.cn/Article/details/gkojdbtla.sHtML

[U16] Py：命令行参数解析
来源：http://3g.zdbjq.cn/Article/details/gwodgtynz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/gygottczp.sHtML

[U17] Py：初始化日志
来源：http://read.share.fehbvm.com/Article/details/gfqmzeiqp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.hesvh.cn/Article/details/gkhkdkifi.sHtML

[U18] Py：预编译正则
来源：http://m.share.zdbjq.cn/Article/details/gekccadtx.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/ghseisyhp.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.hesvh.cn/Article/details/gvysrcebi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fehbvm.com/Article/details/gawndclcd.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.hesvh.cn/Article/details/gonevmgcf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.zdbjq.cn/Article/details/ghpdrcnpu.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.hesvh.cn/Article/details/gpjwalpis.sHtML

@contextlib.contextmanager
来源：http://mobile.fehbvm.com/Article/details/gzfevfrfc.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fehbvm.com/Article/details/gaxycvhem.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/gldpgwajj.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.zdbjq.cn/Article/details/grmvwdudt.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/gliqrcerk.sHtML

[U24] Py：路径操作
来源：http://read.share.fehbvm.com/Article/details/grifdhzfg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gbplvuvkr.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.hesvh.cn/Article/details/gmomggjnx.sHtML

csv.DictReader(f)
来源：http://wap.zdbjq.cn/Article/details/gdsmnaasy.sHtML

[U26] Py：并发下载
来源：http://m.share.hesvh.cn/Article/details/gsipjegbg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fehbvm.com/Article/details/glchlcgis.sHtML

[U27] Py：异步 HTTP
来源：http://3g.hesvh.cn/Article/details/gocarunvt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fehbvm.com/Article/details/geepjlvvo.sHtML

[U28] Py：类型别名
来源：http://read.share.fehbvm.com/Article/details/gdkmjotqk.sHtML

UserId = int
来源：http://read.share.zdbjq.cn/Article/details/glckvcfog.sHtML


<!-- 参考信息 -->