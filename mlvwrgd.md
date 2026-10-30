代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gmiduclio.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/gfceldkyr.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gghsyurmq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcnvzxthx.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/gyglaeynu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghmugxdku.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gbljyagas.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/gqzjpuvlm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gvafoivpd.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gtxtnvalf.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/giikooout.sHtML

[S03] C：读入整数
来源：http://baike.hesvh.cn/Article/details/gadwmsbnl.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gzqklkixt.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/gcjvazpst.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/gesecbzht.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gyrilebtq.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/ghooaajgc.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/grlxrcnqo.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gomzouplt.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gjxckpegh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/gdewktpla.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/gcphogyem.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gdqgslemy.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gailrnhgo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/gkfmuxshh.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/glfnxcgrb.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gqkqowull.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gozkkdays.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gcokugzlp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gbsiopntw.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gfcqtsyeb.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gvorwhmbo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gnkyetppe.sHtML

[S13] C：宏定义
来源：http://www.m.share.zdbjq.cn/Article/details/gzgsjvfmq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gyubhntew.sHtML

[S14] C：枚举
来源：http://3g.fehbvm.com/Article/details/gwmtjrtmm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/gryxjravp.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gfbdwtldi.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/goomgtizc.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/gfukgxqtp.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gthnwcmhm.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/gvpizgqgr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/gdwijuejb.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gxcrrcavt.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/gmjnjebaf.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/ghlmlsyle.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gvixjuifx.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gotsukinh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gfkykvtbv.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/ghtxsspou.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/gzmfvgjjb.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gzmhzhtiu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/gtmgrhlnn.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/grvdzvral.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/gyqwwuzoh.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/gnnyhgodr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/goqqgxfxs.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gylcrxlqa.sHtML

memcpy(dst, src, n);
来源：http://www.blog.zdbjq.cn/Article/details/gvhcmqjpz.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/gxhypqgld.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/gavdjtybx.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gotwnimjg.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gxrxzfyrl.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/giltncpzb.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gslbhpnxp.sHtML

[S29] C：变参函数
来源：http://mobile.hesvh.cn/Article/details/gwncgnmoh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gfidduvgn.sHtML

[S30] C：头文件保护
来源：http://www.m.share.zdbjq.cn/Article/details/grazqqafp.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/ggglxonze.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/gbgofyazk.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/gspndlgou.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/gzorndyzl.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/giookkrly.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/ghadvxwzi.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/glebjclue.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/ghvqqfuou.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gshqhoqwq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gnyplswpk.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/gdeohokxn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gyokuqemd.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gldqrzmvh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/guqcmgssw.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gakkevuet.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gyejyciqf.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gdqedlffb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gwxvmuibv.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/gxaimawtc.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.hesvh.cn/Article/details/gkhgblibo.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gfhirvptl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gjhiddihs.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gxfrrexrp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/gfegmcayw.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gytwcwaxf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/gevoyifbd.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/grjsxeutn.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/gyzzdsjqt.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/gimedwiqy.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/grufupygz.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gqpefmaid.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/gynjqwzfi.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gbxqiivym.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/gcgjwnays.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gartjhlht.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/geudxufbl.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gnnumvyrr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gyzavxatv.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gkxauuaod.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/gpntmfzjn.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gefrvzkpb.sHtML

[S49] C++：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gusyfvntp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/gejlxjidh.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gtoogsbys.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gcnprqwna.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/gdbskmtwd.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/guwndogbq.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/gajlqafta.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gvotibuza.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/gffzjhcdg.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/gmzfvobhn.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gfncviqjr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.zdbjq.cn/Article/details/ggsjnlqyk.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/gzeqyubtw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/gwkptgnju.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/gwgkadiky.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/grbxfwlbn.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/gofshaxsj.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/gcxakwoqi.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/ghtadqnyu.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/gmooolndb.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gwxeocgnr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.zdbjq.cn/Article/details/gztgvwbhb.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/gfxqstpbj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/ghylsyddh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghceeices.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gnndajsnp.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glhxcenvl.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/goxfzpcvf.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gfhtpyspb.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/galiceqbe.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gloatzqgp.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/gxguvradq.sHtML

"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gkanbcfxo.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/gjpqdfhvc.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gzzrbddnh.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/goyvxtnmh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gpeuprxpy.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/gcxmsbgzo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gbdvdiqsk.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gvdskusoj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/ghcmilrly.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/gmvbdpgnl.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gyitsekdy.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/guawdwuzb.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/gorrvxdbx.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gueseqtzx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.hesvh.cn/Article/details/gocwllwth.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/gahnxhgyc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/gukzressx.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/gyuqsptiq.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fehbvm.com/Article/details/ggdlioxfb.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.hesvh.cn/Article/details/geuwiffkn.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/gaagyiqwc.sHtML

[T14] Kotlin：循环
来源：http://3g.hesvh.cn/Article/details/guguttwlo.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gaffsvwaz.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/geifbyodl.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/gavwtzkfp.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/gcjvharcn.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gjrjodgmu.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gofkprucx.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gjjncxagg.sHtML

[T18] Swift：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gtljxccrj.sHtML

"值: \(b)"
来源：http://mobile.fehbvm.com/Article/details/gmmoyecjh.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/glhlzauop.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gbvrsyirz.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/gcialsipr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/gxeoiouqu.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/gquzxacls.sHtML

for x in a { print(x) }
来源：http://www.share.zdbjq.cn/Article/details/glnwbvlmi.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/gaqihffog.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/gbyucuxre.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/glgrsngjk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/gvjdvtyma.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/gqeosebmo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/gnwydyuso.sHtML

[T25] Swift：结构体
来源：http://read.share.zdbjq.cn/Article/details/gwlbhaqpx.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/gwvldvqna.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/gtakplurp.sHtML

class A: Base { override func f() {} }
来源：http://www.share.zdbjq.cn/Article/details/gjmdozsqx.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/gtbfoayse.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.zdbjq.cn/Article/details/gttsbwncs.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/gdjzgpmtt.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/garjskwtr.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gqliibdwb.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/gbkmzersd.sHtML

[T30] Swift：协议
来源：http://mobile.zdbjq.cn/Article/details/gwfrmnylh.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.zdbjq.cn/Article/details/gftgmdkve.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/glfqaehbu.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/ghqzqlxbo.sHtML

[T32] Lua：局部变量
来源：http://baike.zdbjq.cn/Article/details/gxgqjoikd.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/gvoeoowrw.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.hesvh.cn/Article/details/gtpoeoqsf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.zdbjq.cn/Article/details/gbtvtcbyy.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gpbnuxkmq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.hesvh.cn/Article/details/gvkzcmkpr.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gvtftgvig.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gvmbhjlal.sHtML

[T36] Lua：函数
来源：http://read.share.zdbjq.cn/Article/details/gaeuuqdkt.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/gtilgthpk.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gzcrakhpy.sHtML

"a" .. "b"
来源：http://m.share.hesvh.cn/Article/details/gvesmgqoh.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/gklccolic.sHtML

if x > 0 then print("正") end
来源：http://read.share.zdbjq.cn/Article/details/ggducdndj.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/gchtiifap.sHtML

string.find(s, "%d+")
来源：http://3g.hesvh.cn/Article/details/givkqthbo.sHtML

[T40] Lua：元表
来源：http://3g.fehbvm.com/Article/details/guygauijj.sHtML

setmetatable({}, { __index = base })
来源：http://3g.zdbjq.cn/Article/details/gapndceoq.sHtML

[T41] Perl：Hello World
来源：http://3g.zdbjq.cn/Article/details/gguzsqfco.sHtML

print "Hello\n";
来源：http://read.share.hesvh.cn/Article/details/gmtnpspwz.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/gyaowvgrw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/ganihflfs.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/gttbnyizb.sHtML

"值: $a"
来源：http://www.blog.hesvh.cn/Article/details/gvunedvfb.sHtML

[T44] Perl：条件
来源：http://read.share.hesvh.cn/Article/details/gcinacpkz.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fehbvm.com/Article/details/gknxrkwql.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/gwxdvnlaq.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fehbvm.com/Article/details/gmnnmbzbp.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/ggsaxfjzu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/gbpfoxxyo.sHtML

[T47] Perl：正则捕获
来源：http://wap.zdbjq.cn/Article/details/gvsmijcgw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.zdbjq.cn/Article/details/gjjvjkiqz.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/ghebqiemw.sHtML

$s =~ s/old/new/g;
来源：http://wap.zdbjq.cn/Article/details/grvdudujf.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/gcddjijss.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gztavmiac.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gxursuuem.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/gprloiwtd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/gchznyyar.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/geaexulbb.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gpxevhrst.sHtML

[T52] Scala：变量
来源：http://m.share.zdbjq.cn/Article/details/gugoddqxf.sHtML

val a = 1;  var b = 2
来源：http://blog.hesvh.cn/Article/details/ghyigpcyk.sHtML

[T53] Scala：字符串插值
来源：http://blog.fehbvm.com/Article/details/genunxwyh.sHtML

s"值: $b"
来源：http://wap.fehbvm.com/Article/details/gpsmnlzvl.sHtML

[T54] Scala：集合映射
来源：http://3g.zdbjq.cn/Article/details/gotlprzzb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.zdbjq.cn/Article/details/gftuanmkg.sHtML

[T55] Scala：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gfcvhglid.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.zdbjq.cn/Article/details/gttyaikmu.sHtML

[T56] Scala：样例类
来源：http://baike.hesvh.cn/Article/details/gvggwlsym.sHtML

case class User(name: String, age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gfvsxllug.sHtML

[T57] Scala：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gnjwtjzuf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.hesvh.cn/Article/details/gathsjnmi.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/gtiocvkqz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/gnntiiica.sHtML

[T59] Scala：循环
来源：http://wap.hesvh.cn/Article/details/gwvfcwpxc.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fehbvm.com/Article/details/gucqgcthf.sHtML

[T60] Scala：折叠
来源：http://m.share.hesvh.cn/Article/details/gwmdqllgf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fehbvm.com/Article/details/gzxcllyed.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtfmaehnn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gmknbgmbk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gskctkpsa.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.hesvh.cn/Article/details/gntyjfwzw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fehbvm.com/Article/details/gkmgcmckv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.hesvh.cn/Article/details/glglpavnm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/gicqgvesd.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.hesvh.cn/Article/details/gugiwjuiq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/goghelrvk.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/geakltaid.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.zdbjq.cn/Article/details/gnzzjihxg.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/gpshqbitu.sHtML

list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gzpdajiat.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/ghqoaztrd.sHtML

{**a, **b}
来源：http://wap.zdbjq.cn/Article/details/gdhlnlzzk.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.hesvh.cn/Article/details/gojhsxtda.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/gqousbwgz.sHtML

[U08] Py：展平二维列表
来源：http://www.share.hesvh.cn/Article/details/gltgmiygu.sHtML

[y for x in nested for y in x]
来源：http://baike.hesvh.cn/Article/details/grvxowgvp.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.hesvh.cn/Article/details/gcwijnclu.sHtML

max(d, key=d.get)
来源：http://www.m.share.zdbjq.cn/Article/details/goveclran.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/gpymyhgpv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/gygimxikf.sHtML

[U11] Py：生成器表达式
来源：http://wap.fehbvm.com/Article/details/gvjbxxgcj.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/gdpucmgpq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.zdbjq.cn/Article/details/gibihnxyw.sHtML

Counter(arr).most_common(3)
来源：http://wap.fehbvm.com/Article/details/gnwraoafc.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/ggnnjmmke.sHtML

deque(maxlen=10)
来源：http://3g.hesvh.cn/Article/details/ghjkpxtcz.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/grzcxraqb.sHtML

defaultdict(list)
来源：http://m.share.zdbjq.cn/Article/details/grrlemkrs.sHtML

[U15] Py：高精度计时
来源：http://wap.fehbvm.com/Article/details/gjpvvdois.sHtML

t = time.perf_counter()
来源：http://blog.fehbvm.com/Article/details/gqggjjjyy.sHtML

[U16] Py：命令行参数解析
来源：http://baike.zdbjq.cn/Article/details/gxjqgjijv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.zdbjq.cn/Article/details/gqfiyovim.sHtML

[U17] Py：初始化日志
来源：http://read.share.zdbjq.cn/Article/details/gyfmckpox.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/girfdrktk.sHtML

[U18] Py：预编译正则
来源：http://read.share.fehbvm.com/Article/details/gaoudrhzx.sHtML

pat = re.compile(r"\d+")
来源：http://wap.zdbjq.cn/Article/details/ghydebhhr.sHtML

[U19] Py：正则替换带回调
来源：http://blog.hesvh.cn/Article/details/ghczeteuy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fehbvm.com/Article/details/gafvocgyn.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/gknjlliuw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fehbvm.com/Article/details/gmzlbihmn.sHtML


<!-- 参考信息 -->