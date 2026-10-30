代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/gfeiheros.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/gvceeqwof.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.zdbjq.cn/Article/details/gcviueddc.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/giqfobrdn.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gejemiewp.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/gtkhnqmrk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/ghywuotua.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gzzhhytks.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gsypzynpp.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/gkssfuhmi.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/gtivcsoiu.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gsyxudmgr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.hesvh.cn/Article/details/gwfpsarov.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/givstmatu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gudnandif.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gqgiqgjex.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gvufzrmjc.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gphwqvptx.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gydijzzks.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/ghkillltm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/gpuyzhzxn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gfoxfkada.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gwlfgonem.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gnzqpuslk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gwvhewylw.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/gguzzwucq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gnqhvnjnn.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gjmvoxmtl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gbpglxndj.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gaqrrhidt.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/ggwsalkgl.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/gagxmmqne.sHtML

x |= (1 << 3);
来源：http://www.blog.hesvh.cn/Article/details/gyydngtbu.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/guplmtqsw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/gfodjzwae.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/gwismikmm.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/gtzrezgdd.sHtML

[S19] C：快速排序
来源：http://mobile.hesvh.cn/Article/details/gegibzbau.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gsbnraowg.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gqgovxgul.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gawmvjcxe.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/ghkvormxg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/gqjxosdwa.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/grofukgyf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/gqnkxtgiy.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gffjpcjkw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/gmmkhzgco.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gnznhedls.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/gaynwpfto.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/gqhvumtdk.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gnofdpwzx.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gyvzkmizi.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gbjlsgdvl.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/godsxzatk.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gzkjfhzjp.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/ggznecqbn.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/gfwprqskt.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gronkariz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gzfbvdtfh.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gzgbjiqik.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/gtisrjbkh.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/giznxwelu.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/gignzvmwa.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/gafvqrqsp.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gpmgcgkxw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/gnmvfwehr.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/gikqvhkph.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/gtziehrfd.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gxwnkqrph.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gcejgnbsi.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gaqusvkmd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/gmlkdopyw.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gafiactsn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gqvlhurez.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/gxkbagjxi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gudcfkfqv.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gkjnljozb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gjswgyync.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/gcmxavhuu.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gcutwswtq.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/gtpfrqhhd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/giqgyzekz.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/grxjorpah.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/gqwrlnryp.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/gflwwnvcv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/giasbyhae.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gsvbiuysn.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/gzzsnqchv.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gbdcbemjn.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/guedcefen.sHtML

[S44] C++：引用传参
来源：http://read.share.zdbjq.cn/Article/details/gzaorgivu.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gipfwydcf.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gpbczstrd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gmxfigive.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gryzbeboc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/gfeptdxsl.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/gbyatdhml.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwblmrszt.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gefbvmrpc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/ghiktxtwi.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/gxxtgwnwm.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/gihujznhr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/grjsupywx.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/grlzgyppq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gwjqkxbej.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/gnwbyievs.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/gthhjtxvh.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/gnjgyiaus.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/gwpndykik.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/gelgxuswg.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gmfcthqqp.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/grwrhslbp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/gbkjcbnwv.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/gtoesvwiv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gazcsiqpa.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/ggtthrovj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/gigrkncst.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/ghttezcyr.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gjwinifia.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/gmzonkvxm.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/gyassaejx.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/gkydwxxbz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/gccluwwxh.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gltkveirm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gyyfhmlez.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjdwnfshe.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gbkfygmjs.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gudtncgkp.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/gwcezisdd.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gbswzowxc.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/gkrvdrece.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/gfjvqziyf.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/gvamdxkts.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gxwrhscst.sHtML

[T04] Kotlin：空安全
来源：http://mobile.zdbjq.cn/Article/details/gxwtzpyzy.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gjkgmktqe.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gkkvjtcue.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/gggievxhu.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.zdbjq.cn/Article/details/goeaehlij.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gnmfwvzxl.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gzseoghur.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gqrrerprc.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/geumrctof.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/gdzfdmlns.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.zdbjq.cn/Article/details/ggrtxchon.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/gobbrdjsd.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/gbxrupaxg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/guujncsta.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gdvwqikan.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/ggkocheys.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.hesvh.cn/Article/details/gzkdorxxy.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gjirtnrtu.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.zdbjq.cn/Article/details/gswoscmei.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fehbvm.com/Article/details/gckrxkagn.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/gfslubmoa.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/gzpqpifdw.sHtML

[T15] Kotlin：接口
来源：http://baike.zdbjq.cn/Article/details/grukmzohz.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gknitwser.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gpzuqgpdb.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gumnlkzms.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gbcgbhfdn.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gmwtnvehm.sHtML

[T18] Swift：字符串插值
来源：http://blog.fehbvm.com/Article/details/gfipwjxjn.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/gcuedusvx.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gqfvvafrp.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/gpgwwwysn.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/gpltwsljq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/gjqmnthtp.sHtML

[T21] Swift：遍历
来源：http://baike.hesvh.cn/Article/details/gwqpvngkf.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/gyapslmnz.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/ghwnjiwjo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fehbvm.com/Article/details/gppxiphlr.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/ggflcfioy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/gznmmmvbq.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/gsbxicubo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gugwyycqt.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/gsjiufcmg.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/gaxsfwipw.sHtML

[T26] Swift：类与重写
来源：http://read.share.hesvh.cn/Article/details/gemaacnqt.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/gthpnqspw.sHtML

[T27] Swift：错误处理
来源：http://3g.fehbvm.com/Article/details/ghgrpmkpu.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/giccwxhgl.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/gqgiaavax.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gsxvisbpx.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/gnahgsrfq.sHtML

guard let x = opt else { return }
来源：http://www.blog.fehbvm.com/Article/details/gbahdbkqr.sHtML

[T30] Swift：协议
来源：http://mobile.fehbvm.com/Article/details/grdunlzxs.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fehbvm.com/Article/details/gfihbgdok.sHtML

[T31] Lua：Hello World
来源：http://www.share.fehbvm.com/Article/details/gzqenukey.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gwcvjdirt.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/grjghwral.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/gseibbaip.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/gocooucqx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/gvieaqwhv.sHtML

[T34] Lua：遍历表
来源：http://www.blog.zdbjq.cn/Article/details/gaojxgkyx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.hesvh.cn/Article/details/ggnlzazlz.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/gpxwrlnbk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.zdbjq.cn/Article/details/gvhbegcrz.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gnsxsvqqj.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/gyhfrekhm.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/gzwiznewa.sHtML

"a" .. "b"
来源：http://www.share.fehbvm.com/Article/details/gbgupungv.sHtML

[T38] Lua：条件
来源：http://www.share.hesvh.cn/Article/details/gookzcaet.sHtML

if x > 0 then print("正") end
来源：http://mobile.zdbjq.cn/Article/details/gexsiocjy.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gvqjkotlq.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/grznqsmpn.sHtML

[T40] Lua：元表
来源：http://m.share.fehbvm.com/Article/details/gpyijzqvk.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fehbvm.com/Article/details/gcamlwtny.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gxgvcrxlc.sHtML

print "Hello\n";
来源：http://www.blog.fehbvm.com/Article/details/gigkggzup.sHtML

[T42] Perl：变量类型
来源：http://www.blog.hesvh.cn/Article/details/gqztzyqio.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/gjbmcpuwl.sHtML

[T43] Perl：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gbwlruwxt.sHtML

"值: $a"
来源：http://read.share.fehbvm.com/Article/details/gapplorjv.sHtML

[T44] Perl：条件
来源：http://mobile.hesvh.cn/Article/details/gfilqqwci.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.zdbjq.cn/Article/details/glvosbwne.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fehbvm.com/Article/details/gkcadtteb.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.zdbjq.cn/Article/details/ggmuffatp.sHtML

[T46] Perl：哈希操作
来源：http://baike.hesvh.cn/Article/details/gxfkhlbag.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.hesvh.cn/Article/details/gmhbbrkfi.sHtML

[T47] Perl：正则捕获
来源：http://3g.fehbvm.com/Article/details/gqplolzvb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.zdbjq.cn/Article/details/gttujwtni.sHtML

[T48] Perl：正则替换
来源：http://mobile.fehbvm.com/Article/details/gvcorkyqx.sHtML

$s =~ s/old/new/g;
来源：http://m.share.hesvh.cn/Article/details/gxievezvk.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/gyacdnmck.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gdysemzpi.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/guugqurrs.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fehbvm.com/Article/details/gryzjozdi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.hesvh.cn/Article/details/gsyvhbtlr.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/gavrzzeau.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gopnutexq.sHtML

[T52] Scala：变量
来源：http://mobile.fehbvm.com/Article/details/gcrmrylgs.sHtML

val a = 1;  var b = 2
来源：http://www.share.hesvh.cn/Article/details/gmlhpfupo.sHtML

[T53] Scala：字符串插值
来源：http://wap.hesvh.cn/Article/details/govnnwanu.sHtML

s"值: $b"
来源：http://wap.hesvh.cn/Article/details/gwdwpyvyk.sHtML

[T54] Scala：集合映射
来源：http://baike.zdbjq.cn/Article/details/gvtbopvrp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/gjxzermdr.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/grvrmpovw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.hesvh.cn/Article/details/gnxttemgy.sHtML

[T56] Scala：样例类
来源：http://3g.zdbjq.cn/Article/details/gknpdzjut.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/gufynuulk.sHtML

[T57] Scala：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gpfgdncuz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fehbvm.com/Article/details/gkkruvooc.sHtML

[T58] Scala：函数定义
来源：http://read.share.fehbvm.com/Article/details/gpkimshxs.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/geynjssag.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/gxusbwfdv.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gffglrrsp.sHtML

[T60] Scala：折叠
来源：http://mobile.zdbjq.cn/Article/details/gzxwypvcc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.hesvh.cn/Article/details/gjhdmxszf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gyzajobez.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/goxjupaje.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjjtvgdxs.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fehbvm.com/Article/details/gpttaocvz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/gdnhjzrtu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fehbvm.com/Article/details/gohdjdabd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fehbvm.com/Article/details/gsowlywoi.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.zdbjq.cn/Article/details/gewiuztak.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/garyakldq.sHtML

[U04] Py：变量调试打印
来源：http://mobile.zdbjq.cn/Article/details/gzveukthz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fehbvm.com/Article/details/gaugfaebx.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fehbvm.com/Article/details/gtmmxmypt.sHtML

list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gughaphij.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.hesvh.cn/Article/details/gnrsyfsgb.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gkfghdsmn.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.hesvh.cn/Article/details/gmpjtqvex.sHtML

{v: k for k, v in d.items()}
来源：http://baike.zdbjq.cn/Article/details/gnhvjxfbq.sHtML

[U08] Py：展平二维列表
来源：http://m.share.hesvh.cn/Article/details/gfqotasik.sHtML

[y for x in nested for y in x]
来源：http://www.blog.hesvh.cn/Article/details/glrhxacrh.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/gofbocgfy.sHtML

max(d, key=d.get)
来源：http://m.share.hesvh.cn/Article/details/gkkihpxfl.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gxnjwvpwu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fehbvm.com/Article/details/gvxaipish.sHtML

[U11] Py：生成器表达式
来源：http://blog.fehbvm.com/Article/details/gvvmpzsbp.sHtML

(x * 2 for x in arr)
来源：http://wap.fehbvm.com/Article/details/gdzgbiqll.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.hesvh.cn/Article/details/gqahzrxfg.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/gcurdngit.sHtML

[U13] Py：固定长度队列
来源：http://3g.zdbjq.cn/Article/details/gbzirdlbm.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/gqbeleqbq.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.zdbjq.cn/Article/details/gsfvoesxo.sHtML

defaultdict(list)
来源：http://wap.zdbjq.cn/Article/details/gtqpgzrth.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/gepvgtypp.sHtML

t = time.perf_counter()
来源：http://3g.hesvh.cn/Article/details/gkwcotwpf.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/gevmylmji.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fehbvm.com/Article/details/gyzlhekfc.sHtML

[U17] Py：初始化日志
来源：http://baike.hesvh.cn/Article/details/geovgoqjd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fehbvm.com/Article/details/gkpkqniui.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fehbvm.com/Article/details/gqmlyeilo.sHtML

pat = re.compile(r"\d+")
来源：http://3g.hesvh.cn/Article/details/gqmxmpien.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.zdbjq.cn/Article/details/gweueeccx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/gvtxvjkdx.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.hesvh.cn/Article/details/gfqrtkgbi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fehbvm.com/Article/details/gqxuxtmbb.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.zdbjq.cn/Article/details/glpxyrkwz.sHtML

@contextlib.contextmanager
来源：http://blog.hesvh.cn/Article/details/ggjyscclo.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/gkrsopahz.sHtML

list(zip(*m))
来源：http://www.m.share.zdbjq.cn/Article/details/gokzgfxaj.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/gdsdsphua.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fehbvm.com/Article/details/gcvrswyhk.sHtML

[U24] Py：路径操作
来源：http://3g.hesvh.cn/Article/details/gmornwlts.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gfavfdsgz.sHtML


<!-- 参考信息 -->