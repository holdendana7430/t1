代发 wailian999

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gqgrnonoa.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsgdysrjs.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gjhiauind.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gpjfcftoz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/gegiibaqq.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gtnrzxfdc.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gguxpwrtk.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/grhkrqsum.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gsmrdidkr.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/gfildfgdg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/ghdlbgcpo.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gnvsbthmf.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/gewdjsfro.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/gtsuprwmq.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/grcwbfkgl.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gjaaepvci.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gglyzxnjg.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gpxjbktrp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/gbkuwcgzb.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/giiqylmwd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/guymoibut.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gbzcneupw.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/gllseqlaz.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gdxpocgvh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/gmpwulgys.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gpgstfsvv.sHtML

fclose(f);
来源：http://mobile.fehbvm.com/Article/details/ggrgwotmy.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gaqvunmks.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gebdfbevz.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gozoaiwxw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/ganfnalfj.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/gtugrxpwe.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gmcvozczi.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/gplyzzuur.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/gkbfzdzfw.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/gjuwjjikc.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/gnqmagyuz.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gjkxbjnew.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gttuwdzzh.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/ggwgbusxl.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/golswxtqw.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/gmndsvayk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gszueybkv.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/ghdfycmoa.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gouyvfxfl.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/gvdnvqdog.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/guyvuhomg.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gsxiduquf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gnkcdjbyi.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/giecetjuj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/ggboziypb.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gegbohrnn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/gcnveoyhl.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gqkuffato.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/gesxocofn.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/ghatfbatj.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/gnnaphkua.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gagmvuens.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gcupenebv.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/gcrgywydg.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/geetrcvvp.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gevkuvamr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/guuqlvkmj.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/grkljoxip.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gcllynsew.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/gvjyuqewu.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/gofkigxqe.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/ggnuueodr.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gitqbeuif.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/gihjwkubg.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/gblzpoyqr.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/gpgninwrs.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gchztshph.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/ghlrqzudw.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/gfgysxeuv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsknzzmac.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/guhoicyna.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gkcbgvchn.sHtML

[S36] C++：unordered_map
来源：http://wap.fehbvm.com/Article/details/gqxhpxcbi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gplksnhkr.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gofassbgx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/gpgpsldiq.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/gasladngh.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/gqmrervoj.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gkofewsyf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/grdglkqke.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gkpudqwax.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.hesvh.cn/Article/details/glbjrscls.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/gemkvitxb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/gzbflhdqw.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/gwagjednc.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/gtkbsclch.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/glvunalea.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/gjzepqfpc.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gmssbgbhq.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/gwplgqyal.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/guciyxqli.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/gfeytabeo.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/grddnnhuy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gyuvhpkwf.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gcuceytar.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gdjvktbsk.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gewrbaafl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gwsscizof.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gujjxxnth.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gppdpkhrc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/guwvzetto.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/grxibmnfn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gqcemrvzt.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/gmrethyej.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/gjfynhwci.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/guhtcxjjj.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gokoeqfcv.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/gbdvdvgyw.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/gqtorndkm.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/gdxpauedr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/gimoxoyfv.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/glbhhurlj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gweofcmfj.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/gllunzodi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gqkphjadu.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gdmzuwilb.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gueovwwit.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gjouidxcu.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gikngusbn.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gpdnfzqhk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gfdbmgkyp.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gvtpjwqao.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gfzsxbxge.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdqxsyerb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gbxosxmxu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcavlugxt.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gxkbytzws.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gdvniujpq.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/geltuzeos.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.zdbjq.cn/Article/details/gpcpufwje.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fehbvm.com/Article/details/gviawkqio.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gynozjjzm.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gzjzttlsq.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/ghciswuox.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gnjfyiffi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/gnvbrzauy.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gupqknzlf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/gxfqqemdk.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gkaoxwjou.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/gtowwmlwi.sHtML

[T08] Kotlin：数据类
来源：http://wap.fehbvm.com/Article/details/ghudhfplu.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gbfryxjlm.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/gpakdxtpj.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/gnpfynplh.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/gflqxpojk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/gegqvolzc.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/gwzvyjekh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/gxpzoayhz.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/gpjydqqmd.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gogivinqa.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.hesvh.cn/Article/details/gebzsbgur.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gepfesqjt.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/giyabuvos.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gjnzviyqt.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/ggkkwvajh.sHtML

interface Shape { fun area(): Double }
来源：http://blog.hesvh.cn/Article/details/gblhlxkgc.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gjwswisig.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gnsxhcjnj.sHtML

[T17] Swift：变量与常量
来源：http://blog.zdbjq.cn/Article/details/gnzddzycq.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gsnuclncu.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gcfzgxpuo.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/gytffqklc.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/gkduqdfgh.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/grqsxsbkh.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/govhzrizy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gbqcuytuq.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/gfqccvhns.sHtML

for x in a { print(x) }
来源：http://3g.hesvh.cn/Article/details/gjyfsnugu.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/gxmzluezt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gqazsisgs.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/gdizkltin.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.zdbjq.cn/Article/details/gfxsrzgua.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/gndghbiwb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gkfmiaooi.sHtML

[T25] Swift：结构体
来源：http://m.share.fehbvm.com/Article/details/gtwldfaqs.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/guhvmmdbn.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/goralixkr.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/gzbzqmhfo.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/goadpwaqs.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fehbvm.com/Article/details/gpkxjemls.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/gmekrcnzq.sHtML

enum Color { case red, green }
来源：http://www.share.fehbvm.com/Article/details/grnaxbcgl.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.zdbjq.cn/Article/details/gwiueplaa.sHtML

guard let x = opt else { return }
来源：http://baike.zdbjq.cn/Article/details/gbmhqyzkk.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gqkuxngqz.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/gkhscjiyi.sHtML

[T31] Lua：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gznttxogz.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gmrvzhtqg.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/gbgprztpr.sHtML

local a = 1
来源：http://www.share.fehbvm.com/Article/details/grjoftsol.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.hesvh.cn/Article/details/gzmwiboof.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/ggemaiwrt.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gipddkpsm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gjjizuhnl.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/gbqjmggfb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.zdbjq.cn/Article/details/giteisszs.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/ggorsxtcb.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/giaxcjwrb.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gaytkupmk.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/gjdqztmlq.sHtML

[T38] Lua：条件
来源：http://wap.zdbjq.cn/Article/details/gruhvbmwb.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/gxnetftnu.sHtML

[T39] Lua：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gbaveperc.sHtML

string.find(s, "%d+")
来源：http://www.blog.zdbjq.cn/Article/details/gcuorfbxz.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/gkgvpeppx.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fehbvm.com/Article/details/gnpwcyyop.sHtML

[T41] Perl：Hello World
来源：http://www.share.hesvh.cn/Article/details/gdowziwsx.sHtML

print "Hello\n";
来源：http://blog.hesvh.cn/Article/details/ghibtmypa.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/gwgollzgi.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fehbvm.com/Article/details/gmzckqait.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gifpyobbv.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/gbveolxpg.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/gunttioqy.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/gmjdogacd.sHtML

[T45] Perl：数组遍历
来源：http://blog.zdbjq.cn/Article/details/gqhixqvto.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbhmjtehs.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gqtyfqgaq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/glevtdmnt.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fehbvm.com/Article/details/gmaqplqtu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.hesvh.cn/Article/details/gfyeryzeg.sHtML

[T48] Perl：正则替换
来源：http://3g.fehbvm.com/Article/details/goxdbxgmx.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/gdorqdpeu.sHtML

[T49] Perl：函数
来源：http://3g.hesvh.cn/Article/details/gjzddovir.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gvmwbbgss.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gqbouqwvx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/guacbtyti.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gltgkacom.sHtML

[T51] Scala：Hello World
来源：http://blog.zdbjq.cn/Article/details/gnwekjhad.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gopzrajru.sHtML

[T52] Scala：变量
来源：http://mobile.fehbvm.com/Article/details/gtejkspeq.sHtML

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/gnfdtkvbc.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gidbopcbp.sHtML

s"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gkiwiyuqg.sHtML

[T54] Scala：集合映射
来源：http://m.share.fehbvm.com/Article/details/ggdyibwzv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fehbvm.com/Article/details/gfwsqbodo.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/gcaoavpsj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.hesvh.cn/Article/details/gbjrjbrdk.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/ghmnqxfhh.sHtML

case class User(name: String, age: Int)
来源：http://baike.zdbjq.cn/Article/details/gcbzvbrcx.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gzngdeqwi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.hesvh.cn/Article/details/gzkrihsng.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/gvebdjmtl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.zdbjq.cn/Article/details/gasgtgzjx.sHtML

[T59] Scala：循环
来源：http://www.share.fehbvm.com/Article/details/glltjklli.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.hesvh.cn/Article/details/gjdnwkkvw.sHtML

[T60] Scala：折叠
来源：http://read.share.hesvh.cn/Article/details/gaszzicsd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.hesvh.cn/Article/details/gwadjokcj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnhgrpofm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gulumpjpq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggqiqlahv.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/gffbvvjhj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.zdbjq.cn/Article/details/gxaardlkx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fehbvm.com/Article/details/gmuoybkxk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fehbvm.com/Article/details/grlswfecz.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fehbvm.com/Article/details/gnbrzswkw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.zdbjq.cn/Article/details/grgmlgefd.sHtML

[U04] Py：变量调试打印
来源：http://m.share.hesvh.cn/Article/details/gmaozfrhh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/goohvlwih.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/gqlxvrfdm.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gyxaoupkg.sHtML

[U06] Py：合并两个字典
来源：http://m.share.hesvh.cn/Article/details/gndofksau.sHtML

{**a, **b}
来源：http://www.share.zdbjq.cn/Article/details/gwjhbhscv.sHtML

[U07] Py：反转字典键值
来源：http://mobile.hesvh.cn/Article/details/gdcogqjfg.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/gsmcncwtt.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.zdbjq.cn/Article/details/giyzwojad.sHtML

[y for x in nested for y in x]
来源：http://www.share.hesvh.cn/Article/details/guasxbnfx.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.zdbjq.cn/Article/details/gtlzctuxu.sHtML

max(d, key=d.get)
来源：http://www.blog.zdbjq.cn/Article/details/gmxzcgsjz.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/gzipcsohs.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fehbvm.com/Article/details/gycnygjrj.sHtML

[U11] Py：生成器表达式
来源：http://www.share.hesvh.cn/Article/details/glycatjau.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/guhrhwgza.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.zdbjq.cn/Article/details/gkfllnngg.sHtML

Counter(arr).most_common(3)
来源：http://baike.hesvh.cn/Article/details/gkqruiras.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fehbvm.com/Article/details/gikpkwdpx.sHtML

deque(maxlen=10)
来源：http://m.share.zdbjq.cn/Article/details/gepgcmsni.sHtML

[U14] Py：分组收集到列表
来源：http://blog.hesvh.cn/Article/details/gstmadmeg.sHtML

defaultdict(list)
来源：http://m.share.zdbjq.cn/Article/details/gbkauqqzj.sHtML

[U15] Py：高精度计时
来源：http://www.share.fehbvm.com/Article/details/gasxozkpp.sHtML

t = time.perf_counter()
来源：http://wap.hesvh.cn/Article/details/gzfeydgbe.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fehbvm.com/Article/details/gzlnzjrzc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/grpwfmqgw.sHtML

[U17] Py：初始化日志
来源：http://m.share.zdbjq.cn/Article/details/gttymfsha.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.zdbjq.cn/Article/details/gxogofyqv.sHtML

[U18] Py：预编译正则
来源：http://mobile.hesvh.cn/Article/details/gdtfofhqz.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gtlfuavga.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.zdbjq.cn/Article/details/gcbowcujz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.hesvh.cn/Article/details/goafdgypy.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.hesvh.cn/Article/details/gsnmypaqs.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gcoqeudle.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.zdbjq.cn/Article/details/gngyrgrpt.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/gcbuxryeb.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/guztoqppi.sHtML

list(zip(*m))
来源：http://blog.hesvh.cn/Article/details/grldyevhc.sHtML


<!-- 参考信息 -->