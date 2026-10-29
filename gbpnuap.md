代发 wailian999

strlen(s)
来源：http://www.blog.zdbjq.cn/Article/details/gqvdeblkq.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gxhjmfhmq.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gnlwkfhac.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gmkefaxpa.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.zdbjq.cn/Article/details/gwwknlott.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gtjnomhif.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gupzczqyi.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/ggohblcnh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fehbvm.com/Article/details/gdsphktxd.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/gaqhtwvmr.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gstjtyhdb.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gazfvfqfg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fehbvm.com/Article/details/gyuxvswko.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/gwmkujxqx.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gmxwgeeat.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gsgbosfjj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fehbvm.com/Article/details/gmeqmisbq.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/gwvarddhz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/glieipktx.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gpgrmpbor.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/gmtxsysjc.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/gpexsaxhj.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/gvuympidk.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/glpeyouzx.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/gbmniyped.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gwhickqrb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fehbvm.com/Article/details/guuzehamw.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/glviijtxj.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gloupucfj.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gbobljbyg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/ghymjxsns.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gwolmdvbb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gwpyqnzbz.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/giyscxmgu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gilabvbvd.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gotrboxuv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/glhwgojwv.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/gnjvvnigz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/grtwnjpmw.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/ggbuwloao.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gotwtpcev.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gijdizmiw.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/gonuzjrjt.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/gvlxzrsap.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gziwnqhtm.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/glahoxsny.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gswclekbn.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/gcghczzvy.sHtML

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/gjaeemurk.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/gbcyegzpr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/ghyhpwpeg.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gjvwpygzt.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gomaplyob.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gsznqmmxd.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gkrinyweo.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/gofzqjlhj.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/gdqjeutll.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/gjbeeysky.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gwtvfcyyc.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.hesvh.cn/Article/details/gphetsolo.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/gvljhkhct.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/gxcsptbmu.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/gqjchqpmu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gjhhydwsl.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/ghnzspuzr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/ggvibhgru.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gponedwst.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/ghgpkrwes.sHtML

[S37] C++：set
来源：http://blog.hesvh.cn/Article/details/gtwmdkygl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/gjhlmitec.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/grtynzusm.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gwyzxgldt.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gbbhyihjp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gvphcdicv.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/gppjpmkbr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gkdljmlkq.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/guobkzxru.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gmkxbgegv.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gwkflquwz.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fehbvm.com/Article/details/gncywypex.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gccwzexfx.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gfbechtsb.sHtML

[S44] C++：引用传参
来源：http://wap.fehbvm.com/Article/details/gbkqhwndd.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gfjogkczj.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/gfprmmmfc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gsyhasmjt.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/ggggodyzx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gneamvyhz.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gahwlfogq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gopmmkbjx.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gmavswngg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/gofakbeob.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/gpndpkwvk.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/gbeqplsqj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.hesvh.cn/Article/details/gzqyspjte.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/grromyozd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gnfjrbomw.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/ghqukexhk.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gmcwddopb.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gfgrxekel.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/glwkbhakl.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/ggjvksoej.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.hesvh.cn/Article/details/gmrnbqdax.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gpuxvfhex.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gtzvenvkc.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/gpgrjhjlp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/glopinlmf.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gyiypuyom.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/gdtszvwsf.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/gypcwaubt.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/grdvvzzlp.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/grybgicht.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/grkzzfxqz.sHtML

[S59] C++：静态断言
来源：http://www.share.fehbvm.com/Article/details/gtxpavtxh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/gzzpnudwq.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/gcmshaevk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/grqjgsssx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/govumiqaq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gcjlkjrbt.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gyaltdmpp.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gwpvtebps.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gkutljpdp.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/gqhxboizh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gnhitfsry.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gfyocklva.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gxpyukggt.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/glprnwzmy.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/giseujcmk.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gvfranidt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.zdbjq.cn/Article/details/gvsoyjbqe.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/gjdxdxhsn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gtzrlbzre.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gbqtygrym.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/gdkzbalkg.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/gwabveudu.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/gbguukzjz.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gujreotgr.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gsxsosbwv.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/gjchwjsvl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/gdmeqmixe.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/gpexlttjf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fehbvm.com/Article/details/gtoeffbca.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/ggazqyksw.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fehbvm.com/Article/details/gyoqvrbum.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/gtwnlpijj.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gtlxnvxtx.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/ghlqydint.sHtML

for (i in 1..10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gzmnugnof.sHtML

[T15] Kotlin：接口
来源：http://blog.hesvh.cn/Article/details/gfyscahgr.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/gbqkfyaad.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/gnvpdpcyu.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/garalqfha.sHtML

[T17] Swift：变量与常量
来源：http://m.share.hesvh.cn/Article/details/gcwcusfcv.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/goishmatp.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gzrjwhmjf.sHtML

"值: \(b)"
来源：http://www.share.fehbvm.com/Article/details/gfpdsjtvt.sHtML

[T19] Swift：可选绑定
来源：http://3g.hesvh.cn/Article/details/gsgsokouo.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/gjgmcxedw.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gsukytenu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gdhaoltpm.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/gqfzfixbj.sHtML

for x in a { print(x) }
来源：http://wap.hesvh.cn/Article/details/gkzmnxpdn.sHtML

[T22] Swift：字典
来源：http://read.share.fehbvm.com/Article/details/gpflcemzh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/gnibimhwu.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/gprgkpgqw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gvwjmthrj.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/gkstpjawt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gyxrpzadi.sHtML

[T25] Swift：结构体
来源：http://read.share.zdbjq.cn/Article/details/ggqhrtvyt.sHtML

struct P { var x: Int }
来源：http://3g.zdbjq.cn/Article/details/gudwctrpv.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/ggnuutfwo.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gruzemgmg.sHtML

[T27] Swift：错误处理
来源：http://read.share.hesvh.cn/Article/details/gdaheqofg.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fehbvm.com/Article/details/guimobbsf.sHtML

[T28] Swift：枚举
来源：http://blog.fehbvm.com/Article/details/gnsgzmklu.sHtML

enum Color { case red, green }
来源：http://www.m.share.fehbvm.com/Article/details/gxflxvbbx.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/guzletsru.sHtML

guard let x = opt else { return }
来源：http://3g.fehbvm.com/Article/details/gpteosfup.sHtML

[T30] Swift：协议
来源：http://3g.fehbvm.com/Article/details/gmnkrkcct.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fehbvm.com/Article/details/gtrtxpnih.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gchnoefju.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gujufiipz.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/gmoinbfzk.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/ggedvrvch.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/gszbyxoer.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fehbvm.com/Article/details/goebpdhow.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/gtcsbdccs.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/gqiovphaa.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gqnponfey.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.zdbjq.cn/Article/details/ggiyrapuv.sHtML

[T36] Lua：函数
来源：http://read.share.hesvh.cn/Article/details/gkybdqdfw.sHtML

function add(a, b) return a + b end
来源：http://baike.hesvh.cn/Article/details/gtotxnrtu.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/giutnpmas.sHtML

"a" .. "b"
来源：http://3g.hesvh.cn/Article/details/gjqkqunbz.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/grnlyhafx.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/geebczwun.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gafehbbzb.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/glubmgirl.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/gyajiiraa.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/gjqanlils.sHtML

[T41] Perl：Hello World
来源：http://3g.hesvh.cn/Article/details/gqazvazly.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gfxpaidwn.sHtML

[T42] Perl：变量类型
来源：http://baike.fehbvm.com/Article/details/gipkilndc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.hesvh.cn/Article/details/gdnfyycpr.sHtML

[T43] Perl：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gmrwpuhwp.sHtML

"值: $a"
来源：http://www.blog.fehbvm.com/Article/details/gugnliowu.sHtML

[T44] Perl：条件
来源：http://mobile.fehbvm.com/Article/details/gmavfgjlr.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fehbvm.com/Article/details/gorikkjrn.sHtML

[T45] Perl：数组遍历
来源：http://3g.fehbvm.com/Article/details/gkstcyudq.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.zdbjq.cn/Article/details/gdysqyqdd.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fehbvm.com/Article/details/gkfzaytli.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.hesvh.cn/Article/details/gpqwsstlr.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/gngroewkg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.zdbjq.cn/Article/details/ggruvugru.sHtML

[T48] Perl：正则替换
来源：http://3g.fehbvm.com/Article/details/gazvmdtwo.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/glpqgbakj.sHtML

[T49] Perl：函数
来源：http://www.m.share.fehbvm.com/Article/details/guhmntyke.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gejpgjece.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/giavrkadb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.zdbjq.cn/Article/details/gipofegth.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtrqllldd.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gzxhrrfdf.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gtjanoglo.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/gnipnkahv.sHtML

val a = 1;  var b = 2
来源：http://baike.hesvh.cn/Article/details/gjaitpgtx.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gkuektowx.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/gazglrmpb.sHtML

[T54] Scala：集合映射
来源：http://wap.hesvh.cn/Article/details/grznzadty.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.hesvh.cn/Article/details/gusdnemrh.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gvidjrmwq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fehbvm.com/Article/details/gsiiifrne.sHtML

[T56] Scala：样例类
来源：http://wap.hesvh.cn/Article/details/glupqtydt.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gmemuugoj.sHtML

[T57] Scala：模式匹配
来源：http://blog.fehbvm.com/Article/details/gcstqngls.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/gpvojrlvs.sHtML

[T58] Scala：函数定义
来源：http://3g.fehbvm.com/Article/details/gqskzihxe.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.zdbjq.cn/Article/details/grllkoykf.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/gaayexuni.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gudpjsxie.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/gqgfybjel.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.zdbjq.cn/Article/details/ggxgbzmeb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxjzcyhrz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/guoldsebc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gcdyvoyuc.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/gvkrnadzv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.zdbjq.cn/Article/details/grksrvrkm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.zdbjq.cn/Article/details/grdlbeupe.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/gjtpnbeuv.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.zdbjq.cn/Article/details/gwyyshnbw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fehbvm.com/Article/details/gvpyimjlm.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fehbvm.com/Article/details/grpkuiibm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fehbvm.com/Article/details/gbidcbsix.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.hesvh.cn/Article/details/gdmtsyqhv.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gickexhsz.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/glzppuuon.sHtML

{**a, **b}
来源：http://www.share.zdbjq.cn/Article/details/gdkbanufh.sHtML

[U07] Py：反转字典键值
来源：http://blog.fehbvm.com/Article/details/gwezlsusn.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fehbvm.com/Article/details/gbnrvrxzx.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/ghcmfaymj.sHtML

[y for x in nested for y in x]
来源：http://www.share.hesvh.cn/Article/details/gfxqujecy.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fehbvm.com/Article/details/gzdlgvwrw.sHtML

max(d, key=d.get)
来源：http://3g.zdbjq.cn/Article/details/gomeejlwl.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gecvcnkxw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/gzuounqlm.sHtML

[U11] Py：生成器表达式
来源：http://www.share.zdbjq.cn/Article/details/gganpqapx.sHtML

(x * 2 for x in arr)
来源：http://m.share.hesvh.cn/Article/details/gvrqmslpo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/gzspyfkoc.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fehbvm.com/Article/details/gxedcxxko.sHtML

[U13] Py：固定长度队列
来源：http://blog.fehbvm.com/Article/details/gyljlhwsx.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/gpinqxngy.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/gbqbebunj.sHtML

defaultdict(list)
来源：http://www.share.fehbvm.com/Article/details/grjjqcint.sHtML

[U15] Py：高精度计时
来源：http://baike.zdbjq.cn/Article/details/ghrclvdoj.sHtML

t = time.perf_counter()
来源：http://www.blog.zdbjq.cn/Article/details/ghkgvouej.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.zdbjq.cn/Article/details/gjcwoftgx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/gqtjfrxfq.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/gkpqcxbof.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.hesvh.cn/Article/details/gixepxirv.sHtML

[U18] Py：预编译正则
来源：http://mobile.zdbjq.cn/Article/details/grkfeoevs.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/grqgqxpgn.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.zdbjq.cn/Article/details/gbzbsoanr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fehbvm.com/Article/details/gldxijpwq.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.zdbjq.cn/Article/details/gryddnihd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.zdbjq.cn/Article/details/gpqeavvhl.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/gmskcinun.sHtML

@contextlib.contextmanager
来源：http://read.share.hesvh.cn/Article/details/gzmhgtdne.sHtML

[U22] Py：矩阵转置
来源：http://read.share.hesvh.cn/Article/details/gdonbupsy.sHtML

list(zip(*m))
来源：http://www.share.fehbvm.com/Article/details/gsyjnccxc.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/ggnngkrhy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.zdbjq.cn/Article/details/gpsbmlyhq.sHtML

[U24] Py：路径操作
来源：http://www.share.fehbvm.com/Article/details/gndxsuinr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gknbzddch.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.hesvh.cn/Article/details/gzmlyxrle.sHtML

csv.DictReader(f)
来源：http://wap.hesvh.cn/Article/details/ghvgcloaj.sHtML

[U26] Py：并发下载
来源：http://blog.hesvh.cn/Article/details/gqxonortt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.hesvh.cn/Article/details/gswekkmzs.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.hesvh.cn/Article/details/gibtpuzgb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fehbvm.com/Article/details/gdyjrwvah.sHtML

[U28] Py：类型别名
来源：http://www.m.share.zdbjq.cn/Article/details/guxvjicmj.sHtML

UserId = int
来源：http://m.share.hesvh.cn/Article/details/gplmhcdzl.sHtML


<!-- 参考信息 -->