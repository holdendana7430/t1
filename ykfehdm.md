代发 wailian999

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/gsdyjdrvx.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/gatddifyp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gknwryrbm.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gtjxabxvi.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gealpdnsk.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gpvpimcvw.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gpotcvpci.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gausjrill.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.zdbjq.cn/Article/details/gxznwehbl.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/gjhxsutap.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gmvlvbelm.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gbojmrthf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/gjcmbqimj.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/garmwiwbe.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/grtuwosdw.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gpgduphba.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/gqnbsujbw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/gypfuskjk.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gasxchjck.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/gvagnreis.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gptpkppal.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gqfrsyzmm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/gbwpdhsgl.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/gqvzkwgie.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/gtjsfijqi.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gaevdorfw.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/guypuriwj.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/gzdemtqcc.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/guevnkydv.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gdzdzkpux.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gdyhlrbls.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/gxssqcoar.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/gwrabtogh.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gfkzgosrl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gosukkxvj.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/gylcgpxfg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gpshkdnnz.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/glhxzrkyt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/glveoqzaa.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gfimtycoa.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gvvinkmzn.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/gneayqthj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/giezzpprg.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gshgrzqts.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/gphdurwnj.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gumlacmvl.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gzltmltob.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/gjwgkxutt.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gdhwrozua.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gycitvshe.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gfghvjctc.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gdxsuupem.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/glspiaauy.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/ghbjasxhq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fehbvm.com/Article/details/guwleknkd.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gpeargsya.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gvfrescyo.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/gzqvybaqx.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/giboehlqk.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gbxkqaasz.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/gmcshxqys.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/gxsojpans.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gewejjkmn.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gukbbyrwf.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/gepvbbvig.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/giljqyogd.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.zdbjq.cn/Article/details/ggescahlo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.zdbjq.cn/Article/details/gpxeykeek.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/guhegkixd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gkzuxjdvt.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gbmpavcuf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gptxjetct.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/ghoyqtaql.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/goobgfdap.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/ggyajnvxg.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/gxaeymihi.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/ghyzltgcy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/gpvzgbneb.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gogmsuyag.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/ggenifpit.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/giwziiwxg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gwdaligwy.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/gisvsolkg.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gndjgwotc.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gloopkexf.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/galljipsh.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gluplprxh.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gsnccyydp.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gqvudlgvv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gedkuiqiz.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gpperkuhl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gpoztkrtu.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gqxzrocwq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.hesvh.cn/Article/details/gfniownzb.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/goxwzfxum.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gvuqrxiok.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/ggkbjjyrp.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gvlkhtpff.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gbsmrvops.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/gaivkhvfu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/glqrootdv.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gtslfvjgu.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gzmvnazzk.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/gryztwlqs.sHtML

int size() const noexcept { return n_; }
来源：http://3g.hesvh.cn/Article/details/gjfvzlbom.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/gzogtecam.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.hesvh.cn/Article/details/ggjvnyhsr.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/gqwpmrmrm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/gjsbgzojj.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/glvjzmjsy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gwbpuifeq.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/gvzwnmtbw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/gnaftgfyf.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/gupiqnxcv.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gpoqjxurc.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gayadknbt.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/grcfmbcqi.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gppkheght.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/gmhecbuxo.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gzftjisvr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/gmtqypfsz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gscyogice.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gqmbktbvz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnwvqrsyo.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/gtzchxnnj.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/ghlpumktw.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/guljowpuc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gghphonbk.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/gzgwrcmmp.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gudofrrgd.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/glflcfggy.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gqhmwczmt.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/gcmbqkboz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gcntpjlcq.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gmwqbhcmu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gnzaembmh.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gjgaodukr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/gbfbuxihm.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gdawpcfbt.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gmldtjuuc.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gxhnquarv.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/ghfvhnucq.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gkkiqyjzk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/grqfsiuon.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/grgdghonk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fehbvm.com/Article/details/gbhcxlgpi.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/grrrvxgws.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gbpssybtp.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/ghiqvdbzq.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gpiltphmo.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gewzatnri.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gyswgttfi.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gyhodzeue.sHtML

interface Shape { fun area(): Double }
来源：http://3g.hesvh.cn/Article/details/gedbklawz.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/gttnmeyft.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gcevszryo.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/gclcofxgz.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/glfqlgzyk.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/ggomnvqen.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/gejjefqbo.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/gmaszzdsj.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/ggivvhgey.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/gdjokihrs.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/gagykzvca.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/gxldxfkpo.sHtML

for x in a { print(x) }
来源：http://3g.zdbjq.cn/Article/details/gmltabhap.sHtML

[T22] Swift：字典
来源：http://mobile.zdbjq.cn/Article/details/gsaajaukt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/gizaaqyvt.sHtML

[T23] Swift：函数
来源：http://www.blog.hesvh.cn/Article/details/gsytnwsmv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/ggxkenzwk.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/ggrauwgrd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gfofgtbyn.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/gnekzmesy.sHtML

struct P { var x: Int }
来源：http://m.share.fehbvm.com/Article/details/grwkpsves.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/gzwbrjdzo.sHtML

class A: Base { override func f() {} }
来源：http://www.share.hesvh.cn/Article/details/gzlyzbixs.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/grlcyqcvf.sHtML

do { try f() } catch { print(error) }
来源：http://wap.zdbjq.cn/Article/details/gmvpiyigb.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/gkcpurigu.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/gtxnpxbrd.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/gkzsyfmtz.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/gmwuordit.sHtML

[T30] Swift：协议
来源：http://www.blog.hesvh.cn/Article/details/gacswudgh.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fehbvm.com/Article/details/gyuypotrk.sHtML

[T31] Lua：Hello World
来源：http://3g.hesvh.cn/Article/details/ghaucoarq.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/giyedrsqk.sHtML

[T32] Lua：局部变量
来源：http://wap.fehbvm.com/Article/details/gavoqtpnu.sHtML

local a = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gwiggahdd.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/gdcrruelj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.zdbjq.cn/Article/details/gjaaqodhp.sHtML

[T34] Lua：遍历表
来源：http://3g.hesvh.cn/Article/details/grswnblix.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fehbvm.com/Article/details/gdavidqin.sHtML

[T35] Lua：字典表
来源：http://read.share.fehbvm.com/Article/details/gvqcffmja.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gvfjutywk.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/gmgtwvblc.sHtML

function add(a, b) return a + b end
来源：http://mobile.fehbvm.com/Article/details/gtjzltcuy.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/ghwqyutxj.sHtML

"a" .. "b"
来源：http://3g.zdbjq.cn/Article/details/gnwxeikaj.sHtML

[T38] Lua：条件
来源：http://mobile.fehbvm.com/Article/details/gpugnjdrq.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/gohimvtcw.sHtML

[T39] Lua：模式匹配
来源：http://baike.fehbvm.com/Article/details/gouhsdsrr.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/gobpydlmu.sHtML

[T40] Lua：元表
来源：http://wap.hesvh.cn/Article/details/ghtwwahhk.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/gdgpoimcz.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/gcudmknvx.sHtML

print "Hello\n";
来源：http://www.m.share.hesvh.cn/Article/details/gktoxhudw.sHtML

[T42] Perl：变量类型
来源：http://m.share.hesvh.cn/Article/details/gpegbjgvr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/ggrrfkfsb.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gyqejzlnq.sHtML

"值: $a"
来源：http://m.share.zdbjq.cn/Article/details/gnznnhoyc.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/ggmyngjxu.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/gfrhaofck.sHtML

[T45] Perl：数组遍历
来源：http://m.share.zdbjq.cn/Article/details/ggmcfqxuy.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/gmwkptqla.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gbigdoeov.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fehbvm.com/Article/details/gkzhpwkjm.sHtML

[T47] Perl：正则捕获
来源：http://wap.hesvh.cn/Article/details/gqaipihaz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fehbvm.com/Article/details/gzsfhafii.sHtML

[T48] Perl：正则替换
来源：http://blog.hesvh.cn/Article/details/gqvsaczyl.sHtML

$s =~ s/old/new/g;
来源：http://3g.hesvh.cn/Article/details/gfgqyenuk.sHtML

[T49] Perl：函数
来源：http://wap.fehbvm.com/Article/details/glcqwzxri.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gxmpclcqf.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gwiutadnf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fehbvm.com/Article/details/ggzklcnar.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/gcrzawisl.sHtML

[T51] Scala：Hello World
来源：http://wap.zdbjq.cn/Article/details/ggzlizgco.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gnolvostv.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/gpapwdywf.sHtML

val a = 1;  var b = 2
来源：http://wap.zdbjq.cn/Article/details/gfagsswjs.sHtML

[T53] Scala：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gtdzzxnov.sHtML

s"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gtgqmqqzp.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/gzkdzpath.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/ghmkymsos.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gdlcwzgjr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fehbvm.com/Article/details/gumsdqalz.sHtML

[T56] Scala：样例类
来源：http://baike.zdbjq.cn/Article/details/gzzcppxlk.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gihosxmft.sHtML

[T57] Scala：模式匹配
来源：http://3g.fehbvm.com/Article/details/gkmyhzhad.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.hesvh.cn/Article/details/gnndcbuvj.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/glazpsobl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gpurivmsf.sHtML

[T59] Scala：循环
来源：http://wap.fehbvm.com/Article/details/gqunulbrv.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gtrkefrsq.sHtML

[T60] Scala：折叠
来源：http://www.blog.zdbjq.cn/Article/details/gqbvtkhtk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.zdbjq.cn/Article/details/gbrjbfxae.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmfcmeroy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gmlwsoums.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxtfgqyrg.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fehbvm.com/Article/details/gkkiaxzxx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.hesvh.cn/Article/details/gzqhxnqlb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fehbvm.com/Article/details/gvefxocur.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/gpcfzhprt.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fehbvm.com/Article/details/gnlcepjzp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.zdbjq.cn/Article/details/gvkdefrvv.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/gnauaraey.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.zdbjq.cn/Article/details/gxsouzfhc.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.hesvh.cn/Article/details/gkhgoxifi.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gqtidsqtq.sHtML

[U06] Py：合并两个字典
来源：http://blog.hesvh.cn/Article/details/gienzpjcc.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/gyyacjayr.sHtML

[U07] Py：反转字典键值
来源：http://www.share.zdbjq.cn/Article/details/gpkaaulxi.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/garebqdue.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/gilhsdmmd.sHtML

[y for x in nested for y in x]
来源：http://read.share.zdbjq.cn/Article/details/gjumqyfsb.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/ginfaoetq.sHtML

max(d, key=d.get)
来源：http://www.m.share.zdbjq.cn/Article/details/gmeslzjpy.sHtML

[U10] Py：按值排序字典
来源：http://wap.fehbvm.com/Article/details/gdtycsevw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.hesvh.cn/Article/details/gpdphmmoc.sHtML

[U11] Py：生成器表达式
来源：http://www.share.hesvh.cn/Article/details/grlxffhxk.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.hesvh.cn/Article/details/gaowwnrqr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/gplvrupnt.sHtML

Counter(arr).most_common(3)
来源：http://blog.fehbvm.com/Article/details/guddgshay.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.hesvh.cn/Article/details/gzebzllqo.sHtML

deque(maxlen=10)
来源：http://3g.hesvh.cn/Article/details/gfasucneo.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.zdbjq.cn/Article/details/guydfbcuh.sHtML

defaultdict(list)
来源：http://m.share.zdbjq.cn/Article/details/gkmtbgzno.sHtML

[U15] Py：高精度计时
来源：http://www.share.fehbvm.com/Article/details/gxewffcxw.sHtML

t = time.perf_counter()
来源：http://read.share.hesvh.cn/Article/details/glxajoddw.sHtML

[U16] Py：命令行参数解析
来源：http://baike.hesvh.cn/Article/details/gwnrcqzun.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gblxykyen.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gtsubjwsx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.hesvh.cn/Article/details/glmspgojg.sHtML

[U18] Py：预编译正则
来源：http://baike.fehbvm.com/Article/details/gntlmyjbf.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fehbvm.com/Article/details/gwajwspef.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fehbvm.com/Article/details/glrtxthnm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.hesvh.cn/Article/details/ghlypsigc.sHtML

[U20] Py：缓存函数结果
来源：http://baike.zdbjq.cn/Article/details/gsbckdhkq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fehbvm.com/Article/details/gfkxfwofp.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fehbvm.com/Article/details/gxxoeclfm.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/gojtbupod.sHtML

[U22] Py：矩阵转置
来源：http://www.share.hesvh.cn/Article/details/gwkhkbaxs.sHtML

list(zip(*m))
来源：http://mobile.fehbvm.com/Article/details/glffhfeun.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/gqjodoiwa.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fehbvm.com/Article/details/gffeqmyyx.sHtML

[U24] Py：路径操作
来源：http://mobile.fehbvm.com/Article/details/gjjoyymee.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/ggcmtsrla.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.hesvh.cn/Article/details/gtctvugcw.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/gjrcrhtcx.sHtML

[U26] Py：并发下载
来源：http://read.share.hesvh.cn/Article/details/gkeowfwbe.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/grqtpgqua.sHtML


<!-- 参考信息 -->