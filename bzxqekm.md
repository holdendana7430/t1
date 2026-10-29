代发 wailian999

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/gamhlfxmu.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gmuqlvnrs.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/gqmgsnmyk.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/ggulcszbe.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gzytelsit.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/ghqjatrhw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/gkilmphmf.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gcnjedsxn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gybldoxfz.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/gaikuoerq.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/gtxvqdmnw.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gqhwrryju.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gmezmwouk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fehbvm.com/Article/details/gjcyrchnp.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/genveavso.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/gpihnkxdr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/gfrcnusqn.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gkurrybdq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gimbuvybn.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/gpdhfjbjx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gjiynmjxm.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/gpwfelhhy.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gvhwtrynw.sHtML

[S16] C：位操作置位
来源：http://read.share.fehbvm.com/Article/details/gprhyjtee.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/gftegktcq.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/grqaezvsd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/grbktuyjm.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/gtqdvatir.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/guzzzzaqf.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/gnxxbqlxh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gjrssktmr.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/glbbhpzci.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gqpdbdckv.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gapbexxvh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gfnaurncn.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gddigoswx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/ggmeputcv.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/gekxmqxrw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/gdtexbyas.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/gbdycdqhk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gxldbkvyg.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/gtmwqaoan.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/ggexotzif.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/ggbpremre.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gkolvekaq.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gnvultqlh.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/ggrtzuobm.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gauhqsjsx.sHtML

static int counter = 0;
来源：http://m.share.fehbvm.com/Article/details/gzurooisc.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/gufsqsiph.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gouvyuyfs.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/gkhekyecx.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gollpvqia.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/gxokgovdx.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/glogdqsve.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/glqydircl.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gqzwiuqcf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/giuxfkaxz.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gvsfskdhg.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gxvpecltf.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/gmesgzbjn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gembeiifb.sHtML

[S34] C++：遍历 vector
来源：http://wap.zdbjq.cn/Article/details/gzhbeteqj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/gqssdorrj.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/gukuothur.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gxrwqfopc.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/grcivntky.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gbrvyynwx.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/goyawrpah.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/girbxmhaq.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gbtwsdymv.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gztamvtjd.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gfsgrfuzx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/gdmpynqvd.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/glvjxytny.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gvlakipjf.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gnmklnvbc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gneuztjxl.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/gtprfodso.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fehbvm.com/Article/details/gobnsozav.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gbcehjfnj.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/gcpqpjevx.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gmnipbccb.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/gkotlhtfu.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/gagopqzro.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/gljfikaba.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/goaendwif.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/gdttmujne.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/gquturtue.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/ggghfwxrc.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gmpfrddtb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/gfkupmxgh.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gcztgjtto.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gtndzpjde.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gcqzvepwt.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/ghqhudpwh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/gyaisneyo.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/ghkaoatun.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/gbitrdcug.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gectbhxav.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gsxliatcc.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/gnbabgxmf.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/gmzelgmvn.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gsyeitvqx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/guppvtaem.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/glyitqxgq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gupqnxrwj.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gjuxfpdfs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/grcvneuyv.sHtML

[S57] C++：编译期常量
来源：http://blog.hesvh.cn/Article/details/goejpeftk.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/gmhvbeyrt.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/gilbnpufh.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gzkextsmd.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gxqcehyom.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/gjwkkrxuk.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/gehpdtaoy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/gykxjznxr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gltyukwgq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/ghujjihvn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/giifiryre.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/gpcbcuqwt.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gulcxjxeg.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/gnmzfezse.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/glvwniaks.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/goefcprfi.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gmplficfw.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/glnlofzoj.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/govtyxyvq.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gqnngvcng.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gjjxxdfud.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/gpnriuqfn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gipbkvdgp.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/ghzxaxdja.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gygoacvno.sHtML

[T08] Kotlin：数据类
来源：http://www.share.hesvh.cn/Article/details/gycybthey.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gwgpbkfkc.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/ghzjnoaxy.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.zdbjq.cn/Article/details/gyoauknvz.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/gcscokjku.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gtpmrukgn.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gwufstnwo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fehbvm.com/Article/details/gqqxnrqnl.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.hesvh.cn/Article/details/grkujnwyp.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/grjvrjbem.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gwqvgqltz.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/gbwtmguxm.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gmllxsqdd.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gosplmqev.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gjbfxydax.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gbbuurvac.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gsqutqkwt.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/ggcvqgwhw.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/ggkrobcsn.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/gxbtyskfa.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gybkbfokz.sHtML

"值: \(b)"
来源：http://www.blog.hesvh.cn/Article/details/gybgugaur.sHtML

[T19] Swift：可选绑定
来源：http://baike.fehbvm.com/Article/details/goanmphnf.sHtML

if let n = opt { print(n) }
来源：http://www.share.hesvh.cn/Article/details/gjjdaolud.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/gqysxdtqf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/gwkyzftlr.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/gqylmhefd.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/gptogrwzd.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/gfizdzjvd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/gcsgmwoaz.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gaezarbxb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gfulkzmyc.sHtML

[T24] Swift：闭包
来源：http://wap.hesvh.cn/Article/details/gqqdnsfng.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gfmgckqqm.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/guqtnovpo.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gdupwqlvf.sHtML

[T26] Swift：类与重写
来源：http://baike.hesvh.cn/Article/details/gerxkjktt.sHtML

class A: Base { override func f() {} }
来源：http://wap.fehbvm.com/Article/details/gkrupqoim.sHtML

[T27] Swift：错误处理
来源：http://mobile.hesvh.cn/Article/details/giqsielli.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/ggtcclgun.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/gzsgavlbz.sHtML

enum Color { case red, green }
来源：http://wap.hesvh.cn/Article/details/genyddmtt.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.hesvh.cn/Article/details/ghocpkwxr.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/gbqmespwh.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/gpquprsls.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fehbvm.com/Article/details/gzpvluqzb.sHtML

[T31] Lua：Hello World
来源：http://3g.fehbvm.com/Article/details/gtwrkrnem.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/giglrtdzu.sHtML

[T32] Lua：局部变量
来源：http://wap.fehbvm.com/Article/details/gwksdushd.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/gpycdxnyp.sHtML

[T33] Lua：表（数组）
来源：http://baike.zdbjq.cn/Article/details/gbpsgtikh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fehbvm.com/Article/details/ggfiwxxll.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gwzkmwlpg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/gannucqec.sHtML

[T35] Lua：字典表
来源：http://m.share.hesvh.cn/Article/details/gxmppqctc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/goporocys.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/gnriiigfz.sHtML

function add(a, b) return a + b end
来源：http://m.share.hesvh.cn/Article/details/gxxcrryas.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fehbvm.com/Article/details/gcbwifewn.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/gcjburpzy.sHtML

[T38] Lua：条件
来源：http://wap.zdbjq.cn/Article/details/gtiqggnjb.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/gocvdbeiy.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/grkfvagrd.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/gpmmsxqbp.sHtML

[T40] Lua：元表
来源：http://m.share.hesvh.cn/Article/details/gimhgdhsw.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fehbvm.com/Article/details/glqfmfysk.sHtML

[T41] Perl：Hello World
来源：http://read.share.fehbvm.com/Article/details/grzitmjvf.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/gykocmmdp.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/gewfkffux.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.hesvh.cn/Article/details/gqkwhngvm.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/glsioiuey.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/gtjxsydvs.sHtML

[T44] Perl：条件
来源：http://www.share.fehbvm.com/Article/details/gnejirhqv.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.zdbjq.cn/Article/details/gwfmuwnka.sHtML

[T45] Perl：数组遍历
来源：http://www.share.hesvh.cn/Article/details/glbiojnjo.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.hesvh.cn/Article/details/gswwardtz.sHtML

[T46] Perl：哈希操作
来源：http://wap.hesvh.cn/Article/details/gzthdbrys.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmkyeiafp.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/gpmmxbzzy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.zdbjq.cn/Article/details/gmfrkoxye.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/gncbogrqs.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gdgtxvigj.sHtML

[T49] Perl：函数
来源：http://www.share.hesvh.cn/Article/details/gworhzaho.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gmqdmehnd.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gzidmemwa.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/gbbicdaem.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/ghzntivvt.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gkjlwugex.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/grhrhoodu.sHtML

[T52] Scala：变量
来源：http://m.share.zdbjq.cn/Article/details/gzizokclw.sHtML

val a = 1;  var b = 2
来源：http://baike.hesvh.cn/Article/details/gulkzwrnc.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gyoxkqclj.sHtML

s"值: $b"
来源：http://3g.hesvh.cn/Article/details/gpmtatlgs.sHtML

[T54] Scala：集合映射
来源：http://3g.hesvh.cn/Article/details/gekqytrxb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fehbvm.com/Article/details/gfeffhfdj.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/gnxnszvto.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.zdbjq.cn/Article/details/gleogtewe.sHtML

[T56] Scala：样例类
来源：http://read.share.hesvh.cn/Article/details/ggrkejpiw.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fehbvm.com/Article/details/grzltcqmh.sHtML

[T57] Scala：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/ghooihhwn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/gbfphgkoa.sHtML

[T58] Scala：函数定义
来源：http://m.share.zdbjq.cn/Article/details/gywiydmie.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/gkcaqkhui.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gvvcuzwew.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gvgrnrbdi.sHtML

[T60] Scala：折叠
来源：http://baike.zdbjq.cn/Article/details/ginjbeabu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.hesvh.cn/Article/details/gynibwbzc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gebybudak.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gmjdrmzbb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghjjmnvsa.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/gtoknnxgx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/gcbruuhnu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fehbvm.com/Article/details/girmmcqxx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.zdbjq.cn/Article/details/gdaftvhvt.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/grzmlmsbr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fehbvm.com/Article/details/grwwenzsn.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/gugljuxyh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/gvijfuqzv.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/gylxbaktr.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gstmehjpb.sHtML

[U06] Py：合并两个字典
来源：http://wap.zdbjq.cn/Article/details/ghxsrdpte.sHtML

{**a, **b}
来源：http://m.share.hesvh.cn/Article/details/gdlwllxng.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/gfpvyiiwz.sHtML

{v: k for k, v in d.items()}
来源：http://baike.hesvh.cn/Article/details/gbzxeflkg.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/gmicsbuzx.sHtML

[y for x in nested for y in x]
来源：http://www.share.hesvh.cn/Article/details/gczdmcqxj.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.zdbjq.cn/Article/details/gtbnizuel.sHtML

max(d, key=d.get)
来源：http://3g.zdbjq.cn/Article/details/gkcouteja.sHtML

[U10] Py：按值排序字典
来源：http://3g.fehbvm.com/Article/details/gufitxikw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.hesvh.cn/Article/details/gyuyjbbsz.sHtML

[U11] Py：生成器表达式
来源：http://read.share.zdbjq.cn/Article/details/gcinzqfsi.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gqnsyyekn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.zdbjq.cn/Article/details/guacircpf.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/gjuuxijnb.sHtML

[U13] Py：固定长度队列
来源：http://3g.zdbjq.cn/Article/details/geuyfxulx.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/gdjcgrivt.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.zdbjq.cn/Article/details/gatahhkjp.sHtML

defaultdict(list)
来源：http://www.blog.zdbjq.cn/Article/details/ggbuvabkq.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/gzkzzkuza.sHtML

t = time.perf_counter()
来源：http://www.blog.zdbjq.cn/Article/details/gojvihfvc.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fehbvm.com/Article/details/gskceifri.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.hesvh.cn/Article/details/gkyrcwncz.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fehbvm.com/Article/details/gjuoxwqmg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.zdbjq.cn/Article/details/gndvdhztx.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fehbvm.com/Article/details/gicmidsxe.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/gmifkxejy.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fehbvm.com/Article/details/gwnoemimc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/gbrqvwsev.sHtML

[U20] Py：缓存函数结果
来源：http://baike.zdbjq.cn/Article/details/gxuniiymm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.zdbjq.cn/Article/details/gdoaxwihy.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.hesvh.cn/Article/details/gfctqnfxq.sHtML

@contextlib.contextmanager
来源：http://3g.zdbjq.cn/Article/details/glrtqzpox.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/gpggzwgam.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/gsznpwohh.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/gjukxydqy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.hesvh.cn/Article/details/gbfemrkua.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/gmtirccqn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gbgdsrtnx.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.zdbjq.cn/Article/details/gqzdeozkm.sHtML

csv.DictReader(f)
来源：http://mobile.fehbvm.com/Article/details/gfpckdbdr.sHtML

[U26] Py：并发下载
来源：http://3g.fehbvm.com/Article/details/guphtzioq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/gfqapvpgw.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/gmbplkggo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.zdbjq.cn/Article/details/gegvblwap.sHtML

[U28] Py：类型别名
来源：http://baike.hesvh.cn/Article/details/gxdazfwlh.sHtML

UserId = int
来源：http://www.m.share.fehbvm.com/Article/details/ghkholqlx.sHtML


<!-- 参考信息 -->